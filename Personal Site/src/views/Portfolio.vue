<template>
  <main class="portfolio-view">
    <h1 class="fade-in-delay-1">My Portfolio</h1>
    <p class="fade-in-delay-2">A collection of my web development projects, highlighting my skills and passion for creating impactful digital experiences.</p>

    <section class="portfolio-grid">
      <div class="portfolio-item fade-in-delay-3">
        <!-- <img src="/project-placeholder-1.jpg" alt="Project 1 Thumbnail"> -->
        <h3>Personal Website</h3>
        <p>A brief description of Project One. Mention technologies used like HTML, CSS, JavaScript, Vue.js.</p>
        <a href="https://github.com/yourusername/project-one" target="_blank" rel="noopener noreferrer">View on GitHub</a> |
        <a href="https://yourwebsite.com/project-one-demo" target="_blank" rel="noopener noreferrer">Live Demo</a>
      </div>

      <div class="portfolio-item fade-in-delay-4">
        <!-- <img src="/project-placeholder-2.jpg" alt="Project 2 Thumbnail"> -->
        <h3>To do list app</h3>
        <p>A brief description of Project Two. Focus on the problem it solved or the unique features.</p>
        <a href="https://github.com/yourusername/project-two" target="_blank" rel="noopener noreferrer">View on GitHub</a> |
        <a href="https://yourwebsite.com/project-two-demo" target="_blank" rel="noopener noreferrer">Live Demo</a>
      </div>

      <div class="portfolio-item fade-in-delay-5">
        <!-- <img src="/project-placeholder-3.jpg" alt="Project 3 Thumbnail"> -->
        <h3>Weather app</h3>
        <p>A brief description of Project Three. Describe your role and contributions to the project.</p>
        <a href="https://github.com/yourusername/project-three" target="_blank" rel="noopener noreferrer">View on GitHub</a> |
        <a href="https://yourwebsite.com/project-three-demo" target="_blank" rel="noopener noreferrer">Live Demo</a>
      </div>
    </section>
  </main>
</template>

<script setup>
// No specific script needed for simple content
</script>

<style scoped>
.portfolio-view {
  padding: 40px 20px;
  text-align: center;
}

.portfolio-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); /* Responsive grid */
  gap: 30px;
  margin-top: 40px;
}

.portfolio-item {
  background-color: var(--color-background-main); /* Light background for items */
  border: 1px solid var(--color-accent-tan);
  border-radius: 8px;
  padding: 25px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.05);
  text-align: left;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.portfolio-item:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 16px rgba(0, 0, 0, 0.1);
}

.portfolio-item img {
  max-width: 100%;
  height: auto;
  border-radius: 5px;
  margin-bottom: 15px;
}

.portfolio-item h3 {
  font-size: 1.6rem;
  margin-bottom: 10px;
  color: var(--color-dark-brown);
}

.portfolio-item p {
  font-size: 0.95rem;
  color: #666;
  margin-bottom: 15px;
}

.portfolio-item a {
  display: inline-block;
  margin-right: 15px;
  font-weight: bold;
  color: var(--color-dark-brown); /* Link color */
}

.portfolio-item a:hover {
  color: var(--color-link-hover);
}

/* Keyframe Animations (can be the same as HomeView due to 'scoped') */
@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

/* Apply animations to specific elements */
.fade-in-up {
  opacity: 0; /* Start invisible */
  animation: fadeInUp 1s ease-out forwards;
}

/* Add delay to child elements for a staggered effect */
.fade-in-delay-1 { animation: fadeInUp 1s ease-out forwards; animation-delay: 0.3s; }
.fade-in-delay-2 { animation: fadeInUp 1s ease-out forwards; animation-delay: 0.6s; }
.fade-in-delay-3 { animation: fadeInUp 1s ease-out forwards; animation-delay: 0.9s; }
.fade-in-delay-4 { animation: fadeInUp 1s ease-out forwards; animation-delay: 1.2s; }
.fade-in-delay-5 { animation: fadeInUp 1s ease-out forwards; animation-delay: 1.5s; }

/* --- Media Queries for PortfolioView --- */
@media (max-width: 768px) {
  .portfolio-view {
    padding: 20px 10px;
  }

  .portfolio-grid {
    gap: 20px; /* Slightly less gap on smaller screens */
  }

  .portfolio-item {
    padding: 20px; /* Adjust padding inside items */
  }

  .portfolio-item h3 {
    font-size: 1.4rem; /* Smaller heading for project titles */
  }

  .portfolio-item p {
    font-size: 0.9rem; /* Smaller description text */
  }
}

</style>