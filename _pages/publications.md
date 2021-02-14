---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<style>
.btn{
    margin-bottom:0;
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
<a href="https://www.scopus.com/authid/detail.uri?authorId=55675224272">SCOPUS Profile</a>



{% for myyear in site.data.years %}

{% assign yeartest = false %}
{% for publi in site.publications reversed %}
  {% if publi.year == myyear.year %}
   {% assign yeartest = true %}
  {% endif %}
{% endfor %}


{% if yeartest == true %}
## {{ myyear.year }}
{% endif %}

{% for publi in site.publications reversed %}
{% if publi.year == myyear.year %}

  {{ publi.citation }}<br/>
  {% if publi.paperurl %}<a href="{{ publi.paperurl }}" target="_blank"><button type="button" class="btn btn-sm btn-success">DOI</button></a>{% endif %}

{% endif %}
{% endfor %}

{% endfor %}
