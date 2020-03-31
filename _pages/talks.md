---
layout: archive
title: "Talks and presentations"
permalink: /talks/
author_profile: true
---
<!--
S. Reitmann und M. Schultz. “Real-Time Prediction of Aircraft Boarding”. In: Digital Avionics Systems Conference (DASC). London, UK, 2018.

S. Reitmann und M. Schultz. “Recurrent Neural Network based Aircraft Boarding Prediction”. In: Air Transport Research Society (ATRS). Seoul, Süd Korea, 2018.

M. Schultz und S. Reitmann. “Prediction of Aircraft Boarding time Using LSTM network”. In: Winter Simulation Conference. Göteborg, Schweden, 2018.

M. Schultz und S. Reitmann. “Prediction of passenger boarding progress using neural network approach”. In: International Conference on Research in Air Transportation (ICRAT). Barcelona, Spanien, 2018.

S. Reitmann. “Ableitung eines mathematischen Wirkungsmodells durch systematische Analyse von Leistungsindikatoren”. In: Deutscher Luft- und Raumfahrtkongress (DLRK). München, Deutschland, 2017.

S. Reitmann und M. Schultz. “Stability Analysis of Recurrent Neural Networks for Time Series based System Control in Aviation”. In: International Science & Progress Conference. St. Petersburg, Russland, 2017.

S. Reitmann, A. Gillissen und M. Schultz. “Performance Benchmarking in Interdependent ATM Systems”. In: International Conference on Research in Air Transportation (ICRAT). Philadelphia, USA, 2016.

S. Reitmann und K. Nachtigall. “Multivariate Time Series Prediction with Long Short-Term Memory (LSTM)”. In: International Science & Progress Conference. St. Petersburg, Russland, 2016.

P. Bießlich u. a. “Developing Generic Flight Schedules for Airport Clusters”. In: Council of European Aerospace Societies (CEAS). Delft, Niederlande, 2015.


======
-->
{% if site.talkmap_link == true %}

<p style="text-decoration:underline;"><a href="/talkmap.html">See a map of all the places I've given a talk!</a></p>

{% endif %}

{% for post in site.talks reversed %}
  {% include archive-single-talk.html %}
{% endfor %}
