---
layout: single
title: "Veröffentlichungen"
permalink: /publications/
toc: true
toc_label: "Inhalt"
toc_sticky: true
---

Hier finden Sie alle wissenschaftlichen Publikationen und Forschungsergebnisse des ProData-Projekts. Unsere Arbeit trägt zur Weiterentwicklung von Machine Learning Methoden in der Materialforschung und Produktionstechnik bei.

## 📚 Alle Publikationen

{% assign publications = site.posts | where_exp: "post", "post.categories contains 'publications'" | sort: "date" | reverse %}

{% if publications.size > 0 %}
<div class="publications-table">
  <table>
    <thead>
      <tr>
        <th>Titel</th>
        <th>Autoren</th>
        <th>Venue</th>
        <th>Jahr</th>
        <th>Links</th>
      </tr>
    </thead>
    <tbody>
      {% for pub in publications %}
      <tr>
        <td><a href="{{ pub.url | relative_url }}"><strong>{{ pub.title }}</strong></a></td>
        <td>{{ pub.authors | default: "ProData Team" }}</td>
        <td>
          {% if pub.journal %}{{ pub.journal }}{% endif %}
          {% if pub.conference %}{{ pub.conference }}{% endif %}
        </td>
        <td>{{ pub.year | default: pub.date | date: "%Y" }}</td>
        <td>
          <a href="{{ pub.url | relative_url }}" class="btn btn--primary btn--small">Details</a>
          {% if pub.doi %}
          <a href="https://doi.org/{{ pub.doi }}" class="btn btn--inverse btn--small" target="_blank">DOI</a>
          {% endif %}
          {% if pub.pdf_url %}
          <a href="{{ pub.pdf_url }}" class="btn btn--inverse btn--small" target="_blank">PDF</a>
          {% endif %}
        </td>
      </tr>
      {% endfor %}
    </tbody>
  </table>
</div>

## 📖 Publikationen im Detail

{% for publication in publications %}
<article class="publication-preview">
  <header>
    <h3><a href="{{ publication.url | relative_url }}">{{ publication.title }}</a></h3>
    {% if publication.journal %}
      <p class="publication-venue"><strong>{{ publication.journal }}</strong>{% if publication.year %}, {{ publication.year }}{% endif %}</p>
    {% elsif publication.conference %}
      <p class="publication-venue"><strong>{{ publication.conference }}</strong>{% if publication.year %}, {{ publication.year }}{% endif %}</p>
    {% endif %}
  </header>
  
  {% if publication.authors %}
  <p class="authors"><strong>Autoren:</strong> {{ publication.authors }}</p>
  {% endif %}
  
  {% if publication.abstract %}
  <div class="abstract">
    <p>{{ publication.abstract | truncatewords: 50 }}</p>
  </div>
  {% endif %}
  
  <div class="publication-actions">
    <a href="{{ publication.url | relative_url }}" class="btn btn--primary">Vollständige Details</a>
    {% if publication.doi %}
    <a href="https://doi.org/{{ publication.doi }}" target="_blank" class="btn btn--inverse">Paper öffnen</a>
    {% endif %}
  </div>
  
  {% if publication.keywords and publication.keywords.size > 0 %}
  <div class="keywords">
    {% for keyword in publication.keywords %}
    <span class="keyword-tag">{{ keyword }}</span>
    {% endfor %}
  </div>
  {% endif %}
</article>
{% endfor %}

{% else %}
<div class="no-publications">
  <h3>Noch keine Publikationen verfügbar</h3>
  <p>Die ersten wissenschaftlichen Veröffentlichungen des ProData-Projekts werden bald hier erscheinen.</p>
</div>
{% endif %}

---

## 📊 Publikationsstatistiken

<div class="stats-grid">
  <div class="stat-card">
    <h4>{{ publications.size }}</h4>
    <p>Veröffentlichungen</p>
  </div>
  
  <div class="stat-card">
    <h4>{{ site.time | date: "%Y" }}</h4>
    <p>Aktuelle Forschung</p>
  </div>
  
  <div class="stat-card">
    <h4>{{ site.project.partners.size }}</h4>
    <p>Forschungspartner</p>
  </div>
</div>

---

## 🔬 Forschungsgebiete

<div class="research-topics">
  <div class="topic-card">
    <h4>🤖 Machine Learning</h4>
    <p>Unüberwachte Lernverfahren, Anomalieerkennung, Clustering-Algorithmen</p>
  </div>
  
  <div class="topic-card">
    <h4>🏭 Produktionstechnik</h4>
    <p>Qualitätssicherung, Prozessoptimierung, Spritzgießverfahren</p>
  </div>
  
  <div class="topic-card">
    <h4>📊 Data Science</h4>
    <p>Zeitreihenanalyse, Imbalanced Data, Datenkompetenzen</p>
  </div>
  
  <div class="topic-card">
    <h4>🔧 Materialforschung</h4>
    <p>Kunststofftechnik, Schraubverbindungen, Qualitätskontrolle</p>
  </div>
</div>

---

## 📧 Kooperationen

**Interesse an Forschungskooperationen?**

Falls Sie Interesse an einer wissenschaftlichen Zusammenarbeit haben oder unsere Forschungsergebnisse in Ihrer Arbeit verwenden möchten, kontaktieren Sie uns gerne:

{% for partner in site.project.partners %}
- 📧 **{{ partner.name }}:** [{{ partner.email }}](mailto:{{ partner.email }})
{% endfor %}

**Projektförderung erwähnen:**
> "This work was supported by the German Federal Ministry of Education and Research (BMBF) under grant {{ site.project.foerderkennzeichen }} (ProData project)."