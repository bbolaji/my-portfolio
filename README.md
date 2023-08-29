# my-portfolio
code for building my portfolio using html, css and javascript

HTML 
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Your Portfolio</title>
  <link rel="stylesheet" href="styles.css">
</head>
<div class="image-container">
<img src="IMG_20221028_231901_925.jpg" alt="Bolaji babalola">
</div>
<h1>Welcome to My Portfolio</h1>
  <header>
    <h1>Bolaji babalola</h1>
    <p>Data Analyst </p>
  </header>
  <main>
  <div class="about-me">
        <h2>About Me</h2>
        <p>A seasoned professional with over eight (8) year experience as a consumer insight analyst, BI developer, and data analyst, Iexcel in data extraction, cleanup, mining, modeling, and visualization. I specialize in  building business models and automating reporting through complex SQL queries. In a very competitive industry (financial, telecommunication or the oil and gas sector) myattention to detail, experience, insights gives any team am part of, that edge needed to stand out, for growth and profitability</p>
    </div>
    <section id="skills">
      <h2>Skills</h2>
      <ul>
	    <li>customer support</li>
		<li>sql</li>
        <li>HTML</li>
        <li>CSS</li>
        <li>JavaScript</li>
		<li>excel</li>
		<li>Office365</li>
      </ul>
    </section>
	<section>
	<section id = "Certificates">
	<h1> Certificates</h1>
	<ul>
	<li> [CERTIFICATIONS]
<P> IBM project
manager (July,2023)</P>
<P> Google data Analytics
professional (in view)
(March 2022)</P>
<P>HIIT Online training -
python programming
Certification
(Distinction)(Nov
29,2021)</P>
<P>Introduction to data
engineering
(Coursera Feb 2022)</P>
<P>SQL for Data Science
(University of
California Davis)
March 2022 </P>
<P>Business metrics for
data driven
companies(Duke
University USA)
Jan 2021 </P>
<P>Business Analyticsfor
Decision Making
(Jan 27,2021)</P>
<P> Database Oracle
Foundation by learn
quest
(Jan 29,2022)</P>
<P>Business Intelligence
Data Analyst (BIDA)</P>
</ul>
</section>
    <section id="Projects">
      <h2>Projects</h2>
      <ul>
        <li>PROJECT SIRIUS: FIRST BANK</li>
 <p>I led a team of four (4) other developers in developing 42 scripts,validated, tested, moved it to production with the aim of automating the banks reporting.
reporting, </p>
        <li>HISTORICAL DATA MIGRATION (PROJECT); FIRST BANK</li>
<p>Help the bank migrate some of its report from the legacy system from OBIEE to BES</p>
        <li>TABLEAU AS OUR BI SOLUTION: 9PSB </li>
 <p>Been a start-up there was no BI solution in place to help extract data and
 generate insight to enable management make informed decisions</p>
<p>I designed the business requirement document needed to execute this and
worked with the vendors who built our solution in actualizing this</p>
      </ul>
    </section>
  </main>
  <script src="scripts.js"></script>
</body>
</html>



.CSS
/* Reset some default styles */
  image-container {
    width: 50px; /* Adjust this width to your desired size */
    height: auto; /* Automatically adjust height to maintain aspect ratio */
    overflow: hidden; /* Crop any overflow outside the container */
  }
  
  .image-container img {
    width: 10%; /* Make the image fill the container width */
    height: auto; /* Maintain aspect ratio */
  }
/* Reset some default styles */
body, h1, h2, p, ul, li {
  margin: 0;
  padding: 0;
}

body {
  font-family: Arial, sans-serif;
}

header {
  text-align: center;
  background-color: #333;
  color: white;
  padding: 20px;
}

main {
  max-width: 800px;
  margin: 0 auto;
  padding: 20px;
}

h1 {
  font-size: 2.5rem;
}

h2 {
  font-size: 1.5rem;
  margin-bottom: 10px;
}

ul {
  list-style-type: disc;
  margin-left: 20px;
}

li {
  margin-bottom: 5px;
}



                  JAVASCRIPT 
                  // Add a click event to skills to toggle visibility
const skillsSection = document.getElementById('skills');
skillsSection.addEventListener('click', () => {
  const skillsList = skillsSection.querySelector('ul');
  skillsList.classList.toggle('hidden');
});

// Similar click event for achievements
const achievementsSection = document.getElementById('achievements');
achievementsSection.addEventListener('click', () => {
  const achievementsList = achievementsSection.querySelector('ul');
  achievementsList.classList.toggle('hidden');
});

