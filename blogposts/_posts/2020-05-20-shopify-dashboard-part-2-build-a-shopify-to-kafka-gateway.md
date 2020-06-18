---
layout: blogposts
title: "Shopify Dashboard (Part 2): How to aggregate and chart Kafka data in Streamsheets"
date: 2020-05-20
---

In this video post you see how you can build a Streamsheet that receives data from Shopify via Apache Kafka The resulting Streamsheet generates aggregations and charts to serve as a real-time dashboard for a Shopify online shop.
This is the second part of the Shopify/Kafka/Streamsheet use case. In the first part we built a cloud based gateway to connect a Shopify store to Apache Kafka (hosted on the Confluent Cloud). In this second part we build a Streamsheet on a second Streamsheet Server that subscribes to the Kafka cluster and displays the real time data from Shopify in a dashboard. 

This second Streamsheet Server runs on-premise behind the local firewall. Since the Kafka connection is initiated from the local Streamsheet Server, it can easily receive the event driven data from the Kafka cluster in the cloud. This is one of the beauties of the broker concept behind Kafka. 

The following slide shows the setup of this use case.

![Shopify Kafka Streamsheet](assets/images/blogposts/streamsheets-shopify-kafka.png)

In the video you will see how to aggregate and chart the data from the Kafka cluster that we used in the previous post. In the video I demonstrate 2 different ways on how to store the aggregated data. First I simply use Streamsheet cells to store the aggregated data. This will work if you only need the data persisted for a limited time (for example the last 300 sales). At the end of the video I show an alternative way using MongoDB. This allows to store the aggregated data persistently over long periods of time. And it also allows to retrieve the data from other applications. This could be another Streamsheet or even a 3rd party application build with another programming framework.

I recommended to watch the following video in full screen mode. The video is about 12 minutes long. 

# First Video: Build a Shopify-to-Kafka Gateway with Streamsheets

<iframe  allowfullscreen title="youtube Video Player"  data-src="https://www.youtube.com/embed/-pzir2aWcF8?feature=oembed&amp;start&amp;end&amp;wmode=opaque&amp;loop=0&amp;controls=1&amp;mute=0&amp;rel=0&amp;modestbranding=0" class="elementor-video-iframe lazyload" src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw=="></iframe>