---
title: "Choi Lab - Pictures"
layout: piclay
excerpt: "Choi Lab -- Pictures"
permalink: /pictures/
---

# Pictures
Jump to: [Leiden](#leiden), [ETHZ](#ethz), [Cornell](#cornell), [St Andrews](#st-andrews)


## Leiden


#### Gallery
(Right-click *'view image'* to see a larger image.)
{% assign number_printed = 0 %}
{% for pic in site.data.pictures_Leiden %}

{% assign even_odd = number_printed | modulo: 4 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-3 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/Gallery/{{ pic.image }}" class="img-responsive" width="95%" style="float: left" />
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd > 2 %}
</div>
{% endif %}


{% endfor %}

{% assign even_odd = number_printed | modulo: 4 %}
{% if even_odd == 1 %}
</div>
{% endif %}

{% if even_odd == 2 %}
</div>
{% endif %}

{% if even_odd == 3 %}
</div>
{% endif %}

<p> &nbsp; </p>


### Graduate Course Teaching

ME 606: Radiation Heat Transfer
ME 505: Intermediate Heat Transfer

### Undergraduate Course Teaching
ME 497: Optical Nanomaterials
ME 305: Heat and Mass Transfer

### Outreach
Dr. Choi's lecture at the Science Cafe during NanoDays for K-12 students and their parents is archived in NanoHUB.
