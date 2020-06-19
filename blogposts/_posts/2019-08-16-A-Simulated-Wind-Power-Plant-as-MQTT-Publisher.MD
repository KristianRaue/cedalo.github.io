---
layout: blogposts
title: "A Simulated Wind Power Plant as MQTT Publisher"
date: 2019-08-16
image_url: "/assets/images/blogposts/windmill.png"
---

Have you ever wondered how to simulate data for your individual use cases quickly?

In the following 8 minute video you can see how to set up a Streamsheet that simulates a wind mill power plant and and publishes its data in real-time to a MQTT broker.

<img src="{{page.image_url}}" width="100%" height="auto">

There is not input stream for this Streamsheet. Instead the Streamsheet uses the continuous calculation mode and random number functions to simulate varying wind speeds and gusts.

In the second half of the video it is shown how you can animate the wind mill by dynamically linking drawing objects with the output cells of the Streamsheet.

### Video: A sumulated Wind Mill Power Plant as MQTT Publisher

<div class="iframe-container">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/jKSTfNGPv18" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

In a later post, I will show how you can use the MQTT stream of this Streamsheet as an input source for a digital twin and an energy dashboard , both implemented via Streamsheets. 
