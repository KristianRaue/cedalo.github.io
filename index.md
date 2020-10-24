---
layout: default
---

<section id="intro" class="banner" role="banner">
    <div class="container-fluid">
        <div class="row flex-start banner-sides">
            <div class="col-lg-12 col-md-12 col-sm-12 col-xs-12">
                 <div class="banner-text">
                    <h1 class="text-center">Real Time Spreadsheet and Broker<br />for IoT and Stream Processing</h1>
                    <div class="col-lg-6 col-md-6  col-sm-6 col-xs-12 banner-list">
                        <ul class="text-left"><b>Eclipse Streamsheets:</b>
                            <li>Dashboards and Visualizations in Real-Time</li>
                            <li>Continuous Analysis and Processing of Data</li>
                            <li>Monitoring, Alerting and Automation</li>
                            <li>Semantic Mappings between Protocols</li>
                        </ul>
                    </div>
                    <div class="col-lg-6 col-md-6  col-sm-6 col-xs-12 banner-list">
                        <ul class="text-left"><b>Eclipse Mosquitto:</b>
                            <li>The world's fastest<sup>1</sup> and most popular MQTT Broker</li>
                            <li>Apps and Devices connected in Real-Time</li>
                            <li>Secure and Firewall friendly</li>
                            <li>Support for MQTT Version 3.1.1 and 5.0</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
        <div class="row flex-start">
            <div class="col-lg-12 col-md-12 col-sm-12 col-xs-12">
                <p class="text-center">
                    <a href="#" class="js-video-button btn btn-large" data-video-id='cYKJe4FtUFg'>Watch Video</a>
                    <a href="#products" class="btn btn-large">Learn more</a>
                    <a href="#download" class="btn btn-large">Get Started</a>
                    <a href="https://eepurl.com/glV72D" class="btn btn-large">Newsletter</a>
                </p>                
            </div>
        </div>
    </div>
</section><!-- banner -->

<section id="news" class="section news" style="padding-top:0px;padding-bottom:0px;">
    <div class="container-fluid fluid-padding">
        <div class="row">
            <div class="col-md-12 col-sm-12 news_sing">
                <hr>
                <div class="col-md-6 col-sm-6 col-xs-6">
                    <h2><b>News</b></h2>
                </div>
                <div class="col-md-6 col-sm-6 col-xs-6 text-right">
                    <a href="all_news.html" class="btn btn-large">Show All News</a>
                </div>
            </div>
        </div>
        <div class="row">
            <div class="col-md-12 col-sm-12 news_sing">
             {% for post in site.categories["newsposts"] %}
                <!--
                {% increment my_news %}
                -->
                <div class="col-lg-3 col-md-4 col-sm-6 col-xs-12 news_sing text-center">
                    <div class="news-content">
                        <a href="{{post.url}}"><img src="{{ post.image_url }}" alt="" style="width:100%;height:auto;"></a>
                        <div>
                            <h4><b><a href="{{post.url}}">{{post.title}}</a></b></h4>    
                            <p>{{post.excerpt}}</p>
                        </div>
                    </div>
                </div>
                {% if my_news == 4 %}
                    {% break %}
                {% endif %}
            {% endfor %}
            </div>
        </div>
    </div>
</section><!-- news -->

<section id="products" class="products section">
    <div class="container-fluid fluid-padding" style="padding-top:20px;">
        <div class="row no-padding">
            <div class="col-lg-6 col-md-6 col-sm-12 col-xs-12">  
                <div class="products-box">
                    <h1>Eclipse Streamsheets</h1>
                    <h4>The perfect companion for Mosquitto</h4>
                    <p>Our no-code user interface is the all-familiar spreadsheet. But that’s all what Streamsheets have in common with traditional spreadsheets.</p>
                    <p>While spreadsheets are client apps which work with bound and de-coupled batches of data, Streamsheets continuously process, aggregate, visualize and transform unbound data streams in real-time as a server app (microservice).</p>
                    <p>Streamsheets were designed with publish/subcribe streaming protocols like MQTT, Apache Kafka or AMQP in mind, but they also work perfectly with REST-based protocols (request/response)</p>
                    <p class="text-center">
                        <a href="#" class="js-video-button btn btn-large" data-video-id='cYKJe4FtUFg'>Watch Video</a>
                        <a href="#features" class="btn btn-large">Learn More</a>
                    </p>
                </div>
                <div class="products-box">
                    <h1>Eclipse Mosquitto</h1>
                    <h4>Edge & Cloud: Streaming data everywhere</h4>
                    <p>Eclipse Mosquitto is the most popular MQTT broker in the world and the perfect streaming platform for Streamsheets. Mosquitto supports unlimited hierarchical topics and the highly flexible publish/subscribe communication pattern.</p> 
                    <p>With the Mosquitto broker you can connect sensors, devices and apps far more flexible than in the request/response communication pattern of traditional client/server architectures.</p>
                    <p>Eclipse Mosquitto supports guaranteed delivery of messages which allows use cases not only in IoT and Smart Factory, but also in financial and other non-IoT applications.</p>
                    <p class="text-center">
                        <a href="#" class="js-video-button btn btn-large" data-video-id='cYKJe4FtUFg'>Watch Video</a>
                        <a href="#features" class="btn btn-large">Learn More</a>
                    </p>
                </div>
            </div>
            <div class="col-lg-6 col-md-6 col-sm-12 col-xs-12 text-center">
                <div class="products-chart" >
                    <img  src="https://cedalo.com/images/overview.png">
                </div>
            </div>
        </div>
    </div>
</section>

<section id="features" class="features section">
    <div class="container" >
        <div class="row">
            <div class="col-md-4 col-sm-6 feature text-center">
                <div class="feature-content">
                    <span class="icon icon-bargraph"></span>
                    <h3>Powerful<br />Charts</h3>
                    <p>We include extensive charting features including custom and time-series charts that update with real-time data. No need to install third-party chart extensions. Have a look at our <a href="#chartgallery">chart gallery.</a></p>
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
                    <p>Real-time event streams from technical or financial applications can have a very high frequencies. Streamsheets are able to run up to 1000 cycles per second to guarantee precise operations.</p>
                </div>
            </div>
            <div class="col-md-4 col-sm-6 feature text-center">
                <div class="feature-content">
                    <span class="icon icon-browser"></span>
                    <h3>Server-based<br />24/7 Operations</h3>
                    <p>Streamsheets run on their own, even if you close the browser window. They run as microservices, 24 hours a day, receiving data from multiple sources, transforming it, and sending it out again.</p>
                </div>
            </div>
            <div class="col-md-4 col-sm-6 feature text-center">
                <div class="feature-content">
                    <span class="icon icon-streetsign"></span>
                    <h3>Open-Source<br /> & Premium</h3>
                    <p>Both Mosquitto and Streamsheets are Eclipse IoT open-source projects which are commercially sponsored by Cedalo. We also offer premium editions of the products under the name "Cedalo Premium Platform"</p>
                </div>
            </div>
             <div class="col-md-4 col-sm-6 feature text-center">
                <div class="feature-content">
                    <span class="icon icon-download"></span>
                    <h3>On-Premises<br />& Cloud</h3>
                    <p>Our products run as managed service in the Cedalo Cloud, on your AWS or Azure account or on-premises under any major operating system. They even run on edge devices with weak CPUs or on the Raspberry Pi.</p>
                </div>
            </div>
        </div>
    </div>
</section><!-- features -->

<section id="usecases" class="usecases section" >
    <div class="container-fluid fluid-padding">
        <div class="row">
            <div class="col-lg-12 col-md-12 col-sm-12 usecase-intro">  
                <div>
                    <h1 class="section-header">How our Customers use Streamsheets & Mosquitto</h1>
                </div>
            </div>
            <div class="col-lg-4 col-md-6 col-sm-6 usecase">  
                <div class="usecase-box">
                    <div class="overlay-caption">
                        <h2>Smart Factory</h2>
                        <h5>Automotive, Energy, Aerospace</h5>
                    </div>
                    <div class="usecase-body">
                        <p>Streamsheets precisely monitor and analyse industrial processes. Build your individual IIoT applications interactively while the data flows in.</p>
                        <ul>
                        <li>Dashboards and Charting</li>
                        <li>Condition Monitoring</li>
                        <li>Analytics, Digital Twin</li>
                        <li>Gateways for OPCUA/MQTT/KAFKA</li>
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
                        <p>Analyze financial transactions in real-time. Aggregate, compare, detect anomalies and send alerts in real-time when conditions are met.</p>
                        <ul>
                        <li>Fraud Detection</li>
                        <li>Real-time Analytics</li>
                        <li>Regulatory Compliance</li>
                        <li>Customer Tracking </li>
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
                        <p>Real-time information is crucial for efficient treatment. Combine data from medical sub-systems and create event-driven dashboards & processes.</p>
                        <ul>
                        <li>Real-Time Infection Control</li>
                        <li>Utilization Monitoring</li>
                        <li>Real-Time Asset Tracking</li>
                        <li>Gateways for MQTT/FHIR/KAFKA</li>                        
                        </ul>
                    </div>
                </div>
            </div>
             <div class="col-lg-4 col-md-6 col-sm-6 usecase">  
                <div class="usecase-box">
                    <div class="overlay-caption">
                        <h2>Smart Grids</h2>
                        <h5>Oil & Gas, Electric Power</h5>
                    </div>
                    <div class="usecase-body">
                       <p>With the rise of renewable energy sources, plants & energy grids need to react fast. Streamsheets and Mosquitto provide the necessary speed.</p>
                        <ul>
                        <li>Condition Monitoring </li>
                        <li>Dashboards and Charting</li>
                        <li>Real-Time Pricing</li>
                        <li>Gateways for OPCUA/MQTT/KAFKA</li>
                        </ul>
                    </div>
                </div>
            </div>
            <div class="col-lg-4 col-md-6 col-sm-6 usecase">  
                <div class="usecase-box">
                    <div class="overlay-caption">
                        <h2>Retail & Logistics</h2>
                        <h5>POS, eCommerce, Transportation</h5>
                    </div>
                    <div class="usecase-body">
                        <p>Real-time marketing, online shooping and just-in-time delivery need to be in-sync. Streamsheets let you connect and monitor retail chain operations as they happen.</p>
                        <ul>
                        <li>Real-Time Offers</li>
                        <li>Fraud Detection</li>
                        <li>Real-time Inventory</li>
                        <li>Vehicle Tracking</li>
                        </ul>
                    </div>
                </div>
            </div>
            <div class="col-lg-4 col-md-6 col-sm-6 usecase">  
                <div class="usecase-box">
                    <div class="overlay-caption">
                        <h2>Smart Building</h2>
                        <h5>Offices, Facilities, Hotels</h5>
                    </div>
                    <div class="usecase-body">
                         <p>Streamsheets and Mosquitto are an all-in-one solution for analysing, visualising and controlling building and faciltity conditions and operations.</p>
                        <ul>
                        <li>Automation & Control</li>
                        <li>Predictive Maintenance</li>
                        <li>Real-Time Asset Tracking</li>
                        <li>Gateways for BACnet/MQTT/KAFKA</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </div>
</section><!-- usecase -->


<section id="partnerships" class="features section">
    <div class="container" >
        <div class="row">
            <div class="col-lg-12 col-md-12 col-sm-12 usecase-intro">  
                <div>
                    <h1 class="section-header">Where Cedalo plays an active role</h1>
                </div>
            </div>
            <div class="col-md-4 col-sm-6 feature text-center">
                <div class="partnership-content">
                    <a href="https://openindustry4.com/About-Us.html" target="_blank"><img src="https://cedalo.com/assets/images/partnerships/openindustry.png" alt="" style="width:100%;height:auto;"></a>
                    <p>Cedalo is part of the <a href="https://www.eclipse.org/membership/showMember.php?member_id=1376#projects" target="_blank">Open Industry 4.0 Alliance</a> along with big names like SAP, Endress+Hauser, Hilscher and many more.</p>
                </div>
            </div>
            <div class="col-md-4 col-sm-6 feature text-center">
                <div class="partnership-content">
                    <a href="https://www.eclipse.org/membership/showMember.php?member_id=1376#projects" target="_blank"><img src="https://cedalo.com/assets/images/partnerships/eclipse.png" alt="" style="width:100%;height:auto;"></a>
                    <p>Cedalo is an <a href="https://www.eclipse.org/membership/showMember.php?member_id=1376" target="_blank">Eclipse Solution Member</a> and sponsors two key IoT projects: <a href="https://projects.eclipse.org/projects/iot.mosquitto" target="_blank">Eclipse Mosquitto</a> and <a href="https://projects.eclipse.org/projects/iot.streamsheets" target="_blank">Eclipse Streamsheets.</a></p>
                </div>
            </div>
            <div class="col-md-4 col-sm-6 feature text-center">
                <div class="partnership-content">
                    <a href="https://www.plattform-i40.de/PI40/Redaktion/DE/Anwendungsbeispiele/455-cedalo/beitrag-cedalo.html" target="_blank"><img src="https://cedalo.com/assets/images/partnerships/plattform40.png" alt="" style="width:100%;height:auto;"></a>
                    <p>Cedalo was assigned an official entry in the Map of Industrie 4.0 use cases which is maintained by the <a href="https://www.plattform-i40.de/PI40/Navigation/EN/Home/home.html" target="_blank">Plattform Industrie 4.0</a>.</p>
                </div>
            </div>
            <div class="col-md-4 col-sm-6 feature text-center">
                <div class="partnership-content">
                    <a href="https://lni40.de/?lang=en" target="_blank"><img src="https://cedalo.com/assets/images/partnerships/lni40.png" alt="" style="width:100%;height:auto;"></a>
                    <p>Cedalo is actively engaging in two test LNI Test Labs, hosted by the <a href="https://lni40.de/practice/usecases/?lang=en" target="_blank">Labs Network Industrie 4.0</a> association.</p>
                </div>
            </div>
            <div class="col-md-4 col-sm-6 feature text-center">
                <div class="partnership-content">
                    <a href="https://www.i40-bw.de/de/100orte/cedalo-ag/" target="_blank"><img src="https://cedalo.com/assets/images/partnerships/100orte.png" alt="" style="width:100%;height:auto;"></a>
                    <p>Cedalo was awarded in the "100 Places for Industrie 4.0 in Baden-Württemberg" contest from the <a href="https://www.i40-bw.de/en/" target="_blank">Allianz Industrie 4.0 BW.</a></p>
                </div>
            </div>
             <div class="col-md-4 col-sm-6 feature text-center">
                 <div class="partnership-content">
                    <a href="https://www.confluent.io/" target="_blank"><img src="https://cedalo.com/assets/images/partnerships/confluent.png" alt="" style="width:100%;height:auto;"></a>
                    <p>Cedalo is an certified Technology Partner of <a href="https://www.confluent.io/" target="_blank">CONFLUENT</a> - The original creators of streaming platform Apache Kafka®</p>
                </div>
            </div>
        </div>
    </div>
</section><!-- partnerships -->

<section id="chartgallery" class="section gallery"><!-- Chart Gallery -->
    <div class="container-flex text-center fluid-padding" >
            <h1>Powerful charts for bound and unbound data</h1>
            <div class="row no-padding" style="padding-top:20px">
                {% for chartnum in (10..15)  %}
                    <div class="col-md-4 col-sm-6 col-xs-12 text-center" style="padding:20px">
                        <img src="https://cedalo.com/assets/images/chartgallery/chart{{ chartnum }}.jpg" alt="" style="width:100%;height:auto;">
                    </div>
                {% endfor %}
            </div>
            <p>&nbsp;</p>
            <p><a href="all_charts.html" class="btn btn-large">More Charts Types</a></p>
    </div>
</section><!-- Chart Gallery -->

<section id="download" class="section downloads">
    <div class="container" >
        <div class="row">
            <div class="col-md-12 col-sm-12 download">
                <div class="download-intro">
                    <h1 class="section-header">Get Started! Open-Source or Premium.</h1>
                    <p>The two Open-Source projects Eclipse Streamsheets and Eclipse Mosquitto are included in the <b>Cedalo Community Platform</b>. Cedalo also offers premium editions. They are called <b>Cedalo Sheets</b> and <b>Cedalo Broker</b> and are included in the <b>Cedalo Premium Platform</b>.</p>
                </div>
            </div>
            <div class="col-md-4 col-sm-6 download text-center" >
                <span class="icon icon icon-cloud"></span>
                <div class="download-content">
                    <h2>Managed Service</h2>
                    <p>The easiest way to get started with the Premium Platform is our managed service called Cedalo Cloud. It comes with a 14-day money back guarantee.</p>
                    <p><a href="contact.html" class="btn btn-large">Contact us</a></p>
                </div>
            </div>
            <div class="col-md-4 col-sm-6 download text-center">
                <span class="icon icon-desktop"></span>
                <div class="download-content">
                    <h2>On-Premises</h2>
                    <p>You can run both the Community Platform and the Premium Platform on-premises on your local machines. Simply follow the instructions on the download page.</p>
                    <p><a href="download.html" class="btn btn-large">Download Page</a></p>
                </div>
            </div>
            <div class="col-md-4 col-sm-6 download text-center">
                <span class="icon icon-gears"></span>
                <div class="download-content">
                    <h2>Edge Devices</h2>
                    <p>Both platform products are very efficient with CPU power and memory consumption. So you can run them directly on edge devices, controllers or the Raspberry Pi.</p>
                    <p><a href="download.html" class="btn btn-large">Download Page</a></p>
                </div>
            </div>
        </div>
    </div>
</section><!-- download -->

<section id="blog" class="section teams">
    <div class="container-flex fluid-padding">
        <div class="row">
            <div class="col-md-12 col-sm-12">
                <div class="person-intro">
                    <h1 class="section-header">Visit our video blog for more use cases</h1>
                </div>
            </div>
             {% for post in site.categories["blogposts"] %}
                <!--
                {% increment my_post %}
                -->
                <div class="col-md-4 col-sm-6" style="padding:20px">
                    <div class="person">
                        <a href="{{post.url}}"><img src="{{ post.image_url }}" alt="" class="img-responsive"></a>
                        <div>
                            <a href="{{post.url}}"><h4>{{post.title}}</h4></a>    
                            <p>{{post.excerpt}}</p>
                        </div>
                    </div><!-- blog -->
                </div>
                {% if my_post == 6 %}
                    {% break %}
                {% endif %}
            {% endfor %}
            <div class="col-md-12 col-sm-12 text-center">
                <p><a href="all_posts.html" class="btn btn-large">Explore all blog posts</a></p>
            </div>
        </div>
        
    </div>
</section><!-- blog --> 

