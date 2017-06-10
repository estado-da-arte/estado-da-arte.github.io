---
title: Livros
permalink: "/livros/"
layout: page
tags: page livros sugestões leitura
---

Relação de todos os livros sugeridos para leitura:

{% assign livros = (site.categories['livro'] | sort: 'title') %}
{% for post in livros %}
  <div class="post ml2">
    <a href="{{ post.url | prepend: site.baseurl }}" class="post-link">
      <h4 class="post-title">{{ post.title }}</h4>
    </a>
  </div>
{% endfor %}
