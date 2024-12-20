---
layout: default
title: Umer Farooq Bhat - Full Stack Developer
author: Umer Farooq Bhat
---

<header class="hero">
  <h1>Umer Farooq Bhat</h1>
  <p>Full Stack Developer</p>
  <div class="social-links">
    <a href="https://linkedin.com/in/bhat-umer-farooq/">LinkedIn</a> |
    <a href="https://github.com/umer494">GitHub</a> |
    <a href="mailto:umerbhat283@gmail.com">Email</a> |
    <a href="tel:+7889662629">Phone</a>
  </div>
</header>

## About Me

Full-stack developer with around 3 years of experience in MVC.NET, WebApi, Angular, SQL Server, and SSIS. Seeking to leverage technical expertise in software development, database optimization, and regulatory compliance to contribute to dynamic projects.

## Skills

- **Languages & Technologies**:
  <i class="fa fa-cogs"></i> C#, Angular, .NET Framework, WebApi, Typescript, ASP.NET MVC, Entity Framework, Python, Jquery
- **Frameworks & Libraries**:
  <i class="fa fa-cogs"></i> .NET Framework, MVC, EntityFramework, Node.js
- **Database & SQL**:
  <i class="fa fa-database"></i> SQL Server, MySQL, SSIS
- **Tools & Platforms**:
  <i class="fa fa-tools"></i> Visual Studio, Git, Jenkins, SonarQube, IIS, Postman

## Work Experience

### Société Générale Global Solutions Centre Pvt. Ltd.

_Software Engineer_ (June 2022 – Present)

- Designed and developed a regulatory reporting application (FATCOM) using C#, .NET, MVC, and SQL Server.
- Optimized SQL databases for performance and ensured data integrity.
- Developed Windows services to automate data processing tasks.

### Imarticus Learning Private Limited

_Software Analyst_ (Feb 2022 – June 2022)

- Developed MVC.NET-based web applications.
- Optimized SQL data retrieval and designed responsive UIs with Angular.

## Education

- **B.E. (CSE)** – Visvesvaraya Technological University, Bangalore – 2021
- **Diploma in CSE** – KGP College, Jammu & Kashmir – 2018

## Certifications

- Angular Development Basics
- Data Analytics – WorldQuant University (Ongoing)

## Projects

### FATCOM (Regulatory Reporting Application)

- Automated the compliance reporting process for financial institutions using .NET and SQL.

### MIFID II Regulatory Reporting Application

- Developed a platform supporting MIFID II regulatory reporting using MVC.NET and Angular.

## Contact

<p>Email: [umerbhat283@gmail.com](mailto:umerbhat283@gmail.com)</p>
<p>LinkedIn: [linkedin.com/in/bhat-umer-farooq](https://linkedin.com/in/bhat-umer-farooq)</p>

<iframe src="https://www.google.com/maps/embed?pb=..." width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy"></iframe>

### Skills Visualization

<canvas id="skillsChart" width="400" height="400"></canvas>

<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
<script>
  var ctx = document.getElementById('skillsChart').getContext('2d');
  var myChart = new Chart(ctx, {
    type: 'pie',
    data: {
      labels: ['C#', 'Angular', '.NET Framework', 'SQL Server', 'SSIS'],
      datasets: [{
        label: 'Skills Proficiency',
        data: [90, 85, 80, 75, 70],
        backgroundColor: ['#ff5733', '#33c4ff', '#33ff8d', '#ff33c4', '#c4ff33'],
        borderColor: ['#ff5733', '#33c4ff', '#33ff8d', '#ff33c4', '#c4ff33'],
        borderWidth: 1
      }]
    }
  });
</script>

## Interactive Project Gallery

<div class="card-group">
  <div class="card">
    <img src="project-image1.jpg" class="card-img-top" alt="Project 1">
    <div class="card-body">
      <h5 class="card-title">FATCOM (Regulatory Reporting Application)</h5>
      <p class="card-text">Automated the compliance reporting process for financial institutions using .NET and SQL.</p>
    </div>
  </div>
  <div class="card">
    <img src="project-image2.jpg" class="card-img-top" alt="Project 2">
    <div class="card-body">
      <h5 class="card-title">MIFID II Regulatory Reporting Application</h5>
      <p class="card-text">Developed a platform supporting MIFID II regulatory reporting using MVC.NET and Angular.</p>
    </div>
  </div>
</div>

<script>
  document.querySelector('a').addEventListener('click', function (e) {
    e.preventDefault();
    document.querySelector(this.getAttribute('href')).scrollIntoView({ behavior: 'smooth' });
  });
</script>

<style>
.hero {
  background: url('images/Photograph.jpeg') no-repeat center center fixed;
  background-size: cover;
  text-align: center;
  color: white;
  padding: 100px 20px;
}

.hero h1 {
  font-size: 3rem;
  animation: fadeIn 2s ease-in-out;
}

.hero p {
  font-size: 1.5rem;
  animation: fadeIn 3s ease-in-out;
}

.hero .social-links {
  margin-top: 20px;
  font-size: 1.2rem;
}

@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}

.card-group .card {
  margin: 10px;
}

@media screen and (max-width: 768px) {
  .hero {
    padding: 50px 20px;
  }
  .hero h1 {
    font-size: 2rem;
  }
}
</style>
