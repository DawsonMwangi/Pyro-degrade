---
layout: kz-page
title: Our team
permalink: /team/
header: no
widgets:
- url: https://www.linkedin.com/in/dawson-mwangi-ab229659/
  image: dawson.jpg
  title: <a href="https://www.linkedin.com/in/dawson-mwangi-ab229659/" target="_blank">Bryan Dawson Wachira Mwangi</a>
  teaser: "Co-Founder and CEO"
  text: "I've always had a drive to do more. I believe that pushing ourselves to do things outside our comfort zone makes us grow. Collaborating with others enables us to go forward, while working alone keeps us going in circles. We were born with nothing, but we should strive to leave this world in a better state than it was before. I am passionate about doing things that have a positive impact on society and our planet."
  cols: 6

- url: https://www.linkedin.com/in/aaron-milla-1906a21b4/
  image: aaron.jpg
  title: <a href="https://www.linkedin.com/in/aaron-milla-1906a21b4/" target="_blank">Aaron Milla Kangethe</a>
  teaser: "Co-Founder and CTO"
  text: "I am an industrial designer, passionate about designing tech that inspires people to pursue their own dreams. Over time I hope to share my expertise with the future generations. I believe in being one's true self, which requires courage to be different. Only by being ourselves we can bring new solutions to the daily challenges we face."
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
