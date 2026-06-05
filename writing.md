---
layout: page
title: Writing
description: All blog posts
---

<p class="page-intro">This is where my heart and my code meet. Every post is a little story about what I learned, what moved me, and what I hope the future feels like.</p>

<div class="writing-stack">
    {% for post in site.posts %}
    <article class="feed-item">
        <div class="feed-item-left">
            <span class="feed-item-category">{{ post.category | default: 'Writing' }}</span>
            <h3 class="feed-item-title">
                <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
            </h3>
            <p class="feed-item-teaser">
                {{ post.description | default: post.excerpt | strip_html | truncatewords: 25 }}
            </p>
            <div class="feed-item-meta">
                <span class="meta-date">{{ post.date | date: "%b %d, %Y" }}</span>
                <span class="meta-divider">·</span>
                <span class="meta-readtime">{{ post.content | number_of_words | divided_by: 200 | at_least: 1 }} min read</span>
            </div>
        </div>
        <div class="feed-item-right">
            <div class="feed-thumbnail placeholder-thumb{{ forloop.index | modulo: 3 | plus: 1 }}"></div>
        </div>
    </article>
    {% else %}
    <div class="writing-empty">
        <p>No posts available at the moment. Check back soon!</p>
    </div>
    {% endfor %}
</div>


