---
layout: page
title: Writing & Research Notes
description: Complete chronological archive of essays, technical notes, and research journey.
---

<p class="page-intro">
Explore my writing across machine learning, software reliability, federated edge systems, smart grid security, and academic growth.
</p>

<div class="writing-stack post-list-stack">
    {% for post in site.posts %}
    <article class="post-card">
        <div class="post-card-copy">
            <div class="post-card-meta">
                <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%b %d, %Y" }}</time>
                <span class="meta-dot">·</span>
                <span>{{ post.content | number_of_words | divided_by: 200 | at_least: 1 }} min read</span>
                {% if post.category %}
                <span class="meta-dot">·</span>
                <span class="post-category-tag">{{ post.category }}</span>
                {% endif %}
            </div>
            <h2 class="post-card-title">
                <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
            </h2>
            <p class="post-card-excerpt">
                {{ post.description | default: post.excerpt | strip_html | truncatewords: 30 }}
            </p>
            {% if post.tags %}
            <div class="tag-row">
                {% for tag in post.tags %}
                <span class="tag-pill">#{{ tag }}</span>
                {% endfor %}
            </div>
            {% endif %}
        </div>
    </article>
    {% endfor %}
</div>
