<template>
  <main class="home-view">
    <section class="hero-section" fade-in-up>
      <!-- <img src="/your-profile-pic.jpg" alt="Your Profile Picture" class="profile-pic fade-in-delay-1"> -->
      <h1 class="fade-in-delay-2">Hi, I'm Kelvin Augustino Mwashiga</h1>
      <p class="tagline fade-in-delay-3">Passionate Computer Scientist | Building Innovative Web Experiences</p>
      <p class="fade-in-delay-4">Welcome to my personal corner of the internet! I'm a Computer Scientist with a strong foundation in web development, eager to bring creative ideas to life. I specialize in Software Development, Networking and Computer Hardware and Software Maintenance, with a keen eye for detail and a love for elegant solutions.</p>
      <p class="fade-in-delay-5">Explore my <RouterLink to="/portfolio">portfolio</RouterLink> to see some of my recent work, or check out my <RouterLink to="/resume">resume</RouterLink> for a detailed look at my professional journey.</p>
    </section>
  </main>
</template>

<script setup>
// No specific script needed for simple content
</script>

<style scoped>
/* Specific styles for HomeView */
.home-view {
  padding: 40px 20px; /* More padding for home */
  text-align: center;
}

.hero-section {
  background-color: var(--color-secondary-light);
  padding: 60px 20px;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.profile-pic {
  width: 150px;
  height: 150px;
  border-radius: 50%; /* Makes it a circle */
  object-fit: cover; /* Ensures image covers the area */
  margin-bottom: 20px;
  border: 4px solid var(--color-dark-brown); /* Border matching palette */
  box-shadow: 0 0 15px rgba(0, 0, 0, 0.15);
}

h1 {
  font-size: 2.8rem;
  margin-bottom: 15px;
  color: var(--color-dark-brown);
}

.tagline {
  font-size: 1.4rem;
  color: #555;
  margin-bottom: 30px;
}

p {
  font-size: 1.1rem;
  line-height: 1.8;
  max-width: 800px;
  margin: 0 auto 15px auto;
}

p a {
  color: var(--color-dark-brown); /* Link color from palette */
  font-weight: bold;
}

p a:hover {
  text-decoration: underline;
}

/* keyframe animations */
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
.fade-in-delay-1 { animation-delay: 0.3s; }
.fade-in-delay-2 { animation-delay: 0.6s; }
.fade-in-delay-3 { animation-delay: 0.9s; }
.fade-in-delay-4 { animation-delay: 1.2s; }
.fade-in-delay-5 { animation-delay: 1.5s; } /* Adjust delays as you add more content */

/* --- Media Queries for HomeView --- */
@media (max-width: 768px) {
  .home-view {
    padding: 20px 10px; /* Reduce horizontal padding on smaller screens */
  }

  .hero-section {
    padding: 40px 15px; /* Reduce padding inside hero section */
  }

  .profile-pic {
    width: 120px; /* Smaller profile pic on mobile */
    height: 120px;
  }

  h1 {
    font-size: 2.2rem; /* Smaller heading for mobile */
  }

  .tagline {
    font-size: 1.2rem; /* Smaller tagline for mobile */
  }

  p {
    font-size: 1rem; /* Slightly smaller body text */
  }
}

</style>