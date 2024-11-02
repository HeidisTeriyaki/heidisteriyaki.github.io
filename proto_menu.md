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
.menu-page {
  display: flex;
  flex-direction: column;
  align-items: center;
}
  
.options {
  text-align: left;
}

.category-section {
  display: grid;
  grid-template-columns: repeat(2, 1fr); /* Two-column grid */
  gap: 20px; /* Spacing between items */
  width: 100%;
  max-width: 800px; /* Adjust based on desired width */
}

.menu-item {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
}

.menu-item img {
  width: 100%; /* Ensures full width within item container */
  height: 300px; /* Set a uniform height */
  object-fit: cover; /* Crop images to fit container while preserving aspect ratio */
  margin-bottom: 10px;
  border-radius: 8px; /* Optional: rounded corners */
}

.menu-item-title {
  font-weight: bold;
  margin: 5px 0;
}

.menu-item-price {
  color: #555; /* Optional: subtle color for price */
  margin-bottom: 10px;
}

.menu-item-description {
  font-size: 0.9em;
  color: #777;
}

.category-section > .menu-item:last-child:nth-child(odd) {
  grid-column: span 2;
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
          {% if item.image %}
            <img src="{{ item.image }}" alt="{{ item.description }}" style="preview-panel col-sm-4">
          {% endif %}
          <span class="menu-item-title">{{ item.title }}</span>
          <span class="menu-item-price">{{ item.price }}</span>
          {% if item.description %}
            <span class="menu-item-description">{{ item.description }}</span>
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

