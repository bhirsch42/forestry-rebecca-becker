---
layout: home

---
<div class="text-center" id="home"> <div class="header"> <div class="cursive"> Rebecca Paris

</div> </div> </div>

{% include gallery_launcher.html %}

<div class="row" id="about">
<div class="col col-sm-6 bio-img-wrapper">
<div class="bio-img"></div>
</div>
<div class="col col-sm-6">
<div class="about-the-artist">
<h1 class="text-center">About the Artist</h1>
<hr>
<div class="big-read">
{{site.data.about_the_artist.about_the_artist}}
</div>
</div>
</div>
</div>

<div class="row">
<div class="col col-md-12">
<div class="portrait-process">
<h1 class="text-center">
Portrait Process
</h1>
<hr>
<div class="big-read">
{{site.data.about_the_artist.portrait_process}}
</div>
</div>
</div>
</div>

<div class="row" id="pricing">
<div class="col col-md-12">
<h1 class="text-center">
Pricing
</h1>
<hr>
</div>
</div>

<div class="row">
<div class="col col-lg-6 col-12">
<h3 class="text-center">
Oil Prices
</h3>
{% for price in site.data.prices.prices %}
<ul class="price">
<li>
<span class="product">
{{price.type_of_painting}}
</span>
<span class="price">
{{price.oil_price}}
</span>
</li>
</ul>
{% endfor %}
</div>
<div class="col col-lg-6 col-12">
<h3 class="text-center">
Pastel Prices
</h3>
{% for price in site.data.prices.prices %}
<ul class="price">
<li>
<span class="product">
{{price.type_of_painting}}
</span>
<span class="price">
{{price.pastel_price}}
</span>
</li>
</ul>
{% endfor %}
</div>
</div>

<div class="row" id="testimonials">
<div class="col col-md-12">
<h1 class="text-center">
Testimonials
</h1>
<hr>
</div>
</div>

<div class="row">
<div class="col-md-12">
{% include testimonials.html %}
</div>
</div>

<div class="row" id="contact">
<div class="col col-md-12">
<h1 class="text-center">
Contact
</h1>
<hr>
</div>
</div>

<div class="row"> <div class="col col-md-12"> <h2 class="text-center">

Rebecca Paris (formerly Rebecca Becker), Artist

</h2> </div> </div>

<div class="row">
<div class="col col-md-12">
<h2 class="text-center">
Email:
<a href="mailto:{{site.data.footer.email}}">{{site.data.footer.email}}</a>
</h2>
</div>
</div>

<div class="row">
<div class="col col-md-12">
<hr class="dashed">
</div>
</div>

<div class="row">
<div class="col col-md-12 text-center">
<small>
{{site.data.footer.copyright}}
</small>
<br>
<br>
</div>
</div>