---
layout: default
title: The Quiet Sleep
---

<iframe src="https://store.steampowered.com/widget/724510/" frameborder="0" width="646" height="190"></iframe>

<iframe frameborder="0" src="https://itch.io/embed/74272" width="552" height="167"></iframe>

## What Is It?

*The Quiet Sleep* is a city builder/tower defense game set in your mind.

In it you will:
- Build out a personality and watch your mind develop.
- Handle various life situations, including talking to people, finding a job and trying to overthrow a local government.

## Trailer

<iframe width="560" height="315" src="https://www.youtube.com/embed/ucnfiqofNng?rel=0" frameborder="0" allowfullscreen></iframe>

## Explanation

<iframe width="560" height="315" src="https://www.youtube.com/embed/rDcIfRbERR0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Gameplay Video

<iframe width="560" height="315" src="https://www.youtube.com/embed/OPLfJm7VQ8w?rel=0" frameborder="0" allowfullscreen></iframe>
<iframe width="560" height="315" src="https://www.youtube.com/embed/videoseries?list=PLZAuHrQoew0we8kwA9UWJgFmfIDdPzKgp" frameborder="0" allowfullscreen></iframe>

## Screenshots

{% for file in site.static_files %}
   {% if file.path contains 'tqs_shots' %}
<img src="{{ file.path }}">
   {% endif %}
{% endfor %}

## Details

*The Quiet Sleep* was released on Oct. 15, 2017. *The Quiet Sleep* is available for PC and Mac.

## Links
    
- Twitter: [@murthynikhil](https://twitter.com/murthynikhil)
- YouTube: [https://www.youtube.com/channel/UCoFEuEueEt1Z2L-CQM8Uopw](https://www.youtube.com/channel/UCoFEuEueEt1Z2L-CQM8Uopw)
- E-mail: [murthynik1@gmail.com](mailto:murthynik1@gmail.com)
- Presskit: [Presskit](/presskit_tqs)

# Latest Posts

<ul>
  {% for post in site.posts %}
    {% if post.tag == "city" %}
    <li>
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      {{ post.desc }}
    </li>
    {% endif %}
  {% endfor %}
</ul>