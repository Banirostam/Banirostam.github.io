---
layout: page
title: Publications
permalink: /publications/
description: Peer-reviewed articles, conference papers, preprints, and published books and translations.
nav: true
nav_order: 3
---

This page lists my published scholarly work, conference papers, publicly available preprints, and books and translations. Journal publications and preprints are listed separately to distinguish peer-reviewed research from manuscripts deposited in repositories.

## Journal Articles

{% bibliography --query @article %}

## Conference Papers

{% bibliography --query @inproceedings %}

## Preprints

The following works are available as preprints or repository deposits and are not presented here as peer-reviewed journal articles.

{% bibliography --query @unpublished %}

## Books & Scholarly Translations

This section includes co-authored books and Persian translations, including a three-chapter translation contribution. Details of individual roles are provided in each record.

{% bibliography --query @book %}

For additional indexing and citation information, visit my [Google Scholar profile](https://scholar.google.com/citations?user=Igai5DsAAAAJ).


<style>
/* Publications page: compact academic layout */

ol.bibliography {
  list-style: none !important;
  padding-left: 0 !important;
  margin: 0;
}

ol.bibliography > li {
  list-style: none !important;
  border-bottom: 1px solid rgba(150,150,150,0.22);
  padding: 14px 0;
  margin: 0 !important;
  font-size: 16px;
  line-height: 1.55;
}

ol.bibliography > li::marker {
  content: "";
}

ol.bibliography .title {
  font-size: 16px;
  font-weight: 600;
  line-height: 1.5;
}

ol.bibliography .author,
ol.bibliography .periodical {
  font-size: 15px;
  line-height: 1.5;
}

ol.bibliography .links {
  margin-top: 6px;
}

ol.bibliography .links a {
  font-size: 13px;
}

ol.bibliography > li:last-child {
  border-bottom: none;
}

@media (max-width: 768px) {
  ol.bibliography > li {
    font-size: 15px;
    padding: 12px 0;
  }
}
</style>
