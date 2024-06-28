---
layout: default
title: Home
---

# Site Title

<div class="row mt-4">
  <div class="col-md-4">
    <div class="card">
      <img src="assets/images/profile_picture.jpg" class="card-img-top profile-picture" alt="Profile Picture">
    </div>
  </div>
  <div class="col-md-8">
    {% assign about = site.about | first %}
    <div class="card">
      <div class="card-body">
        <h2 class="card-title">{{ about.title }}</h2>
        <p class="card-text">{{ about.content | markdownify }}</p>
      </div>
    </div>
  </div>
</div>
<div class="row mt-4">
  <div class="col-md-6">
    {% assign achievements = site.achievements | first %}
    <div class="card">
      <div class="card-body">
        <h2 class="card-title">{{ achievements.title }}</h2>
        <p class="card-text">{{ achievements.content | markdownify }}</p>
      </div>
    </div>
  </div>
  <div class="col-md-6">
    {% assign projects = site.projects | first %}
    <div class="card">
      <div class="card-body">
        <h2 class="card-title">{{ projects.title }}</h2>
        <p class="card-text">{{ projects.content | markdownify }}</p>
      </div>
    </div>
  </div>
</div>

<style>
  body {
      background-color: #222;
      color: #fff;
  }
  .card {
      background-color: #333;
      border: none;
      border-radius: 10px;
      margin-top: 20px;
  }
  .card-title {
      color: #fff;
  }
  .card-text {
      color: #ccc;
  }
  .profile-picture {
      border-radius: 50%;
      width: 100%;
      height: auto;
  }
</style>
