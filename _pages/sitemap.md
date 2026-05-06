---
layout: archive
title: "Sitemap"
permalink: /sitemap/
author_profile: true
---

{% include base_path %}

A list of all the posts and pages found on the site. For you robots out there, there is an [XML version]({{ base_path }}/sitemap.xml) available for digesting as well.

<h2>Pages</h2>
<ul>
{% assign sorted_pages = site.pages | sort: "title" %}
{% for item in sorted_pages %}
  {% if item.title and item.url != '/sitemap/' and item.url != '/404.html' and item.sitemap != false %}
  <li><a href="{{ base_path }}{{ item.url }}">{{ item.title }}</a></li>
  {% endif %}
{% endfor %}
</ul>

<h2>Posts</h2>
<ul>
{% assign sorted_posts = site.posts | sort: "date" | reverse %}
{% for item in sorted_posts %}
  {% if item.title and item.sitemap != false %}
  <li><a href="{{ base_path }}{{ item.url }}">{{ item.title }}</a> <small>({{ item.date | date: "%Y-%m-%d" }})</small></li>
  {% endif %}
{% endfor %}
</ul>

{% for collection in site.collections %}
  {% unless collection.output == false or collection.label == "posts" %}
    {% assign sorted_docs = collection.docs | sort: "title" %}
<h2>{{ collection.label | capitalize }}</h2>
<ul>
      {% for item in sorted_docs %}
        {% if item.title and item.sitemap != false %}
  <li><a href="{{ base_path }}{{ item.url }}">{{ item.title }}</a></li>
        {% endif %}
      {% endfor %}
</ul>
  {% endunless %}
{% endfor %}
