---
permalink: /
#title: "academicpages is a ready-to-fork GitHub Pages template for academic personal websites"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a Ph.D. student specializing in Educational Technology at the University of California, Irvine, where I am advised by [Dr. Mark Warschauer](http://markwarschauer.com/) and [Dr. Penelope Collins](https://sites.google.com/uci.edu/penelopecollins/home). I also work closely with [Dr. Ying Xu](https://ying-xu.com/) from the University of Michigan, Ann Arbor. Prior to joining UCI, I completed my master's at Harvard Graduate School of Education, advised by [Dr. Catherine Snow](https://www.gse.harvard.edu/directory/faculty/catherine-snow). My research explores the intersection of child-computer interaction and education, with a focus on creating innovative technology solutions to support children's learning. I am currently working on an NSF-funded project that develops conversational science narrative videos to promote children's STEM learning. 

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

