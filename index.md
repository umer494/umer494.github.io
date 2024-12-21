<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Portfolio of Umer Farooq Bhat, Full Stack Developer">
    <meta name="keywords" content="Full Stack Developer, ASP.NET MVC, Angular, React, SQL Server">
    <meta name="author" content="Umer Farooq Bhat">
    <meta property="og:title" content="Portfolio - Umer Farooq Bhat">
    <meta property="og:description" content="Portfolio of Umer Farooq Bhat, Full Stack Developer">
    <meta property="og:image" content="Images/portfolio-preview.jpg">
    <meta property="og:url" content="https://umerbhatportfolio.com">
    <meta name="twitter:card" content="summary_large_image">
    <title>Portfolio - Umer Farooq Bhat</title>
    
    <!-- External Fonts and Icons -->
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    
    <style>
        /* Global Styles */
        body {
            margin: 0;
            font-family: 'Poppins', sans-serif;
            background-color: #1E293B;
            color: #E2E8F0;
            padding: 0;
        }
        a {
            text-decoration: none;
            color: inherit;
        }
        h1, h2, h3, p {
            margin: 0;
            padding: 0;
        }
        .container {
            width: 100%;
            max-width: 1200px;
            margin: auto;
            padding: 0 20px;
        }
        
        /* Navbar */
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 20px;
            background: #0F172A;
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            z-index: 100;
        }
        nav .logo {
            font-size: 1.8rem;
            font-weight: bold;
            color: #38BDF8;
        }
        nav .nav-links {
            display: flex;
            gap: 20px;
        }
        nav .nav-links a {
            color: #E2E8F0;
            font-weight: 500;
            transition: color 0.3s;
        }
        nav .nav-links a:hover {
            color: #38BDF8;
        }

        /* Hero Section */
        .hero {
            text-align: center;
            padding: 150px 0;
            background: linear-gradient(135deg, #1E293B, #0F172A);
            color: #E2E8F0;
        }
        .hero h1 {
            font-size: 4rem;
            color: #38BDF8;
            margin-bottom: 20px;
        }
        .hero p {
            font-size: 1.5rem;
            margin-bottom: 30px;
        }
        .btn-primary {
            padding: 15px 25px;
            background: #38BDF8;
            color: #0F172A;
            border: none;
            border-radius: 5px;
            font-weight: 500;
            font-size: 1.2rem;
            transition: background 0.3s;
        }
        .btn-primary:hover {
            background: #0F172A;
            color: #38BDF8;
        }

        /* About Section */
        #about {
            padding: 60px 0;
            background-color: #1E293B;
            text-align: center;
        }
        #about h2 {
            font-size: 2.5rem;
            color: #38BDF8;
            margin-bottom: 20px;
        }
        #about p {
            max-width: 800px;
            margin: auto;
            font-size: 1.2rem;
            color: #94A3B8;
            line-height: 1.6;
        }

        /* Skills Section */
        #skills {
            padding: 60px 0;
            background-color: #0F172A;
            text-align: center;
        }
        #skills h2 {
            font-size: 2.5rem;
            color: #38BDF8;
            margin-bottom: 20px;
        }
        #skills ul {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            justify-items: center;
        }
        #skills ul li {
            background: #1E293B;
            padding: 20px;
            border-radius: 8px;
            font-size: 1.2rem;
            color: #E2E8F0;
            text-align: center;
            transition: transform 0.3s, box-shadow 0.3s;
        }
        #skills ul li:hover {
            transform: scale(1.05);
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
        }
        #skills ul li i {
            font-size: 2rem;
            margin-bottom: 10px;
            color: #38BDF8;
        }

        /* Gallery Section */
        #gallery {
            padding: 60px 0;
            text-align: center;
        }
        #gallery h2 {
            font-size: 2.5rem;
            color: #38BDF8;
            margin-bottom: 20px;
        }
        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
        }
        .gallery-grid img {
            width: 100%;
            border-radius: 10px;
            transition: transform 0.3s, box-shadow 0.3s;
        }
        .gallery-grid img:hover {
            transform: scale(1.05);
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
        }

        /* Contact Section */
        #contact {
            padding: 60px 0;
            background-color: #1E293B;
            text-align: center;
        }
        #contact h2 {
            font-size: 2.5rem;
            color: #38BDF8;
            margin-bottom: 20px;
        }
        #contact p {
            font-size: 1.2rem;
            color: #94A3B8;
        }
        #contact a {
            color: #38BDF8;
            font-size: 1.2rem;
            transition: color 0.3s;
        }
        #contact a:hover {
            color: #E2E8F0;
        }

        /* Footer */
        footer {
            padding: 20px;
            background: #0F172A;
            text-align: center;
            color: #94A3B8;
        }
        footer a {
            color: #38BDF8;
            transition: color 0.3s;
        }
        footer a:hover {
            color: #E2E8F0;
        }

        /* Responsive Design */
        @media screen and (max-width: 768px) {
            .hero h1 {
                font-size: 3rem;
            }
            .btn-primary {
                font-size: 1rem;
            }
            #skills ul {
                grid-template-columns: 1fr 1fr;
            }
        }
    </style>
</head>
<body>

    <!-- Navbar -->
    <nav>
        <h1 class="logo">Umer Farooq Bhat</h1>
        <ul class="nav-links">
            <li><a href="#about">About</a></li>
            <li><a href="#skills">Skills</a></li>
            <li><a href="#gallery">Gallery</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <!-- Hero Section -->
    <section class="hero">
        <h1>Full Stack Software Developer</h1>
        <p>Building innovative, scalable, and dynamic web applications</p>
        <a href="#projects" class="btn-primary">Previous Projects</a>
    </section>

    <!-- About Section -->
    <section id="about">
        <h2>About Me</h2>
        <p>I am a passionate software developer with 3+ years of experience. I specialize in building full-stack web applications using ASP.NET MVC, Angular, and React. My goal is to create seamless and intuitive digital experiences for users worldwide.</p>
    </section>

    <!-- Skills Section -->
    <section id="skills">
        <h2>Technical Skills</h2>
        <ul>
            <li><i class="fab fa-react"></i> React</li>
            <li><i class="fab fa-angular"></i> Angular</li>
            <li><i class="fab fa-node-js"></i> Node.js</li>
            <li><i class="fas fa-database"></i> SQL Server</li>
            <li><i class="fab fa-html5"></i> HTML5</li>
            <li><i class="fab fa-css3-alt"></i> CSS3</li>
            <li><i class="fab fa-js"></i> JavaScript</li>
            <li><i class="fas fa-cogs"></i> .NET MVC</li>
        </ul>
    </section>

    <!-- Gallery Section -->
    <section id="gallery">
        <h2>Gallery</h2>
        <div class="gallery-grid">
            <div>
                <img src="Images/event1.jpg" alt="Event 1">
            </div>
            <div>
                <img src="Images/event2.jpg" alt="Event 2">
            </div>
            <div>
                <img src="Images/event3.jpg" alt="Event 3">
            </div>
            <div>
                <img src="Images/event4.jpg" alt="Event 4">
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact">
        <h2>Contact Me</h2>
        <p>Email: <a href="mailto:umerbhat283@gmail.com">umerbhat283@gmail.com</a></p>
        <p>GitHub: <a href="https://github.com/umer494" target="_blank">github.com/umer494</a></p>
        <p>LinkedIn: <a href="https://linkedin.com/in/umer494" target="_blank">linkedin.com/in/umer494</a></p>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2024 Umer Farooq Bhat | <a href="#">Privacy Policy</a></p>
        <p><a href="#">Back to Top</a></p>
    </footer>

</body>
</html>
