---
layout: archive
title: "Sitemap"
permalink: /sitemap/
author_profile: true
---

{% include base_path %}

A list of all the posts and pages found on the site. For you robots out there, there is an [XML version]({{ base_path }}/sitemap.xml) available for digesting as well.

{% assign visible_pages = site.pages | where_exp: "item", "item.title and item.url != '/sitemap/' and item.url != '/404.html' and item.sitemap != false" | sort: "title" %}
{% assign visible_posts = site.posts | where_exp: "item", "item.title and item.sitemap != false" | sort: "date" | reverse %}

<h2>Pages</h2>
<ul>
{% for item in visible_pages %}
  <li><a href="{{ base_path }}{{ item.url }}">{{ item.title }}</a></li>
{% endfor %}
</ul>

{% if visible_posts.size > 0 %}
<h2>Posts</h2>
<ul>
{% for item in visible_posts %}
  <li><a href="{{ base_path }}{{ item.url }}">{{ item.title }}</a> <small>({{ item.date | date: "%Y-%m-%d" }})</small></li>
{% endfor %}
</ul>
{% endif %}

{% for collection in site.collections %}
  {% unless collection.output == false or collection.label == "posts" %}
    {% assign visible_docs = collection.docs | where_exp: "item", "item.title and item.sitemap != false" | sort: "title" %}
    {% if visible_docs.size > 0 %}
<h2>{{ collection.label | capitalize }}</h2>
<ul>
      {% for item in visible_docs %}
  <li><a href="{{ base_path }}{{ item.url }}">{{ item.title }}</a></li>
      {% endfor %}
</ul>
    {% endif %}
  {% endunless %}
{% endfor %}
