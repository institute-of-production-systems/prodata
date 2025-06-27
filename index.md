---
layout: splash
title: "ProData Projekt"
permalink: /
header:
  overlay_color: "#2c5aa0"
  overlay_image: /assets/images/prodata-header.jpg
  overlay_filter: 0.5
  actions:
    - label: "Mehr erfahren"
      url: "/research/"
      class: "btn--light-outline btn--large"
excerpt: "Prozessketten-übergreifende Detektion von Material- und Prozessanomalien bei Imbalanced Data für technische Kunststoffbaugruppen"
intro: 
  - excerpt: "Ein BMBF-Vorhaben zur 'Stärkung der Datenkompetenzen des wissenschaftlichen Nachwuchses'"
feature_row:
  - image_path: /assets/images/problemstellung.jpg
    title: "🎯 Problemstellung"
    excerpt: "Die zentrale Problemstellung des Vorhabens besteht darin, **Anomalien in der Kunststoffverarbeitung und Montage** zu erkennen und vorherzusagen, insbesondere in Szenarien mit **unausgeglichenen Daten (Imbalanced Data)**."
    url: "/research/#problemstellung"
    btn_label: "Details"
    btn_class: "btn--primary"
  - image_path: /assets/images/forschung.jpg
    title: "🔬 Forschungsbedarf"
    excerpt: "Es besteht ein Bedarf an **effektiven Techniken und Methoden**, um diese Daten effizient zu analysieren und Prozess- und Materialanomalien zu erkennen, um die Prozess- und Bauteilqualität proaktiv und prädiktiv zu überwachen."
    url: "/research/#forschungsbedarf"
    btn_label: "Mehr erfahren"
    btn_class: "btn--primary"
  - image_path: /assets/images/zielsetzung.jpg
    title: "🎯 Zielsetzung"
    excerpt: "Das Ziel ist, eine **durchgängige Beschreibung der Prozesszustände** im Spritzgießprozess sowie im Montageprozess auf der Grundlage der verfügbaren Material- und Prozessdaten zu erstellen."
    url: "/research/#zielsetzung"
    btn_label: "Erfahren Sie mehr"
    btn_class: "btn--primary"
feature_row2:
  - image_path: /assets/images/rif-logo.png
    alt: "RIF Institut"
    title: "RIF Institut für Forschung und Transfer e.V."
    excerpt: "Die Abteilung Arbeits- und Produktionssysteme verfügt über umfassende Datenkompetenzen durch eine lange Historie heterogener ML-Umsetzungen in der produzierenden Industrie."
    url: "https://www.rif-ev.de/"
    btn_label: "Website besuchen"
    btn_class: "btn--inverse"
  - image_path: /assets/images/ifw-logo.png
    alt: "Institut für Werkstofftechnik"
    title: "Institut für Werkstofftechnik, Universität Kassel"
    excerpt: "Das Fachgebiet Kunststofftechnik beschäftigt sich unter anderem mit der Verknüpfung von Prozessparametern in der Kunststoffverarbeitung und den resultierenden Prüfkörpereigenschaften."
    url: "https://www.uni-kassel.de/maschinenbau/institute/werkstofftechnik"
    btn_label: "Website besuchen"
    btn_class: "btn--inverse"
---

{% include feature_row id="intro" type="center" %}

{% include feature_row %}

## 🏛️ Projektpartner

{% include feature_row id="feature_row2" %}

## 📢 Aktuelle News

<div class="news-preview">
{% assign recent_posts = site.posts | where_exp: "post", "post.categories contains 'news'" | limit: 3 %}
{% if recent_posts.size > 0 %}
  {% for post in recent_posts %}
  <div class="news-item">
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <p class="post-meta">{{ post.date | date: "%d.%m.%Y" }}{% if post.categories %} • {{ post.categories | join: ", " }}{% endif %}</p>
    <p>{{ post.excerpt | strip_html | truncatewords: 25 }}</p>
    <a href="{{ post.url | relative_url }}" class="btn btn--primary btn--small">Weiterlesen</a>
  </div>
  {% endfor %}
{% else %}
  <p>Bald finden Sie hier aktuelle Neuigkeiten zum ProData-Projekt.</p>
{% endif %}
</div>

[Alle News anzeigen](/news/){: .btn .btn--primary .btn--large}

---

## 📞 Kontakt

**Kontaktieren Sie uns bei weiteren Fragen!**

Falls Sie Anregungen zum Forschungsvorhaben, Rückfragen zu Zwischenergebnissen oder weiterführendes Interesse an einer Zusammenarbeit haben, kontaktieren Sie uns gerne.

<div class="contact-grid">
{% for partner in site.project.partners %}
<div class="contact-card">
  <h4>{{ partner.name }}</h4>
  <p><strong>{{ partner.leader }}</strong></p>
  <p>📧 <a href="mailto:{{ partner.email }}">{{ partner.email }}</a></p>
  <p>🌐 <a href="{{ partner.url }}" target="_blank">{{ partner.name }}</a></p>
</div>
{% endfor %}
</div>

---

<div class="funding-notice">
  <h4>Förderhinweis</h4>
  <p>Das Forschungsvorhaben <strong>ProData</strong> (Förderkennzeichen: <strong>{{ site.project.foerderkennzeichen }}</strong>) wird im Rahmen des Förderprogramms „{{ site.project.funding_program }}" vom Bundesministerium für Bildung und Forschung (BMBF) sowie im Rahmen des Förderprogramms „NextGenerationEU" von der Europäischen Union gefördert und vom Projektträger VDI/VDE betreut.</p>
</div>