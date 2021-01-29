---
layout: kz-page
header: no
image:
    title: Processing_Plant.jpg
permalink: /index.html
homepage: true
teaser: At Pyro-degrade Energy we've developed a technology to produce pyro-diesel from plastic waste. We’ve designed our processor to be self-sufficient - able to run off-grid powered by the fuel it produces. Pyro-diesel is an environmentally friendly diesel substitute - it is almost sulphur free and has a low carbon footprint. Our efficient production process means that we are able to supply pyro-diesel at a lower cost than ordinary diesel.
widgets:
- image: sdg2.png
  text: Both of our main products - pyro-diesel and basic pyrolysis plants designed to fit inside a standard 20ft container - are aimed to provide an affordable solution to enable farmers to produce more food.
- image: sdg7.png
  text: Pyro-diesel is an environmentally friendly diesel substitute - it is almost sulphur free and has a low carbon footprint. Our efficient production process means that we are able to supply pyro-diesel at a lower cost than ordinary diesel.
- image: sdg9.jpg
  text: We've developed our technology from the ground up. We provide infrastructure to farmers.
- image: sdg11.png
  text: Our solution provides a solution both to the plastic waste problem and the need for affordable fuel.
- image: sdg13.png
  text: Pyro-diesel has a low carbon footprint. By using plastic waste to produce our fuel we prevent additional GHG emissions.
- image: sdg14.png
  text: Ocean pollution is detrimental to marine ecosystem health. By using plastic waste to produce our fuel we reduce the amount of pollution entering our oceans. 
---



<div class="row t60 b60">
    <div class="small-12 text-center columns">
        <a class="button large radius {{ page.callforaction.style }}" href="https://youtu.be/pTas6aR1kx8?t=70">Watch the video!</a>
    </div><!-- /.small-12.columns -->
</div><!-- /.row -->

<h3>With our work we contribute to 6 Sustainable Development Goals set by the UN:</h3>


<hr style="height:1px; visibility:hidden;" />
<div class="row">
  {% for widget in page.widgets %}
    {% assign loopindex = forloop.index | modulo: 3 %}
    <div id="{{ widget.anchor }}">{% include _frontpage-widget.html widget=widget %}</div>
    {% if loopindex == 0 %}
  <hr style="height:1px; visibility:hidden;" /> <!-- Prevents long first column items from pushing new rows to the right -->
    {% endif %}
  {% endfor %}
</div>



