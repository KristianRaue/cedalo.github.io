---
layout: blogposts
title: "Analytics, Dashboards and Predictive Maintenance with Streamsheets"
date: 2019-09-11
image_url: "/assets/images/blogposts/factoryio_analytics.png"
---
Find out how to build a dynamic dashboard that analyzes and visualizes data in realtime.

In a previous blog posts I demonstrated how to set up a Streamsheet that controls a industrial machinery. I you haven’t read this previous post you might consider reading it before continuing with this new post.

In this blog post I will extend the Streamsheet application to serve as an analytical dashboard for the industrial machinery introduced in the previous blog post. The following screenshot gives a quick graphical impression of the dashboard.

<img src="{{page.image_url}}" width="100%" height="auto">

The dashboard continuously reads the current position of the pushers to find out if all 4 pushers are extending the full way or if they stop earlier. If they average value of the pusher extensions gets below the standard value of (in this case) 10, some maintenance is needed for this machinery.

The dashboard uses time charts to show the pusher signal and the actual position of the pusher in real-time. It also shows the history of the readings in a table view.

In the following 5 minute video I will show how to build the dashboard. I suggest that you view this video in full screen mode.

### Video: Analyzing the accuracy of a industrial process with Streamsheets

<div class="iframe-container">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/xQPmsTYvpes" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>
 