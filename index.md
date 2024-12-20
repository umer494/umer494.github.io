<html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        /* General Reset */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Roboto', sans-serif;
            background: linear-gradient(135deg, #00203F, #004F71);
            color: #fff;
        }

        /* Navigation Bar */
        header {
            position: sticky;
            top: 0;
            background: #00172D;
            padding: 1rem 2rem;
            box-shadow: 0px 2px 5px rgba(0, 0, 0, 0.2);
            z-index: 1000;
        }

        .nav-bar {
            display: flex;
            justify-content: center;
            list-style: none;
        }

        .nav-bar li {
            margin: 0 15px;
        }

        .nav-bar a {
            text-decoration: none;
            color: #fff;
            font-size: 1rem;
            font-weight: 500;
            transition: color 0.3s ease;
        }

        .nav-bar a:hover {
            color: #00C8FF;
        }

        /* Hero Section */
        .hero {
            text-align: center;
            padding: 5rem 2rem;
        }

        .hero img {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            border: 5px solid #00C8FF;
        }

        .hero h1 {
            font-size: 2.5rem;
            margin: 1rem 0;
            color: #00C8FF;
        }

        .hero p {
            font-size: 1rem;
            margin-bottom: 1.5rem;
            color: #A9D8F0;
        }

        .hero .btn {
            padding: 0.8rem 1.5rem;
            background: #00C8FF;
            color: #fff;
            text-decoration: none;
            border-radius: 5px;
            font-weight: 600;
            transition: background 0.3s ease;
        }

        .hero .btn:hover {
            background: #0085B3;
        }

        /* Social Icons */
        .social-icons {
            display: flex;
            justify-content: center;
            margin-top: 2rem;
        }

        .social-icons a {
            margin: 0 10px;
            color: #fff;
            font-size: 1.5rem;
            transition: transform 0.3s ease, color 0.3s ease;
        }

        .social-icons a:hover {
            transform: scale(1.2);
            color: #00C8FF;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 1rem 0;
            background: #00172D;
            color: #A9D8F0;
            margin-top: 2rem;
        }
    </style>
</head>
<body>

    <!-- Navigation -->
    <header>
        <nav>
            <ul class="nav-bar">
                <li><a href="#about">About</a></li>
                <li><a href="#experience">Experience</a></li>
                <li><a href="#skills">Skills</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <img src="your-photo.jpg" alt="Profile Picture">
        <h1>Your Name</h1>
        <p>Frontend Web Developer | Website Designer</p>
        <a href="your-cv-link.pdf" class="btn">Download CV</a>

        <!-- Social Icons -->
        <div class="social-icons">
            <a href="https://github.com" target="_blank"><i class="fab fa-github"></i></a>
            <a href="https://linkedin.com" target="_blank"><i class="fab fa-linkedin"></i></a>
            <a href="https://twitter.com" target="_blank"><i class="fab fa-twitter"></i></a>
            <a href="https://instagram.com" target="_blank"><i class="fab fa-instagram"></i></a>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2024 Your Name. All Rights Reserved.</p>
    </footer>

</body>
</html>
