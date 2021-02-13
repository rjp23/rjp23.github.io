---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

You can find my peer-reviewed publications at:
<p>
<a href="https://www.scopus.com/authid/detail.uri?authorId=55675224272">SCOPUS Profile</a>
<br />
<a href="{{author.orcid}}"><img src="https://orcid.org/sites/default/files/images/orcid_16x16.png" style="width:1em;margin-right:.5em;" alt="ORCID iD icon">ORCID profile</a>
<p>


<h2>A regularly(ish!) updated list based on <a href="https://www.scopus.com/authid/detail.uri?authorId=55675224272">SCOPUS </a>can be found below:</h2>

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
