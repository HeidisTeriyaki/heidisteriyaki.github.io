---
title: Menu
permalink: "/proto_menu"
position: 2
layout: page
---

<div class="menu-page">

  {% for category in site.data.menu.categories %}
    <h2>{{ category.name }}</h2>
    <div class="category-section">
      
      {% for item in category.items %}
        <div class="menu-item">
          <span><strong>{{ item.title }}</strong> {{ item.price }}</span>
          <br>
          
          {% if item.description %}
            <span>{{ item.description }}</span>
            <br>
          {% endif %}
          
          {% if item.image %}
            <img src="{{ item.image }}" alt="{{ item.description }}" class="preview-panel col-sm-4">
          {% endif %}
        </div>
      {% endfor %}
      
    </div>
  {% endfor %}
</div>

