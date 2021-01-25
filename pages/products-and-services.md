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
  text: This is our core business with the construction of the plant we intend on distributing fuel to small and middle scale farmers through direct purchase from the farmers and though satellite fuel stations that are normally found in most villages. 
  In our first year in operations we intend on supplying up to 500,000 Liters of fuel with a goal of tripling that amount by the second year.

  At a rate of approximately 600 -700ml of fuel per Kg of plastic waste. 

  cols: 4

- url: 
  image: logo_image.png
  title: Construction of processing plants
  text: a.  In this division we specialize in construction of private processing units for own personal use. The plants are customized to fit the specific needs of the client with our main focus being large scale farms with high consumption of diesel and a need for safe disposal of their plastic waste. 

  At a rates starting from of 20,000 USD depending on the consumption needs of the client.

  cols: 4

- url: 
  image: logo_image.png
  title: Sorting and Shredding of Plastic Waste
  text: This divisions main purpose will be to supply our plant with clean, graded and shredded plastic, however this division will also sell the clean, graded and shredded plastics to the other consumers in the market that already purchase waste plastic from dumpsites. 
  
  In our first year of operations we intend riding the environment of 1,000,000 tonnes of plastic. We also intend on redirecting 10% of our income towards awareness creation on the value of plastic waste.

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

