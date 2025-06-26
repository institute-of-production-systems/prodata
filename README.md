# ProData Projekt Website

Diese Website dokumentiert das BMBF-geförderte Forschungsprojekt "ProData" zur prozessketten-übergreifenden Detektion von Material- und Prozessanomalien bei Imbalanced Data.

## 🚀 Quick Start

1. **Repository klonen**
   ```bash
   git clone https://github.com/institute-of-production-systems/prodata.git
   cd prodata
   ```

2. **Jekyll installieren** (einmalig)
   ```bash
   gem install bundler jekyll
   bundle install
   ```

3. **Lokal starten**
   ```bash
   bundle exec jekyll serve
   ```
   → Website ist verfügbar unter `http://localhost:4000`

## 📁 Dateistruktur

```
prodata/
├── _config.yml              # Haupt-Konfiguration
├── _layouts/                # Templates
│   ├── default.html         # Basis-Layout
│   └── post.html           # News-Artikel Layout
├── _posts/                  # News-Artikel
│   └── 2025-06-26-projekt-gestartet.md
├── assets/                  # Bilder, CSS, etc.
│   ├── css/style.css       # Haupt-Stylesheet
│   └── images/             # Bilder-Ordner
├── index.md                 # Startseite
├── news.md                 # News-Übersicht
├── Gemfile                 # Jekyll Dependencies
└── README.md               # Diese Datei
```

## 📝 Neue News-Artikel erstellen

### 1. Neue Datei erstellen
Erstelle eine neue `.md` Datei im `_posts/` Ordner:
```
_posts/YYYY-MM-DD-titel-des-artikels.md
```

### 2. Artikel-Template
```markdown
---
layout: post
title: "Titel des Artikels"
date: 2025-06-26 14:00:00 +0200
category: Forschung  # oder: Allgemein, Veröffentlichungen, etc.
author: ProData Team
lang: de
tags: [Machine Learning, Kunststofftechnik, BMBF]
excerpt: "Kurze Beschreibung des Artikels für die Vorschau..."
reading_time: 5  # Geschätzte Lesezeit in Minuten
---

# Artikel-Inhalt hier

Hier kommt der vollständige Artikel-Text in **Markdown** Format...

## Unterüberschrift

- Listen funktionieren
- Genau wie erwartet

### Weitere Features:
- **Fett** und *kursiv*
- [Links](https://example.com)
- Bilder: ![Alt-Text](pfad/zum/bild.png)
```

### 3. Kategorien verwenden
Verfügbare Kategorien:
- `Forschung` - Forschungsergebnisse, Studien
- `Allgemein` - Allgemeine Projekt-Updates
- `Veröffentlichungen` - Papers, Präsentationen
- `Veranstaltungen` - Konferenzen, Workshops
- `Kooperationen` - Partner-Updates
- `Meilensteine` - Projektfortschritte

## 🖼️ Bilder hinzufügen

### 1. Bilder hochladen
Lade Bilder in den `assets/images/` Ordner hoch.

### 2. In Artikeln verwenden
```markdown
![Beschreibung]({{ '/assets/images/mein-bild.png' | relative_url }})
```

### 3. Logo-Bilder benötigt
Folgende Logos sollten hinzugefügt werden:
- `assets/images/bmbf-logo.png` - BMBF Logo
- `assets/images/eu-logo.png` - EU Logo  
- `assets/images/vdi-logo.png` - VDI/VDE Logo
- `assets/images/rif-logo.png` - RIF Institut Logo
- `assets/images/ifw-logo.png` - Uni Kassel Logo
- `assets/images/startseite-hintergrund.png` - Hero-Bild

## 🌐 GitHub Pages Setup

### 1. Repository Settings
1. Gehe zu **Settings** → **Pages**
2. Source: **Deploy from a branch**
3. Branch: **main** / (root)
4. Klicke **Save**

### 2. Automatische Veröffentlichung
- Jeder Push zum `main` Branch triggert automatisch den Build
- Website ist verfügbar unter: `https://institute-of-production-systems.github.io/prodata/`

### 3. Custom Domain (optional)
Falls gewünscht, kann eine eigene Domain konfiguriert werden:
1. Datei `CNAME` im Repository-Root erstellen
2. Domain eintragen: `prodata-projekt.de`
3. DNS-Einstellungen beim Domain-Provider anpassen

## 🔧 Konfiguration anpassen

### Website-Informationen ändern
Bearbeite `_config.yml`:
```yaml
title: "Dein Projekt-Titel"
description: "Projekt-Beschreibung"
url: "https://deine-domain.de"
```

### Navigation ändern
```yaml
navigation:
  - title: "Start"
    url: "/"
  - title: "News"
    url: "/news/"
  - title: "Ergebnisse"
    url: "/ergebnisse/"
```

### Partner-Informationen
```yaml
project:
  partners:
    - name: "Neuer Partner"
      location: "Stadt"
      leader: "Prof. Dr. Name"
      url: "https://partner-website.de"
```

## 🎨 Design anpassen

### CSS ändern
Bearbeite `assets/css/style.css` für:
- Farben (CSS Variables am Anfang der Datei)
- Schriftarten
- Layout-Anpassungen

### Farbschema
```css
:root {
  --primary-color: #2c5aa0;    /* Hauptfarbe */
  --secondary-color: #004494;   /* Sekundärfarbe */
  --accent-color: #ffd700;      /* Akzentfarbe */
}
```

## 🌍 Mehrsprachigkeit

### Google Translate (bereits aktiv)
- Automatische Übersetzung in 100+ Sprachen
- Erscheint in der Navigation
- Keine weitere Konfiguration nötig

### Manuelle Übersetzungen (später)
Für professionelle Übersetzungen:
1. Englische Versionen der Artikel erstellen
2. Sprachauswahl implementieren
3. Separate Ordnerstruktur für Sprachen

## 📊 Analytics & SEO

### SEO bereits optimiert
- Meta-Tags automatisch generiert
- Sitemap wird automatisch erstellt
- Strukturierte Daten für Suchmaschinen

### Google Analytics hinzufügen (optional)
1. Google Analytics Account erstellen
2. Tracking-Code in `_config.yml` eintragen:
```yaml
google_analytics: UA-XXXXXXXXX-X
```

## 🔍 Wartung & Updates

### Regelmäßige Tasks
- [ ] Neue News-Artikel erstellen
- [ ] Bilder optimieren (vor Upload komprimieren)
- [ ] Partner-Informationen aktualisieren
- [ ] Kontaktdaten prüfen

### Jekyll Updates
```bash
bundle update
```

### Backup
- Repository ist automatisch gesichert auf GitHub
- Zusätzliche Backups der `assets/images/` empfohlen

## 🆘 Hilfe & Support

### Häufige Probleme

**Jekyll startet nicht lokal:**
```bash
bundle install
bundle exec jekyll serve --trace
```

**Änderungen erscheinen nicht:**
- Hard Refresh: `Ctrl+F5` (Windows) / `Cmd+Shift+R` (Mac)
- Browser-Cache leeren

**Build-Fehler auf GitHub:**
- Prüfe GitHub Actions Tab für Fehlermeldungen
- YAML-Syntax in Front Matter prüfen

### Markdown Cheat Sheet
```markdown
# H1 Überschrift
## H2 Überschrift
### H3 Überschrift

**Fett** und *kursiv*

[Link](https://example.com)

![Bild](pfad/zum/bild.png)

- Liste
- Item 2

1. Nummerierte Liste
2. Item 2

> Zitat-Block

`Code inline`

```code
Code-Block
```

### Nützliche Links
- [Jekyll Dokumentation](https://jekyllrb.com/docs/)
- [Markdown Guide](https://www.markdownguide.org/)
- [GitHub Pages Docs](https://docs.github.com/en/pages)
- [BMBF Förderhinweise](https://www.bildung-forschung.digital/)

## 📞 Kontakt für Website-Fragen

Bei technischen Fragen zur Website:
- GitHub Issues erstellen
- Pull Requests für Verbesserungen willkommen

Bei inhaltlichen Fragen zum Projekt:
- **RIF Institut:** deuse@rif-ev.de
- **Universität Kassel:** heim@uni-kassel.de

---

**Status:** ✅ Produktionsbereit  
**Letztes Update:** 26.06.2025  
**Jekyll Version:** 4.3.x  
**GitHub Pages:** Kompatibel