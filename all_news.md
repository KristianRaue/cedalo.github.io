---
layout: default
title: Cedalo - News
---

<section id="intro" class="downloadpage" role="banner">   
    <div class="container text-center">
        <div class="row flex-start" class="align-items: flex-start;">
            <div class="col-md-12 col-sm-12">
                <div class="downloadpage-spacer">
                    <h1>Cedalo News</h1>
                </div>
            </div>
        </div>
    </div>
</section><!-- banner -->

<section id="blog" class="section teams">
    <div class="container-flex fluid-padding">
        <div class="row">
             {% for post in site.categories["newsposts"] %}
                <div class="col-md-4 col-sm-6" style="padding:20px">
                    <div class="news-content">
                        <a href="{{post.url}}"><img src="{{ post.image_url }}" alt="" class="img-responsive"></a>
                        <div>
                            <a href="{{post.url}}"><h4>{{post.title}}</h4></a>    
                            <p>{{post.excerpt}}</p>
                        </div>
                    </div><!-- blog -->
                </div>
            {% endfor %}
        </div>
    </div>
</section><!-- blog --> 





