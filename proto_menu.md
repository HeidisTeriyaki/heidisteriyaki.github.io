---
title: Menu
permalink: "/proto_menu"
position: 2
layout: page
---

<div class="menu-page">
  <span>*<i>Menu and prices are subject to change without notice --- 01/01/2023</i>*</span><br/>

  {% for category in site.data.menu.categories %}
    {% if category.head %}
      <div>{{ category.head }}</div>
    {% endif %}
    <h2>{{ category.name }}</h2>
    <div class="category-section">
      
      {% for item in category.items %}
        <div class="menu-item">
          <span><strong>{{ item.title }}</strong> {{ item.price }}</span>
          <br>
          
          {% if item.description %}
            <span style="margin-left: 25px;">{{ item.description }}</span>
            <br>
          {% endif %}
          
          {% if item.image %}
            <img src="{{ item.image }}" alt="{{ item.description }}" class="preview-panel col-sm-4">
          {% endif %}
        </div>
      {% endfor %}

    </div>

    
    {% if category.foot %}
      <div>{{ category.foot }}</div>
    {% endif %}
  {% endfor %}
  <div>
    <strong>
      ***Please let us know if you have any FOOD ALLERGIES before you order***<br>
      ***Please order according to the menu, a surcharge may incur if modifications to dishes are made***<br>
      ***Additional fees for extra sauce, meats, vegetables, etc. may apply***<br>
      ***No replacements can be done after food is served, please order accordingly***<br>
      ***Consuming raw or undercooked meats, poultry, seafood, shellfish, or eggs may increase your risk of food borne illness.***<br>
      ***Menu and prices subject to change without notice (Effective 01/01/2023)***<br>
    </strong>
  </div>
</div>

