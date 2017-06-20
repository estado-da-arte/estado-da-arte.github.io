---
title: Livros
permalink: "/livros/"
layout: page
tags: page livros sugestões leitura
---
Nesta página você encontra todos os livros sugeridos para leitura.

Destaque especial para o [Portal Domínio Público][PDP]{:target="_blank"} <i class="fa fa-external-link" aria-hidden="true"></i> que disponibiliza inúmeros títulos gratuitamente e para a editora [Packt][PACKTPUB]{:target="_blank"} <i class="fa fa-external-link" aria-hidden="true"></i> que oferece um título de se acervo por dia de forma gratuíta.

Relação de todos os livros sugeridos para leitura:

{% assign livros = (site.categories['livro'] | sort: 'title') %}
{% for post in livros %}
  <div class="post ml2">
    <a href="{{ post.url | prepend: site.baseurl }}" class="post-link">
      <h4 class="post-title">{{ post.title }}</h4>
    </a>
  </div>
{% endfor %}

[PDP]: http://www.dominiopublico.gov.br
[PACKTPUB]: https://www.packtpub.com/packt/offers/free-learning
