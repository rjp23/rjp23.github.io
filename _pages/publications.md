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


{% for myyear in site.data.years %}

{% assign yeartest = false %}
{% for publi in publications reversed %}
  {% if publi.year == myyear.year %}
  {{ myyear.year }} - {{ publi.year }}
   {% assign yeartest = true %}
  {% endif %}
{% endfor %}

Test - {{ yeartest }} - {{ myyear.year }} - {{ publi.year }}

{% if yeartest == true %}
### {{ myyear.year }}
{% endif %}

{% for publi in site.publications reversed %}
{% if publi.year == myyear.year %}

  {{ publi.year }} - {{ publi.citation }}<br/>
  {% if publi.paperurl %}<a href="{{ publi.paperurl }}" target="_blank"><button type="button" class="btn btn-sm btn-success">DOI</button></a>{% endif %}

{% endif %}
{% endfor %}

{% endfor %}
