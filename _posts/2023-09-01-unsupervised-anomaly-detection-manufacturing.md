---
layout: publication
title: "Comparative Study of Machine Learning Methods for Anomaly Detection in Screwing Data"
date: 2024-01-03 14:00:00 +0200
category: Publikation
lang: de
conference: "57th Hawaii International Conference on System Sciences (HICSS-57)"
year: "2024"
location: "Honolulu, Hawaii, USA"
doi: "10.24251/HICSS.2024.127"
authors: "West, N., Deuse, J."
keywords: ["Machine Learning", "Anomaly Detection", "Screwing Process", "Supervised Learning", "Unsupervised Learning", "Manufacturing", "Quality Control"]
abstract: "Effective and reliable quality assurance for screw connections is particularly important due to their frequency in manufacturing. Quality assurance includes the detection of anomalies at the earliest possible time, ideally during assembly. To reduce error rates, rework or scrap costs, and reputational damage, many companies have so far relied on statistical process control (SPC). Statistical methods for quality monitoring are usually associated with high personnel and time costs. For this reason, various machine learning methods for detecting anomalies in screwing data are analyzed. The goal is to minimize the need for human data inspection and anomaly detection while detecting errors with higher accuracy, consistency, and efficiency. This study compares eight different machine learning approaches (four supervised and four unsupervised) on real-world screwing data from an automated assembly station. The dataset contains torque-angle curves from screw connections with OK/NOK classifications, representing typical imbalanced data scenarios in manufacturing. Random Forest achieved the highest accuracy and macro-average F1-score, while unsupervised methods showed potential for detecting unknown anomaly patterns."
bibtex_key: "west2024comparative"
pdf_url: "https://scholarspace.manoa.hawaii.edu/items/c9ab7a99-c96e-47c1-b220-d516823795a3"
excerpt: "Vergleichsstudie von acht Machine Learning Methoden zur Anomalieerkennung in Schraubdaten mit Fokus auf überwachte vs. unüberwachte Ansätze."
reading_time: 8
---

# Systematischer Vergleich von ML-Methoden für Schraubdaten

Diese Publikation präsentiert eine **umfassende Vergleichsstudie** verschiedener Machine Learning Ansätze zur Anomalieerkennung in Schraubprozessen und adressiert damit ein zentrales Problem der modernen Qualitätssicherung.

## 🔧 Industrieller Kontext

### **Herausforderung der Schraubverbindungen:**
Aufgrund ihrer **Häufigkeit in der Fertigung** ist die effektive und zuverlässige Qualitätssicherung bei Schraubverbindungen besonders wichtig. Die Detektion von Anomalien sollte zum **frühestmöglichen Zeitpunkt** erfolgen, im besten Fall während der Montage.

### **Limitierungen bisheriger Ansätze:**
Viele Unternehmen setzen bisher auf **statistische Prozesskontrolle (SPC)**, die jedoch mit erheblichen Nachteilen verbunden ist:
- **Hoher personeller Aufwand** für Datenanalyse
- **Zeitaufwändige manuelle Inspektion**
- **Begrenzte Erkennungsgenauigkeit** bei komplexen Mustern
- **Reaktive statt proaktive** Qualitätssicherung

## 🎯 Zielsetzung der Studie

Das Ziel ist die **Minimierung menschlicher Inspektionen** bei gleichzeitiger Verbesserung der:
- ✅ **Genauigkeit** der Fehlererkennung
- ✅ **Konsistenz** der Qualitätsbewertung  
- ✅ **Effizienz** des Überwachungsprozesses

## 🔬 Experimenteller Aufbau

### **Datengrundlage:**
Die Studie verwendet Daten von einer **automatisierten Schraubstation** aus der industriellen Fertigung:

- **Zwei identische Verschraubungen** zur Verbindung von Kunststoffgehäuse-Elementen
- **Drehmoment-Drehwinkel-Verläufe** für jede Verschraubung aufgezeichnet
- **OK/NOK Klassifikation** basierend auf Zielwerten für Drehmoment und -winkel
- **Imbalanced Data** aufgrund der hohen Prozessstabilität

### **Besondere Herausforderungen:**
- **25 Wiederholungen** pro Bauteil mit progressiver Gewindeschneidung
- **Kein vorgeschnittenes Gewinde** - jede Verschraubung schneidet ein Gewinde
- **Prozessveränderungen** durch fortschreitende Materialermüdung

## 🧠 Untersuchte ML-Methoden

### **Vier Unüberwachte Verfahren:**

#### **1. Autoencoder**
- **Neural Network** basierte Dimensionsreduktion
- **Rekonstruktionsfehler** als Anomalie-Indikator
- Besonders geeignet für **komplexe, nichtlineare Muster**

#### **2. DBSCAN** 
- **Density-Based Spatial Clustering**
- Erkennt Cluster **beliebiger Form**
- **Automatische Ausreißer-Identifikation**

#### **3. Isolation Forest**
- **Tree-based** Anomalieerkennung
- **Effizient** bei hochdimensionalen Daten
- **Robuste Performance** bei imbalanced data

#### **4. Local Outlier Factor (LOF)**
- **Dichtebasierte** Anomalieerkennung
- Berücksichtigt **lokale Datenstrukturen**
- **Adaptive Schwellwerte** je nach Datenregion

### **Vier Überwachte Verfahren:**

#### **1. Random Forest**
- **Ensemble** von Entscheidungsbäumen
- **Robuste Performance** bei verschiedenen Datentypen
- **Feature Importance** für Interpretierbarkeit

#### **2. Long Short-Term Memory (LSTM)**
- **Recurrent Neural Network** für Zeitreihen
- **Memory-Mechanismus** für temporale Dependencies
- Ideal für **sequentielle Drehmoment-Drehwinkel-Verläufe**

#### **3. Convolutional Neural Network (CNN)**
- **Convolutional Layers** für Mustererkennung
- **Translation Invariance** für robuste Feature-Extraktion
- **Hierarchical Feature Learning**

#### **4. Encoder**
- **Neural Network** für Feature-Kompression
- **Dimensionsreduktion** mit Klasseninformation
- **Supervised Autoencoder** Architektur

## 📊 Evaluationsmetriken

### **Standardmetriken für Klassifikation:**
- **Accuracy** - Gesamtgenauigkeit der Vorhersagen
- **Precision** - Anteil echter Anomalien an erkannten Anomalien
- **Recall** - Anteil erkannter Anomalien an tatsächlichen Anomalien
- **Macro Average F1-Score** - Harmonisches Mittel für unbalancierte Klassen

### **Besondere Beachtung von Imbalanced Data:**
Da es sich um **stark unausgeglichene Daten** handelt (sehr wenige NOK gegenüber vielen OK), wurde besonderer Fokus auf **Precision-Recall Balance** gelegt.

## 🏆 Hauptergebnisse

### **Beste Performance: Random Forest**
- ✅ **Höchste Accuracy** unter allen getesteten Methoden
- ✅ **Höchster Macro Average F1-Score**
- ✅ **Robuste Performance** auch bei verschiedenen Datenaufteilungen
- ✅ **Interpretierbare Ergebnisse** durch Feature Importance

### **LSTM: Hohe Variabilität**
- **Große Schwankungen** in der Performance
- **Starke Abhängigkeit** von Hyperparameter-Einstellungen
- Verdeutlicht die **Bedeutung von Datenvorbereitung** und Parameteranpassung
- **Potenzial vorhanden**, aber **konsistente Optimierung** erforderlich

### **Unüberwachte Methoden: Vielversprechende Ergebnisse**
- **Effiziente Erkennung** bekannter Anomalien
- **Potential für unbekannte Fehlermuster**
- **Keine Labeling-Kosten** in der Anwendung
- **Reduzierte Abhängigkeit** von Expertenwissen

## 💡 Praktische Implikationen

### **Für die Industrie:**
- **Qualitätsverbesserung** durch frühe Fehlererkennung
- **Kostensenkung** durch reduzierte manuelle Inspection
- **Skalierbarkeit** auf verschiedene Schraubprozesse
- **Integration** in bestehende Qualitätssysteme möglich

### **Für die Forschung:**
- **Benchmark-Datensatz** für weitere Studien
- **Methodenvergleich** als Basis für Algorithmusentwicklung
- **Erkenntnisse** über Datenaufbereitung und Hyperparameter-Tuning

## 🔬 Methodische Beiträge

### **Systematische Evaluation:**
- **Konsistente Datenaufteilung** für alle Methoden
- **Standardisierte Metriken** für Vergleichbarkeit
- **Statistische Signifikanz** der Ergebnisse

### **Praxisrelevante Erkenntnisse:**
- **Feature Engineering** Strategien für Zeitreihen
- **Hyperparameter-Optimierung** für verschiedene Algorithmen
- **Data Preprocessing** Pipelines für industrielle Daten

## 🚀 Ausblick und zukünftige Arbeiten

### **Geplante Weiterentwicklungen:**
- **Detailliertere Untersuchungen** für ausgewählte Top-Performer
- **Vereinfachte Datensatz-Zugänglichkeit** für die Community
- **Detaillierte Dokumentation** von Hardware/Software Setup
- **Erweiterung** auf weitere Produktionsprozesse

### **Methodische Erweiterungen:**
- **Ensemble-Methoden** aus überwachten und unüberwachten Ansätzen
- **Deep Learning** Architekturen für Zeitreihenanalyse
- **Explainable AI** für bessere Interpretierbarkeit
- **Real-time Implementation** für Online-Monitoring

## 🌟 Bedeutung für ProData

Diese Studie ist ein **wichtiger Meilenstein** im ProData-Projekt und zeigt:
- **Systematischen Ansatz** zur Methodenevaluation
- **Praktische Anwendbarkeit** von ML in der Qualitätssicherung
- **Grundlage** für weitere Forschung in der Anomalieerkennung

Die Erkenntnisse fließen direkt in die **Entwicklung verbesserter Algorithmen** für die Kunststoffverarbeitung ein.

---

**Open Access:** Die vollständige Veröffentlichung ist frei verfügbar unter [ScholarSpace](https://scholarspace.manoa.hawaii.edu/items/c9ab7a99-c96e-47c1-b220-d516823795a3).

**Datenverfügbarkeit:** Zukünftig wird der Datensatz für die Forschungsgemeinschaft zugänglich gemacht, um weitere Studien und Methodenvergleiche zu ermöglichen.