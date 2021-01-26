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
  text: "CEO and Co-founder. I have always had a drive to do more, I believe pushing ourselves to doing things that are outside the norm makes us grow.  We came into this world and with nothing but we all should strive to leave a mark that will leave this world better than we found it. I am very passionate in doing things that make an impact in the society."
  cols: 6

- url: https://www.linkedin.com/in/aaron-milla-1906a21b4/
  image: aaron.jpg
  title: <a href="https://www.linkedin.com/in/aaron-milla-1906a21b4/" target="_blank">Aaron Milla Kangethe</a>
  text: "CTO and Co-founder. I'm an industrial designer, passionate about designing tech that inspires people to pursue their own dreams. I hope over time share my expertise with the future generation. I believe in being different, being one’s true self for only by being ourselves can we only bring new solutions to challenges we face on the daily."
  cols: 6

---

<div class="row">
  {% for widget in page.widgets %}
    {% assign loopindex = forloop.index | modulo: 2 %}
    <div id="{{ widget.anchor }}">{% include _frontpage-widget.html widget=widget %}</div>
    {% if loopindex == 0 %}
  <hr style="height:1px; visibility:hidden;" /> <!-- Prevents long first column items from pushing new rows to the right -->
    {% endif %}
  {% endfor %}
</div>

