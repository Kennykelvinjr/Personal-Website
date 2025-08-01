<template>
    <nav class="navbar">
      <div class="container">
        <RouterLink to="/" class="site-title">Kelvin Augustino Mwashiga</RouterLink>
        <ul>
          <li><RouterLink to="/">Home</RouterLink></li>
          <li><RouterLink to="/portfolio">Portfolio</RouterLink></li>
          <li><RouterLink to="/resume">Resume</RouterLink></li>
          <li>
          <a href="/KelvinCV.pdf" download class="nav-download-link">
            Download CV
          </a>
        </li>
        </ul>
      </div>
    </nav>
  </template>
  
  <script setup>
  import { RouterLink } from 'vue-router';
  </script>
  
  <style scoped>
  .navbar {
    background-color: var(--color-dark-brown); /* Using your color palette */
    padding: 1rem 0;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  }
  
  .navbar .container {
    max-width: 960px;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 20px;
    flex-wrap: wrap;
  }
  
  .site-title {
    font-size: 1.8rem;
    font-weight: bold;
    color: var(--color-background-main); /* Light text on dark background */
    text-decoration: none;
    flex-basis: auto;
  }
  
  .navbar ul {
    list-style: none;
    display: flex;
    gap: 1.5rem; /* Space between navigation items */
    margin: 0;
    padding: 0;
  }
  
  .navbar a {
    color: var(--color-secondary-light); /* Light text for links */
    text-decoration: none;
    font-size: 1.1rem;
    transition: color 0.3s ease;
  }
  
  .navbar a:hover {
    color: var(--color-primary-light); /* Lighter on hover */
    text-decoration: none; /* Remove underline on hover if preferred */
  }

  .nav-download-link {
    /* Inherit current link styles for consistency */
    color: var(--color-secondary-light); /* Light text for links */
    text-decoration: none;
    font-size: 1.1rem;
    transition: color 0.3s ease;
    /* Make it stand out slightly if you want */
    border: 1px solid var(--color-secondary-light);
    padding: 0.5em 1em;
    border-radius: 5px;
}

.nav-download-link:hover {
    color: var(--color-primary-light);
    border-color: var(--color-primary-light);
    background-color: rgba(255, 255, 255, 0.1); /* Subtle hover background */
}

/* --- Media Queries for NavBar --- */
@media (max-width: 768px) {
  .navbar .container {
    flex-direction: column; /* Stack items vertically */
    align-items: flex-start; /* Align items to the left */
  }

  .site-title {
    width: 100%; /* Make title take full width */
    text-align: center; /* Center title */
    margin-bottom: 1rem; /* Add space below title */
  }

  .navbar ul {
    flex-direction: column; /* Stack nav links vertically */
    width: 100%; /* Make list take full width */
    gap: 0.5rem; /* Reduce gap between stacked links */
    text-align: center; /* Center text within each li */
  }

  .navbar ul li {
    width: 100%; /* Ensure each list item takes full width */
  }

  .navbar a {
    display: block; /* Make links block-level for full width clickable area */
    padding: 0.5rem 0; /* Add padding for easier tapping */
    width: 100%;
  }

  .navbar a, .nav-download-link { /* Apply block display to both regular links and download link */
    display: block;
    padding: 0.5rem 0;
    width: 100%;
  }

  .nav-download-link {
    /* Adjust padding for stacked mobile view */
    padding: 0.8rem 1em; /* Give it a bit more vertical padding for button feel */
    margin-top: 0.5rem; /* Space from other links */
  }
}

</style>