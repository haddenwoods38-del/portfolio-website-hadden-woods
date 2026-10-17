<script setup>
import profile from './assets/profile.jpg'
</script>

<template>
  <div>
    <nav>
      <div class="nav-container">
        <h2>Hadden Woods</h2>

        <ul>
          <li><a href="#">Home</a></li>
          <li><a href="#">About</a></li>
          <li><a href="#">Projects</a></li>
          <li><a href="#">Skills</a></li>
          <li><a href="#">Contact</a></li>
        </ul>
      </div>
    </nav>

    <section class="hero">
      <div class="content">
        <h1>Welcome to My Portfolio</h1>

        <h3>Hadden Woods</h3>

        <img
          :src="profile"
          alt="Profile Photo"
          class="profile-image"
        />

        <p>I am currently studying Web Development and programming with the goal of becoming a software developer.</p>

        <p>
          This portfolio will showcase my projects, education, technical skills, and growth as I continue developing my knowledge and experience.
        </p>

        <p>
          There will be more to come!
        </p>
      </div>
    </section>
  </div>
</template>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  background: linear-gradient(to bottom, #f4f4f4, #e7eef7);
  font-family: Arial, sans-serif;
}

nav {
  background-color: #1e3a5f;
  color: white;
  padding: 1rem 2rem;
}

.nav-container {
  max-width: 1100px;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

nav ul {
  list-style: none;
  display: flex;
  gap: 20px;
}

nav a {
  color: white;
  text-decoration: none;
  font-weight: bold;
}

nav a:hover {
  text-decoration: underline;
}

.hero {
  display: flex;
  justify-content: center;
  padding: 50px 20px;
}

.content {
  max-width: 900px;
  text-align: center;
}

.profile-image {
  width: 300px;
  max-width: 100%;
  border-radius: 12px;
  border: 4px solid #4f86c6;
  margin: 25px 0;
}

h1 {
  color: #1e3a5f;
  font-size: 3rem;
  margin-bottom: 20px;
}

h3 {
  color: #4f86c6;
  font-size: 2rem;
  margin-bottom: 20px;
}

p {
  color: #7a8494;
  font-size: 1.3rem;
  margin-bottom: 15px;
  line-height: 1.6;
}

@media (max-width: 768px) {
  .nav-container {
    flex-direction: column;
    gap: 10px;
  }

  nav ul {
    flex-wrap: wrap;
    justify-content: center;
  }

  h1 {
    font-size: 2rem;
  }

  h3 {
    font-size: 1.5rem;
  }

  p {
    font-size: 1rem;
  }

  .profile-image {
    width: 220px;
  }
}
</style>