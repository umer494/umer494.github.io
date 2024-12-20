<html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
  
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
        }

        header {
            background-color: #333;
            color: #fff;
            text-align: center;
            padding: 20px 0;
        }

        header h1 {
            margin: 0;
            font-size: 2.5rem;
        }

        header p {
            font-size: 1.2rem;
        }

        section {
            padding: 20px;
        }

        .contact-info {
            list-style-type: none;
            padding: 0;
        }

        .contact-info li {
            font-size: 18px;
            margin-bottom: 10px;
        }

        .skills, .projects, .education, .work-experience {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
            gap: 20px;
        }

        .card {
            background-color: #fff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            transition: all 0.3s ease-in-out;
            cursor: pointer;
            position: relative;
        }

        .card:hover {
            transform: scale(1.05);
            background-color: #f0f0f0;
        }

        .card h4 {
            margin: 0;
            font-size: 1.5rem;
        }

        .card p {
            display: none;
            font-size: 1rem;
            color: #555;
        }

        .card:hover p {
            display: block;
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            color: #333;
            background-color: rgba(255, 255, 255, 0.8);
            padding: 10px;
            border-radius: 4px;
        }

        .map-container {
            text-align: center;
            margin: 20px 0;
        }

        iframe {
            border: 0;
            width: 100%;
            max-width: 800px;
            height: 450px;
        }

        /* Skills Hover Effects */
        .skill-item {
            background-image: linear-gradient(to bottom, #ff7e5f, #feb47b);
            color: white;
            padding: 20px;
            border-radius: 8px;
            text-align: center;
            transition: all 0.3s ease-in-out;
            position: relative;
        }

        .skill-item:hover {
            transform: scale(1.05);
            background-color: #f4a261;
            color: #fff;
        }

        .skill-item:hover .skill-details {
            display: block;
        }

        .skill-details {
            display: none;
            position: absolute;
            bottom: 10px;
            left: 50%;
            transform: translateX(-50%);
            background-color: rgba(0, 0, 0, 0.7);
            color: white;
            padding: 5px;
            border-radius: 4px;
        }

        /* Interactive Grid */
        .interactive-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
        }

        .interactive-grid div {
            position: relative;
            background-color: #ddd;
            padding: 20px;
            border-radius: 10px;
            text-align: center;
            cursor: pointer;
        }

        .interactive-grid div:hover {
            background-color: #ff6f61;
            color: white;
        }

        .interactive-grid div span {
            display: none;
            position: absolute;
            bottom: 10px;
            left: 50%;
            transform: translateX(-50%);
            background-color: rgba(0, 0, 0, 0.7);
            color: white;
            padding: 5px;
            border-radius: 4px;
        }

        .interactive-grid div:hover span {
            display: block;
        }

    </style>

</head>
<body>

<section>
    <h2>About Me</h2>
    <p>Full-stack developer with around 3 years of experience in MVC.NET, WebApi, Angular, SQL Server, and SSIS. Seeking to leverage technical expertise in software development, database optimization, and regulatory compliance to contribute to dynamic projects.</p>

    <h3>Skills</h3>
    <div class="skills">
        <div class="skill-item">
            <h4>C#</h4>
            <div class="skill-details">Used in Backend development, APIs, and Data handling.</div>
        </div>
        <div class="skill-item">
            <h4>Angular</h4>
            <div class="skill-details">Used for building responsive single-page web applications.</div>
        </div>
        <div class="skill-item">
            <h4>.NET Framework</h4>
            <div class="skill-details">Used for web applications, APIs, and system integrations.</div>
        </div>
        <div class="skill-item">
            <h4>SQL Server</h4>
            <div class="skill-details">Used for database design, querying, and optimization.</div>
        </div>
        <div class="skill-item">
            <h4>WebApi</h4>
            <div class="skill-details">Used to create RESTful services and APIs.</div>
        </div>
        <div class="skill-item">
            <h4>SSIS</h4>
            <div class="skill-details">Used for automating data extraction, transformation, and loading (ETL).</div>
        </div>
    </div>

    <h3>Work Experience</h3>
    <div class="interactive-grid">
        <div>
            <h4>Société Générale Global Solutions Centre Pvt. Ltd.</h4>
            <span>Software Engineer (June 2022 – Present)</span>
        </div>
        <div>
            <h4>Imarticus Learning Private Limited</h4>
            <span>Software Analyst (Feb 2022 – June 2022)</span>
        </div>
    </div>

    <h3>Education</h3>
    <div class="interactive-grid">
        <div>
            <h4>B.E. (CSE)</h4>
            <span>Visvesvaraya Technological University, Bangalore – 2021</span>
        </div>
        <div>
            <h4>Diploma in CSE</h4>
            <span>KGP College, Jammu & Kashmir – 2018</span>
        </div>
    </div>

    <h3>Certifications</h3>
    <ul>
        <li>Angular Development Basics</li>
        <li>Data Analytics – WorldQuant University (Ongoing)</li>
    </ul>

    <h3>Projects</h3>
    <div class="projects">
        <div class="card">
            <h4>FATCOM (Regulatory Reporting Application)</h4>
            <p>Automated the compliance reporting process for financial institutions using .NET and SQL.</p>
            <a href="https://github.com/umer494/FATCOM" target="_blank">View on GitHub</a>
        </div>
        <div class="card">
            <h4>MIFID II Regulatory Reporting Application</h4>
            <p>Developed a platform supporting MIFID II regulatory reporting using MVC.NET and Angular.</p>
            <a href="https://github.com/umer494/MIFID-II" target="_blank">View on GitHub</a>
        </div>
    </div>

    <h3>Contact</h3>
    <ul class="contact-info">
        <li>Email: <a href="mailto:umerbhat283@gmail.com">umerbhat283@gmail.com</a></li>
        <li>LinkedIn: <a href="https://linkedin.com/in/bhat-umer-farooq" target="_blank">linkedin.com/in/bhat-umer-farooq</a></li>
    </ul>

    <div class="map-container">
        <h3>My Location</h3>
        <!-- Embedded Map with your provided location -->
        <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3887.837006902847!2d77.7376163!3d12.982274799999999!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3bae0df955555555%3A0x44f047ba18cc2e67!2sSociete%20Generale%20Global%20Solution%20Center!5e0!3m2!1sen!2sin!4v1734705681787!5m2!1sen!2sin" width="100%" height="400" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
    </div>

</section>

</body>
</html>
