---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: SAVE Model Documentation
---

The Systematic Assessment of Vessel Emissions (SAVE) model, is a Python-based model developed by ICCT marine team that combines ships’ Automatic Identification System (AIS) data and ships’ characteristics data to understand historical operational behavior, voyage pattern, routing network, and estimate energy consumption, and tank-to-wake (TTW) emissions from the global shipping industry. SAVE was first developed in 2017 with the release of a flagship report [Greenhouse gas emissions from global shipping, 2013–2015 (Olmer et al., 2017)](https://theicct.org/publication/greenhouse-gas-emissions-from-global-shipping-2013-2015/). 

In 2020 SAVE went through a series of major updates with the release of [IMO’s 4th Greenhouse Gas Study](https://www.imo.org/en/ourwork/Environment/Pages/Fourth-IMO-Greenhouse-Gas-Study-2020.aspx) which ICCT shared authorship with a consortium led by CE-Delft. In early 2025, we published the updated global ship emissions inventory, 2016-2023, in which SAVE was further updated (SAVE v2025.1) to reflect updated understandings of ship engine performance and policy development. 


## Versions

SAVE is under continuing development. Documentation of all versions since v2025.03.1 can be found here.

{% assign pages = site.pages | sort: "title" | reverse %}
{% for page in pages %}
{% if page.dir contains '/versions/' and page.title contains 'SAVE v'%}
<li><a class="page-link" href="{{ page.url | relative_url }}">{{ page.title | escape }}</a></li>
{% endif %}
{% endfor %}
