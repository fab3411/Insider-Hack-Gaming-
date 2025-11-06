---
layout: default
title: Accueil
---

<section class="hero">
  <h1>INSIDER HACK GAMING</h1>
  <p class="tagline">ONE HACK AT A TIME</p>
</section>

<section class="content wrap">
  <h2>Bienvenue</h2>
  <p>Bienvenue sur le site d'Insider Hack Gaming. Ici tu trouveras des actualités, des guides et des projets.</p>

  <h3>Derniers articles</h3>
  <ul>
    {% for post in site.posts limit:5 %}
      <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a> — <small>{{ post.date | date: "%Y-%m-%d" }}</small></li>
    {% endfor %}
  </ul>
</section>
