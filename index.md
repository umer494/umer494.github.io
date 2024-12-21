<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Portfolio of Umer Farooq Bhat, showcasing skills, projects, and professional experience as a .NET and SQL developer.">
    <title>Umer Farooq Bhat - Portfolio</title>
    <link rel="stylesheet" href="styles.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
</head>
<body>
    <header>
        <nav>
            <ul class="nav-links">
                <li><a href="#about">About</a></li>
                <li><a href="#skills">Skills</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
        <div class="hero">
            <h1>Hi, I'm Umer Farooq Bhat</h1>
            <p>.NET and SQL Developer | Angular Enthusiast</p>
            <a href="#contact" class="btn">Hire Me</a>
        </div>
    </header>

    <section id="about">
        <h2>About Me</h2>
        <p>I'm a passionate developer with over 2 years of experience in .NET Framework and SQL. I specialize in creating efficient web applications and enjoy exploring front-end technologies like Angular. My goal is to build impactful software solutions.</p>
    </section>

    <section id="skills">
        <h2>Technical Skills</h2>
        <div class="skills-container">
            <div class="skill">
                <h3>.NET Development</h3>
                <div class="progress-bar" data-skill="90">90%</div>
            </div>
            <div class="skill">
                <h3>SQL Development</h3>
                <div class="progress-bar" data-skill="85">85%</div>
            </div>
            <div class="skill">
                <h3>Angular</h3>
                <div class="progress-bar" data-skill="70">70%</div>
            </div>
        </div>
    </section>

    <section id="projects">
        <h2>Projects</h2>
        <div class="projects-container">
            <div class="project-card">
                <h3>FATCOM Regulatory Reporting</h3>
                <p>Automated SQL operations and designed an interactive UI for managing database updates.</p>
                <a href="#" target="_blank">View Project</a>
            </div>
            <div class="project-card">
                <h3>Library Management System</h3>
                <p>Built a cataloging system for managing library acquisitions, accessioning, and e-resource management.</p>
                <a href="#" target="_blank">View Project</a>
            </div>
        </div>
    </section>

    <section id="contact">
        <h2>Contact Me</h2>
        <form id="contact-form">
            <input type="text" name="name" placeholder="Your Name" required>
            <input type="email" name="email" placeholder="Your Email" required>
            <textarea name="message" placeholder="Your Message" required></textarea>
            <button type="submit" class="btn">Send Message</button>
        </form>
    </section>

    <footer>
        <p>© 2024 Umer Farooq Bhat. All Rights Reserved.</p>
        <div class="social-icons">
            <a href="https://github.com/username" target="_blank">GitHub</a>
            <a href="https://linkedin.com/in/username" target="_blank">LinkedIn</a>
        </div>
    </footer>

    <script>
        // Skill bar animation
        const progressBars = document.querySelectorAll('.progress-bar');
        window.addEventListener('scroll', () => {
            progressBars.forEach(bar => {
                const skillValue = bar.getAttribute('data-skill');
                const rect = bar.getBoundingClientRect();
                if (rect.top <= window.innerHeight - 50) {
                    bar.style.width = skillValue + '%';
                }
            });
        });

        // Contact form validation
        const form = document.getElementById('contact-form');
        form.addEventListener('submit', (e) => {
            e.preventDefault();
            alert('Thank you for reaching out! I will get back to you soon.');
            form.reset();
        });
    </script>
</body>
</html>
