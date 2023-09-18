---
permalink: /
#title: "academicpages is a ready-to-fork GitHub Pages template for academic personal websites"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a Ph.D. student specializing in Educational Technology at the University of California, Irvine, where I am advised by [Dr. Mark Warschauer](http://markwarschauer.com/) and [Dr. Penelope Collins](https://sites.google.com/uci.edu/penelopecollins/home). Prior to joining UCI, I completed my master's at Harvard Graduate School of Education, advised by [Dr. Catherine Snow](https://www.gse.harvard.edu/directory/faculty/catherine-snow). My research explores the intersection of **child-computer interaction** and **education**, with a focus on creating innovative technology solutions to support children's learning.

My current research focuses on designing and evaluating conversational interface to promote early learning in various domains, including language, science, and computational thinking. I design with and for children from diverse backgrounds, such as low-income Hispanic bilingual children. I am committed to creating digital learning experiences that are inclusive and accessible to families from diverse linguistic, cultural, and socio-economic backgrounds. 

## News
{% include base_path %}
{% capture written_year %}'None'{% endcapture %}
{% for post in site.posts limit:10 %}
  {% capture year %}{{ post.date | date: '%Y' }}{% endcapture %}
  {% if year != written_year %}
    {% capture written_year %}{{ year }}{% endcapture %}
  {% endif %}
  {% include archive-single.html %}
{% endfor %}

