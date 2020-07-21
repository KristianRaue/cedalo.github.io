---
layout: default
title: Cedalo - Download
---

<section id="banner" class="banner" role="banner">
    {% include _nav.html %}      
    <div class="container text-center">
        <div class="row flex-start" class="align-items: flex-start;">
            <div class="col-md-12 col-sm-12">
                <div class="banner-spacer">
                </div>
            </div>
        </div>
    </div>
</section><!-- banner -->

<section id="intro" class="downloadpage" role="banner">   
    <div class="container text-center">
        <div class="row flex-start" class="align-items: flex-start;">
            <div class="col-md-12 col-sm-12">
                <div class="downloadpage-spacer">
                    <h1>Streamcharts Gallery</h1>
                </div>
            </div>

        </div>
    </div>
</section><!-- banner -->

<section id="chartgallery" class="section gallery"><!-- Chart Gallery -->
    <div class="container-flex text-center fluid-padding" >
        <div class="row no-padding">
            {% for chartnum in (10..33)  %}
                <div class="col-md-4 col-sm-6 col-xs-12 text-center" style="padding:20px">
                    <img src="https://cedalo.com/assets/images/chartgallery/chart{{ chartnum }}.jpg" alt="" style="width:100%;height:auto;">
                </div>
            {% endfor %}
        </div>
        <p>&nbsp;</p>
        <h2>This is just a small sample of possible chart types, there are many more...</h2>
    </div>
</section>





