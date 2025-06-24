---
title: Research
nav:
  order: 2
  tooltip: Published works
---

# {% include icon.html icon="fa-solid fa-microscope" %}Research

Our research focusses on development and application neuroimaging and modelling approaches to study brain physiology. The group is composed of multiple PIs with research spanning measurements of cerebrovascular (dys)function, brain microstructure, brain circuits and connectivity and glymphatic function. The group predominantly uses magnetic resonance imaging, however other approaches such as EEG, multiphoton microscopy, and functional ultrasound are developed and used. 

{% include section.html %}

## Latest

{% assign latest = site.data.citations | sort: "date" | reverse | first %}
{% include citation.html
  id=latest.id
  title=latest.title
  authors=latest.authors
  publisher=latest.publisher
  date=latest.date
  link=latest.link
  orcid=latest.orcid
  plugin=latest.plugin
  file=latest.file
  style="rich"
%}

{% include section.html %}

## All

{% include search-box.html %}

{% include search-info.html %}

{% include list.html data="citations" component="citation" style="rich" %}
