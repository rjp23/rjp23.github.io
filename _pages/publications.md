---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

You can also find my articles on:
<p>
<u><a href="https://www.scopus.com/authid/detail.uri?authorId=55675224272">SCOPUS Profile</a>.</u>
<p>
<u><a href="{{author.orcid}}">ORCID profile</a>.</u>
<p>

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
