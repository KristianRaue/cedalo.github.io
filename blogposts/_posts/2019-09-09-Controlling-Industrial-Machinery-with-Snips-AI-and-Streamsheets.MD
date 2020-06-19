---
layout: blogposts
title: "Controlling Industrial Machinery with Snips AI and Streamsheets"
date: 2019-09-09
image_url: "/assets/images/blogposts/snips_ai_and_streamsheets.jpg"
---

In this post I will integrate an artificial intelligence based technology named Snips to control a sorting process in real-time.

In my previous post I showed how to connect industrial machinery to Streamsheets over MQTT, analyze and visualize its data as well as control it. If you haven’t read that post yet you might consider having a look at it first.

Snips is able to receive and process voice commands without having to go through the cloud while processing the input. Snips runs locally (for example on a Raspberry Pi) and all the artificial intelligence happens locally on-premises. Another nice thing about Snips is its ability to directly share its data through MQTT which makes it a perfect companion for Streamsheets.

It is recommended that you watch the following video in full screen mode.

### Video: Controlling Machinery with MQTT, Streamsheets and Snips AI

<div class="iframe-container">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/Po2UR_7nFD0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

In the video its shown how a Snips intent is defined and how it is connected to a MQTT topic. Then a 2nd Streamsheet is created und subscribed to the topic. Whenever a new voice command is received, the second Streamsheet (on the right) will run and lookup the part code of the specified part (using a standard VLOOKUP() function and will then supply this part code to the 1st Streamsheet (on the right) along with the specified pusher assignment. The Streamsheet on the left is using external cell references to get the values from the Streamsheet on the right.

Hint: The IF column at the right side of the 1st Streamsheet controls whether the corresponding row is calculated or not. If the formula in the IF column evaluates to TRUE the row is calculated, otherwise not. Since the 1st Streamsheet is continuously recalculating it will get the values from the 2nd Streamsheets within milliseconds.

In addition to specifying a pusher the voice commands can also “free” the pushers from a specified part assignment by using the word “nothing” as part code.

In a future blog post we will show a video on how to build a real-time condition monitoring app for this use case. Stay tuned. 