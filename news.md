---
layout: default
title: "News & Aktuelles"
---

# News & Aktuelles

Hier finden Sie alle Neuigkeiten rund um das ProData-Projekt - von Zwischenergebnissen über Veröffentlichungen bis hin zu Veranstaltungen und Kooperationen.

---

<div class="news-list">
{% assign all_posts = site.posts | where: "lang", "de" %}

{% if all_posts.size > 0 %}
  {% for post in all_posts %}
  <article class="news-article">
    <header class="news-header">
      <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
      <div class="news-meta">
        <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%d. %B %Y" }}</time>
        {% if post.category %}
          <span class="category">{{ post.category }}</span>
        {% endif %}
        {% if post.author %}
          <span class="author">von {{ post.author }}</span>
        {% endif %}
      </div>
    </header>
    
    {% if post.image %}
    <div class="news-image">
      <img src="{{ post.image | relative_url }}" alt="{{ post.title }}">
    </div>
    {% endif %}
    
    <div class="news-excerpt">
      {{ post.excerpt }}
    </div>
    
    <footer class="news-footer">
      <a href="{{ post.url | relative_url }}" class="read-more-btn">Vollständigen Artikel lesen →</a>
      
      {% if post.tags and post.tags.size > 0 %}
      <div class="tags">
        <span class="tags-label">Tags:</span>
        {% for tag in post.tags %}
          <span class="tag">{{ tag }}</span>{% unless forloop.last %}, {% endunless %}
        {% endfor %}
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

## 📧 Newsletter & Updates

Möchten Sie über neue Entwicklungen im ProData-Projekt informiert bleiben? 

**Kontaktieren Sie uns**, um in unseren Verteiler für Projektupdates aufgenommen zu werden:

- 📧 **RIF Institut:** [deuse@rif-ev.de](mailto:deuse@rif-ev.de)
- 📧 **Universität Kassel:** [heim@uni-kassel.de](mailto:heim@uni-kassel.de)

<div class="news-categories">
  <h3>Themenbereich</h3>
  <div class="category-tags">
    <span class="category-tag">Forschung</span>
    <span class="category-tag">Veröffentlichungen</span>
    <span class="category-tag">Veranstaltungen</span>
    <span class="category-tag">Kooperationen</span>
    <span class="category-tag">Meilensteine</span>
    <span class="category-tag">Allgemein</span>
  </div>
</div>