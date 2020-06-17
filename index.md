---
layout: default
---

<section id="banner" class="banner" role="banner">
    {% include _nav.html %}
    <!-- sectiinclude needed here because nav is always in first container :-(  -->
    <div class="container-fluid">
        <div class="row flex-start" class="align-items: flex-start;">
            <div class="col-md-12">
                <div class="banner-spacer">
                    <p>&nbsp;</p>
                </div><!-- banner text -->
            </div>
            <div class="col-lg-7 col-lg-offset-1 col-md-7 col-md-offset-1 col-sm-7 col-sm-offset-1 col-xs-12">
                <div class="banner-text text-center">
                    <h1>Stream processing for everybody</h1>
                    <p><b> Eclipse Streamsheets</b> - Anybody who knows how to use a spreadsheet can quickly build server-based, real-time applications, for any purpose. No programming required.</p>
                    <p><b>Eclipse Mosquitto</b> -  Devices and apps communicate in real-time, based the most popular broker technology in the world.</p>
                    <p>
                        <a href="#" class="js-video-button btn btn-large" data-video-id='cYKJe4FtUFg'>Watch Video</a>
                        <a href="#products" class="btn btn-large">Cedalo Cloud</a>
                        <a href="#download" class="btn btn-large">Download</a>
                    </p>
                </div><!-- banner text -->
            </div>
            <div class="col-lg-3 col-lg-offset-1 col-md-3 col-md-offset-1 col-sm-3 col-sm-offset-1 col-xs-12">
                <div class="banner-chart text-center">
                    <img  src="images/screenshot_orig.png" alt="">
                </div><!-- banner text -->
            </div>
        </div>
    </div>
</section><!-- banner -->
<section id="products" class="products section">
    <div class="container-fluid" style="padding-left: 40px;padding-right: 40px;">
        <div class="row no-padding">
            <div class="col-lg-12 col-md-12 col-sm-12 products-intro">  
                <div>
                    <h1 class="section-header">The democratization of stream processing solutions</h1>
                </div>
            </div>
            <div class="col-lg-6 col-md-6 col-sm-12 col-xs-12">  
                <div class="products-box">
                    <h2>Eclipse Streamsheets</h2>
                    <p>Our no-code user interface is the all-familiar spreadsheet. But that’s all what Streamsheets have in common with traditional spreadsheets.</p>
                    <p>While spreadsheets are client apps which work with bound and de-coupled batches of data, Streamsheets continuously process, aggregate, visualize and transform unbound data streams in real-time as a server app (microservice).</p>
                    <p>Streamsheets were designed with publish/subcribe streaming protocols like MQTT, Apache Kafka or AMQP in mind, but they also work perfectly with REST-based protocols (request/response)</p>
                    <p class="text-center">
                        <a href="#banner" class="btn btn-large">Watch Video</a>
                        <a href="#blog" class="btn btn-large">Learn More</a>
                    </p>
                </div>
                <div class="products-box">
                    <h2>Eclipse Mosquitto</h2>
                    <p>Eclipse Mosquitto is the most popular MQTT broker in the world and the perfect streaming platform for Streamsheets. Mosquitto supports unlimited hierarchical topics and the highly flexible publish/subscribe communication pattern.</p> 
                    <p>With the Mosquitto broker you can connect sensors, devices and apps far more flexible than in the request/response communication pattern of traditional client/server architectures.</p>
                    <p>Eclipse Mosquitto supports guaranteed delivery of messages which allows use cases not only in IoT and Smart Factory, but also in financial and other non-IoT applications.</p>
                    <p class="text-center">
                        <a href="#banner" class="btn btn-large">Watch Video</a>
                        <a href="#blog" class="btn btn-large">Learn More</a>
                    </p>
                </div>
            </div>
            <div class="col-lg-6 col-md-6 col-sm-12 col-xs-12 text-center">
                <div class="products-chart" >
                    <img  src="images/overview.png">
                </div>
            </div>
        </div>
    </div>
</section>

<section id="features" class="features section">
    <div class="container-flex" style="padding-left: 40px;padding-right: 40px;">
        <div class="row">
            <div class="col-md-4 col-sm-6 feature text-center">
                <div class="feature-content">
                    <span class="icon icon-bargraph"></span>
                    <h3>Powerful<br />Dashboards</h3>
                    <p>We include extensive charting features including custom charts that update immediately with real-time data. No need to install third-party chart extensions. Have a look at the charts gallery.</p>
                </div>
            </div>
            <div class="col-md-4 col-sm-6 feature text-center">
                <div class="feature-content">
                    <span class="icon icon-refresh"></span>
                    <h3>On-Event<br />or Cyclic</h3>
                    <p>Streamsheets calculate their formulas on each incoming stream event or based on a cycle timer. You can set the cycle timer to control how often a Sheet receives, processes and sends data.</p>
                </div>
            </div>
            <div class="col-md-4 col-sm-6 feature text-center">
                <div class="feature-content">
                    <span class="icon icon-speedometer"></span>
                    <h3>Milliseconds<br />Automation</h3>
                    <p>Real-time event streams from technical or financial applications can have a very high frequencies. Streamsheets are able to run 1000 up to cycles per second to guarantee precise results.</p>
                </div>
            </div>
            <div class="col-md-4 col-sm-6 feature text-center">
                <div class="feature-content">
                    <span class="icon icon-browser"></span>
                    <h3>Server-based<br />24/7 - non-stop</h3>
                    <p>Streamsheets run on their own, even if you close the browser window. They run as microservices, 24 hours a day, receiving data from multiple sources, transforming it, and sending it out again.</p>
                </div>
            </div>
            <div class="col-md-4 col-sm-6 feature text-center">
                <div class="feature-content">
                    <span class="icon icon-streetsign"></span>
                    <h3>Open-Source<br /> & Premium</h3>
                    <p>Both Mosquitto and Streamsheets are Eclipse IoT open-source projects which are commercially sponsored by Cedalo. We also offer premium editions of both products named Cedalo Sheets and Cedalo Broker.</p>
                </div>
            </div>
             <div class="col-md-4 col-sm-6 feature text-center">
                <div class="feature-content">
                    <span class="icon icon-download"></span>
                    <h3>On-Premises<br />& Cloud</h3>
                    <p>Our products run  as managed service in the Cedalo Cloud, on your AWS or Azure account or on-premises under any major operating system. They even run on edge devices with weak CPUs or on the Raspberry Pi.</p>
                </div>
            </div>
        </div>
    </div>
</section><!-- features -->

<section id="usecases" class="usecases section" >
    <div class="container-fluid">
        <div class="row">
            <div class="col-lg-12 col-md-12 col-sm-12 usecase-intro">  
                <div>
                    <h1 class="section-header">Use Cedalo Sheets to build solutions for wide variety of use cases</h1>
                </div>
            </div>
            <div class="col-lg-4 col-md-6 col-sm-6 usecase">  
                <div class="usecase-box">
                    <div class="overlay-caption">
                        <h2>Smart Factory & IIoT</h2>
                        <h5>Automotive, Energy, Aerospace</h5>
                    </div>
                    <div class="usecase-body">
                        <p>With Cedalo Sheets, anybody who knows how to use a spreadsheet can quickly build real-time, stream processing applications, for any purpose.</p>
                        <ul>
                        <li>Dashboards and Stream Charting</li>
                        <li>Condition Monitoring and Alerts</li>
                        <li>Analytics, Visualization, Digital Twin</li>
                        <li>Protocol conversion (OPC UA ↔ MQTT ↔ KAFKA)</li>
                        </ul>
                    </div>
                </div>
            </div>
            <div class="col-lg-4 col-md-6 col-sm-6 usecase">  
                <div class="usecase-box">
                    <div class="overlay-caption">
                        <h2>Financial Services</h2>
                        <h5>Banking, Payments, Securities</h5>
                    </div>
                    <div class="usecase-body">
                        <p>With Cedalo Sheets, anybody who knows how to use a spreadsheet can quickly build real-time, stream processing applications, for any purpose.</p>
                        <ul>
                        <li>Real-time Analytics</li>
                        <li>Fraud Detection</li>
                        <li>Regulatory compliance</li>
                        <li>Customer tracking </li>
                        </ul>
                    </div>
                </div>
            </div>
            <div class="col-lg-4 col-md-6 col-sm-6 usecase">  
                <div class="usecase-box">
                    <div class="overlay-caption">
                        <h2>Medical Services</h2>
                        <h5>Healthcare, Clinics, Pharmaceutical </h5>
                    </div>
                    <div class="usecase-body">
                        <p>With Cedalo Sheets, anybody who knows how to use a spreadsheet can quickly build real-time, stream processing applications, for any purpose.</p>
                        <ul>
                        <li>Dashboards and Stream Charting</li>
                        <li>Condition Monitoring and Alerts</li>
                        <li>Analytics, Visualization, Digital Twin</li>
                        <li>Protocol conversion (OPC UA ↔ MQTT ↔ KAFKA)</li>
                        </ul>
                    </div>
                </div>
            </div>
            <div class="col-lg-4 col-md-6 col-sm-6 usecase">  
                <div class="usecase-box">
                    <div class="overlay-caption">
                        <h2>Smart Grids & Logistics</h2>
                        <h5>Oil & Gas, Electric Power, Transportation</h5>
                    </div>
                    <div class="usecase-body">
                       <p>With Cedalo Sheets, anybody who knows how to use a spreadsheet can quickly build real-time, stream processing applications, for any purpose.</p>
                        <ul>
                        <li>Dashboards and Stream Charting</li>
                        <li>Condition Monitoring and Alerts</li>
                        <li>Analytics, Visualization, Digital Twin</li>
                        <li>Protocol conversion (OPC UA ↔ MQTT ↔ KAFKA)</li>
                        </ul>
                    </div>
                </div>
            </div>
            <div class="col-lg-4 col-md-6 col-sm-6 usecase">  
                <div class="usecase-box">
                    <div class="overlay-caption">
                        <h2>Stream Charts</h2>
                        <h5>Streaming data everywhere.</h5>
                    </div>
                    <div class="usecase-body">
                        <p>With Cedalo Sheets, anybody who knows how to use a spreadsheet can quickly build real-time, stream processing applications, for any purpose.</p>
                        <ul>
                        <li>Dashboards and Stream Charting</li>
                        <li>Condition Monitoring and Alerts</li>
                        <li>Analytics, Visualization, Digital Twin</li>
                        <li>Protocol conversion (OPC UA ↔ MQTT ↔ KAFKA)</li>
                        </ul>
                    </div>
                </div>
            </div>
            <div class="col-lg-4 col-md-6 col-sm-6 usecase">  
                <div class="usecase-box">
                    <div class="overlay-caption">
                        <h2>Stream Gateways</h2>
                        <h5>Streaming data everywhere.</h5>
                    </div>
                    <div class="usecase-body">
                        <p>With Cedalo Sheets, anybody who knows how to use a spreadsheet can quickly build real-time, stream processing applications, for any purpose.</p>
                        <ul>
                        <li>Dashboards and Stream Charting</li>
                        <li>Condition Monitoring and Alerts</li>
                        <li>Analytics, Visualization, Digital Twin</li>
                        <li>Protocol conversion (OPC UA ↔ MQTT ↔ KAFKA)</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </div>
</section><!-- usecase -->

<section id="download" class="section downloads">
    <div class="container-flex" style="padding-left: 40px;padding-right: 40px;">
        <div class="row">
            <div class="col-md-12 col-sm-12 download">
                <div class="download-intro">
                    <h1 class="section-header">Get Started! Open-Source or Premium.</h1>
                    <p>In addition to sponsoring the two Open-Source projects "Eclipse Streamsheets" and "Eclipse Mosquitto" Cedalo also offers premium editions of both products. They are called "Cedalo Sheets" and "Cedalo Broker". Try the Cedalo premium edition free for 14 days.</p>
                </div>
            </div>
            <div class="col-md-4 col-sm-6 download text-center" >
                <span class="icon icon icon-cloud"></span>
                <div class="download-content">
                    <h2>Managed Service</h2>
                    <p>Cras justo odio, dapibus ac facilisis in, egestas eget quam. Nullam quis risus eget urna mollis ornare vel eu leo. Donec ullamcorper nulla non metus auctor fringilla.</p>
                    <p><a href="#cloud" class="btn btn-large">Cedalo Cloud</a></p>
                </div>
            </div>
            <div class="col-md-4 col-sm-6 download text-center">
                <span class="icon icon-desktop"></span>
                <div class="download-content">
                    <h2>On-Premises</h2>
                    <p>Cras justo odio, dapibus ac facilisis in, egestas eget quam. Nullam quis risus eget urna mollis ornare vel eu leo. Donec ullamcorper nulla non metus auctor fringilla.</p>
                    <p><a href="#cloud" class="btn btn-large">Download</a></p>
                </div>
            </div>
            <div class="col-md-4 col-sm-6 download text-center">
                <span class="icon icon-gears"></span>
                <div class="download-content">
                    <h2>Edge Devices</h2>
                    <p>Cras justo odio, dapibus ac facilisis in, egestas eget quam. Nullam quis risus eget urna mollis ornare vel eu leo. Donec ullamcorper nulla non metus auctor fringilla.</p>
                    <p><a href="#cloud" class="btn btn-large">Download</a></p>
                </div>
            </div>
        </div>
    </div>
</section><!-- download -->

<section id="blog" class="section teams">
    <div class="container">
        <div class="row">
            <div class="col-md-12 col-sm-12">
                <div class="person-intro">
                    <h1 class="section-header">Visit our blog for more use cases</h1>
                    <p>In addition to sponsoring the two Open-Source projects "Eclipse Streamsheets" and "Eclipse Mosquitto" Cedalo also offers premium editions of both products. They are called "Cedalo Sheets" and "Cedalo Broker" and you can try them free for 14 days.</p>
                </div>
            </div>
            <div class="col-md-3 col-sm-6">
                <div class="person">
                    <img src="images/team-1.jpg" alt="" class="img-responsive">
                    <div class="person-content">
                        <h4>Ruth Wood</h4>
                        <h5 class="role">Founder, CEO</h5>
                        <p>Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Maecenas sed diam eget risus varius blandit sit amet non magna. Nullam quis risus eget urna mollis ornare vel eu leo.</p>
                    </div>
                </div><!-- person -->
            </div>
            <div class="col-md-3 col-sm-6">
                <div class="person">
                    <img src="images/team-2.jpg" alt="" class="img-responsive">
                    <div class="person-content">
                        <h4>Timothy Reed</h4>
                        <h5 class="role">Co-Founder, Developer</h5>
                        <p>Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Maecenas sed diam eget risus varius blandit sit amet non magna. Nullam quis risus eget urna mollis ornare vel eu leo.</p>
                    </div>
                </div><!-- person -->
            </div>
            <div class="col-md-3 col-sm-6">
                <div class="person">
                    <img src="images/team-3.jpg" alt="" class="img-responsive">
                    <div class="person-content">
                        <h4>Victoria Valdez</h4>
                        <h5 class="role">UI Designer</h5>
                        <p>Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Maecenas sed diam eget risus varius blandit sit amet non magna. Nullam quis risus eget urna mollis ornare vel eu leo.</p>
                    </div>
                </div><!-- person -->
            </div>
            <div class="col-md-3 col-sm-6">
                <div class="person">
                    <img src="images/team-4.jpg" alt="" class="img-responsive">
                    <div class="person-content">
                        <h4>Beverly Little</h4>
                        <h5 class="role">Data Scientist</h5>
                        <p>Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Maecenas sed diam eget risus varius blandit sit amet non magna. Nullam quis risus eget urna mollis ornare vel eu leo.</p>
                    </div>
                </div><!-- person -->
            </div>
        </div>
    </div>
</section><!-- blog -->

