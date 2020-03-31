---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<a id="publications"></a>Publications
======
M. Schultz und S. Reitmann. “Consideration of Passenger Interactions for the Prediction of Aircraft Boarding Time”. In: Aerospace 5.4 (Sep. 2018), S. 101. DOI: 10 . 3390 / aerospace5040101. URL: https://www.mdpi.com/2226-4310/5/4/101.

M. Schultz und S. Reitmann. “Machine learning approach to predict aircraft boarding”. In: Journal of Transportation Research Part C: Emerging Technologies (2018).

S. Reitmann und M. Schultz. “Computation of Air Traffic Flow Management Performance with Long Short-Term Memories Considering Weather Impact”. In: Artificial Neural Networks and Machine Learning – ICANN 2018. Bd. 11140. Lecture Notes in Computer Science. Springer, 2018, S. 532–541. ISBN: 978-3-030-01421-6. DOI: 10.1007/978-3-030-01421-6_51. URL: http://dx.doi.org/10.1007/978-3-030-01421-6_51.

S. Reitmann und K. Nachtigall. “Applying Bidirectional Long Short-Term Memories (BLSTM) to Performance Data in Air Traffic Management for System Identification.” In: ICANN (2). Hrsg. von Alessandra Lintas u. a. Bd. 10614. Lecture Notes in Computer Science. Springer, 2017, S. 528–536. ISBN: 978-3-319-68612-7. URL: https://doi.org/10.1007/978-3-319-68612-7_60.

======
{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
