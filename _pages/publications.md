---
layout: page
title: Publications
permalink: /publications/
description: Peer-reviewed articles, conference papers, preprints, and published books and translations.
nav: true
nav_order: 3
---

<style>
/* Compact publications layout */

ol.bibliography {
  list-style: none !important;
  padding-left: 0 !important;
  margin: 0 !important;
}

ol.bibliography > li {
  list-style: none !important;
  padding: 10px 0 14px !important;
  margin: 0 !important;
  border-bottom: 1px solid rgba(150,150,150,0.18);
  font-size: 14px !important;
  line-height: 1.45 !important;
}

ol.bibliography > li::marker {
  content: "";
}

/* Article titles */
ol.bibliography .title,
ol.bibliography .title a {
  font-size: 15px !important;
  font-weight: 500 !important;
  line-height: 1.4 !important;
}

/* Authors */
ol.bibliography .author {
  font-size: 14px !important;
  line-height: 1.45 !important;
}

/* Journal and conference information */
ol.bibliography .periodical {
  font-size: 13px !important;
  line-height: 1.45 !important;
}

/* Publication links */
ol.bibliography .links {
  margin-top: 5px !important;
}

ol.bibliography .links a {
  font-size: 12px !important;
}

/* Year headings */
.publications h2,
.publications h3 {
  font-size: 21px !important;
  font-weight: 400 !important;
}

/* Mobile */
@media (max-width: 768px) {
  ol.bibliography .title,
  ol.bibliography .title a {
    font-size: 14px !important;
  }

  ol.bibliography .author {
    font-size: 13px !important;
  }

  ol.bibliography .periodical {
    font-size: 12px !important;
  }
}
</style>

This page lists my published scholarly work, conference papers, publicly available preprints, and published books and translations. Journal articles and preprints are listed separately to distinguish peer-reviewed research from manuscripts deposited in repositories.

## Journal Articles

{% bibliography --query @article %}

## Conference Papers

{% bibliography --query @inproceedings %}

## Preprints

{% bibliography --query @unpublished %}

## Books & Scholarly Translations

{% bibliography --query @book %}
