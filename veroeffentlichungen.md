---
layout: default
title: "Veröffentlichungen"
---

# Veröffentlichungen

Hier finden Sie alle wissenschaftlichen Publikationen und Forschungsergebnisse des ProData-Projekts. Unsere Arbeit trägt zur Weiterentwicklung von Machine Learning Methoden in der Materialforschung und Produktionstechnik bei.

---

## 📚 Wissenschaftliche Papers

<div class="publications-list">
{% assign publications = site.posts | where: "category", "Publikation" | sort: "date" | reverse %}

{% if publications.size > 0 %}
  {% for publication in publications %}
  <article class="publication-item">
    <div class="publication-header">
      <h3><a href="{{ publication.url | relative_url }}">{{ publication.title }}</a></h3>
      {% if publication.journal %}
        <p class="publication-venue">{{ publication.journal }}{% if publication.year %}, {{ publication.year }}{% endif %}</p>
      {% elsif publication.conference %}
        <p class="publication-venue">{{ publication.conference }}{% if publication.year %}, {{ publication.year }}{% endif %}</p>
      {% endif %}
    </div>
    
    <div class="publication-meta">
      {% if publication.authors %}
        <p class="authors"><strong>Autoren:</strong> {{ publication.authors }}</p>
      {% endif %}
      
      {% if publication.doi %}
        <p class="doi"><strong>DOI:</strong> <a href="https://doi.org/{{ publication.doi }}" target="_blank" rel="noopener">{{ publication.doi }}</a></p>
      {% endif %}
    </div>
    
    {% if publication.abstract %}
    <div class="publication-abstract">
      <h4>Abstract</h4>
      <p>{{ publication.abstract | truncatewords: 50 }}</p>
    </div>
    {% endif %}
    
    <div class="publication-links">
      <a href="{{ publication.url | relative_url }}" class="btn btn-primary">Details anzeigen</a>
      {% if publication.doi %}
        <a href="https://doi.org/{{ publication.doi }}" target="_blank" rel="noopener" class="btn btn-outline">Paper öffnen ↗</a>
      {% endif %}
      {% if publication.pdf_url %}
        <a href="{{ publication.pdf_url }}" target="_blank" rel="noopener" class="btn btn-outline">PDF Download</a>
      {% endif %}
    </div>
    
    {% if publication.keywords and publication.keywords.size > 0 %}
    <div class="publication-keywords">
      {% for keyword in publication.keywords %}
        <span class="keyword">{{ keyword }}</span>
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
</div>

---

## 📊 Publikationsstatistiken

<div class="publication-stats">
  <div class="stat-item">
    <h4>{{ publications.size }}</h4>
    <p>Veröffentlichungen</p>
  </div>
  
  <div class="stat-item">
    <h4>{{ site.time | date: "%Y" }}</h4>
    <p>Aktuelle Forschung</p>
  </div>
  
  <div class="stat-item">
    <h4>2+</h4>
    <p>Forschungspartner</p>
  </div>
</div>

---

## 🔬 Forschungsgebiete

Unsere Publikationen decken folgende Schwerpunktbereiche ab:

<div class="research-areas">
  <div class="research-area">
    <h4>🤖 Machine Learning</h4>
    <p>Unüberwachte Lernverfahren, Anomalieerkennung, Clustering-Algorithmen</p>
  </div>
  
  <div class="research-area">
    <h4>🏭 Produktionstechnik</h4>
    <p>Qualitätssicherung, Prozessoptimierung, Spritzgießverfahren</p>
  </div>
  
  <div class="research-area">
    <h4>📊 Data Science</h4>
    <p>Zeitreihenanalyse, Imbalanced Data, Datenkompetenzen</p>
  </div>
  
  <div class="research-area">
    <h4>🔧 Materialforschung</h4>
    <p>Kunststofftechnik, Schraubverbindungen, Qualitätskontrolle</p>
  </div>
</div>

---

## 📧 Kooperationen

**Interesse an Forschungskooperationen?**

Falls Sie Interesse an einer wissenschaftlichen Zusammenarbeit haben oder unsere Forschungsergebnisse in Ihrer Arbeit verwenden möchten, kontaktieren Sie uns gerne:

- 📧 **RIF Institut:** [deuse@rif-ev.de](mailto:deuse@rif-ev.de)
- 📧 **Universität Kassel:** [heim@uni-kassel.de](mailto:heim@uni-kassel.de)

---

## 📖 Zitationen

Bei der Verwendung unserer Forschungsergebnisse bitten wir um entsprechende Zitation. Die vollständigen Zitierinformationen finden Sie auf den jeweiligen Publikationsseiten.

**Projektförderung erwähnen:**
> "This work was supported by the German Federal Ministry of Education and Research (BMBF) under grant 16DKWN119A (ProData project)."