---
layout: single
title: "Projektpartner"
permalink: /partners/
toc: true
toc_label: "Partner"
toc_sticky: true
header:
  overlay_color: "#2c5aa0"
  overlay_filter: 0.5
---

Das ProData-Projekt wird von zwei führenden deutschen Forschungseinrichtungen durchgeführt, die ihre komplementären Expertisen in **Datenanalyse/Machine Learning** und **Kunststofftechnik/Materialforschung** zusammenbringen.

---

## 🏢 Projektpartner im Detail

<div class="partners-overview">
  {% for partner in site.project.partners %}
  <div class="partner-section">
    <div class="partner-header">
      <div class="partner-logo">
        {% if partner.name contains "RIF" %}
          <img src="/assets/images/rif-logo.png" alt="{{ partner.name }} Logo">
        {% elsif partner.name contains "Kassel" %}
          <img src="/assets/images/ifw-logo.png" alt="{{ partner.name }} Logo">
        {% endif %}
      </div>
      <div class="partner-basic-info">
        <h3><a href="{{ partner.url }}" target="_blank" rel="noopener">{{ partner.name }}</a></h3>
        <p class="partner-location">📍 {{ partner.location }}</p>
        <p class="partner-leader"><strong>Projektleitung:</strong> {{ partner.leader }}</p>
        <p class="partner-contact">📧 <a href="mailto:{{ partner.email }}">{{ partner.email }}</a></p>
      </div>
    </div>
    
    <div class="partner-details">
      {% if partner.name contains "RIF" %}
        <h4>🤖 Expertise: Machine Learning & Produktionssysteme</h4>
        <p>Die <strong>Abteilung Arbeits- und Produktionssysteme</strong> vom RIF Institut für Forschung und Transfer e.V. aus Dortmund verfügt über umfassende <strong>Datenkompetenzen</strong> durch eine lange Historie heterogener ML-Umsetzungen in der produzierenden Industrie.</p>
        
        <h5>Forschungsschwerpunkte:</h5>
        <ul>
          <li><strong>Machine Learning in der Produktion</strong> - Anomalieerkennung, Predictive Maintenance</li>
          <li><strong>Industrial Data Science</strong> - Big Data Analytics für Fertigungsprozesse</li>
          <li><strong>Digitale Transformation</strong> - Industrie 4.0 Implementierung</li>
          <li><strong>Produktionssystemoptimierung</strong> - Effizienzsteigerung durch Datenanalyse</li>
        </ul>
        
        <h5>Rolle im ProData-Projekt:</h5>
        <ul>
          <li>🧠 <strong>ML-Methodenentwicklung</strong> für Anomalieerkennung</li>
          <li>📊 <strong>Datenanalysealgorithmen</strong> für imbalanced datasets</li>
          <li>🎓 <strong>Wissenschaftlicher Nachwuchs</strong> - Training in Data Science</li>
          <li>🔬 <strong>Clustering-Verfahren</strong> für Zeitreihenanalyse</li>
        </ul>
        
      {% elsif partner.name contains "Kassel" %}
        <h4>🧪 Expertise: Kunststofftechnik & Materialforschung</h4>
        <p>Das <strong>Fachgebiet Kunststofftechnik</strong> des Instituts für Werkstofftechnik der Universität Kassel unter der Leitung von Prof. Dr.-Ing. Hans-Peter Heim beschäftigt sich unter anderem mit der <strong>Verknüpfung von Prozessparametern</strong> in der Kunststoffverarbeitung und den resultierenden Prüfkörpereigenschaften.</p>
        
        <h5>Forschungsschwerpunkte:</h5>
        <ul>
          <li><strong>Spritzgießtechnik</strong> - Prozessoptimierung und Qualitätssicherung</li>
          <li><strong>Materialcharakterisierung</strong> - Prüfkörpereigenschaften und Prozessparameter</li>
          <li><strong>Prozessüberwachung</strong> - Inline-Qualitätskontrolle</li>
          <li><strong>Nachhaltige Kunststoffe</strong> - Recycling und Biokunststoffe</li>
        </ul>
        
        <h5>Rolle im ProData-Projekt:</h5>
        <ul>
          <li>🏭 <strong>Prozessdatensammlung</strong> aus Spritzgießanlagen</li>
          <li>📈 <strong>Datenaufbereitung</strong> für ML-Anwendungen</li>
          <li>🔍 <strong>Domänenexpertise</strong> für Kunststoffverarbeitung</li>
          <li>⚙️ <strong>Prozessvalidierung</strong> entwickelter ML-Methoden</li>
        </ul>
      {% endif %}
    </div>
  </div>
  {% endfor %}
</div>

---

## 🤝 Synergie der Zusammenarbeit

<div class="collaboration-grid">
  <div class="collaboration-item">
    <h4>🔄 Interdisziplinärer Ansatz</h4>
    <p>Die Kombination aus <strong>ML-Expertise</strong> (RIF) und <strong>Materialwissenschaft</strong> (Uni Kassel) ermöglicht eine ganzheitliche Betrachtung der Qualitätssicherung in der Kunststoffverarbeitung.</p>
  </div>
  
  <div class="collaboration-item">
    <h4>📊 Datenkompetenzen</h4>
    <p>Während das RIF fortschrittliche <strong>Datenanalysemethoden</strong> einbringt, steuert die Uni Kassel <strong>domänenspezifisches Wissen</strong> über Kunststoffprozesse bei.</p>
  </div>
  
  <div class="collaboration-item">
    <h4>🎓 Nachwuchsförderung</h4>
    <p>Beide Partner arbeiten gemeinsam an der <strong>Stärkung der Datenkompetenzen</strong> des wissenschaftlichen Nachwuchses durch praktische ML-Anwendungen.</p>
  </div>
  
  <div class="collaboration-item">
    <h4>🚀 Technologietransfer</h4>
    <p>Die Ergebnisse fließen direkt in die <strong>industrielle Anwendung</strong> ein und schaffen echten Mehrwert für die produzierende Industrie.</p>
  </div>
</div>

---

## 📈 Gemeinsame Forschungsaktivitäten

### **🔬 Methodenentwicklung**
- **Anomalieerkennung** in imbalanced Produktionsdaten
- **Zeitreihenanalyse** für Prozessüberwachung  
- **Unüberwachte Lernverfahren** für Qualitätssicherung

### **📚 Wissensvermittlung**
- **Workshops** zum maschinellen Lernen (RapidMiner, Python)
- **Schulungen** in Datenanalysemethoden
- **Best Practice** Austausch zwischen den Instituten

### **📊 Datenintegration**
- **Prozessketten-übergreifende** Datensammlung
- **Standardisierte Datenformate** für ML-Anwendungen
- **Validierung** in realen Produktionsumgebungen

---

## 🌐 Institutionelle Profile

<div class="institution-profiles">
  <div class="institution">
    <h4>🏢 RIF Institut für Forschung und Transfer e.V.</h4>
    <div class="institution-facts">
      <p><strong>Gründung:</strong> 1999</p>
      <p><strong>Standort:</strong> Dortmund, NRW</p>
      <p><strong>Mitarbeiter:</strong> 120+ Wissenschaftler und Ingenieure</p>
      <p><strong>Fokus:</strong> Angewandte Forschung für die produzierende Industrie</p>
      <p><strong>Besonderheit:</strong> Enge Verzahnung von Universität und Industrie</p>
    </div>
    <p>Das RIF Institut ist ein <strong>An-Institut der TU Dortmund</strong> und führt anwendungsorientierte Forschung in den Bereichen Produktionstechnik, Logistik und Industrial Data Science durch.</p>
    <p><a href="https://www.rif-ev.de/" target="_blank" class="btn btn--primary">🌐 RIF Website besuchen</a></p>
  </div>
  
  <div class="institution">
    <h4>🎓 Institut für Werkstofftechnik, Universität Kassel</h4>
    <div class="institution-facts">
      <p><strong>Gründung:</strong> 1971 (Universität), 1980er (Institut)</p>
      <p><strong>Standort:</strong> Kassel, Hessen</p>
      <p><strong>Studierende:</strong> 25.000+ an der Universität</p>
      <p><strong>Fokus:</strong> Materialwissenschaft und Kunststofftechnik</p>
      <p><strong>Besonderheit:</strong> Starke Praxisorientierung und Industriekooperationen</p>
    </div>
    <p>Das Institut für Werkstofftechnik ist Teil der <strong>Universität Kassel</strong> und forscht in den Bereichen Kunststofftechnik, Metallurgie und Materialcharakterisierung mit Fokus auf nachhaltige Materialien.</p>
    <p><a href="https://www.uni-kassel.de/maschinenbau/institute/werkstofftechnik" target="_blank" class="btn btn--primary">🌐 Institut Website besuchen</a></p>
  </div>
</div>

---

## 📞 Kooperationsanfragen

Interessiert an einer **Zusammenarbeit** mit dem ProData-Konsortium?

### **Mögliche Kooperationsformen:**
- 🤝 **Industriepartnerschaft** - Anwendung der Methoden in Ihrem Unternehmen
- 🔬 **Forschungskooperation** - Gemeinsame Projektanträge und Studien  
- 🎓 **Abschlussarbeiten** - Bachelor/Master-Arbeiten zu ProData-Themen
- 💼 **Beratung** - Expertenwissen in ML und Kunststofftechnik

### **Kontakt aufnehmen:**
<div class="cooperation-contact">
  {% for partner in site.project.partners %}
  <div class="contact-option">
    <h5>{{ partner.name }}</h5>
    <p><strong>{{ partner.leader }}</strong></p>
    <p>📧 <a href="mailto:{{ partner.email }}">{{ partner.email }}</a></p>
    <p>🌐 <a href="{{ partner.url }}" target="_blank">{{ partner.url }}</a></p>
  </div>
  {% endfor %}
</div>

---

<div class="funding-acknowledgment">
  <h4>🏛️ Projektförderung</h4>
  <p>Das ProData-Projekt wird gefördert durch das <strong>Bundesministerium für Bildung und Forschung (BMBF)</strong> im Rahmen des Programms „{{ site.project.funding_program }}" sowie durch die <strong>Europäische Union</strong> im Rahmen von „NextGenerationEU".</p>
  
  <div class="funding-logos">
    <img src="/assets/images/bmbf-logo.png" alt="BMBF Logo" class="funding-logo">
    <img src="/assets/images/eu-logo.png" alt="EU Logo" class="funding-logo">
    <img src="/assets/images/vdi-logo.png" alt="VDI/VDE Logo" class="funding-logo">
  </div>
</div>