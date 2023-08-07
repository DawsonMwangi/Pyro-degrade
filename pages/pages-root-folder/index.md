---
layout: kz-page
header: no
image:
    title: Processing_Plant.jpg
permalink: /index.html
homepage: true
teaser: At Pyro-degrade Energy we've developed a technology to produce pyro-diesel from plastic waste. Pyro-diesel is an environmentally friendly diesel substitute - it is almost sulphur free and has a low carbon footprint. We’ve designed our processor to be self-sufficient - able to run off-grid powered by the fuel it produces. Our efficient production process means that we are able to supply pyro-diesel at a lower cost than conventional diesel.
widgets:
- image: sdg2.png
  text: Both of our main products - pyro-diesel and pyrolysis plants designed to fit inside a standard 20ft container - have been created with the aim to provide affordable fuel to farmers to enable them to grow crops all year round.
- image: sdg7.png
  text: Pyro-diesel is an environmentally friendly diesel substitute - it is almost sulphur free and has a low carbon footprint. Our efficient production process means that we are able to supply pyro-diesel at a lower cost than conventional diesel.
- image: sdg9.jpg
  text: There was no market for plastic waste because there was no infrastructure to convert it into a resource. We've developed our technology from scratch - an efficient process to process plastic waste into environmentally friendly fuel.
- image: sdg11.png
  text: At Pyro-degrade Energy we've developed a single solution that addresses both the plastic waste challenge and the need for affordable fuel to power irrigation systems in the agricultural sector.
- image: sdg13.png
  text: "Pyro-diesel we produce has a low carbon footprint. Our impact is: reduced emissions of CO2 and carbon black from open burning of plastic waste, reduced  emissions of CO2 and sulphur from conventional diesel usage."
- image: sdg14.png
  text: Plastic pollution of the ocean is detrimental to marine ecosystem health. By creating a market for plastic waste and by using it to produce our fuel we reduce the amount of pollution entering our oceans. 

---



<div class="row t60 b60">
    <div class="small-12 text-center columns">
        <a class="button large radius {{ page.callforaction.style }}" href="https://youtu.be/vURta5cMttI?t=570">Watch a video!</a>
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



