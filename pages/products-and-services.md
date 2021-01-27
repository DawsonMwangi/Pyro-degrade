---
layout: kz-page
title: Products & Services
permalink: /products-and-services/
header:
  title: ""
  image_fullwidth: logo_image.png
widgets:
- url: 
  image: Fuel.jpg
  title: Sale of Fuel
  text: "This is our core business. Our fuel; Pyro-diesel has many beneficial properties to both the users and the environment. To the users the most important is the pricing point which is 30% less than ordinary diesel. To the environment Pyro-diesel is free of Sulphur and has less carbon emission as compared to ordinary diesel."
  cols: 4

- url: 
  image: logo_image.png
  title: Construction of processing plants
  text: "We specialize in construction of private processing units for large scale farms with high consumption of diesel and a need for safe disposal of their plastic waste. The plants vary in sizes mainly based on the specific clients demands and storage capacity. A standard plant is designed to fit inside a standard 20ft container, this also comes with fuel, water and gas storage tanks which are set up outside the container and the package also includes a plastic shredder which is also a separate set up."
  cols: 4

- url: 
  image: plastic_trash.jpg
  title: Sorting and Shredding of Plastic Waste
  text: "We are producing clean, graded and shredded plastic for supplying our plant. We are also selling this feedstock to other consumers in the market who are already purchasing waste plastic from dumpsites."
  cols: 4

---

<div class="row">
  {% for widget in page.widgets %}
    {% assign loopindex = forloop.index | modulo: 3 %}
    <div id="{{ widget.anchor }}">{% include _frontpage-widget.html widget=widget %}</div>
    {% if loopindex == 0 %}
  <hr style="height:1px; visibility:hidden;" /> <!-- Prevents long first column items from pushing new rows to the right -->
    {% endif %}
  {% endfor %}
</div>



