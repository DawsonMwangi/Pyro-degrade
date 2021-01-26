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
  text: "This is our core business. Once we build our first commercial plant we will be distributing fuel to small and medium scale farmers through direct purchase from the farmers and through satellite fuel stations that are found in most villages. During our first year of operation we are planning to supply about 500,000 liters of fuel, with a goal of tripling this amount next year. We are able to produce 600-700ml of fuel from 1kg of plastic waste."
  cols: 4

- url: 
  image: logo_image.png
  title: Construction of processing plants
  text: "We specialize in construction of private processing units for large scale farms with high consumption of diesel and a need for safe disposal of their plastic waste. The plants can be customized to fit the specific needs of each client. The rates are starting from USD 20,000, depending on the capacity required."
  cols: 4

- url: 
  image: plastic_trash.jpg
  title: Sorting and Shredding of Plastic Waste
  text: "We are producing clean, graded and shredded plastic for supplying our plant. We are also selling this feedstock to other consumers in the market who are already purchasing waste plastic from dumpsites. During our first year of operation we are planning to remove 1,000,000 tonnes of plastic waste from the environment. We will use 10% of our profit towards raising the awareness about the value of plastic waste."
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



