---
layout: home
---
<h1 class="text-center">Gallery</h1>
<ul class="gallery-nav">
  <li id=""><a href="/gallery">All</a></li>
  <li id=""><a href="oil_portraits.html">Oil Portraits</a></li>
  <li id=""><a href="pastel_portraits.html">Pastel Portraits</a></li>
  <li id=""><a href="pet_portraits.html">Pet Portraits</a></li>
  <li id="selected"><a href="abstracts_and_landscapes.html">Abstracts/Landscapes</a></li>
</ul>
<div class="grid">
    {% assign portraits = site.data.portraits.portraits | where_exp: "portrait", "portrait.categories contains 'Abstracts/Landscapes'" %}

    {% for portrait in portraits %}
        <a class="grid-item" href="http://res.cloudinary.com/bhirsch-cloud/image/upload{{portrait.image}}" target="_blank">
            <img src="http://res.cloudinary.com/bhirsch-cloud/image/upload/c_thumb,w_300,h_300{{portrait.image}}" alt="">
            {% if portrait.caption.size > 0 %}
                <div class="caption">{{portrait.caption}}</div>
            {% endif %}
        </a>
    {% endfor %}
</div>
