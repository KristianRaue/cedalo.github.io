---
layout: blogposts
title: "Shopify Dashboarding (Part 1): Build a Shopify-to-Kafka Gateway"
date: 2020-05-17
image_url: "/assets/images/blogposts/streamsheets-shopify-kafka2.png"
---

In this video post you learn how you can build a cloud-based Streamsheet that serves as a gateway between Shopify webhooks (executed by a Shopify Online Store) and Apache Kafka (hosted on Confluent Cloud).

In my previous blog posts I concentrated on IoT examples and using MQTT as a message broker. In this and in the following post I will demonstrate that the scope of Streamsheets goes far beyond this. I will show a use case with two Streamsheets. One Streamsheets runs in the cloud and connects a Shopify online store with a Apache Kafka in the cloud. 

The second Streamsheet runs locally behind the firewall and will provide a real time sales dashboard, consuming the data from the Kafka Cluster. The following slide shows the setup of this use case.

<img src="{{page.image_url}}" width="100%" height="auto">

I split the whole use case in two blog posts (and 2 videos respectively). In this post I talk about the first Streamsheet that runs in the cloud and connects a Shopify online store with the Apache Kafka Cluster in the Confluent Cloud. In the the second post you will see the Streamsheet which runs locally behind the firewall and provides a real time sales dashboard, consuming the data from the Kafka Cluster.

I recommended to watch the following video in full screen mode. The video is 12 minutes long. 

### Video: Build a Shopify-to-Kafka Gateway with Streamsheets

<div class="iframe-container">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/3BeZI898z6k" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div> 