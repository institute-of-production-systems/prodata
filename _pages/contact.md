---
layout: single
title: "Kontakt"
permalink: /contact/
toc: true
toc_label: "Kontakt"
toc_sticky: true
header:
  overlay_color: "#2c5aa0"
  overlay_filter: 0.5
---

**Kontaktieren Sie uns bei weiteren Fragen!**

Falls Sie Anregungen zum Forschungsvorhaben, Rückfragen zu Zwischenergebnissen oder weiterführendes Interesse an einer Zusammenarbeit haben, kontaktieren Sie uns gerne.

---

## 📞 Projektleitung

<div class="project-contacts">
  {% for partner in site.project.partners %}
  <div class="contact-card-detailed">
    <div class="contact-header">
      <div class="contact-logo">
        {% if partner.name contains "RIF" %}
          <img src="/assets/images/rif-logo.png" alt="{{ partner.name }} Logo">
        {% elsif partner.name contains "Kassel" %}
          <img src="/assets/images/ifw-logo.png" alt="{{ partner.name }} Logo">
        {% endif %}
      </div>
      <div class="contact-info">
        <h3>{{ partner.name }}</h3>
        <h4>{{ partner.leader }}</h4>
        <p class="title">Projektleiter ProData</p>
      </div>
    </div>
    
    <div class="contact-details">
      <div class="contact-method">
        <h5>📧 E-Mail</h5>
        <p><a href="mailto:{{ partner.email }}">{{ partner.email }}</a></p>
      </div>
      
      <div class="contact-method">
        <h5>🌐 Institution</h5>
        <p><a href="{{ partner.url }}" target="_blank" rel="noopener">{{ partner.name }}</a></p>
      </div>
      
      <div class="contact-method">
        <h5>📍 Standort</h5>
        <p>{{ partner.location }}</p>
      </div>
      
      {% if partner.name contains "RIF" %}
      <div class="contact-method">
        <h5>🏢 Adresse</h5>
        <p>
          RIF Institut für Forschung und Transfer e.V.<br>
          Joseph-von-Fraunhofer-Str. 20<br>
          44227 Dortmund<br>
          Deutschland
        </p>
      </div>
      
      <div class="expertise-area">
        <h5>🤖 Expertise</h5>
        <p><strong>Machine Learning & Industrial Data Science</strong><br>
        Anomalieerkennung, Clustering-Verfahren, Zeitreihenanalyse</p>
      </div>
      
      {% elsif partner.name contains "Kassel" %}
      <div class="contact-method">
        <h5>🏢 Adresse</h5>
        <p>
          Institut für Werkstofftechnik<br>
          Fachgebiet Kunststofftechnik<br>
          Universität Kassel<br>
          Mönchebergstraße 3<br>
          34125 Kassel<br>
          Deutschland
        </p>
      </div>
      
      <div class="expertise-area">
        <h5>🧪 Expertise</h5>
        <p><strong>Kunststofftechnik & Materialforschung</strong><br>
        Spritzgießtechnik, Prozessüberwachung, Qualitätssicherung</p>
      </div>
      {% endif %}
    </div>
  </div>
  {% endfor %}
</div>

---

## 💼 Projektteam

### **🧑‍🔬 Wissenschaftliche Mitarbeiter**

<div class="team-grid">
  <div class="team-member">
    <h4>Nikolai West</h4>
    <p class="team-role">Wissenschaftlicher Mitarbeiter</p>
    <p class="team-affiliation">RIF Institut</p>
    <p class="team-focus"><strong>Schwerpunkt:</strong> Machine Learning, Anomalieerkennung, Zeitreihenanalyse</p>
    <p class="team-publications">📊 Hauptautor der ProData-Publikationen zu ML-Methoden</p>
  </div>
  
  <div class="team-member">
    <h4>Thomas Schlegl</h4>
    <p class="team-role">Wissenschaftlicher Mitarbeiter</p>
    <p class="team-affiliation">RIF Institut</p>
    <p class="team-focus"><strong>Schwerpunkt:</strong> Data Mining, Clustering, Industrial Data Science</p>
    <p class="team-publications">🔬 Experte für Dynamic Time Warping und unüberwachte Verfahren</p>
  </div>
</div>

### **👨‍🎓 Studentische Hilfskräfte & Abschlussarbeiten**

Interessiert an einer **Abschlussarbeit** im ProData-Projekt?

**Mögliche Themen:**
- 🤖 ML-Algorithmen für Kunststoffverarbeitung
- 📊 Datenanalysemethoden für Prozessüberwachung
- 🔍 Anomalieerkennung in Zeitreihendaten
- 🏭 Industrie 4.0 Anwendungen in der Fertigung

**Kontakt für Abschlussarbeiten:**
- **RIF Institut:** [deuse@rif-ev.de](mailto:deuse@rif-ev.de)
- **Uni Kassel:** [heim@uni-kassel.de](mailto:heim@uni-kassel.de)

---

## 🤝 Kooperationsanfragen

### **Für Industrieunternehmen:**

**Sie haben Interesse an:**
- ✅ **Anwendung unserer ML-Methoden** in Ihrem Unternehmen?
- ✅ **Gemeinsame Forschungsprojekte** zu Qualitätssicherung?
- ✅ **Beratung** bei Data Science Projekten?
- ✅ **Schulungen** für Ihre Mitarbeiter?

### **Für Forschungseinrichtungen:**

**Sie möchten:**
- 🔬 **Gemeinsame Publikationen** zu ML in der Fertigung?
- 📊 **Datenaustausch** für Validierungsstudien?
- 🎓 **Studentenaustausch** und gemeinsame Abschlussarbeiten?
- 💰 **Gemeinsame Projektanträge** bei Fördergebern?

### **Für die Öffentlichkeit:**

**Sie sind interessiert an:**
- 📰 **Presseinterviews** zum Projekt?
- 🎤 **Vorträge** für Ihr Event/Ihre Konferenz?
- 📚 **Gastbeiträge** für Fachmagazine?
- 🏫 **Schulbesuche** oder Universitätsvorlesungen?

---

## 📝 Kontaktformular

**Schreiben Sie uns direkt:**

<div class="contact-form-info">
  <p><strong>Für allgemeine Anfragen:</strong> Wählen Sie den entsprechenden Projektpartner basierend auf Ihrem Anliegen:</p>
  
  <div class="contact-routing">
    <div class="routing-option">
      <h5>🤖 Machine Learning & Data Science Fragen</h5>
      <p>Kontaktieren Sie das <strong>RIF Institut</strong></p>
      <p>📧 <a href="mailto:deuse@rif-ev.de?subject=ProData Anfrage - ML/Data Science">deuse@rif-ev.de</a></p>
    </div>
    
    <div class="routing-option">
      <h5>🧪 Kunststofftechnik & Materialfragen</h5>
      <p>Kontaktieren Sie die <strong>Universität Kassel</strong></p>
      <p>📧 <a href="mailto:heim@uni-kassel.de?subject=ProData Anfrage - Kunststofftechnik">heim@uni-kassel.de</a></p>
    </div>
  </div>
</div>

**E-Mail Vorlage für Ihre Anfrage:**
```
Betreff: ProData Anfrage - [Ihr Thema]

Sehr geehrte Damen und Herren,

ich interessiere mich für das ProData-Projekt und hätte 
folgende Frage/Anliegen:

[Ihre Nachricht hier]

Mit freundlichen Grüßen
[Ihr Name]
[Ihre Organisation]
[Ihre Kontaktdaten]
```

---

## 📅 Veranstaltungen & Termine

### **Kommende Events:**
Aktuelle Termine für Konferenzen, Workshops und Präsentationen finden Sie in unserem [News-Bereich](/news/).

### **Workshop-Anfragen:**
Interessiert an einem **Workshop zu Machine Learning** in Ihrem Unternehmen/Ihrer Institution?

**Mögliche Workshop-Themen:**
- 📊 Einführung in Machine Learning für die Fertigung
- 🔍 Anomalieerkennung in Produktionsdaten  
- 🛠️ Hands-On RapidMiner Training
- 🐍 Python für Industrial Data Science

---

## 🌍 Social Media & Updates

**Folgen Sie uns für aktuelle Updates:**

<div class="social-links">
  <div class="social-item">
    <h5>🔗 LinkedIn</h5>
    <p>Folgen Sie den beteiligten Instituten auf LinkedIn für professionelle Updates</p>
  </div>
  
  <div class="social-item">
    <h5>📧 Newsletter</h5>
    <p>Tragen Sie sich in unseren E-Mail-Verteiler ein für Projektupdates</p>
  </div>
  
  <div class="social-item">
    <h5>📰 RSS Feed</h5>
    <p>Abonnieren Sie unseren <a href="/feed.xml">RSS Feed</a> für automatische News-Updates</p>
  </div>
</div>

---

<div class="contact-footer">
  <h4>🔍 Weitere Informationen</h4>
  <p>Mehr Details zum Projekt finden Sie unter:</p>
  <ul>
    <li>📊 <a href="/research/">Forschungsdetails</a> - Umfassende Projektbeschreibung</li>
    <li>📚 <a href="/publications/">Veröffentlichungen</a> - Alle wissenschaftlichen Papers</li>
    <li>🏢 <a href="/partners/">Partner</a> - Detaillierte Institutsprofile</li>
    <li>📰 <a href="/news/">News</a> - Aktuelle Projektupdates</li>
  </ul>
</div>