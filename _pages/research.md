---
title: "Choi Lab - Research"
layout: textlay
excerpt: "Choi Lab -- Research"
sitemap: false
permalink: /research/
---

# Research

The overall theme of our research is to understand kinetics, mechanics, and thermodynamics of engineered nanosystems, and to use the observed phenomena for various applications including renewable energy and bioengineering. Our ideas for technological breakthroughs are often inspired by biological processes in nature. Our effort includes design and fabrication of DNA nanostructures from self-assembly, which are integrated with nanocrystals, carbon nanotubes, graphene, and transition metal dichalcogenides. These nanosystems are explored to study energy conversion and transport processes, and to develop novel devices with new levels of system control at the nanoscale. Characterization techniques include absorption, Raman, and photoluminescence spectroscopy ranging from UV to near-infrared, with an emphasis on single molecule/particle imaging and spectroscopy. Additionally, atomic force microscopy and spectro-electrochemistry are methods commonly used in the lab. While we focus on fundamental nanoscience and nanoengineering, we aim to make transformative impacts in our society as well as scientific community. 

Here are some themes and techniques that we currently work on:

## Research highlights


{% assign number_printed = 0 %}
{% for publi in site.data.research_highlights %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>

