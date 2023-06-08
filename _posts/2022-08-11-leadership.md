---
layout: post-layout
title: Executive Leadership
description: Meet our executive team
image: /img/teaser.jpg
content-class: wide-12
no_index_headline: true
---

{% for leader in site.data.leaders %}
{% assign card-id = leader.id | append: '-card' %}
{% assign card-text = leader.id | append: '-bio' %}
{% assign card-img = 'img/leaders/' | append: leader.img %}
{% include
    widgets/user-card.html
    card-id=card-id
    card-text=card-text
    card-img=card-img
    name=leader.name
    lname=leader.lname
%}
{% endfor %}

<div id="all-leaders" class="container-fluid mw-9">
    <div class="row no-gutter">
        {% for leader in site.data.leaders %}
            <div class="col-lg-4 col-sm-6 leader-box">
                <div class="dark-bg" onclick="replace('all-leaders', '{{ leader.id }}-card')">
                    <img src="img/leaders/{{ leader.img }}"
                        class="img-responsive leader-img">
                    <div class="overlay-text">
                        <div class="text">Click for more</div>
                    </div>
                </div>
                <p class="leader-name">{{ leader.name }} {{ leader.lname }}</p>
                <p class="leader-role">{{ leader.role }}</p>
            </div>
        {% endfor %}
    </div>
</div>