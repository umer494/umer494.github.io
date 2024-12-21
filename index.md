<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Umer Farooq Bhat | Portfolio</title>
  <link rel="stylesheet" href="styles.css">
  <script src="https://kit.fontawesome.com/a076d05399.js" crossorigin="anonymous"></script>
  <style>
    /* Reset */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
      color: #333;
      background-color: #f4f4f9;
    }

    .navbar {
      display: flex;
      justify-content: center;
      position: sticky;
      top: 0;
      background-color: #333;
      padding: 1em;
      z-index: 1000;
    }

    .navbar ul {
      list-style: none;
      display: flex;
    }

    .navbar ul li {
      margin: 0 1em;
    }

    .navbar ul li a {
      text-decoration: none;
      color: #fff;
      font-weight: bold;
      transition: color 0.3s;
    }

    .navbar ul li a:hover {
      color: #ffa500;
    }

    .hero {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
      background: linear-gradient(to right, #4facfe, #00f2fe);
      color: #fff;
      text-align: center;
    }

    .hero button {
      padding: 10px 20px;
      background-color: #ffa500;
      color: #fff;
      border: none;
      cursor: pointer;
      font-size: 1rem;
      border-radius: 5px;
      transition: background-color 0.3s;
    }

    .hero button:hover {
      background-color: #333;
    }

    .profile-pic {
      display: block;
      margin: 20px auto;
      border-radius: 50%;
      width: 150px;
      height: 150px;
    }

    #skills .skills-container {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 20px;
    }

    .skill {
      width: 300px;
      background-color: #fff;
      padding: 10px;
      border: 1px solid #ccc;
      border-radius: 5px;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    }

    .skill-bar {
      background-color: #f4f4f9;
      border: 1px solid #ccc;
      border-radius: 5px;
      overflow: hidden;
      margin-top: 5px;
    }

    .skill-bar .level {
      height: 20px;
      background-color: #4caf50;
      text-align: right;
      padding-right: 5px;
      color: #fff;
      line-height: 20px;
    }

    .projects-container {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 20px;
    }

    .project {
      background-color: #fff;
      border: 1px solid #ccc;
      padding: 15px;
      border-radius: 5px;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    }

    footer {
      background-color: #333;
      color: #fff;
      text-align: center;
      padding: 1em 0;
    }

    .social-media a {
      color: #fff;
      margin: 0 10px;
      text-decoration: none;
      font-size: 1.2rem;
      transition: color 0.3s;
    }

    .social-media a:hover {
      color: #ffa500;
    }
  </style>
</head>
<body>
  <header>
    <nav class="navbar fixed">
      <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#experience">Experience</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <section id="home" class="hero">
    <h1>Welcome to My Portfolio</h1>
    <p>Hi, I'm Umer Farooq Bhat, a passionate .NET and SQL developer.</p>
    <button id="downloadCV">Download CV</button>
  </section>

  <section id="profile">
    <img src="profile.jpg" alt="Profile Picture" class="profile-pic">
    <p>A motivated developer specializing in .NET, SQL, and front-end technologies like Angular and React.</p>
  </section>

  <section id="skills">
    <h2>Skills</h2>
    <div class="skills-container">
      <div class="skill">
        <span>Frontend</span>
        <div class="skill-bar"><div class="level" style="width: 85%;">85%</div></div>
      </div>
      <div class="skill">
        <span>Backend</span>
        <div class="skill-bar"><div class="level" style="width: 90%;">90%</div></div>
      </div>
      <div class="skill">
        <span>Database</span>
        <div class="skill-bar"><div class="level" style="width: 95%;">95%</div></div>
      </div>
    </div>
  </section>

  <section id="projects">
    <h2>Projects</h2>
    <div class="projects-container">
      <div class="project">
        <h3>Project 1</h3>
        <p>Details about project 1.</p>
        <a href="https://github.com/username/project1" target="_blank">View on GitHub</a>
      </div>
      <div class="project">
        <h3>Project 2</h3>
        <p>Details about project 2.</p>
        <a href="https://github.com/username/project2" target="_blank">View on GitHub</a>
      </div>
    </div>
  </section>

  <section id="experience">
    <h2>Experience</h2>
    <ul>
      <li>
        <h3>Société Générale</h3>
        <p>Role: .NET Developer</p>
        <p>Responsibilities: ACR, automation, KT sessions, and project ownership.</p>
      </li>
      <li>
        <h3>Accenture</h3>
        <p>Role: Packaged Application Developer Analyst</p>
        <p>Responsibilities: Technical training, SSIS packages, and database migration.</p>
      </li>
    </ul>
  </section>

  <section id="contact">
    <h2>Contact Me</h2>
    <form action="#" method="post">
      <label for="name">Name:</label>
      <input type="text" id="name" name="name" required>

      <label for="email">Email:</label>
      <input type="email" id="email" name="email" required>

      <label for="message">Message:</label>
      <textarea id="message" name="message" required></textarea>

      <button type="submit">Send</button>
    </form>
    <p id="confirmationMessage"></p>
  </section>

  <footer>
    <p>&copy; 2024 Umer Farooq Bhat. All Rights Reserved.</p>
    <div class="social-media">
      <a href="https://linkedin.com/in/username" target="_blank"><i class="fab fa-linkedin"></i></a>
      <a href="https://github.com/username" target="_blank"><i class="fab fa-github"></i></a>
      <a href="https://twitter.com/username" target="_blank"><i class="fab fa-twitter"></i></a>
    </div>
  </footer>

  <script>
    document.querySelector('form').addEventListener('submit', function(e) {
      e.preventDefault();
      document.getElementById('confirmationMessage').textContent = 'Thank you for your message!';
    });
  </script>
</body>
</html>
