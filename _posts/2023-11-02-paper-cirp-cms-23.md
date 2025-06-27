---
layout: single
title: "Unsupervised Anomaly Detection in Unbalanced Time Series Data from Screw Driving Processes using k-means Clustering"
date: 2023-11-02 14:00:00 +0200
categories: [news, publications]  # 👈 KEY CHANGE: appears in BOTH sections!
tags: [Anomaly Detection, Time Series Clustering, Unsupervised Learning, Screw Driving, Machine Learning, Manufacturing, K-Means, Dynamic Time Warping]
author: ProData Team
toc: true
toc_sticky: true
share: true
related: true

# Publication-specific metadata
journal: "Procedia CIRP"
volume: "120"
pages: "1185-1190"
year: "2023"
doi: "10.1016/j.procir.2023.09.146"
authors: "West, N., Schlegl, T., Deuse, J."
keywords: [Anomaly Detection, Time Series Clustering, Unsupervised Learning, Screw Driving, Machine Learning, Tightening Data, Manufacturing, Open Source]
bibtex_key: "west2023unsupervised"
pdf_url: "https://doi.org/10.1016/j.procir.2023.09.146"
reading_time: 6

# Header image (optional)
header:
  teaser: /assets/images/clustering-teaser.jpg
  overlay_image: /assets/images/time-series-bg.jpg
  overlay_filter: 0.4

# Abstract and excerpt
abstract: "Since bolted joints are ubiquitous in manufacturing, their effective and reliable quality assurance is particularly important. Most tightening processes rely on statistical methods to detect faulty screw connections already during assembly. In this paper, we address the detection of faulty tightening processes using a clustering based approach from the field of Unsupervised Machine Learning. In particular, we deploy the k-Means algorithm on a real-world dataset from the automotive industry. The model uses Dynamic Time Warping to determine the similarity between the normal and abnormal tightening processes, treating each one as an independent temporal sequence. This approach offers three advantages compared to existing supervised methods: 1.) time series with different lengths can be utilized without extensive preprocessing steps, 2.) errors never seen before can be detected using the unsupervised approach, and 3.) extensive manual efforts to generate labels are no longer necessary. To evaluate the approach, it is applied in a scenario where actual class labels are available. This allows evaluating the clustering results using traditional classification scores. The approach manages to achieve an accuracy of up to 88.89% and a macro-average F1-score of up to 63.65%."

excerpt: "Clustering-basierter Ansatz zur unüberwachten Erkennung von Anomalien in Schraubprozessen mit k-Means und Dynamic Time Warping. Erreicht 88,89% Genauigkeit ohne manuelle Labels."
---

# Ansatz zur unüberwachten Erkennung von Anomalien erschienen

Da **Schraubverbindungen in der Fertigung allgegenwärtig** sind, ist ihre effektive und zuverlässige Qualitätssicherung besonders wichtig. Wir stellen einen **clusterbasierten Ansatz zur unüberwachten Erkennung** von fehlerhaften Schraubvorgängen vor.

## 🔩 Herausforderung: Qualitätssicherung bei Schraubverbindungen

Die meisten Anziehverfahren stützen sich auf **statistische Methoden**, um fehlerhafte Schraubverbindungen bereits während der Montage zu erkennen. Diese traditionellen Ansätze haben jedoch Limitierungen:

- **Hoher manueller Aufwand** für Labeling
- **Begrenzte Erkennungsrate** für unbekannte Fehler
- **Aufwändige Datenvorverarbeitung** für unterschiedliche Zeitreihenlängen

## 🧠 Unser innovativer Ansatz

In diesem Beitrag befassen wir uns mit der **Erkennung von fehlerhaften Schraubvorgängen** mit Hilfe eines **clusterbasierten Ansatzes** aus dem Bereich des unüberwachten maschinellen Lernens.

### 🎯 Methodischer Ansatz

Insbesondere wenden wir den **k-Means-Algorithmus** auf einen realen Datensatz aus der **Automobilindustrie** an. Das Modell verwendet **Dynamic Time Warping**, um die Ähnlichkeit zwischen normalen und abnormalen Schraubvorgängen zu bestimmen, wobei jeder Vorgang als **unabhängige zeitliche Sequenz** behandelt wird.

### ⚡ Technische Innovation

**Dynamic Time Warping (DTW)** ist eine Technik, die es ermöglicht:
- **Zeitreihen unterschiedlicher Längen** zu vergleichen
- **Ähnlichkeitsmuster** auch bei zeitlichen Verschiebungen zu erkennen
- **Robuste Distanzmessungen** zwischen Sequenzen durchzuführen

## ✅ Drei entscheidende Vorteile

Dieser Ansatz bietet **drei Vorteile** gegenüber bestehenden überwachten Methoden:

### 1. 📏 Flexible Zeitreihenlängen
**Zeitreihen mit unterschiedlichen Längen** können ohne umfangreiche Vorverarbeitungsschritte genutzt werden

### 2. 🔍 Erkennung unbekannter Fehler  
**Bisher unbekannte Fehler** können mit dem unüberwachten Ansatz erkannt werden

### 3. 🏷️ Keine manuellen Labels nötig
**Umfangreiche manuelle Anstrengungen** zur Erzeugung von Labels sind nicht mehr notwendig

## 📊 Beeindruckende Ergebnisse

Um den Ansatz zu evaluieren, wird er in einem **Szenario angewendet, in dem tatsächliche Klassenlabels verfügbar** sind. Dies ermöglicht die Bewertung der Clustering-Ergebnisse anhand traditioneller Klassifizierungsergebnisse.

### 🎯 Leistungskennzahlen

Der Ansatz erreicht:
- ✅ **Genauigkeit von bis zu 88,89%**
- ✅ **Makro-durchschnittlicher F1-Score von bis zu 63,65%**

Diese Ergebnisse zeigen, dass **unüberwachte Verfahren** eine viable Alternative zu überwachten Methoden darstellen, insbesondere in Szenarien mit:
- **Limitierten gelabelten Daten**
- **Unbekannten Fehlermustern**
- **Zeitreihen unterschiedlicher Längen**

## 🔬 Wissenschaftliche Methodik

### **k-Means Clustering mit Dynamic Time Warping**

Die Kombination von **k-Means Clustering** mit **Dynamic Time Warping** ermöglicht:
- **Gruppierung ähnlicher Schraubprozesse** basierend auf Zeitreihenmustern
- **Flexible Behandlung** von Zeitreihen unterschiedlicher Längen
- **Automatische Anomalieerkennung** ohne Vorabwissen über Fehlertypen

### **Unbalanced Time Series Data**

Ein besonderer Fokus liegt auf **unausgeglichenen Zeitreihendaten**:
- **Viele normale Schraubvorgänge** vs. wenige fehlerhafte
- **Realistische Produktionsszenarien** mit hoher Prozessstabilität
- **Statistische Herausforderungen** bei der Anomalieerkennung

## 🔬 Wissenschaftlicher Beitrag

Diese Veröffentlichung ist ein wichtiger **Beitrag im ProData-Projekt** und zeigt, wie **fortschrittliche Machine Learning Methoden** zur Lösung realer Industrieprobleme eingesetzt werden können.

### 📖 Open Source Verfügbarkeit

Die **Schritte zur Analyse** wurden **öffentlich zugänglich** gemacht, um die Reproduzierbarkeit und weitere Forschung zu fördern:
- **GitHub Repository** verfügbar unter: [github.com/nikolaiwest/2022-anomaly-detection-cirp](https://github.com/nikolaiwest/2022-anomaly-detection-cirp)
- **Vollständige Implementierung** des k-Means + DTW Ansatzes
- **Datensatz-Struktur** und Preprocessing-Pipeline

## 🚀 Ausblick

Diese Forschungsarbeit bildet eine **wichtige Grundlage** für weitere Entwicklungen im Bereich der:
- **Unüberwachten Anomalieerkennung**
- **Industriellen Qualitätssicherung**  
- **Zeitreihenanalyse in der Produktion**

Die Ergebnisse werden auch in die **Spritzgussdaten-Analyse** des ProData-Projekts einfließen, um ähnliche Ansätze in der **Kunststoffverarbeitung** zu entwickeln.

## 🔗 Technische Details

### **Algorithmus-Pipeline:**
1. **Datensammlung** von Schraubprozessen (Drehmoment-Zeit-Verläufe)
2. **Dynamic Time Warping** zur Ähnlichkeitsmessung
3. **k-Means Clustering** zur Gruppierung ähnlicher Prozesse
4. **Anomalieerkennung** basierend auf Cluster-Zugehörigkeit
5. **Evaluierung** mit traditionellen Klassifizierungsmetriken

### **Datencharakteristika:**
- **Zeitreihen unterschiedlicher Längen** (flexibel)
- **Automotive Produktionsdaten** (real-world)
- **Unbalancierte Verteilung** (realistisch)
- **Temporal sequential data** (Drehmoment-Verläufe)

## 🌟 Bedeutung für ProData

Diese Studie demonstriert:
- **Erfolgreiche Anwendung** unüberwachter ML-Methoden in der Produktion
- **Praktikabilität** von Clustering-Ansätzen für Anomalieerkennung
- **Grundlagen** für die Übertragung auf Kunststoffverarbeitungsprozesse
- **Open Science Ansatz** mit verfügbarer Implementierung

---

## 📚 Publikationsdetails

**Vollständige Zitation:**
> West, N., Schlegl, T., & Deuse, J. (2023). Unsupervised anomaly detection in unbalanced time series data from screw driving processes using k-means clustering. *Procedia CIRP*, 120, 1185-1190. https://doi.org/10.1016/j.procir.2023.09.146

**BibTeX:**
```bibtex
@article{west2023unsupervised,
  title={Unsupervised anomaly detection in unbalanced time series data from screw driving processes using k-means clustering},
  author={West, Nikolai and Schlegl, Thomas and Deuse, Jochen},
  journal={Procedia CIRP},
  volume={120},
  pages={1185--1190},
  year={2023},
  publisher={Elsevier},
  doi={10.1016/j.procir.2023.09.146}
}
```

**Links:**
- 📄 [Volltext (Open Access)](https://doi.org/10.1016/j.procir.2023.09.146)
- 💻 [GitHub Repository](https://github.com/nikolaiwest/2022-anomaly-detection-cirp)
- 🔗 [DOI: 10.1016/j.procir.2023.09.146](https://doi.org/10.1016/j.procir.2023.09.146)

---

**Open Access:** Die vollständige Veröffentlichung ist unter Creative Commons Lizenz verfügbar.

**Reproduzierbarkeit:** Code und Implementierungsdetails sind öffentlich auf GitHub verfügbar für weitere Forschung und industrielle Anwendungen.