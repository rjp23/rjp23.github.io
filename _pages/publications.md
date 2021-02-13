---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

You can find my peer-reviewed publications at:
<br />
<a href="https://www.scopus.com/authid/detail.uri?authorId=55675224272">SCOPUS Profile</a>
<br />
<a href="http://orcid.org/0000-0002-0801-0831"><img src="https://orcid.org/sites/default/files/images/orcid_16x16.png" style="width:1em;margin-right:.5em;" alt="ORCID iD icon">ORCID profile</a>
<p>


<h3>A regularly(ish!) updated list based on <a href="https://www.scopus.com/authid/detail.uri?authorId=55675224272">SCOPUS </a>can be found below:</h3>

{% include base_path %}
s
{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
