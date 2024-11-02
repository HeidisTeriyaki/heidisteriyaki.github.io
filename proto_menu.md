---
title: Menu
permalink: "/proto_menu"
position: 2
layout: page
---
<!---
<div class="menu-page">
  <span>*<i>Menu and prices are subject to change without notice --- 01/01/2023</i>*</span><br/>

  {% for category in site.data.menu.categories %}
    <h2>{{ category.name }}</h2>
    {% if category.head %}
      <div style="margin-bottom: 25px;">{{ category.head }}</div>
    {% endif %}
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
      <div style="margin-top: 25px;">{{ category.foot }}</div>
    {% endif %}
  {% endfor %}
  <div style="margin-top: 50px;">
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
-->

<style>
.menu-item {
  margin-bottom: 20px;
}

.menu-item-content {
  display: flex;
  align-items: flex-start;
}

.menu-item-text {
  flex: 1; /* This will take up the remaining space */
}

.menu-item-image img {
  max-width: 150px; /* Adjust the width as needed */
  margin-left: 15px; /* Add some space between text and image */
}
</style>

<div class="menu-page">
  <span>*<i>Menu and prices are subject to change without notice --- 01/01/2023</i>*</span><br/>

  {% for category in site.data.menu.categories %}
    <h2>{{ category.name }}</h2>
    {% if category.head %}
      <div style="margin-bottom: 25px;">{{ category.head }}</div>
    {% endif %}
    <div class="category-section">
      {% for item in category.items %}
        <div class="menu-item">
          <div class="menu-item-content">
            <!-- Text Content Column -->
            <div class="menu-item-text">
              <span><strong>{{ item.title }}</strong> {{ item.price }}</span>
              <br>
              {% if item.description %}
                <span style="margin-left: 25px;">{{ item.description }}</span>
                <br>
              {% endif %}
            </div>
            <!-- Image Column -->
            {% if item.image %}
              <div class="menu-item-image">
                <img src="{{ item.image }}" alt="{{ item.description }}" class="preview-panel col-sm-4">
              </div>
            {% endif %}
          </div>
        </div>
      {% endfor %}
    </div>
    {% if category.foot %}
      <div style="margin-top: 25px;">{{ category.foot }}</div>
    {% endif %}
  {% endfor %}
  
  <div style="margin-top: 50px;">
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
