---
layout: single
title: "News & Aktuelles"
permalink: /news/
toc: false
---

Hier finden Sie alle Neuigkeiten rund um das ProData-Projekt - von Zwischenergebnissen über Veröffentlichungen bis hin zu Veranstaltungen und Kooperationen.

---

<div class="news-archive">
{% assign all_posts = site.posts | where_exp: "post", "post.categories contains 'news'" %}

{% if all_posts.size > 0 %}
  {% for post in all_posts %}
  <article class="news-entry">
    <header class="entry-header">
      <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
      <div class="entry-meta">
        <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%d. %B %Y" }}</time>
        {% if post.categories %}
          {% for category in post.categories %}
            <span class="category-tag">{{ category }}</span>
          {% endfor %}
        {% endif %}
        {% if post.author %}
          <span class="author">von {{ post.author }}</span>
        {% endif %}
        {% if post.reading_time %}
          <span class="reading-time">{{ post.reading_time }} Min. Lesezeit</span>
        {% endif %}
      </div>
    </header>
    
    {% if post.image %}
    <div class="entry-image">
      <img src="{{ post.image | relative_url }}" alt="{{ post.title }}">
    </div>
    {% endif %}
    
    <div class="entry-content">
      {{ post.excerpt }}
    </div>
    
    <footer class="entry-footer">
      <a href="{{ post.url | relative_url }}" class="btn btn--primary">Vollständigen Artikel lesen →</a>
      
      {% if post.tags and post.tags.size > 0 %}
      <div class="entry-tags">
        <span class="tags-label">Tags:</span>
        {% for tag in post.tags %}
          <span class="tag">{{ tag }}</span>{% unless forloop.last %}, {% endunless %}
        {% endfor %}
      </div>
      {% endif %}
      
      {% if post.doi %}
      <div class="publication-links">
        <a href="https://doi.org/{{ post.doi }}" target="_blank" class="btn btn--inverse btn--small">📄 Paper öffnen</a>
      </div>
      {% endif %}
    </footer>
  </article>
  {% endfor %}
  
{% else %}
  <div class="no-posts">
    <h3>Noch keine News verfügbar</h3>
    <p>Die ersten Neuigkeiten zum ProData-Projekt werden bald hier erscheinen. Schauen Sie regelmäßig vorbei oder folgen Sie uns für Updates!</p>
  </div>
{% endif %}
</div>

---

## 📂 Nach Kategorien filtern

<div class="category-filter">
  <a href="/news/" class="btn btn--primary">Alle</a>
  <a href="/categories/#forschung" class="btn btn--inverse">Forschung</a>
  <a href="/categories/#veröffentlichungen" class="btn btn--inverse">Veröffentlichungen</a>
  <a href="/categories/#veranstaltungen" class="btn btn--inverse">Veranstaltungen</a>
  <a href="/categories/#kooperationen" class="btn btn--inverse">Kooperationen</a>
  <a href="/categories/#meilensteine" class="btn btn--inverse">Meilensteine</a>
</div>

---

## 📧 Newsletter & Updates

Möchten Sie über neue Entwicklungen im ProData-Projekt informiert bleiben? 

**Kontaktieren Sie uns**, um in unseren Verteiler für Projektupdates aufgenommen zu werden:

{% for partner in site.project.partners %}
- 📧 **{{ partner.name }}:** [{{ partner.email }}](mailto:{{ partner.email }})
{% endfor %}