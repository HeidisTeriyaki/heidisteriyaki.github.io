---
title: Menu
permalink: "/proto_menu"
position: 2
layout: page
---

<div class="menu-page">
<span>*<i>Menu and prices are subject to change without notice --- 01/01/2023</i>*</span><br/>

  {% for category in site.data.menu.categories %}
    <h2>{{ category.name }}</h2>
    <div class="category-section">
      
      {% for item in category.items %}
        <div class="menu-item">
          <span><strong>{{ item.title }}</strong> {{ item.price }}</span>
          <br>
          
          {% if item.description %}
            <span style="margin-left: 40px;">{{ item.description }}</span>
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

