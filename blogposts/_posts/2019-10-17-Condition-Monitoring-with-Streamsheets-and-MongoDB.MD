---
layout: blogposts
title: "Condition Monitoring with Streamsheets and MongoDB"
date: 2019-10-17
image_url: "/assets/images/blogposts/condition-monitoring-with-streamsheets-and-mongoDB-picture.png"
---
This blog post introduces the basic operation of Streamsheets. Using the example of a smart WiFi switch with an integrated power consumption meter (Shelly 2.5), we set up a complete Streamsheet use case within 10 minutes.

<img src="{{page.image_url}}" width="100%" height="auto">

Streamsheets are a great tool to visualize and analyse real-time data that comes from event streaming platforms like MQTT or Kafka. In a previous post we showed how you can create real-time dashboards to display the current data of now (or just a few seconds or minutes ago).

But how do you persistently store your data or your analysis results for a longer time using Streamsheets ? In the following video I demonstrate how you can feed a database like MongoDB with data from Streamsheets, just using one easy-to-use function called MONGO.STORE().

Once the data is send to MongoDB, it is not only permanently saved, it can of course also be queried in any way using Streamsheets (which we will show in a future post) or any other query tool that supports MongoDB.

The following video is also the first video of a new and more professional presentation format that I call “Streamsheet TV”. I suggest that you view this video in full screen mode.


### Video: Production Monitoring with Streamsheets, MQTT and MongoDB

<div class="iframe-container">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/xtxOWX2YCQg" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div> 