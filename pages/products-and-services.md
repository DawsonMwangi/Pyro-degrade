---
layout: kz-page
title: Products & Services
permalink: /products-and-services/
header:
  title: ""
  image_fullwidth: logo_image.png
widgets:
- url: 
  image: logo_image.png
  title: Sale of Fuel
  text: From a kilogram of plastic we extract an approximate of 600 milliliters of diesel that is free from sulfur.
  cols: 4

- url: 
  image: logo_image.png
  title: Construction of processing plants
  text: To build a simple domestic plant for a customer it would cost us an average of 20,000 to 30,000 USD depending the consumption needs of the customer.
  cols: 4

- url: 
  image: logo_image.png
  title: Sorting and Shredding of Plastic Waste
  text: To build a simple domestic plant for a customer it would cost us an average of 20,000 to 30,000 USD depending the consumption needs of the customer.
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

