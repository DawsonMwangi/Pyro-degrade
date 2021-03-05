---
layout: kz-page
title: Our products
permalink: /products/
header:
  title: ""
  image_fullwidth: dumpsite-with-people.jpg
widgets:
- url: 
  image: plastic-to-fuel.jpg
  title: Pyro-diesel
  text: "We make pyro-diesel from plastic waste, thus preventing it from contaminating the environment. Pyro-diesel is an environmentally friendly diesel substitute - it is almost sulphur free and has a low carbon footprint. Our efficient production process means that we are able to supply pyro-diesel at a lower cost than ordinary diesel."
  cols: 4

- url: 
  image: Processing_Plant-cropped.jpg
  title: Pyrolysis plants
  text: "For large-scale farmers, or indeed anyone who has a large amount of plastic waste and a demand for diesel, it makes sense to operate their own plant to avoid transportation costs. A basic plant is designed to fit inside a standard 20ft container. The shredder for plastic waste and storage tanks for fuel, water and gas will be set up outside the container. Each plant will be customised to fit the customers specifications and desired capacity."
  cols: 4

- url: 
  image: plastic_flakes.jpg
  title: Shredded plastic
  text: "Clean, sorted and shredded plastic that we use to operate our plants is also available for sale. Please contact us to discuss if we can fulfil your specific requirements in terms of the type of plastic and the volume."
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
