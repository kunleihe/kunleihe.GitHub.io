---
permalink: /
#title: "academicpages is a ready-to-fork GitHub Pages template for academic personal websites"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a Ph.D. student specializing in Educational Technology at the University of California, Irvine, where I am advised by [Dr. Mark Warschauer](http://markwarschauer.com/) and [Dr. Penelope Collins](https://sites.google.com/uci.edu/penelopecollins/home). I also work closely with [Dr. Ying Xu](https://ying-xu.com/) from the University of Michigan, Ann Arbor. Prior to joining UCI, I completed my master's at Harvard Graduate School of Education, advised by [Dr. Catherine Snow](https://www.gse.harvard.edu/directory/faculty/catherine-snow). 

My research explores the intersection of child-computer interaction and education, with a focus on creating innovative conversational interfaces to support children's learning by leveraging AI technologies. I am currently working on an NSF-funded project, in partnership with PBS KIDS,  focusing on the development and evaluation of conversational science narrative videos to promote children's STEM learning. Simultaneously, I am developing a bilingual conversational agent integrated into culturally engaging e-books, aiming to support parent-child joint engagement in reading.

As a mixed-methods researcher, I combine lend design-based implementation research with experimental designs to innovate in the educational technology space. My work involves collaborating with young children and their families to design engaging, accessible conversational interfaces tailored to young learners' needs. Concurrently, I design experiments to rigorously evaluate the effectiveness of these tools, combining qualitative insights from the design phase with quantitative outcomes from the experiments. This approach not only assesses the impact of these interfaces on learning but also uncovers the mechanisms behind their success.

In my research, I actively collaborate with children and parents from diverse language, cultural, and ethnic backgrounds, ensuring that the conversational interfaces are inclusive to users from various communities. 

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

