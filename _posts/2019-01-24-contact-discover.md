---
title: contact discover team
layout: directory
tags: [project, exhibition, classhome, conference, digital, fot, marketing]
---
<ul class="contacts">
  {% for contact in site.data.contacts %}
    <li class="name">
     <b>{{ contact.name }}</b> <i style="font-size:10px">{{contact.role}}</i>
      <ul class="info">
      	{% if contact.email != null %}<li><a href="mailto:{{contact.email}}">{{contact.email}}</a></li>{% endif %}
      	{% if contact.phone != null %}<li>{{contact.phone}}</li>{% endif %}
        {% if contact.platform != null %}<li>{{contact.platform}} me</li>{% endif %}
      </ul>
    </li>
  {% endfor %}
</ul>