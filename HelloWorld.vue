<template>
  <div class="portfolio">
    <!-- Header Section -->
    <header class="header">
      <h1>{{ msg }}</h1>
    </header>
    <br />
    <br />

    <!-- Image Section -->
    <div class="image-container">
      <img
        alt="Vue logo"
        src="../assets/logo.png"
        style="max-width: 200px; height: auto"
      />
    </div>

    <!-- Full Stack Developer Section -->
    <section
      class="full-stack"
      style="background-color: #f2f2f2; padding: 20px; border-radius: 10px"
    >
      <h2 style="font-size: 24px; color: #333; text-align: center">
        Full Stack Developer
      </h2>
      <p
        style="
          font-size: 18px;
          line-height: 1.6;
          color: #555;
          text-align: justify;
        "
      >
        <!-- Full Stack Developer Description -->
        As a Full Stack Developer, I bring a versatile skill set to the table,
        encompassing both front-end and back-end development. With a strong
        foundation in programming languages such as HTML, CSS, JavaScript, and
        proficiency in server-side technologies like Node.js and Python, I have
        the ability to create responsive and dynamic web applications. My
        experience in database management and API integration further enhances
        my capability to deliver end-to-end solutions.
      </p>
      <h3
        style="
          background: linear-gradient(135deg, #ff6b6b, #ffda77);
          display: inline;
          padding: 10px;
          border-radius: 5px;
          color: #fff;
          font-size: 20px;
        "
      >
        Skills
      </h3>

      <ul>
        <!-- Skills List -->
        <li>
          <button class="skill-button">
            Front-end development with Vue.js, React, and Angular
          </button>
        </li>
        <li>
          <button class="skill-button">
            Back-end development with Node.js, Express.js, and Ruby on Rails
          </button>
        </li>
        <li>
          <button class="skill-button">
            Database design and management with SQL and NoSQL databases
          </button>
        </li>
        <li>
          <button class="skill-button">RESTful API development</button>
        </li>
        <li>
          <button class="skill-button">
            Version control with Git and GitHub
          </button>
        </li>
      </ul>
    </section>

    <!-- Additional Projects Section -->
    <section
      class="projects"
      style="
        background: linear-gradient(135deg, #69d2e7, #a7dbd8);
        padding: 20px;
        border-radius: 10px;
        margin-top: 20px;
      "
    >
      <h2
        style="
          background: linear-gradient(135deg, #f38630, #ef3340);
          display: inline;
          padding: 10px;
          border-radius: 5px;
          color: #fff;
          font-size: 24px;
        "
      >
        Additional Projects
      </h2>
      <ul
        style="
          list-style-type: none;
          display: flex;
          justify-content: space-around;
        "
      >
        <!-- Project Links -->
        <li>
          <a
            href="#"
            target="_blank"
            rel="noopener"
            style="
              display: inline-block;
              padding: 10px 20px;
              background-color: #00008b;
              color: #fff;
              text-decoration: none;
              border-radius: 5px;
            "
            >E-commerce</a
          >
        </li>
        <li>
          <a
            href="#"
            target="_blank"
            rel="noopener"
            style="
              display: inline-block;
              padding: 10px 20px;
              background-color: #800080;
              color: #ffffff;
              text-decoration: none;
              border-radius: 5px;
            "
            >Blog Platform</a
          >
        </li>
        <li>
          <a
            href="#"
            target="_blank"
            rel="noopener"
            style="
              display: inline-block;
              padding: 10px 20px;
              background-color: #f38630;
              color: #fff;
              text-decoration: none;
              border-radius: 5px;
            "
            >Weather App</a
          >
        </li>
      </ul>
    </section>

    <!-- About Me Section -->
    <section class="about">
      <h2>About Me</h2>
      <p style="font-style: italic; color: #a52a2a">
        <!-- About Me Description -->
        I am a passionate
        <span style="font-weight: bold; color: #333">Vue.js</span>
        developer with a strong background in web development. I love creating
        interactive and dynamic web applications. With a keen eye for design and
        a commitment to clean, efficient code, I consistently strive to create
        seamless user experiences. I am passionate about staying up-to-date with
        the latest industry trends and technologies, ensuring that my projects
        are cutting-edge and future-proof.
      </p>
    </section>

    <!-- Contact Section -->
    <section class="contact">
      <h2>Contact</h2>
      <p>
        Feel free to contact me at
        <a href="mailto:youremail@example.com">youremail@example.com</a>.
      </p>
      <div class="contact-buttons">
        <button class="btn-primary">Email Me</button>
        <button class="btn-secondary">LinkedIn</button>
        <button class="btn">GitHub</button>
      </div>
    </section>
  </div>
</template>

<script>
// Vue component definition
export default {
  name: "PortfolioPage",
  props: {
    msg: String, // Define a prop for the component
  },
};
</script>

<style scoped>
/* Portfolio Container Styles */
.portfolio {
  font-family: Arial, sans-serif;
  max-width: 800px;
  margin: 0 auto;
  padding: 20px;
  background-color: #f0f0f0;
  animation: fadeIn 1s ease-in-out; /* Fade-in animation */
}

/* Animation Keyframes */
@keyframes fadeIn {
  from {
    opacity: 0; /* Start with zero opacity */
  }
  to {
    opacity: 1; /* Fade to full opacity */
  }
}

/* Body Background */
body {
  background-color: #e6f7ff; /* Light blue background color */
}

/* Header Styles */
.header {
  display: flex;
  align-items: center;
  background-color: #6495ed; /* Blue header background */
  color: white; /* Text color */
  padding: 10px;
  border-radius: 5px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1); /* Box shadow */
  animation: slideDown 1s ease-in-out; /* Slide-down animation */
}

/* Animation Keyframes */
@keyframes slideDown {
  from {
    transform: translateY(-20px); /* Start position */
    opacity: 0; /* Start with zero opacity */
  }
  to {
    transform: translateY(0); /* End position */
    opacity: 1; /* Fade to full opacity */
  }
}

h1 {
  font-size: 24px;
  animation: fadeInUp 1s ease-in-out; /* Animation */
}

@keyframes fadeInUp {
  from {
    transform: translateY(-20px);
    opacity: 0;
  }
  to {
    transform: translateY(0);
    opacity: 1;
  }
}

.header {
  display: flex;
  align-items: center;
  background-color: #42b983;
  color: white;
  padding: 10px;
  border-radius: 5px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
}

h1 {
  font-size: 24px;
}

.projects h2,
.about h2,
.contact h2 {
  font-size: 24px;
  margin-top: 30px;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  margin: 10px 0;
}

a {
  color: #42b983;
  text-decoration: none;
}

a:hover {
  text-decoration: underline;
}

.contact-buttons {
  margin-top: 20px;
}

.btn-primary,
.btn-secondary {
  padding: 10px 20px;
  font-size: 16px;
  margin-right: 10px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

.btn {
  padding: 10px 20px;
  font-size: 16px;
  margin-right: 10px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

.btn-primary {
  background-color: #ffa500;
  color: white;
}

.btn {
  background-color: #ffa500;
  color: white;
}

.btn-secondary {
  background-color: #00008b;
  color: white;
}

h3 {
  font-weight: bold;
}

.skill-button {
  font-weight: bold;
  background-color: #3498db;
  color: #fff;
  padding: 10px 20px;
  border: none;
  border-radius: 5px;
  margin: 5px 0;
}
.skill-button:hover {
  background-color: #007bff;
}

.projects {
  background-color: #f0f0f0;
  padding: 20px;
  border-radius: 10px;
  max-height: 150px;
}

.projects h2 {
  font-size: 24px;
  color: #333;
  margin-bottom: 10px;
}

.projects ul {
  list-style: none;
  padding: 0;
}

.projects li {
  font-size: 18px;
  margin-bottom: 10px;
}

.projects a {
  text-decoration: none;
  color: #0077cc;
  font-weight: bold;
  transition: color 0.3s;
}

.projects a:hover {
  color: #ff6600;
}
</style>
