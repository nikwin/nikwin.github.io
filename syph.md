---
layout: base
title: Syphilisation
---

<iframe src="https://store.steampowered.com/widget/1712530/" frameborder="0" width="646" height="190"></iframe>

<iframe src="https://itch.io/embed/660700" width="552" height="167" frameborder="0"><a href="https://whynotgames.itch.io/nikhil-murthys-syphilisation">Nikhil Murthy's Syphilisation by Why Not Games</a></iframe>

## What Is It?

*Nikhil Murthy's Syphilisation* is a post-colonial 4X game in which you play a student doing a group report on Gandhi, Churchill and the Raj.

## Trailer

<iframe width="560" height="315" src="https://www.youtube.com/embed/jH2GzGH18M0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Gameplay Video

<iframe width="560" height="315" src="https://www.youtube.com/embed/videoseries?list=PLZAuHrQoew0wIFKMTz_-wzOzWtmxBuLVI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

# Latest Posts

<ul>
  {% for post in site.posts %}
    {% if post.tag == "syph" %}
    <li>
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      {{ post.desc }}
    </li>
    {% endif %}
  {% endfor %}
</ul>