
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Fhariyazunnisa Abdul - Cybersecurity Portfolio and SOC Analyst Projects">
  <title>Fhariyazunnisa Abdul | Cybersecurity Portfolio</title>

  <style>
    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: #f4f7fb;
      color: #243044;
      line-height: 1.7;
    }

    header {
      background: linear-gradient(135deg, #102b4e, #17619a);
      color: white;
      text-align: center;
      padding: 65px 20px;
    }

    header h1 {
      font-size: 36px;
      margin: 0 0 10px;
    }

    header h2 {
      font-size: 19px;
      font-weight: normal;
      margin: 0 0 18px;
    }

    header p {
      margin: 8px 0;
    }

    .hero-links {
      margin-top: 25px;
    }

    .hero-links a {
      display: inline-block;
      margin: 5px;
      padding: 10px 18px;
      border: 1px solid white;
      border-radius: 6px;
      color: white;
      text-decoration: none;
      font-weight: bold;
    }

    .hero-links a:hover {
      background: white;
      color: #102b4e;
    }

    main {
      max-width: 1100px;
      margin: 35px auto;
      padding: 0 20px;
    }

    section {
      background: white;
      border-radius: 12px;
      padding: 30px;
      margin-bottom: 25px;
      box-shadow: 0 3px 15px rgba(0,0,0,0.06);
    }

    h2 {
      color: #153c66;
    }

    section h2 {
      border-bottom: 2px solid #dbe6f0;
      padding-bottom: 12px;
      margin-top: 0;
    }

    h3 {
      color: #174c80;
      margin-top: 0;
    }

    .project-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 20px;
    }

    .project-card {
      border: 1px solid #d9e3ef;
      border-radius: 10px;
      padding: 22px;
      background: #fcfdff;
      display: flex;
      flex-direction: column;
    }

    .project-card p {
      margin: 8px 0;
    }

    .project-card ul {
      padding-left: 20px;
    }

    .project-card li {
      margin-bottom: 6px;
    }

    .project-link {
      display: inline-block;
      background: #155a95;
      color: white;
      text-decoration: none;
      padding: 10px 16px;
      border-radius: 6px;
      font-weight: bold;
      margin-top: auto;
      align-self: flex-start;
    }

    .project-link:hover {
      background: #103e69;
    }

    .coming-soon {
      color: #667085;
      font-size: 14px;
      font-weight: bold;
      margin-top: auto;
    }

    .skills-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 18px;
    }

    .skill-box {
      background: #f2f6fb;
      border-radius: 8px;
      padding: 18px;
    }

    .skill-box h3 {
      margin-bottom: 8px;
    }

    .education-item {
      margin-bottom: 20px;
    }

    .contact-links a {
      display: inline-block;
      margin: 6px 12px 6px 0;
      color: #155a95;
      font-weight: bold;
    }

    footer {
      background: #102b4e;
      color: white;
      text-align: center;
      padding: 25px;
    }

    @media (max-width: 600px) {
      header h1 {
        font-size: 28px;
      }

      section {
        padding: 22px;
      }
    }
  </style>
</head>

<body>

<header>
  <h1>Fhariyazunnisa Abdul</h1>
  <h2>Cybersecurity Portfolio | Aspiring SOC Analyst</h2>

  <p>
    M.S. in Management Information Systems
  </p>

  <p>
    Auburn University at Montgomery | May 2026
  </p>

  <div class="hero-links">
    <a href="#projects">View My Projects</a>

    <a href="https://github.com/fhariyaz0802-dev"
       target="_blank" rel="noopener noreferrer">
       GitHub
    </a>

    <a href="https://www.linkedin.com/in/fhariyazunnisa-abdul"
       target="_blank" rel="noopener noreferrer">
       LinkedIn
    </a>
  </div>
</header>

<main>

  <!-- ABOUT ME -->
  <section id="about">
    <h2>About Me</h2>

    <p>
      I am an aspiring SOC Analyst with a Master's degree in
      Management Information Systems from Auburn University
      at Montgomery.
    </p>

    <p>
      My cybersecurity interests include security monitoring,
      threat detection, authentication log analysis, network
      security, and incident investigation.
    </p>

    <p>
      I am building hands-on cybersecurity projects using
      Splunk, Microsoft Sentinel, KQL, Wireshark, and Python
      to strengthen my technical skills and prepare for
      entry-level SOC Analyst opportunities.
    </p>
  </section>

  <!-- CYBERSECURITY PROJECTS -->
  <section id="projects">
    <h2>Cybersecurity Projects</h2>

    <div class="project-grid">

      <!-- PROJECT 1 -->
      <article class="project-card">
        <h3>1. Splunk SOC Brute-Force Detection</h3>

        <p>
          <strong>Tools:</strong>
          Splunk, SPL, Windows Authentication Logs
        </p>

        <p>
          Developed a SOC monitoring project to identify
          suspicious failed login activity using Splunk.
        </p>

        <ul>
          <li>Analyzed failed authentication events.</li>
          <li>Investigated suspicious source IP addresses.</li>
          <li>Created SPL detection queries.</li>
          <li>Developed a monitoring dashboard.</li>
          <li>Documented investigation findings.</li>
        </ul>

        <a class="project-link"
           href="https://github.com/fhariyaz0802-dev/Splunk-SOC-Brute-Force-Detection"
           target="_blank" rel="noopener noreferrer">
           View Project
        </a>
      </article>

      <!-- PROJECT 2 -->
      <article class="project-card">
        <h3>2. Microsoft Sentinel SOC Monitoring &amp; Brute-Force Detection</h3>

        <p>
          <strong>Tools:</strong>
          Microsoft Sentinel, Azure Log Analytics, KQL
        </p>

        <p>
          Investigated simulated Windows authentication
          events to detect repeated failed logins followed
          by a successful login from the same IP address.
        </p>

        <ul>
          <li>Configured a Microsoft Sentinel lab.</li>
          <li>Created simulated security events using KQL.</li>
          <li>Detected six failed login attempts.</li>
          <li>Correlated failed and successful logins.</li>
          <li>Prepared a SOC incident investigation report.</li>
        </ul>

        <a class="project-link"
           href="https://github.com/fhariyaz0802-dev/Microsoft-Sentinel-SOC-Detection"
           target="_blank" rel="noopener noreferrer">
           View Project
        </a>
      </article>

      <!-- PROJECT 3 -->
      <article class="project-card">
        <h3>3. Windows Security Monitoring Lab</h3>

        <p>
          <strong>Tools:</strong>
          Windows 11, Sysmon, Windows Event Viewer
        </p>

        <p>
          Windows security monitoring project focused on
          analyzing authentication events, system activity,
          and process creation.
        </p>

        <ul>
          <li>Windows Security Event Logs</li>
          <li>Sysmon Event Analysis</li>
          <li>Process Creation Monitoring</li>
          <li>Authentication Investigation</li>
        </ul>

        <p class="coming-soon">
          Project details coming soon
        </p>
      </article>

      <!-- PROJECT 4 -->
      <article class="project-card">
        <h3>4. Threat Hunting with Wireshark</h3>

        <p>
          <strong>Tools:</strong>
          Wireshark, DNS, Packet Analysis
        </p>

        <p>
          Network traffic analysis project focused on
          identifying suspicious communication patterns
          and investigating DNS activity.
        </p>

        <ul>
          <li>Network Packet Analysis</li>
          <li>DNS Traffic Investigation</li>
          <li>Suspicious Activity Identification</li>
          <li>Threat Hunting Fundamentals</li>
        </ul>

        <p class="coming-soon">
          Project details coming soon
        </p>
      </article>

      <!-- PROJECT 5 -->
      <article class="project-card">
        <h3>5. Phishing Email Analysis</h3>

        <p>
          <strong>Tools:</strong>
          VirusTotal, SPF, DKIM, DMARC
        </p>

        <p>
          Email security investigation project focused on
          phishing indicators, spoofed sender domains,
          suspicious URLs, and email authentication.
        </p>

        <ul>
          <li>Email Header Analysis</li>
          <li>Sender Domain Investigation</li>
          <li>Suspicious URL Analysis</li>
          <li>Phishing Indicator Documentation</li>
        </ul>

        <p class="coming-soon">
          Project details coming soon
        </p>
      </article>

      <!-- PROJECT 6 -->
      <article class="project-card">
        <h3>6. Credit Card Fraud Detection</h3>

        <p>
          <strong>Tools:</strong>
          Python, Pandas, NumPy, Scikit-learn, Tkinter
        </p>

        <p>
          Machine learning project focused on identifying
          potentially fraudulent credit card transactions.
        </p>

        <ul>
          <li>Transaction Data Analysis</li>
          <li>Data Preprocessing</li>
          <li>Random Forest Classification</li>
          <li>Fraud Prediction Interface</li>
        </ul>

        <p class="coming-soon">
          Project details coming soon
        </p>
      </article>

    </div>
  </section>

  <!-- TECHNICAL SKILLS -->
  <section id="skills">
    <h2>Technical Skills</h2>

    <div class="skills-grid">

      <div class="skill-box">
        <h3>SIEM &amp; Monitoring</h3>
        <p>
          Microsoft Sentinel, Splunk, KQL, SPL,
          Authentication Log Analysis
        </p>
      </div>

      <div class="skill-box">
        <h3>Security Operations</h3>
        <p>
          Threat Detection, SOC Monitoring,
          Incident Investigation, Security Event Correlation
        </p>
      </div>

      <div class="skill-box">
        <h3>Network Security</h3>
        <p>
          Wireshark, DNS, Packet Analysis,
          Network Security Fundamentals
        </p>
      </div>

      <div class="skill-box">
        <h3>Endpoint Security</h3>
        <p>
          Windows Event Viewer, Sysmon,
          Windows Authentication Events
        </p>
      </div>

      <div class="skill-box">
        <h3>Cloud Security</h3>
        <p>
          Microsoft Azure, Azure Log Analytics,
          Microsoft Sentinel
        </p>
      </div>

      <div class="skill-box">
        <h3>Programming</h3>
        <p>
          Python, Pandas, NumPy,
          Scikit-learn, GitHub
        </p>
      </div>

    </div>
  </section>

  <!-- EDUCATION -->
  <section id="education">
    <h2>Education</h2>

    <div class="education-item">
      <h3>Auburn University at Montgomery</h3>
      <p>
        Master of Science in Management Information Systems
      </p>
      <p>Graduated: May 2026</p>
    </div>

    <div class="education-item">
      <h3>SRK Institute of Technology</h3>
      <p>
        Bachelor of Technology in Computer Science Engineering
      </p>
      <p>Graduated: April 2023</p>
    </div>
  </section>

  <!-- CONTACT -->
  <section id="contact">
    <h2>Connect With Me</h2>

    <p>
      Explore my cybersecurity projects and professional
      profile through the links below.
    </p>

    <div class="contact-links">
      <a href="https://www.linkedin.com/in/fhariyazunnisa-abdul"
         target="_blank" rel="noopener noreferrer">
         LinkedIn
      </a>

      <a href="https://github.com/fhariyaz0802-dev"
         target="_blank" rel="noopener noreferrer">
         GitHub
      </a>

      <a href="https://github.com/fhariyaz0802-dev/portfolio-site"
         target="_blank" rel="noopener noreferrer">
         Portfolio Repository
      </a>
    </div>
  </section>

</main>

<footer>
  <p>© 2026 Fhariyazunnisa Abdul</p>
  <p>Cybersecurity Portfolio | Aspiring SOC Analyst</p>
</footer>

</body>
</html>











