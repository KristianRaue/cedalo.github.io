---
layout: blogposts
title: "Connecting Streamsheets to Industrial Machinery via MQTT"
date: 2019-09-09
image_url: "/assets/images/blogposts/industrial-machinery-image.png"
image_url1: "/assets/images/blogposts/mqtt-bridge.png"
image_url2: "/assets/images/blogposts/factoryio_analytics (1).png"
---

In this blog you find a 4 minute video that shows how to control an industrial machinery that sorts incoming parts according to their color and shape.

Streamsheets are suitable for many use cases in industrial environments (e.g. Smart Factory, Industrie 4.0, Industrial IoT). To connect the machinery and the Streamsheet server a MQTT Broker (www.mosquitto.org) is used.

In order to visualize the machinery I have installed a factory simulation program called FactoryIO (www.factoryio.com). This easy-to-use program allows to build virtual industrial machinery in a 3D environment including sensors and actuators that operate in real-time.

<img src="{{page.image_url}}" width="100%" height="auto">

To make FactoryIO compatible with MQTT I am using a special gateway for FactoryIO that Cedalo has developed. It converts the internal memory map of FactoryIO into a simple JSON payload and publishes the payload on a MQTT broker at a high-speed frequency.


<img src="{{page.image_url1}}" width="100%" height="auto">

At the same time the MQTT gateway is also able to subscribe to a MQTT topic and receive JSON based payloads to control the actuators (e.g. Pusher 1 to 4) on the machinery.

In the following video you can see how the Streamsheet is build from the ground up. It is very much recommended that you view the video in full screen mode.

### Video: Controlling Industrial Machinery with Streamsheets and MQTT


<div class="iframe-container">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/1DNqw0Js1Ks" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

The Streamsheet works in a cyclic mode that recalculates the formulas every 20 ms. In the first part of the video the sensor status of Sensor 1 to 4 is linked with the corresponding Streamsheet cells.

To synchronize all actions timewise the Streamsheet uses a function called EDGE.DETECT(). This function determines whether a certain condition is true and is then able to hold and delay the signal for a given number of milliseconds. This makes sure that the pusher is activated at the right moment.

In the next part of this use case I will show how to integrate some AI capabilities in this scenario. A locally installed voice recognition system (Snips, see http://www.snips.ai) will then allow the user to voice control which belt will pick which parts.

In another blog post for this use case I show an analytic dashboard of the sorter station with charts and statistical functionality. In the following screenshot you can see a short preview of this analytic dashboard. Follow this link to see how I created the dashboard.

<img src="{{page.image_url2}}" width="100%" height="auto"> 
