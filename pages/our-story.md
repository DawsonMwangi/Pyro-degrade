---
layout: kz-page
title: Our story
permalink: /our-story/
header: no
image:
    title: plastic-to-fuel.jpg
widgets:
- url: 
  image: story1.jpg
  cols: 4
- url: 
  image: story2.jpg
  cols: 4
- url: 
  image: story3.jpg
  cols: 4

---

<!-- how it all started -->
It all began in late 2017 when two entrepreneurs from Chandaria Business Innovation and Incubation Center decided to do something together to tackle the challenges associated with plastic waste. 
We realized that we have to change people's perception of plastic waste; and this will only be possible if we find a way to turn plastic waste into a resource. 
This is when we decided to build a machine that could produce fuel from plastic waste.
If we could supply affordable fuel for stationary diesel engines widely used in Kenya, that would create a market for post-consumer plastic and thus prevent it from becoming waste.


<!-- prototyping -->
By 2018 our research had paid off - we've built and tested our first proof of concept model from the ground up. 
This was a very simple processor with the capacity of 6kgs of plastic per batch. 
In June 2018 we exhibited it at the African Youth Innovation Summit in Kigali, Rwanda. 
We were noticed and we subsequently received a prototyping grant from the UN Development Fund.
This allowed us to design a better processor with the capacity of 30kgs per batch, though we could only proces three batches per day.


<!-- commercialization -->
In 2019 we were selected for the UK's Royal Academy of Engineering fellowship.
This was followed by a commercialization grant from the Kenya National Innovation Agency.
Through extensive research and experimentation we've developed a more efficient processor that requires less time and energy per batch. 
We could now process ten 30kg batches of plastic per day, producing 0.6-0.7 liters of pyro-diesel from each kg of plastic waste.
We've designed our processor to be self-sufficient - able to run off-grid powered by the fuel it produces.

<div class="row">
  {% for widget in page.widgets %}
    {% assign loopindex = forloop.index | modulo: 3 %}
    <div id="{{ widget.anchor }}">{% include _frontpage-widget.html widget=widget %}</div>
    {% if loopindex == 0 %}
  <hr style="height:1px; visibility:hidden;" /> <!-- Prevents long first column items from pushing new rows to the right -->
    {% endif %}
  {% endfor %}
</div>

<!-- target market -->
To prevent as much plastic waste from contaminating the environment as possible, we decided to focus on producing pyro-diesel as our core business.
We've identified farmers practicing irrigation as our initial target market - there are more than 100 farmers in just a single county in Kenya who are already using diesel powered generators for irrigation.
Small and medium scale farms will benefit from our pyro-diesel as it is both cheaper and more environmentally friendly than ordinary diesel.
We will be supplying our fuel both directly to farmers and to satellite fuel stations found in most villages. 
For large farms that generate a lot of plastic waste and consume large amounts of diesel it makes financial sense to operate their own processing plant.
We've developed plants that fit inside a standard 20ft container specifically for them.


<!-- 2021 -->
For 2021 our ambition is to build our first commercial scale plant. <!-- and process 1,000,000 tonnes of plastic waste into 650,000 liters of pyro-diesel. --> 
Next year we are planning to increase our rate of production threefold. 
Regardless of how much we grow, we intend to spend 10% of our profit to raise awareness about the value of plastic waste, change attitudes and thus protect our planet.
