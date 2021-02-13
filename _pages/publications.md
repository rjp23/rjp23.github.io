---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

You can find my peer-reviewed publications at:
<p>
<a href="https://www.scopus.com/authid/detail.uri?authorId=55675224272">SCOPUS Profile</a>.
<a href="{{author.orcid}}">ORCID profile</a>.
<p>
A regularly(ish!) updated list can be found below:

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
