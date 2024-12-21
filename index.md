<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Umer Farooq Bhat - Portfolio</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;700&display=swap" rel="stylesheet">
    <link rel="icon" href="favicon.ico">
    <script src="https://kit.fontawesome.com/a076d05399.js"></script>
     <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500&family=Open+Sans:wght@300;400;600&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <script src="https://cdnjs.cloudflare.com/ajax/libs/scrollreveal/4.0.0/scrollreveal.min.js"></script>
    <style>
        /* Global styles */
        body {
            font-family: 'Poppins', sans-serif;
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            color: #333;
            background-color: #f7fafc;
            scroll-behavior: smooth;
        }

        h1, h2, h3 {
            margin: 0;
            font-weight: 700;
        }

        header {
            background: #1E293B;
            padding: 40px;
            color: white;
            text-align: center;
        }

        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            max-width: 1200px;
            margin: 0 auto;
        }

        .logo {
            font-size: 2rem;
            font-weight: 700;
        }

        .nav-links {
            display: flex;
            gap: 30px;
            list-style-type: none;
        }

        .nav-links li {
            padding: 10px;
        }

        .nav-links a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
        }

        .nav-links a:hover {
            color: #ff5722;
        }

        .hamburger {
            display: none;
            cursor: pointer;
        }

        .hero {
            background: linear-gradient(145deg, #1E293B, #4A6D7C);
            padding: 100px 20px;
            text-align: center;
            color: white;
            margin-bottom: 50px;
        }

        .hero h1 {
            font-size: 3.5rem;
            font-weight: 900;
        }

        .hero p {
            font-size: 1.5rem;
            margin: 20px 0;
        }

        .profile-container {
            text-align: center;
            margin-top: -50px;
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

        .skills-container, .projects-container, .experience-container {
            display: flex;
            flex-wrap: wrap;
            gap: 30px;
            justify-content: center;
        }

        .skill, .project-card ,.experience-card{
            background: #fff;
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 6px 10px rgba(0, 0, 0, 0.1);
            width: 100%;
            max-width: 250px;
            text-align: center;
            transition: transform 0.3s ease-in-out, box-shadow 0.3s ease;
        }

        .skill:hover, .project-card:hover, .experience-card:hover {
            transform: scale(1.05);
            box-shadow: 0 8px 15px rgba(0, 0, 0, 0.2);
        }

        .skills-container .skill i, .projects-container .project-card img,.experience-container {
            font-size: 40px;
            color: #1E293B;
        }

        .tech-stack span {
            background-color: #E5E7EB;
            padding: 8px 15px;
            margin: 5px;
            border-radius: 25px;
            font-size: 0.9rem;
        }

        /* Skill Bars */
        .progress-container {
            width: 100%;
            height: 20px;
            background-color: #E5E7EB;
            border-radius: 10px;
            margin: 15px 0;
        }

        .progress-bar {
            height: 100%;
            border-radius: 10px;
            text-align: center;
            line-height: 20px;
            color: white;
        }

        /* Contact Section */
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
            transition: background-color 0.3s;
        }

        button:hover {
            background-color: #ff5722;
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
            color: #ff5722;
        }

        .social-icons a {
            text-decoration: none;
        }

        /* Testimonials Section */
        .testimonials {
            background-color: #f7fafc;
            padding: 50px 20px;
            text-align: center;
        }

        .testimonial-card {
            background-color: white;
            padding: 30px;
            border-radius: 15px;
            width: 100%;
            max-width: 350px;
            margin: 0 10px;
            box-shadow: 0 6px 10px rgba(0, 0, 0, 0.1);
            text-align: center;
        }

        .testimonial-card p {
            font-style: italic;
            color: #555;
        }

        .testimonial-card h4 {
            margin-top: 15px;
            font-weight: 600;
            color: #1E293B;
        }

        /* Mobile responsive */
        @media (max-width: 768px) {
            .nav-links {
                display: none;
                flex-direction: column;
                align-items: center;
            }

            .nav-links.active {
                display: flex;
            }

            .hamburger {
                display: block;
            }

            .hero h1 {
                font-size: 2.5rem;
            }

            .skills-container, .projects-container,.experience-container {
                flex-direction: column;
                align-items: center;
            }

            .contact form {
                display: flex;
                flex-direction: column;
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
                <li><a href="#experience">Experience</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
            <div class="hamburger" id="hamburger">
                <i class="fas fa-bars"></i>
            </div>
        </nav>
    </header>

    <section id="hero" class="hero">
        <h1>Welcome to My Portfolio</h1>
        <p>I am Umer Farooq Bhat, a passionate Fullstak .NET Developer</p>
        <a href="Images/Umer_Bhat_Updated-Resume.pdf" download>
            <button>Download CV</button>
        </a>
    </section>

    <section class="profile-container">
        <img src="Images/Photograph.jpeg" alt="Umer Farooq Bhat">
        <h2>Umer Farooq Bhat</h2>
        <p>Experienced .NET Developer & Data Analyst with expertise in MVC, SQL, and data-driven solutions.</p>
    </section>

    <section id="about">
        <h2>About Me</h2>
        <p>A Passionate Full-stack developer with around 3 years of experience in MVC.NET, WebApi, Angular, SQL Server and SSIS.Seeking to leverage technical expertise in software development, database optimization, and regulatory compliance to contribute to dynamic projects.</p>
    </section>

    <section id="skills">
        <h2> Skills</h2>
        <div class="skills-container">
            <div class="skill">
                <i class="fas fa-cogs"></i>
                <h3>.NET Development</h3>
                <div class="progress-container">
                    <div class="progress-bar" style="width: 70%; background-color: #4CAF50;">70%</div>
                </div>
            </div>
            <div class="skill">
                <i class="fas fa-database"></i>
                <h3>SQL Development</h3>
                <div class="progress-container">
                    <div class="progress-bar" style="width: 80%; background-color: #2196F3;">80%</div>
                </div>
            </div>
            
            
                <div class="skill">
                    <i class="fas fa-code"></i>
                    <h4>Web Development</h4>
                    <p>C#, ASP.NET MVC, WebApi, Angular, TypeScript</p>
                    <div class="progress-container">
                    <div class="progress-bar" style="width: 80%; background-color: #2196F3;">80%</div>
                </div>
                </div>
                <div class="skill">
                    <i class="fas fa-database"></i>
                    <h4>Database</h4>
                    <p>SQL Server, SSIS, MySQL</p>
                   <div class="progress-container">
                    <div class="progress-bar" style="width: 80%; background-color: #2196F3;">80%</div>
                </div>
                </div>
                <div class="skill">
                    <i class="fas fa-tools"></i>
                    <h4>Tools & Technologies</h4>
                    <p>Visual Studio, Jenkins, Git, Docker</p>
                    <div class="progress-container">
                    <div class="progress-bar" style="width: 80%; background-color: #2196F3;">80%</div>
                </div>
                </div>
                <div class="skill">
                    <i class="fas fa-laptop-code"></i>
                    <h4>Programming Languages</h4>
                    <p>Python, Node.js, JavaScript</p>
                   <div class="progress-container">
                    <div class="progress-bar" style="width: 80%; background-color: #2196F3;">80%</div>
                </div>
                </div>
            </div>
        </div>

             <div class="skill">
                <i class="fas fa-server"></i>
                <h3>SSIS</h3>
                <div class="progress-container">
                    <div class="progress-container">
                    <div class="progress-bar" style="width: 80%; background-color: #2196F3;">80%</div>
                </div>
                </div>
            </div>
            <div class="skill">
                <i class="fas fa-code"></i>
                <h3>Angular</h3>
                <div class="progress-container">
                <div class="progress-container">
                    <div class="progress-bar" style="width: 80%; background-color: #2196F3;">80%</div>
                </div>
                </div>
            </div>
        </div>
    </section>

    <section id="projects">
        <h2>Projects</h2>
        <div class="projects-container">
            <div class="project-card">
                <h3>FATCOM</h3>
                <p>A regulatory reporting tool used for automating and streamlining the compliance process for financial institutions.</p>
            </div>
            <div class="project-card">
                <h3>MIFID</h3>
                <p>A regulatory reporting tool used for automating and streamlining the compliance process for Europian financial institutions reporting.</p>
            </div>
        </div>
    </section>

    <section id="experience">
        <h2>Experience</h2>
        <div class="experience-container">
            <div class="experience-card">
                <h3>FATCOM</h3>
                <p>Software Engineer
Société Générale Global Solutions Centre Pvt. Ltd. – Bangalore, Karnataka
June 2022 – Present</p>
            </div>
            <div class="experience-card">
                <h3>MIFID</h3>
                <p>Software Analyst
Imarticus Learning Private Limited – Bangalore, Karnataka
Feb 2022 – June 2022</p>
            </div>
        </div>
    </section>

    <section id="contact" class="contact">
        <section id="contact" class="contact">
    <h2>Contact Me</h2>
    <form action="https://formspree.io/f/mlddrjdk" method="POST">
        <input type="text" name="name" placeholder="Your Name" required>
        <input type="email" name="email" placeholder="Your Email" required>
        <input type="number" name="number" placeholder="Your Number" required>
        <textarea name="message" placeholder="Your Message" required></textarea>
        <button type="submit">Send Message</button>
    </form>

</section>

    </section>

 <!-- Contact Section -->


    <!-- Footer Section -->

    <footer>
        <div class="social-icons">
        <a href="mailto:umerbhat283@gmail.com"><i class="fas fa-envelope"></i></a>
            <a href="https://github.com/umerfarooq" target="_blank"><i class="fab fa-github"></i></a>
            <a href="https://www.linkedin.com/in/umerfarooq" target="_blank"><i class="fab fa-linkedin"></i></a>
            <a href="https://twitter.com/umerfarooq" target="_blank"><i class="fab fa-twitter"></i></a>
            <a href="https://www.instagram.com/bhat_umer_farooq" target="_blank"><i class="fab fa-instagram"></i></a>
            <a href="+917889662629"><i class="fas fa-phone"></i></a>
        </div>
        <p>&copy; 2024 Umer Farooq Bhat. All rights reserved.</p>
    </footer>

    <script>
        document.getElementById('hamburger').addEventListener('click', function() {
            document.querySelector('.nav-links').classList.toggle('active');
        });
    </script>

</body>
</html>
