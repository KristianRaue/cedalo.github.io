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
                    <h1 class="section-header">Contact us</h1>
                    <p>Please enter your name and email and we will contact you shortly.</p>
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
                                <label for="inputMessage" class="col-sm-2">Text:</label>
                                <div class="col-sm-8">
                                <textarea name="Message" class="form-control" rows="8" id="inputMessage" placeholder="Your message" required></textarea>
                                </div>
                            </div>
                            <div class="form-group">
                                <div class="col-sm-2 col-sm-offset-2">
                                <button type="submit" class="btn btn-large">Submit</button>
                                </div>
                            </div>
                        </form>
                </div>
            </div>
        </div>
    </div>
</section><!-- banner -->





