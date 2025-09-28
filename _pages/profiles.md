<head>
  <style>
    .profiles {
      display: flex;
      flex-wrap: wrap; /* 自动换行 */
      justify-content: space-evenly; /* 图片间隔自动分配 */
    }

    .profile {
      margin: 10px;
      max-width: 250px;  /* 控制每个 profile 的最大宽度 */
      text-align: center;
    }

    .profile img {
      max-width: 100%;
      height: auto;
    }

    .more-info {
      margin-top: 10px;
    }
  </style>
</head>

<div class="profiles">
  {% if page.profiles %}
    {% for profile in page.profiles %}
      <div class="profile">
        {% if profile.image %}
          <img src="{{ profile.image }}" alt="Profile Image">
        {% endif %}
        {% if profile.more_info %}
          <div class="more-info">{{ profile.more_info }}</div>
        {% endif %}
      </div>
    {% endfor %}
  {% endif %}
</div>

---
<!-- layout: profiles -->
permalink: /people/
title: Hobbies
# description: members of the lab or group
nav: true
nav_order: 7

profiles:
  - image: karate1.jpg
    image_circular: false
    more_info: >
      <p>Karate</p>

  - image: karate2.jpg
    image_circular: false
    more_info: >
      <p>Karate</p>

  - image: hiking1.jpg
    image_circular: false
    more_info: >
      <p>Hiking</p>

  - image: hiking2.jpg
    image_circular: false
    more_info: >
      <p>Hiking</p>
