---
layout: page
title: Publications
permalink: /publications/
description: Peer-reviewed articles, conference papers, preprints, and published books and translations.
nav: true
nav_order: 3
---

/* Reduce spacing around publication links */
ol.bibliography .links {
  margin-top: 2px !important;
  margin-bottom: 0 !important;
  padding: 0 !important;
}

ol.bibliography .links a,
ol.bibliography .links .btn {
  margin-top: 0 !important;
  margin-bottom: 0 !important;
}

ol.bibliography .links + * {
  margin-top: 0 !important;
}

<style>
/* Publications: clean, compact academic style */

/* Publication list */
ol.bibliography {
  list-style: none !important;
  padding: 0 !important;
  margin: 0 0 24px !important;
}

/* Individual publications */
ol.bibliography > li {
  list-style: none !important;
  padding: 14px 0 !important;
  margin: 0 !important;
  border-bottom: 1px solid rgba(150, 150, 150, 0.22);
  font-size: 14px !important;
  line-height: 1.5 !important;
}

ol.bibliography > li::marker {
  content: "";
}

/* Paper titles */
ol.bibliography .title,
ol.bibliography .title a,
ol.bibliography .title b,
ol.bibliography .title strong {
  font-size: 15px !important;
  font-weight: 500 !important;
  line-height: 1.45 !important;
}

/* Authors */
ol.bibliography .author,
ol.bibliography .author a {
  font-size: 14px !important;
  font-weight: 400 !important;
  line-height: 1.5 !important;
}

/* Journal or conference */
ol.bibliography .periodical {
  font-size: 13px !important;
  font-weight: 400 !important;
  line-height: 1.5 !important;
}

/* DOI and publication buttons */
ol.bibliography .links {
  margin-top: 6px !important;
}

ol.bibliography .links a,
ol.bibliography .links .btn {
  font-size: 12px !important;
}

/* Year headings */
h2.bibliography,
h3.bibliography {
  font-size: 20px !important;
  font-weight: 400 !important;
  line-height: 1.3 !important;
  color: #888 !important;
  margin: 20px 0 8px !important;
}

/* Mobile */
@media (max-width: 768px) {
  ol.bibliography > li {
    padding: 12px 0 !important;
  }

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

  h2.bibliography,
  h3.bibliography {
    font-size: 18px !important;
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
