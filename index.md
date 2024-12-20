---
layout: default
title: Umer Farooq Bhat - Full Stack Developer
author: Umer Farooq Bhat
---

<header class="hero">
  <div class="hero-content">
    <h1 class="animate__animated animate__fadeIn">Umer Farooq Bhat</h1>
    <p class="animate__animated animate__fadeIn">Full Stack Developer</p>
    <div class="social-links">
      <a href="https://linkedin.com/in/bhat-umer-farooq/" target="_blank">LinkedIn</a> |
      <a href="https://github.com/umer494" target="_blank">GitHub</a> |
      <a href="mailto:umerbhat283@gmail.com">Email</a> |
      <a href="tel:+7889662629">Phone</a>
    </div>
  </div>
</header>

## About Me

<p class="animate__animated animate__fadeIn animate__delay-1s">Full-stack developer with around 3 years of experience in MVC.NET, WebApi, Angular, SQL Server, and SSIS. I seek to leverage my technical expertise in software development, database optimization, and regulatory compliance to contribute to dynamic projects.</p>

## Skills

<div class="skills-container">
  <canvas id="skillsChart" width="400" height="400"></canvas>
  <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
  <script>
    var ctx = document.getElementById('skillsChart').getContext('2d');
    var skillsChart = new Chart(ctx, {
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
      },
      options: {
        responsive: true,
        plugins: {
          legend: {
            position: 'top',
          },
          tooltip: {
            callbacks: {
              label: function(tooltipItem) {
                return tooltipItem.label + ': ' + tooltipItem.raw + '%';
              }
            }
          }
        }
      }
    });
  </script>
</div>

## Work Experience

### Société Générale Global Solutions Centre Pvt. Ltd.

_Software Engineer_ (June 2022 – Present)

- Designed and developed a regulatory reporting application (FATCOM) using C#, .NET, MVC, and SQL Server.
- Optimized SQL databases for performance and ensured data integrity.
- Developed Windows services to automate data processing tasks.
- [FATCOM Project Link](https://github.com/umer494/FATCOM)

### Imarticus Learning Private Limited

_Software Analyst_ (Feb 2022 – June 2022)

- Developed MVC.NET-based web applications.
- Optimized SQL data retrieval and designed responsive UIs with Angular.
- [MIFID II Project Link](https://github.com/umer494/MIFID-II)

## Education

- **B.E. (CSE)** – Visvesvaraya Technological University, Bangalore – 2021
- **Diploma in CSE** – KGP College, Jammu & Kashmir – 2018

## Certifications

- Angular Development Basics
- Data Analytics – WorldQuant University (Ongoing)

## Projects

### FATCOM (Regulatory Reporting Application)

- Automated the compliance reporting process for financial institutions using .NET and SQL.
- [View Project on GitHub](https://github.com/umer494/FATCOM)

### MIFID II Regulatory Reporting Application

- Developed a platform supporting MIFID II regulatory reporting using MVC.NET and Angular.
- [View Project on GitHub](https://github.com/umer494/MIFID-II)

## Contact

<p>Email: [umerbhat283@gmail.com](mailto:umerbhat283@gmail.com)</p>
<p>LinkedIn: [linkedin.com/in/bhat-umer-farooq](https://linkedin.com/in/bhat-umer-farooq)</p>

<iframe src="https://www.google.com/maps/embed?pb=globalsolutioncenter.societegenerale.in/en/" width="100%" height="400" style="border:0;" allowfullscreen="" loading="lazy"></iframe>

### Interactive Project Gallery

<div class="project-gallery">
  <div class="card">
    <img src="https://via.placeholder.com/400x250" class="card-img-top" alt="FATCOM Project">
    <div class="card-body">
      <h5 class="card-title">FATCOM (Regulatory Reporting Application)</h5>
      <p class="card-text">Automated the compliance reporting process for financial institutions using .NET and SQL.</p>
      <a href="https://github.com/umer494/FATCOM" class="btn btn-primary">View Project</a>
    </div>
  </div>

  <div class="card">
    <img src="https://via.placeholder.com/400x250" class="card-img-top" alt="MIFID II Project">
    <div class="card-body">
      <h5 class="card-title">MIFID II Regulatory Reporting Application</h5>
      <p class="card-text">Developed a platform supporting MIFID II regulatory reporting using MVC.NET and Angular.</p>
      <a href="https://github.com/umer494/MIFID-II" class="btn btn-primary">View Project</a>
    </div>
  </div>
</div>

<script>
  document.querySelectorAll('.project-gallery .card').forEach(card => {
    card.addEventListener('mouseenter', function() {
      card.style.transform = "scale(1.05)";
      card.style.transition = "transform 0.3s ease";
    });
    card.addEventListener('mouseleave', function() {
      card.style.transform = "scale(1)";
    });
  });
</script>

<style>
.hero {
  background: url('https://via.placeholder.com/1920x800') no-repeat center center fixed;
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

.card {
  border: none;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s ease;
}

.card:hover {
  transform: scale(1.05);
}

.project-gallery {
  display: flex;
  justify-content: space-around;
  margin-top: 40px;
}

.project-gallery .card {
  width: 45%;
  margin: 20px;
}

@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}

@media screen and (max-width: 768px) {
  .hero {
    padding: 50px 20px;
  }
  .hero h1 {
    font-size: 2rem;
  }
  .project-gallery {
    flex-direction: column;
    align-items: center;
  }
  .project-gallery .card {
    width: 90%;
    margin: 10px 0;
  }
}
</style>
