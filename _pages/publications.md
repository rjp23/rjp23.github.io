---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<style>
.btn{
    margin-bottom:0;
    padding: 0.2em 0.5em;
}
.jumbotron{
    padding-bottom:0px;
    padding-top:5px;
    margin-top:10px;
    margin-bottom:10px
}
</style>

You can find my peer-reviewed publications at:
<br />
<a href="https://www.scopus.com/authid/detail.uri?authorId=55675224272">SCOPUS Profile</a> ({{ site.data.hindex.name }} - h-index: {{ site.data.hindex.hindex }})
<br />
<a href="http://orcid.org/0000-0002-0801-0831"><img src="https://orcid.org/sites/default/files/images/orcid_16x16.png" style="width:1em;margin-right:.5em;" alt="ORCID iD icon">ORCID profile</a>

<h3>A regularly(ish!) updated list based on <a href="https://www.scopus.com/authid/detail.uri?authorId=55675224272">SCOPUS </a>can be found below:</h3>





{% for myyear in site.data.years %}

{% assign yeartest = false %}
{% for publi in site.data.publist %}
  {% if publi.year == myyear.year %}
   {% assign yeartest = true %}
  {% endif %}
{% endfor %}


{% if yeartest == true %}
## {{ myyear.year }}
{% endif %}

{% for publi in site.data.publist %}
{% if publi.year == myyear.year %}

  {{ publi.citation }}<br/>
  {% if publi.paperurl %}<a href="{{ publi.paperurl }}" target="_blank"><button type="button" class="btn btn-sm btn-success">DOI</button></a>{% endif %}

{% endif %}
{% endfor %}

{% endfor %}
