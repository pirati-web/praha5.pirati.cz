---
layout: communal-elections
title: Volby do Zastupitelstva hl. města Prahy 2022
campaignGroupUid: volby-2022
campaignCategoryUid: 2022-komunalni
candidateListUid: 2022-komunalni
customizeHeader: true
---

{% capture mainContent %}
  <h1 class="head-alt-lg md:head-alt-xl text-center">Máme odvahu řídit Prahu 5 správně</h1>
{% endcapture %}

{% capture subContent %}
  <h2 class="head-xs md:head-base mt-2 text-center"><strong>Přijďte k volbám: 23.-24.9.2022!</strong></h2>
  <h2 class="head-xs md:head-base mt-2 text-center"><strong>Naše kandidátní listina má číslo 8!</strong></h2>
{% endcapture %}

{% assign candidates = site.candidatelists | where: "uid", page.candidateListUid | first %}

{% include elections-header.html img=page.img bgImg=page.heroBgImg mainContent=mainContent subContent=subContent candidateListNumber=candidates.number %}
