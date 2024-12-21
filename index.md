<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Umer Farooq Bhat - Portfolio</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&display=swap" rel="stylesheet">
    <link rel="icon" href="favicon.ico">
    <script src="https://kit.fontawesome.com/a076d05399.js"></script>
    <style>
        /* Global styles */
        body {
            font-family: 'Roboto', sans-serif;
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            color: #333;
        }

        h1, h2, h3 {
            margin: 0;
            font-weight: 700;
        }

        header {
            background: #1E293B;
            padding: 20px 40px;
            color: white;
        }

        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .nav-links {
            display: flex;
            gap: 20px;
            list-style-type: none;
        }

        .nav-links li {
            padding: 10px;
        }

        .nav-links a {
            color: white;
            text-decoration: none;
        }

        .hamburger {
            display: none;
            cursor: pointer;
        }

        .hero {
            background: #f7fafc;
            padding: 80px 20px;
            text-align: center;
        }

        .hero h1 {
            font-size: 3rem;
        }

        .profile-container {
            text-align: center;
            margin-top: -60px;
        }

        .profile-container img {
            width: 150px;
            height: 150px;
            border-radius: 50%;
        }

        .profile-container h2 {
            margin-top: 20px;
        }

        .profile-container p {
            color: #555;
        }

        .skills-container, .projects-container {
            display: flex;
            flex-wrap: wrap;
            gap: 30px;
            justify-content: center;
        }

        .skill, .project-card {
            background: #fff;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            width: 100%;
            max-width: 250px;
            text-align: center;
            transition: transform 0.3s ease-in-out;
        }

        .skill:hover, .project-card:hover {
            transform: scale(1.05);
        }

        .skills-container .skill i {
            font-size: 40px;
            color: #1E293B;
        }

        .projects-container .project-card h3 {
            margin-top: 10px;
        }

        .contact {
            background: #e5e7eb;
            padding: 50px 20px;
            text-align: center;
        }

        input, textarea {
            width: 100%;
            padding: 12px;
            margin: 10px 0;
            border: 1px solid #ccc;
            border-radius: 5px;
        }

        button {
            padding: 15px 25px;
            background-color: #1E293B;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }

        footer {
            background-color: #1E293B;
            color: white;
            padding: 20px;
            text-align: center;
        }

        .social-icons i {
            font-size: 24px;
            margin: 10px;
            color: #fff;
            transition: color 0.3s ease;
        }

        .social-icons i:hover {
            color: #1E293B;
        }

        .social-icons a {
            text-decoration: none;
        }

        /* Mobile responsive */
        @media (max-width: 768px) {
            .nav-links {
                display: none;
                flex-direction: column;
            }
            .nav-links.active {
                display: flex;
            }
            .hamburger {
                display: block;
            }
        }
    </style>
</head>
<body>
    <header>
        <nav class="navbar">
            <h1 class="logo">Umer Farooq Bhat</h1>
            <ul class="nav-links">
                <li><a href="#about">About</a></li>
                <li><a href="#skills">Skills</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
            <div class="hamburger" id="hamburger">
                <i class="fas fa-bars"></i>
            </div>
        </nav>
    </header>

    <section id="hero" class="hero">
        <div class="hero-content">
            <h1>Welcome to My Portfolio</h1>
            <p>I am Umer Farooq Bhat, a passionate .NET Developer & Data Analyst.</p>
            <a href="cv/Umer_Farooq_Bhat_CV.pdf" download>
                <button>Download CV</button>
            </a>
        </div>
    </section>

    <section class="profile-container">
        <img src="images/profile.jpg" alt="Umer Farooq Bhat">
        <h2>Umer Farooq Bhat</h2>
        <p>Experienced .NET Developer & Data Analyst with expertise in MVC, SQL, and data-driven solutions.</p>
    </section>

    <section id="about" class="about">
        <h2>About Me</h2>
        <p>I am a software developer with a focus on creating efficient and scalable applications. I love learning new technologies and collaborating with teams to solve complex problems.</p>
    </section>

    <section id="skills" class="skills">
        <h2>Skills</h2>
        <div class="skills-container">
            <div class="skill">
                <i class="fab fa-html5"></i>
                <h3>HTML</h3>
                <p>Proficient in creating responsive and structured web pages.</p>
            </div>
            <div class="skill">
                <i class="fab fa-css3-alt"></i>
                <h3>CSS</h3>
                <p>Experienced in styling web pages with modern CSS techniques.</p>
            </div>
            <div class="skill">
                <i class="fab fa-js"></i>
                <h3>JavaScript</h3>
                <p>Skilled in client-side scripting and dynamic web functionality.</p>
            </div>
            <div class="skill">
                <i class="fas fa-database"></i>
                <h3>SQL</h3>
                <p>Expert in working with relational databases and query optimization.</p>
            </div>
            <div class="skill">
                <i class="fab fa-dot-net"></i>
                <h3>.NET Framework</h3>
                <p>Experienced in developing applications with MVC and C#.</p>
            </div>
            <div class="skill">
                <i class="fab fa-react"></i>
                <h3>React</h3>
                <p>Building dynamic, responsive user interfaces with React.</p>
            </div>
        </div>
    </section>

    <section id="experience" class="experience">
        <h2>Experience</h2>
        <div class="experience-item">
            <h3>Imarticus Learning</h3>
            <p><strong>Role:</strong> Data Analyst | <strong>Duration:</strong> June 2023 - Present</p>
            <p>Worked on projects involving data analysis and business intelligence, helping clients derive actionable insights from large datasets.</p>
        </div>
        <div class="experience-item">
            <h3>Société Générale</h3>
            <p><strong>Role:</strong> .NET Developer | <strong>Duration:</strong> January 2022 - Present</p>
            <p>Involved in developing and maintaining applications using .NET Framework, focusing on scalability and performance optimization.</p>
        </div>
    </section>

    <section id="projects" class="projects">
        <h2>My Projects</h2>
        <div class="projects-container" id="projects-container">
            <!-- Dynamic projects will be loaded here -->
        </div>
    </section>

    <section id="contact" class="contact">
        <h2>Contact Me</h2>
        <form id="contact-form">
            <input type="text" id="name" placeholder="Your Name" required>
            <input type="email" id="email" placeholder="Your Email" required>
            <textarea id="message" placeholder="Your Message" required></textarea>
            <button type="submit">Send Message</button>
        </form>
    </section>

    <footer class="footer">
        <div class="social-icons">
            <a href="https://www.linkedin.com/in/umer-farooq-bhat" target="_blank">
                <i class="fab fa-linkedin"></i>
            </a>
            <a href="https://github.com/umer494" target="_blank">
                <i class="fab fa-github"></i>
            </a>
            <a href="mailto:umerfarooq@example.com">
                <i class="fas fa-envelope"></i>
            </a>
        </div>
        <p>&copy; 2024 Umer Farooq Bhat. All Rights Reserved.</p>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            // Projects Data
            const projects = [
                {
                    title: "Portfolio Website",
                    description: "A personal portfolio website built using HTML, CSS, and JavaScript.",
                    image: "images/portfolio.jpg",
                    link: "https://github.com/umer494/portfolio",
                    tech: ["HTML", "CSS", "JavaScript"]
                },
                {
                    title: "Weather App",
                    description: "A weather application using React and an external API to fetch data.",
                    image: "images/weather.jpg",
                    link: "https://github.com/umer494/weather-app",
                    tech: ["React", "API", "CSS"]
                }
            ];

            // Function to render Projects
            const renderProjects = () => {
                const projectsContainer = document.getElementById('projects-container');
                projects.forEach(project => {
                    const projectCard = document.createElement('div');
                    projectCard.classList.add('project-card');
                    projectCard.innerHTML = `
                        <img src="${project.image}" alt="${project.title}">
                        <h3>${project.title}</h3>
                        <p>${project.description}</p>
                        <a href="${project.link}" target="_blank">View on GitHub</a>
                        <div class="tech-stack">
                            ${project.tech.map(tech => `<span class="tech">${tech}</span>`).join('')}
                        </div>
                    `;
                    projectsContainer.appendChild(projectCard);
                });
            };

            // Handle Hamburger Menu
            const hamburger = document.getElementById('hamburger');
            const navLinks = document.querySelector('.nav-links');
            hamburger.addEventListener('click', () => {
                navLinks.classList.toggle('active');
            });

            // Render Projects
            renderProjects();
        });
    </script>
</body>
</html>
