<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Portfolio of Umer Farooq Bhat, a Full Stack Software Developer specializing in modern web solutions.">
    <meta name="keywords" content="Full Stack Developer, ASP.NET MVC, Angular, React, SQL Server">
    <meta name="author" content="Umer Farooq Bhat">
    <meta property="og:title" content="Portfolio - Umer Farooq Bhat">
    <meta property="og:description" content="Portfolio of Umer Farooq Bhat, a Full Stack Software Developer specializing in modern web solutions.">
    <meta property="og:image" content="Images/portfolio-preview.jpg">
    <meta property="og:url" content="https://umerbhatportfolio.com">
    <meta name="twitter:card" content="summary_large_image">
    <title>Portfolio - Umer Farooq Bhat</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        /* General Reset */
        body {
            margin: 0;
            font-family: 'Poppins', sans-serif;
            background: #0F172A;
            color: #E2E8F0;
        }
        a {
            text-decoration: none;
            color: inherit;
        }
        ul {
            list-style: none;
            padding: 0;
        }

        /* Navbar */
        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 40px;
            background: #1E293B;
            position: sticky;
            top: 0;
            z-index: 1000;
        }
        .navbar .logo {
            font-size: 1.8rem;
            font-weight: 700;
            color: #38BDF8;
        }
        .navbar .nav-links {
            display: flex;
            gap: 20px;
        }
        .navbar .nav-links a {
            color: #E2E8F0;
            font-weight: 500;
            transition: color 0.3s;
        }
        .navbar .nav-links a:hover, .navbar .nav-links a:focus {
            color: #38BDF8;
            text-decoration: underline;
        }

        /* Hero Section */
        .hero {
            text-align: center;
            padding: 100px 20px;
            background: linear-gradient(135deg, #1E293B, #0F172A);
            position: relative;
        }
        .hero h1 {
            font-size: 3.5rem;
            color: #38BDF8;
        }
        .hero p {
            font-size: 1.5rem;
            margin: 20px 0;
            color: #94A3B8;
        }
        .btn-primary {
            padding: 12px 25px;
            background: #38BDF8;
            color: #0F172A;
            border: none;
            border-radius: 5px;
            font-weight: 500;
            font-size: 1.1rem;
            transition: background 0.3s, color 0.3s, border 0.3s;
        }
        .btn-primary:hover {
            background: #0F172A;
            color: #38BDF8;
            border: 2px solid #38BDF8;
        }

        /* Section Headings */
        section h2 {
            font-size: 2.5rem;
            margin-bottom: 20px;
            text-align: center;
            color: #38BDF8;
        }

        /* About Section */
        .about {
            padding: 60px 40px;
        }
        .about p {
            text-align: center;
            max-width: 800px;
            margin: 0 auto;
            font-size: 1.2rem;
            line-height: 1.6;
        }

        /* Skills Section */
        .skills {
            padding: 60px 40px;
            background: #1E293B;
        }
        .skills ul {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 15px;
        }
        .skills ul li {
            background: #0F172A;
            padding: 15px 25px;
            border-radius: 8px;
            font-weight: 500;
            font-size: 1.1rem;
            transition: transform 0.3s, box-shadow 0.3s;
        }
        .skills ul li:hover {
            transform: scale(1.05);
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
        }

        /* Gallery Section */
        .gallery {
            padding: 60px 40px;
        }
        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }
        .gallery img {
            width: 100%;
            border-radius: 10px;
            transition: transform 0.3s, box-shadow 0.3s;
        }
        .gallery img:hover {
            transform: scale(1.05);
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
        }
        .gallery .caption {
            text-align: center;
            color: #94A3B8;
            margin-top: 5px;
        }

        /* Contact Section */
        .contact {
            padding: 60px 40px;
            background: #1E293B;
            text-align: center;
        }
        .contact a {
            color: #38BDF8;
            font-weight: 500;
            font-size: 1.1rem;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 20px;
            background: #0F172A;
            color: #94A3B8;
        }
        footer a {
            color: #38BDF8;
            transition: color 0.3s;
        }
        footer a:hover {
            color: #E2E8F0;
        }
    </style>
</head>
<body>
    <!-- Header Section -->
    <header>
        <nav class="navbar">
            <h1 class="logo">Umer Farooq Bhat</h1>
            <ul class="nav-links">
                <li><a href="#about">About</a></li>
                <li><a href="#skills">Skills</a></li>
                <li><a href="#gallery">Gallery</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <h1>I'm a Full Stack Software Developer</h1>
        <p>Crafting dynamic, responsive, and user-focused web solutions.</p>
        <a href="#projects" class="btn-primary">Previous Projects</a>
    </section>

    <!-- About Section -->
    <section id="about" class="about">
        <h2>About Me</h2>
        <p>I am a passionate software developer with over 3 years of experience in building modern web applications, focusing on creating user-friendly and scalable solutions using technologies like C#, MVC.NET, Angular, and SQL Server.</p>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="skills">
        <h2>Technical Skills</h2>
        <ul>
            <li>Web Development: C#, ASP.NET MVC, Angular</li>
            <li>Database: SQL Server, SSIS</li>
            <li>Frontend: React, JavaScript</li>
            <li>Programming: Python</li>
        </ul>
    </section>

    <!-- Gallery Section -->
    <section id="gallery" class="gallery">
        <h2>Gallery</h2>
        <div class="gallery-grid">
            <div>
                <img src="Images/event1.jpg" alt="Event 1">
                <div class="caption">CSR Event</div>
            </div>
            <div>
                <img src="Images/event2.jpg" alt="Event 2">
                <div class="caption">Team Building Activity</div>
            </div>
            <div>
                <img src="Images/event3.jpg" alt="Event 3">
                <div class="caption">Codeathon Participation</div>
            </div>
            <div>
                <img src="Images/event4.jpg" alt="Event 4">
                <div class="caption">Corporate Marathon</div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact">
        <h2>Contact Me</h2>
        <p>Email: <a href="mailto:umerbhat283@gmail.com">umerbhat283@gmail.com</a></p>
        <p>GitHub: <a href="https://github.com/umer494">github.com/umer494</a></p>
        <p>LinkedIn: <a href="https://linkedin.com/in/umer494">linkedin.com/in/umer494</a></p>
        <p><a href="#">Contact Form</a></p>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2024 Umer Farooq Bhat | <a href="#">Privacy Policy</a></p>
        <p><a href="#">Back to Top</a></p>
    </footer>
</body>
</html>
