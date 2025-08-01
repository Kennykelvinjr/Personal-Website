<template>
  <main class="resume-view">
    <h1>My Resume & CV</h1>
    <p>A comprehensive overview of my professional journey, skills, and educational background.</p>

    <section class="cv-download-section">
      <h2>Download My CV</h2>
      <p>Prefer a traditional document? Download my full CV in PDF format.</p>
      <a href="/KelvinCV.pdf" download class="download-button">
        Download CV (PDF)
      </a>
    </section>
    <section class="resume-section">
      <h2>Summary</h2>
      <p>Motivated and detail-oriented software developer with a strong foundation in computer science and a passion for building innovative, user-centric digital solutions. Skilled in programming, web development, and problem-solving, with a commitment to continuous learning and delivering high-quality applications that meet user needs.</p>
    </section>

    <section class="resume-section">
      <h2>Work Experience</h2>
      <div class="experience-item">
        <h3>Software Development Practical Training at President's Office - Regional Administration & Local Government Authorities (PO - RALG)</h3>
        <p class="duration">July 2023 - September 2023</p>
        <ul>
          <li>Developed and maintained web applications using Laravel.</li>
          <li>Collaborated with a team of trainees to develop a practical training management system.</li>
          <li>Conducted code reviews and debugging, reducing application errors.</li>
          <li>Conducted routine computer hardware and software maintenance.</li>
        </ul>
      </div>
      <div class="experience-item">
        <h3>Web Development Practical Training at University of Dar es Salaam ICT Innovation Hub (UDICTI-FINHUB)</h3>
        <p class="duration">July 2024 - September 2024</p>
        <ul>
          <li>Designed and developed responsive websites for CRDB Bank Innovation Challenge of "Banking for Unbanked" using Vue JS.</li>
          <li>Trained on Human - Centric Design.</li>
        </ul>
      </div>
    </section>

    <section class="resume-section">
      <h2>Education</h2>
      <div class="education-item">
        <h3>Bachelor of Science in Computer Science</h3>
        <p>University of Dar es Salaam | Expected Graduation: November 2025</p>
        <p>Relevant Coursework: Data Structures, Algorithms, Artificial Intelligence, Web Development, Database Systems, Data Mining, Software Engineering, Mobile Applications Development & Principles of System Security.</p>
      </div>
      <div class="education-item">
        <h3>Advanced Level Education</h3>
        <p>St. Augustine Tagaste Secondary School | 2020-2022</p>
        <p>Subjects: Physics, Chemistry, Mathematics (PCM)</p>
      </div>
      <div class="education-item">
        <h3>Ordinary Level Education</h3>
        <p>Centennial Christian Seminary | 2016-2019</p>
        <p>Division I, Certificate of Secondary Education Examination (CSEE)</p>
      </div>
      <div class="education-item">
        <h3>Primary School Education</h3>
        <p>Rocken Hill Primary School | 2009-2015</p>
        <p>Primary School Leaving Examination (PSLE)</p>
      </div>
    </section>

    <section class="resume-section">
      <h2>Skills</h2>
      <div class="skills-category">
        <h3>Programming Languages:</h3>
        <p>Python, JavaScript & Java</p>
      </div>
      <div class="skills-category">
        <h3>Web Development:</h3>
        <p>HTML, CSS, Vue.js, Django, Flask, Express JS, Laravel</p>
      </div>
      <div class="skills-category">
        <h3>Tools & Technologies:</h3>
        <p>Git, Docker, MySQL, REST APIS</p>
      </div>
      <div class="skills-category">
        <h3>Soft Skills:</h3>
        <p>Teamwork, Problem-Solving, Communication, Time Management</p>
      </div>
      <div class="skills-category">
        <h3>Microsoft Tools:</h3>
        <p>Word, Excel, PowerPoint, Outlook</p>
      </div>
    </section>

    <section class="resume-section">
      <h2>Projects</h2>
      <div class="experience-item">
        <h3>Red Light Violation System</h3>
        <p class="duration">University Final Year Project, 2025</p>
        <ul>
          <li>Used Python Programming Language and packages such as NumPy and cv for coding and training a YOLO model to detect red light signal on traffic lights and license plates of detecting vehicles.</li>
          <li>Used paddle OCR for Optical Character Recognition so as to read the violating plates.</li>
          <li>Implemented MySQL database for data storage and extracting details for reporting.</li>
          <li>Used SMS gateway to send texts containing violation details and control number for payments to violators.</li>
        </ul>
      </div>
      <div class="experience-item">
        <h3>Personal Portfolio Website</h3>
        <p class="duration">Personal Project, 2023</p>
        <ul>
          <li>Built a responsive portfolio website using HTML, CSS, and JavaScript to showcase projects and skills.</li>
          <li>Outcome: Increased professional visibility, receiving positive feedback from potential employers.</li>
        </ul>
      </div>
    </section>

    <section class="resume-section">
      <h2>Certifications</h2>
      <p>Coursiv certification on in-depth training and skill development in using AI tools such as ChatGPT, Jasper AI and Midjourney.</p>
    </section>

    <section class="resume-section">
      <h2>Language Proficiency</h2>
      <ul>
        <li>English: Fluent</li>
        <li>Kiswahili: Native and Fluent</li>
      </ul>
    </section>

    <section class="resume-section">
      <h2>Hobbies & Interests</h2>
      <ul>
        <li>Contributing to open-source projects on GitHub.</li>
        <li>Exploring new programming frameworks, updates and technologies.</li>
      </ul>
    </section>

    <section class="resume-section">
      <h2>References</h2>
      <p>Available upon request.</p>
    </section>

    <section class="resume-section">
        <h2>Contact Me</h2>
        <p>Feel free to reach out to me via email at <a href="mailto:mwashigakelvin@gmail.com">mwashigakelvin@gmail.com</a> or connect with me on <a href="https://github.com/Kennykelvinjr" target="_blank" rel="noopener noreferrer">GitHub</a>.</p>
    </section>

  </main>
</template>

<script setup>
// No specific script needed for simple content
</script>

<style scoped>
/* Keep all your existing styles here. The new sections will automatically pick up the .resume-section styling. */
/* You might want to remove the specific .cv-download-section styles if you removed the section from template */
.resume-view {
  padding: 40px 20px;
  max-width: 800px;
  margin: 0 auto;
}

.resume-section {
  background-color: var(--color-background-main);
  border-radius: 8px;
  padding: 30px;
  margin-bottom: 30px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.05);
}

.resume-section h2 {
  font-size: 2.2rem;
  color: var(--color-dark-brown);
  margin-bottom: 20px;
  border-bottom: 2px solid var(--color-accent-tan);
  padding-bottom: 10px;
}

.experience-item, .education-item {
  margin-bottom: 25px;
  padding-left: 15px;
  border-left: 4px solid var(--color-primary-light);
}

.experience-item h3, .education-item h3 {
  font-size: 1.5rem;
  margin-bottom: 5px;
  color: var(--color-dark-brown);
}

.duration {
  font-style: italic;
  color: #666;
  margin-bottom: 10px;
}

.experience-item ul {
  list-style: disc;
  margin-left: 20px;
  margin-top: 10px;
}

.experience-item li {
  margin-bottom: 5px;
}

.skills-category h3 {
  font-size: 1.3rem;
  margin-top: 15px;
  margin-bottom: 5px;
  color: var(--color-dark-brown);
}

.skills-category p {
  font-size: 1.05rem;
  color: #555;
}

.resume-section a {
    font-weight: bold;
    color: var(--color-dark-brown);
}

/* NEW: Styles for CV Download Section (KEEP if you want the section here) */
.cv-download-section {
  background-color: var(--color-primary-light); /* Use one of your lighter colors */
  border-radius: 8px;
  padding: 30px;
  margin-bottom: 30px;
  text-align: center; /* Center the content */
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
  animation: fadeInUp 0.8s ease-out forwards; /* Add an animation to it */
  animation-delay: 0.2s; /* Give it a slight delay */
}

.cv-download-section h2 {
  font-size: 2rem;
  color: var(--color-dark-brown);
  margin-bottom: 15px;
  border-bottom: none; /* No border for this section heading */
  padding-bottom: 0;
}

.cv-download-section p {
  font-size: 1.1rem;
  margin-bottom: 25px;
  color: #555;
}

.download-button {
  display: inline-block; /* Allows padding and margin */
  background-color: var(--color-dark-brown); /* Your primary accent color */
  color: var(--color-background-main); /* Light text on dark button */
  padding: 15px 30px;
  border-radius: 5px;
  text-decoration: none;
  font-weight: bold;
  font-size: 1.2rem;
  transition: background-color 0.3s ease, transform 0.2s ease;
  box-shadow: 0 3px 6px rgba(0, 0, 0, 0.2);
}

.download-button:hover {
  background-color: var(--color-link-hover); /* A slightly darker shade on hover */
  transform: translateY(-2px); /* Subtle lift effect */
  text-decoration: none; /* Ensure no underline on hover */
}

/* Keep or add the fadeInUp keyframes if not already present in this file's scoped style */
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


/* --- Media Queries for ResumeView --- */
@media (max-width: 768px) {
  .resume-view {
    padding: 20px 10px;
  }

  .resume-section {
    padding: 20px;
    margin-bottom: 20px;
  }

  .resume-section h2 {
    font-size: 1.8rem;
  }

  .experience-item h3, .education-item h3 {
    font-size: 1.3rem;
  }

  .experience-item ul {
    margin-left: 15px;
  }

  .experience-item li, .skills-category p {
    font-size: 0.95rem;
  }
}
</style>