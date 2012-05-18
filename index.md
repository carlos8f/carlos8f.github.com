---
layout: default
title: Carlos Rodriguez
---

<nav id="social">
  <h2>hi, I'm Carlos. I&hellip;</h2>
  <ul>
    <li>play <a href="{{ site.baseurl }}music/everything-reminds-me-of-her.html">music</a></li>
    <li>work at <a href="http://www.terraeclipse.com/" target="_blank">terra eclipse</a></li>
    <li>code on <a href="http://github.com/carlos8f" target="_blank">github</a></li>
    <li>contribute to <a href="http://drupal.org/user/454578" target="_blank">drupal</a></li>
    <li>am not big on <a href="http://twitter.com/#!/carlos8f" target="_blank">twitter</a></li>
    <li>have some friends on <a href="https://www.facebook.com/carlos8f" target="_blank">facebook</a></li>
    <li>buy records on <a href="http://www.discogs.com/collection?user=carlos8f" target="_blank">discogs</a></li>
    <li>listen on <a href="http://www.rdio.com/people/carlos8f" target="_blank">rdio</a></li>
    <li>love to make coffee with my <a href="http://amzn.com/B0047BIWSK" target="_blank">aeropress</a></li>
    <li>play <a href="https://www.google.com/search?q=disc+golf" target="_blank">disc golf</a></li>
  </ul>

  <h2>meta</h2>
  <ul>
    <li>about <a href="{{ site.baseurl }}README.html">{{ site.title }}</a></li>
    <li><a href="javascript:alert('carlos [at] s8f [dot] org')">email</a></li>
  </ul>
</nav>

{% if site.categories.music %}
music
-----

<ul class="posts">
{% for post in site.categories.music %}
<li>{{ post.date || date_to_string}} &mdash; <a href="{{ site.root }}{{ post.url }}">{{ post.title}}</a></li>
{% endfor %}
</ul>
{% endif %}

{% if site.categories.code %}
code
----

<ul class="posts">
{% for post in site.categories.code %}
<li>{{ post.date || date_to_string}} &mdash; <a href="{{ site.root }}{{ post.url }}">{{ post.title}}</a></li>
{% endfor %}
</ul>
{% endif %}

{% if site.categories.photos %}
photos
------

<ul class="photos">
{% for post in site.categories.photos %}
<li><a href="{{ site.root }}{{ post.url }}"><img alt="{{ post.title }}" src="{{ post.thumb}}" /></a></li>
{% endfor %}
</ul>
{% endif %}

{% if site.categories.misc %}
misc
----

<ul class="posts">
{% for post in site.categories.misc %}
<li>{{ post.date || date_to_string}} &mdash; <a href="{{ site.root }}{{ post.url }}">{{ post.title}}</a></li>
{% endfor %}
</ul>
{% endif %}
