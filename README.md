<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Portfolio</title>
    <style>
      html {
        box-sizing: border-box;
        font-size: 16px;
      }

      *,
      *:before,
      *:after {
        box-sizing: inherit;
      }

      body {
        margin: 0;
        padding: 0;
        font-family: Arial, sans-serif;
        line-height: 1.6;
        color: white;
        background: #1a1a1a;
      }

      #particles-js {
        position: fixed;
        width: 100%;
        height: 100%;
        z-index: -1;
      }

      header {
        background-color: rgba(20, 31, 31, 0.9);
        padding: 20px;
        position: sticky;
        top: 0;
        z-index: 10;
      }

      header nav ul {
        list-style: none;
        padding: 0;
        margin: 0;
        display: flex;
        justify-content: center;
        gap: 20px;
      }

      header nav ul li a {
        text-decoration: none;
        color: white;
        font-size: 18px;
        transition: color 0.3s;
      }

      header nav ul li a:hover {
        color: #f39c12;
      }

      .hero {
        color: white;
        text-align: center;
        padding: 100px 20px;
        position: relative;
      }

      .section {
        padding: 50px 20px;
        text-align: center;
        position: relative;
      }

      .portfolio {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        gap: 20px;
      }

      .project-link {
        display: block;
        text-decoration: none;
        transition: transform 0.3s;
      }

      .project-link:hover {
        transform: scale(1.1);
      }

      .portfolio img {
        width: 300px;
        border-radius: 10px;
        cursor: pointer;
      }

      footer {
        background-color: rgba(31, 31, 31, 0.9);
        color: white;
        padding: 20px 0;
        text-align: center;
        font-size: 0.9em;
        position: relative;
      }
    </style>
  </head>
  <body>
    <div id="particles-js"></div>

  <header>
      <nav>
        <ul>
          <li><a href="#about">About</a></li>
          <li><a href="#projects">Projects</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </nav>
    </header>

   <section class="hero">
      <h1>Irfan Ali Portfolio</h1>
      <p>Showcasing my passion for physics and coding</p>
    </section>

  <section class="section" id="about">
      <h2>About Me</h2>
      <p>
        Hi! I'm Irfan Ali, a versatile in artificial intelligence,
        technology, and problem-solving. Passionate about crafting innovative
        solutions and creating impactful projects.
      </p>
    </section>

   <section class="section" id="projects">
      <h2>My Projects</h2>
      <div class="portfolio">
        <a href="https://www.linkedin.com/feed/" class="project-link">
          <img src="https://cdn.glitch.global/5c431103-fdca-4afe-a020-4e5645f34df1/Screenshot%202025-01-22%20at%201.56.04%E2%80%AFAM.png?v=1737482203496project1.jpg" alt="Project 1" />
        </a>
        <a href="project2-details.html" class="project-link">
          <img src="project2.jpg" alt="Project 2" />
        </a>
        <a href="project3-details.html" class="project-link">
          <img src="project3.jpg" alt="Project 3" />
        </a>
        <a href="project4-details.html" class="project-link">
          <img src="project4.jpg" alt="Project 4" />
        </a>
      </div>
    </section>

  <section class="section" id="contact">
      <h2>Contact Me</h2>
      <p>
        If you'd like to work together or have any questions, feel free to reach
        out!
      </p>
      <p>
        Email:
        <a href="mailto:irfanalinazri4@gmail.com" style="color: #f39c12"
          >irfanalinazri4@gmail.com</a
        >
      </p>
      <p>
        Phone: <a href="https://wa.me/601154095214" style="color: #f39c12">+601154095214</a>
      </p>
    </section>

    <footer>
      <p>&copy; Irfan Ali Nazri. All Rights Reserved.</p>
    </footer>

    <script src="https://cdn.jsdelivr.net/particles.js/2.0.0/particles.min.js"></script>
    <script>
      particlesJS('particles-js',
        {
          particles: {
            number: { value: 80, density: { enable: true, value_area: 800 } },
            color: { value: "#ffffff" },
            shape: {
              type: "circle",
              stroke: { width: 0, color: "#000000" },
              polygon: { nb_sides: 5 }
            },
            opacity: {
              value: 0.5,
              random: false,
              anim: { enable: false, speed: 1, opacity_min: 0.1, sync: false }
            },
            size: {
              value: 3,
              random: true,
              anim: { enable: false, speed: 40, size_min: 0.1, sync: false }
            },
            line_linked: {
              enable: true,
              distance: 150,
              color: "#ffffff",
              opacity: 0.4,
              width: 1
            },
            move: {
              enable: true,
              speed: 6,
              direction: "none",
              random: false,
              straight: false,
              out_mode: "out",
              bounce: false,
              attract: { enable: false, rotateX: 600, rotateY: 1200 }
            }
          },
          interactivity: {
            detect_on: "canvas",
            events: {
              onhover: { enable: true, mode: "repulse" },
              onclick: { enable: true, mode: "push" },
              resize: true
            },
            modes: {
              grab: { distance: 400, line_linked: { opacity: 1 } },
              bubble: { distance: 400, size: 40, duration: 2, opacity: 8 },
              repulse: { distance: 200, duration: 0.4 },
              push: { particles_nb: 4 },
              remove: { particles_nb: 2 }
            }
          },
          retina_detect: true
        }
      );
    </script>
  </body>
</html>
