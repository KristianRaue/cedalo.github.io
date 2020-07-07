---
layout: default
title: Cedalo - Download
---

<section id="banner" class="downloadpage" role="banner">
<!-- leave unchanged from here  --> 
    {% include _nav.html %}      
    <div class="container">
        <div class="row flex-start" class="align-items: flex-start;">
            <div class="col-md-12 col-sm-12">
                <div class="downloadpage-spacer">
                    <p>&nbsp;</p>
                </div>
            </div>
<!-- until here for nav menus to work smoothly  -->
            <div class="downloadpage-box">
                <div class="col-md-8 col-sm-8 col-md-offset-2 col-sm-offset-2">
                    <h2 class="section-header">Watch Webinar Recording</h2>
                    <p>Please enter your name and email.</p>
                        <form accept-charset="UTF-8" method="POST" action="https://api.cedalo.cloud/rest/request/website/cloudcontacts" class="form-horizontal control-label contactcedalo">
                            <div class="form-group">
                                <label for="inputName" class="col-sm-2">Name:</label>
                                <div class="col-sm-8">
                                <input name="Name" type="text" class="form-control" id="inputName" placeholder="Name" required>
                                </div>
                            </div>
                            <div class="form-group">
                                <label for="inputEmail" class="col-sm-2">Email:</label>
                                <div class="col-sm-8">
                                <input name="Email" type="email" class="form-control" id="inputEmail" placeholder="Email" required>
                                </div>
                            </div>
                            <div class="form-group">
                                <div class="col-sm-2 col-sm-offset-2">
                                <button name="Webinar" type="submit" class="btn btn-large">Watch Webinar Recording</button>
                                </div>
                            </div>
                        </form>
                </div>
            </div>
        </div>
    </div>
</section><!-- banner -->





