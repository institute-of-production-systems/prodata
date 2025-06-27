---
layout: single
title: "Forschung"
permalink: /research/
toc: true
toc_label: "Forschungsübersicht"
toc_sticky: true
header:
  overlay_color: "#2c5aa0"
  overlay_filter: 0.5
---

# Prozessketten-übergreifende Detektion von Material- und Prozessanomalien bei Imbalanced Data für technische Kunststoffbaugruppen (ProData)

## Ein BMBF-Vorhaben zur „Stärkung der Datenkompetenzen des wissenschaftlichen Nachwuchses"

---

## 🎯 Problemstellung {#problemstellung}

Die zentrale Problemstellung des Vorhabens besteht darin, **Anomalien in der Kunststoffverarbeitung und Montage** zu erkennen und vorherzusagen, insbesondere in Szenarien mit **unausgeglichenen Daten (Imbalanced Data)**. 

Die verfügbaren Daten aus diesen Prozessen haben typischerweise viele Normalzustände, aber nur wenige Beispiele für anomale Zustände, was das Machine-Learning-Modelltraining herausfordernd macht.

### Herausforderungen:
- **Unausgeglichene Datensätze** mit wenigen Anomalien
- **Komplexe Prozessketten** in der Kunststoffverarbeitung
- **Vielfältige Fehlerquellen** in Spritzgieß- und Montageprozessen
- **Zeitkritische Fehlererkennung** für Qualitätssicherung

---

## 🔬 Forschungsbedarf {#forschungsbedarf}

Es besteht ein Bedarf an **effektiven Techniken und Methoden**, um diese Daten effizient zu analysieren und Prozess- und Materialanomalien zu erkennen, um die Prozess- und Bauteilqualität proaktiv und prädiktiv zu überwachen und zu verbessern. 

Da die Datenauswertung und -analyse im Kontext der Kunststoffverarbeitung bislang überwiegend **manuell und mit einfachen Werkzeugen** wie Excel durchgeführt wird, besteht ein großes Potenzial für Verbesserungen durch die Anwendung fortschrittlicher datenwissenschaftlicher Methoden.

### Aktuelle Limitierungen:
- **Manuelle Datenauswertung** mit Excel
- **Reaktive statt prädiktive** Qualitätssicherung
- **Begrenzte Mustererkennung** bei komplexen Daten
- **Fehlende prozessketten-übergreifende** Analyse

---

## 🎯 Zielsetzung {#zielsetzung}

Das Ziel ist, eine **durchgängige Beschreibung der Prozesszustände** im Spritzgießprozess sowie im Montageprozess auf der Grundlage der verfügbaren Material- und Prozessdaten zu erstellen, um letztendlich die Prozess- und Bauteilqualität zu verbessern.

### Konkrete Ziele:
1. **Entwicklung** von ML-Methoden für Anomalieerkennung in imbalanced data
2. **Prozessketten-übergreifende** Qualitätssicherung implementieren
3. **Prädiktive Wartung** und Prozessoptimierung ermöglichen
4. **Datenkompetenzen** des wissenschaftlichen Nachwuchses stärken

---

## 🔬 Forschungsfragen

Im Rahmen des Projekts **„ProData"** werden folgende zentrale Fragen untersucht:

### 1. Datenbasierte Anomalien in Spritzgießprozessen
**Inwieweit lassen sich mithilfe datenbasierter Methoden Anomalien in den Spritzgießprozessen identifizieren?**

### 2. Imbalanced Data für unüberwachte Anomaliedetektion  
**Wie können ungleichgewichtete Datensätze aus Schraubprozessen systematisch für die unüberwachte Anomaliedetektion unter Verwendung von Zeitreihen-Clustering-Verfahren genutzt werden?**

### 3. Prozessketten-übergreifende Anomalieidentifikation
**Welche Anomalien können prozessketten-übergreifend basierend auf den Rohmaterialien sowie potenziellen Fehlerclustern in Spritzgieß- und Schraubprozessen identifiziert werden?**

### 4. Assoziationen und Fehlerursachen
**Welche Assoziationen und Fehlerursachen können auf der Grundlage der identifizierten Anomalien ermittelt werden?**

---

## 🤖 Methodischer Ansatz

### Machine Learning Verfahren
Das Projekt setzt auf eine breite Palette von ML-Verfahren:

- **Überwachte Lernverfahren** (Supervised Learning)
- **Unüberwachte Lernverfahren** (Unsupervised Learning)  
- **Semi-überwachte Lernverfahren** (Semi-supervised Learning)
- **Bestärkende Lernverfahren** (Reinforcement Learning)

### Anwendungsgebiete
- **Spritzgießprozesse**
- **Montage und Schraubverbindungen**
- **Materialcharakterisierung**
- **Qualitätsprüfung**

---

## 📊 Projektdaten

<div class="project-info-grid">
  <div class="info-card">
    <h4>Projektlaufzeit</h4>
    <p>{{ site.project.start_date }} - {{ site.project.end_date }}</p>
  </div>
  
  <div class="info-card">
    <h4>Förderkennzeichen</h4>
    <p>{{ site.project.foerderkennzeichen }}</p>
  </div>
  
  <div class="info-card">
    <h4>Projektpartner</h4>
    <p>{{ site.project.partners.size }} Institutionen</p>
  </div>
  
  <div class="info-card">
    <h4>Förderprogramm</h4>
    <p>{{ site.project.funding_program }}</p>
  </div>
</div>

---

## 🚀 Erwartete Ergebnisse

### Wissenschaftliche Beiträge
- **Neue ML-Algorithmen** für imbalanced data in der Fertigung
- **Prozessketten-übergreifende** Anomalieerkennungsverfahren
- **Validierte Methoden** für Kunststoffverarbeitung
- **Open-Source Software** und Datensätze

### Praktische Auswirkungen
- **Verbesserte Qualitätssicherung** in der Produktion
- **Reduzierte Ausschussraten** und Kosten
- **Prädiktive Wartungsstrategien**
- **Erhöhte Prozessstabilität**

### Kompetenzentwicklung
- **Geschulte Nachwuchswissenschaftler** in Data Science
- **Transferable Skills** für Industrie 4.0
- **Interdisziplinäre Zusammenarbeit** zwischen Instituten

---

## 📈 Aktueller Projektstand

{% assign latest_milestone = site.posts | where_exp: "post", "post.categories contains 'news'" | first %}
{% if latest_milestone %}
**Neueste Entwicklung:** [{{ latest_milestone.title }}]({{ latest_milestone.url | relative_url }}) ({{ latest_milestone.date | date: "%B %Y" }})
{% endif %}

Für aktuelle Projektupdates besuchen Sie unsere [News-Seite](/news/).

---

## 🔗 Weiterführende Informationen

- **BMBF Förderprogramm:** [Stärkung der Datenkompetenzen des wissenschaftlichen Nachwuchses](https://www.bildung-forschung.digital/digitalezukunft/de/wissen/forschungsdaten/datenkompetenzen-wiss-nachwuchs/datenkompetenz-wiss-nachwuchs_node.html)
- **Publikationen:** [Alle Veröffentlichungen](/publications/)
- **Projektpartner:** [Partner-Informationen](/partners/)