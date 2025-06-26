---
layout: post
title: "Ansatz zur unüberwachten Erkennung von Anomalien erschienen"
date: 2023-11-02 14:00:00 +0200
category: Veröffentlichungen
author: ProData Team
lang: de
tags: [Forschung, Anomalieerkennung, Machine Learning, Schraubverbindungen, Clustering, K-Means]
excerpt: "Da Schraubverbindungen in der Fertigung allgegenwärtig sind, ist ihre effektive und zuverlässige Qualitätssicherung besonders wichtig. Wir stellen einen clusterbasierten Ansatz zur unüberwachten Erkennung von fehlerhaften Schraubvorgängen vor."
reading_time: 5
---

# Ansatz zur unüberwachten Erkennung von Anomalien erschienen

## 🔩 Herausforderung: Qualitätssicherung bei Schraubverbindungen

Da **Schraubverbindungen in der Fertigung allgegenwärtig** sind, ist ihre effektive und zuverlässige Qualitätssicherung besonders wichtig. Die meisten Anziehverfahren stützen sich auf statistische Methoden, um fehlerhafte Schraubverbindungen bereits während der Montage zu erkennen.

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

## 🏭 Anwendung in der Automobilindustrie

Der praktische Test erfolgte mit **realen Daten aus der Automobilindustrie**, was die Übertragbarkeit und **industrielle Relevanz** des Ansatzes unterstreicht. In dieser Branche ist die **Qualitätssicherung bei Schraubverbindungen** von kritischer Bedeutung für:

- **Sicherheit der Fahrzeuge**
- **Produktionseffizienz**
- **Kosteneinsparungen**
- **Qualitätsstandards**

## 🔬 Wissenschaftlicher Beitrag

Diese Veröffentlichung ist ein wichtiger **Meilenstein im ProData-Projekt** und zeigt, wie **fortschrittliche Machine Learning Methoden** zur Lösung realer Industrieprobleme eingesetzt werden können.

### 📖 Weitere Informationen

Die **Schritte zur Analyse** wurden **öffentlich zugänglich** gemacht, um die Reproduzierbarkeit und weitere Forschung zu fördern.

## 🚀 Ausblick

Diese Forschungsarbeit bildet eine **wichtige Grundlage** für weitere Entwicklungen im Bereich der:
- **Unüberwachten Anomalieerkennung**
- **Industriellen Qualitätssicherung**  
- **Zeitreihenanalyse in der Produktion**

Die Ergebnisse werden auch in die **Spritzgussdaten-Analyse** des ProData-Projekts einfließen, um ähnliche Ansätze in der **Kunststoffverarbeitung** zu entwickeln.

---

**Publikations-Details:**
- **Erscheinungsdatum:** November 2023
- **Bereich:** Unüberwachtes Maschinelles Lernen
- **Anwendungsgebiet:** Automotive Schraubverbindungen
- **Methode:** K-Means Clustering mit Dynamic Time Warping
- **Ergebnis:** 88,89% Genauigkeit in realen Industriedaten