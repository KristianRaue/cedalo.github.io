---
layout: blogposts
title: "Snips, Shelly and Streamsheets"
date: 2019-08-19
image_url: "/assets/images/blogposts/snips_shelly_bitmap0.png"
image_url1: "/assets/images/blogposts/snips_shelly_bitmap1.png
snips_shelly_bitmap1.png
---
We will build our own intelligent speech assistant to control the lighting in several rooms.

In a previous blog I already introduced the Wi-Fi switch Shelly 1 (www.shelly.cloud). Basically this IoT-enabled switch allows to open or close a electrical circuit by sending the value “on” or “off” to a a predefined MQTT topic. The electrical circuit can then be used to control a electrical light or electrically operated machine.

Another very nice IoT component is Snips (www.snips.ai). Snips basically is an Alexa-like speech recognition system that runs locally on a Raspberry PI without sending your voice data to the cloud. Snips uses MQTT and it simply translates you speech commands into MQTT Messages which makes it very easy to integrate Snips into any kind of automation solution.

You can build you own speech assistants using their easy-to-use web interface. Building speech assistants happens in the cloud, but as said before all speech processing is done locally on the Raspi.

I used Snips web interface to build an assistant that allows to switch on or off the light in different rooms of the house. In the following screenshot you can see that the process is pretty straightforward and easy. Basically you define intents (here “OnOff”) and then you define slots that allow to parameterize your speech command (here “room” and “onoff”).


<img src="{{page.image_url}}" width="100%" height="auto">

If you have a look at the training examples in the middle of the screen, you can see what kind of phrases the intent is trained to understands (e.g. “Switch off the light in the bathroom”).

Once the assistant is deployed on the Raspi you activate Snips by saying “Hey Snips” and then maybe “Switch on the light in the bathroom”. Snips processes the input and then delivers a MQTT message to a given topic (here “hermes/intent/kristianraue:OnOff”).

In the JSON payload of the messages you find the name of the intent (here: kristianraue:OnOff”) and the values for the slots of the intent (Slot 0: “on” or “off”, Slot 1: “bathroom”, “bedroom”, “kitchen”, etc).

You can then build a Streamsheet that subscribes to the given topic and reads the JSON payload of the incoming messages. If you link the JSON fields slots.0.rawValue and slots.1.rawValue to cells in the Streamsheets via Drag-and-Drop, you can build some senseful spreadsheet logic based on theses values. This is shown in the following screenshot (which is in formula view).

<img src="{{page.image_url1}" width="100%" height="auto">

Everytime a message arrives, the Streamsheet will publish data to two topics simultaneously. In cell B19 the Streamsheet publishes the payload in cell A12:B13 as JSON to the topic “dialogueManager/endSession”. This very handy MQTT command ends the Snips session and sends the given voice output to the speakers of the Raspi, telling the user what action has been executed.

The second MQTT message is published to the topic where Shelly is listening. As explained in the beginning, Shelly is subscribed to a MQTT topic (here: “shellies/shelly1-BA01F8/relay/0/command”) and waits for text payloads of “on” or “off” to switch on and off the light.

Note: In this demo were are not making use of the slot 1 value, instead we are always switch on and off the same Shelly device. But of course you could easily extend the Streamsheet to use a VLOOKUP() function to look up the corresponding Shelly device name for each room and then change the topic for Shelly respectively.


### Video: Connecting Snips, Shelly and Streamsheets via MQTT

<div class="iframe-container">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/b60ZLrHoCOo" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div> 
