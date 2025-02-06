<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>About Me - Irfan Alinazri</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/particles.js"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" integrity="sha512-Fo3rlrZj/k7ujTnH2N2o33r5m14JWpHJph8HU6/3vl89v5k51FJg5Cef+xVSTCwq1rI5D07D4Myhht5Jp6Iw3Q==" crossorigin="anonymous" referrerpolicy="no-referrer" />
    <style>
      body {
        font-family: 'Inter', sans-serif;
      }
      #particles-js {
        position: fixed;
        width: 100%;
        height: 100%;
        top: 0;
        left: 0;
        z-index: -1;
        background: linear-gradient(135deg, #1f2937, #3b82f6);
      }
    </style>
  </head>
  <body class="bg-gray-50 font-sans leading-normal tracking-normal">
    <div id="particles-js"></div>
    <header class="bg-gray-800 text-white py-4">
      <div class="container mx-auto px-6 flex justify-between items-center">
        <h1 class="text-2xl font-bold">Irfan Alinazri</h1>
        <nav>
          <a href="index.html" class="text-white hover:text-gray-300 px-3">Home</a>
          <a href="projects.html" class="text-white hover:text-gray-300 px-3">Projects</a>
          <a href="contact.html" class="text-white hover:text-gray-300 px-3">Contact</a>
        </nav>
      </div>
    </header>

   <section class="container mx-auto px-6 py-10">
      <h2 class="text-4xl font-bold text-gray-800 mb-6">About Me</h2>
      <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
        <div>
          <p class="text-gray-700 text-lg mb-4">
            Hello! I’m Irfan Ali Nazri, a versatile professional with expertise in Islamic Studies, Applied Physics, tutoring, sales analysis, and design. I enjoy exploring the intersection of technology, education, and creativity.
          </p>
          <p class="text-gray-700 text-lg mb-4">
            I’m passionate on solving problems, building meaningful connections, and contributing to impactful projects. As a neurodivergent learner, I excel in practical, analytical thinking and leveraging innovative methods to stay engaged in my learning and work.
          </p>
          <button onclick="toggleTheme()" class="bg-gray-800 text-white py-2 px-4 mt-4 rounded shadow">Toggle Dark Mode</button>
        </div>
        <div>
          <img src="https://via.placeholder.com/400x300" alt="Irfan Alinazri Profile Picture" class="rounded-lg shadow-lg" />
        </div>
      </div>
    </section>

   <section class="bg-gray-100 py-10">
      <div class="container mx-auto px-6">
        <h3 class="text-3xl font-bold text-gray-800 mb-4">Skills</h3>
        <div class="grid grid-cols-2 md:grid-cols-3 gap-4">
          <span class="bg-white p-4 rounded shadow">Physics Tutoring</span>
          <span class="bg-white p-4 rounded shadow">Arabic Transcription</span>
          <span class="bg-white p-4 rounded shadow">Sales Analysis</span>
          <span class="bg-white p-4 rounded shadow">Power BI</span>
          <span class="bg-white p-4 rounded shadow">Excel Analysis</span>
          <span class="bg-white p-4 rounded shadow">Fusion 360</span>
        </div>
      </div>
    </section>

   <section class="py-10">
      <div class="container mx-auto px-6">
        <h3 class="text-3xl font-bold text-gray-800 mb-4">My Philosophy</h3>
        <p class="text-gray-700 text-lg mb-6">
          I believe in continuous learning and adaptability. By combining my interests in strategy, upskilling, and motivation, I aim to deliver creative solutions and impactful results.
        </p>
        <form id="subscribeForm" class="bg-white p-6 rounded shadow-md">
          <label for="email" class="block text-gray-700 font-bold mb-2">Subscribe to Updates:</label>
          <input type="email" id="email" name="email" class="w-full p-2 border rounded mb-4" placeholder="Enter your email..." required />
          <button type="submit" class="bg-gray-800 text-white py-2 px-4 rounded">Subscribe</button>
        </form>
        <div id="formResponse" class="mt-4"></div>
      </div>
    </section>

  <footer class="bg-gray-800 text-white py-6">
      <div class="container mx-auto px-6 text-center">
        <p>&copy; 2025 Irfan Ali Nazri. All rights reserved.</p>
        <p class="mt-2">
          <a href="https://github.com" target="_blank" class="text-gray-300 hover:text-white mx-2"><i class="fab fa-github"></i></a>
          <a href="https://linkedin.com" target="_blank" class="text-gray-300 hover:text-white mx-2"><i class="fab fa-linkedin"></i></a>
        </p>
      </div>
    </footer>

  <script>
      // Initialize Particles.js
      particlesJS.load('particles-js', 'https://cdn.jsdelivr.net/particles.js/2.0.0/particles.json', function() {
        console.log('Particles.js configuration loaded.');
      });

      // Dark Mode Toggle
      function toggleTheme() {
        document.body.classList.toggle('bg-gray-900');
        document.body.classList.toggle('text-white');
      }

      // Form Submission Handling
      document.getElementById('Form').addEventListener('submit', function (event) {
        event.preventDefault();
        const email = document.getElementById('email').value;
        document.getElementById('formResponse').innerText = `Thank you, ${email}!`;
      });
    </script>
  </body>
</html>
