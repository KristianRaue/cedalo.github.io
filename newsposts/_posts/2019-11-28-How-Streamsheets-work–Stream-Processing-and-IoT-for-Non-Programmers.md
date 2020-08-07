---
layout: newsposts
title: "How Streamsheets work"
date: 2019-11-28
image_url: "/assets/images/blogposts/blog_shelly_introduction.png"
excerpt: "sjkldj klasj lkasjd askljd aslkdj aslkd kldfjasl djaslk jslkfj lskfa ldj ask sakldj asdj asdjl las dad sadas"
---

This blog post introduces the basic operation of Streamsheets. Using the example of a smart WiFi switch with an integrated power consumption meter (Shelly 2.5), we set up a complete Streamsheet use case within 10 minutes.

<img src="{{page.image_url}}" width="100%" height="auto">

This post contains 3 video sessions:

In the first video just below you see how the data connection is established and how the necessary spreadsheet formulas and charts are created. This includes an energy monitoring and an automatic shutdown if the energy consumption or operating temperature is too high. In addition, the first video shows how to set up the Streamsheet to automatically send emails in the event of an alarm and how to make entries in a log database (here MongoDB).

The second video extends the demo to show how you can created visual representations of the device status directly in the Streamsheets. This is done simply by dynamically linking the attributes of graphical objects with the contents of Streamsheet cells (cells, which then in turn are linked to the JSON data from the MQTT messages)

In the third video we confess, that we actually did not use the MQTT connectivity of the Shelly 2.5 device. Instead we used the REST API which delivers very complete JSON payloads. This gave us another use case, namely to show how easy it is to use a Streamsheet to build a highly flexible REST-to-MQTT Gateway just using spreadsheet formulas.

I recommended to watch the following video in full screen mode. The video is 10 minutes long, but the first 5 minutes are enough to understand the basic principle of Streamsheets.


### Video: Introduction to Streamsheets (Main Video)

<div class="iframe-container">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/Y_7Irtc-d08" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

 