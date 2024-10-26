---
title: Menu
permalink: "/proto_menu"
position: 2
layout: page
---

<div class="menu-page">
  <h1>{{ page.title }}</h1>

  {% for category in site.data.menu.categories %}
    <h2>{{ category.name }}</h2>
    <div class="category-section">
      
      {% for item in category.items %}
        <div class="menu-item">
          <p>{{ item.title }}</p>
          <p>{{ item.description }}</p>
          <p><strong>Price:</strong> {{ item.price }}</p>
          
          <!-- Display image if it exists -->
          {% if item.image %}
            <img src="{{ item.image }}" alt="{{ item.description }}" class="preview-panel">
          {% endif %}
        </div>
      {% endfor %}
      
    </div>
  {% endfor %}
</div>
