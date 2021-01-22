---
layout: kz-page
title: The team
permalink: /team/
header:
  title: ""
  image_fullwidth: logo_image.png
widgets:
- url: https://www.linkedin.com/in/dawson-mwangi-ab229659/
  image: dawson.jpg
  title: <a href="https://www.linkedin.com/in/dawson-mwangi-ab229659/" target="_blank">Bryan Dawson Wachira Mwangi</a>
  text: CEO and Co-founder

- url: https://www.linkedin.com/in/aaron-milla-1906a21b4/
  image: aaron.jpg
  title: <a href="https://www.linkedin.com/in/aaron-milla-1906a21b4/" target="_blank">Aaron Milla Kangethe</a>
  text: CTO and Co-founder

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

