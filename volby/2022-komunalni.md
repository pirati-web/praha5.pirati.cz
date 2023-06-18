---
layout: communal-elections
title: Volby do Zastupitelstva hl. města Prahy 2022
campaignGroupUid: volby-2022
campaignCategoryUid: 2022-komunalni
candidateListUid: 2022-komunalni
customizeHeader: true
---

{% capture mainContent %}
  <h1 class="head-alt-lg md:head-alt-xl text-center">Děkujeme za vaše hlasy ve volbách!</h1>

<h3> Koaliční smlouva pro období 2022-2026 ke stažení [zde](https://praha5.pirati.cz/assets/Koaliční_smlouva-P5-2022-2026.pdf).</h3>

{% endcapture %}


{% assign candidates = site.candidatelists | where: "uid", page.candidateListUid | first %}

{% include elections-header.html img=page.img bgImg=page.heroBgImg mainContent=mainContent subContent=subContent candidateListNumber=candidates.number %}
