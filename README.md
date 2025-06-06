<!DOCTYPE html>
<html lang="en" >
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <meta name="description" content="Kapil Rohilla - QA Engineer Portfolio showcasing Selenium, Postman, Java, Python skills and real-time projects." />
  <meta name="author" content="Kapil Rohilla" />
  <title>Kapil Rohilla - QA Engineer Portfolio</title>
  <link rel="icon" href="https://avatars.githubusercontent.com/u/86894088?v=4" type="image/png" sizes="32x32" />

  <!-- Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap" rel="stylesheet" />
  <!-- AOS Animation -->
  <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet" />

  <style>
    /* CSS Custom Properties for light and dark themes */
    :root {
      --bg-color: #ffffff;
      --text-color: #4b5563;
      --heading-color: #111827;
      --body-color: #6b7280;
      --card-bg: #ffffff;
      --card-shadow: rgba(0,0,0,0.05);
      --link-color: #2563eb;
      --link-hover: #1d4ed8;
      --scrollbar-bg: #f9fafb;
      --scrollbar-thumb: #2563eb;
      --btn-bg: #2563eb;
      --btn-hover-bg: #1d4ed8;
      --progress-bar-bg: #3b82f6;
      --social-icon-filter: grayscale(40%);
      --social-icon-hover-filter: none;
    }
    @media (prefers-color-scheme: dark) {
      :root {
        --bg-color: #121212;
        --text-color: #d1d5db;
        --heading-color: #e5e7eb;
        --body-color: #9ca3af;
        --card-bg: #1f2937;
        --card-shadow: rgba(255,255,255,0.05);
        --link-color: #60a5fa;
        --link-hover: #3b82f6;
        --scrollbar-bg: #1f2937;
        --scrollbar-thumb: #60a5fa;
        --btn-bg: #2563eb;
        --btn-hover-bg: #1e40af;
        --progress-bar-bg: #2563eb;
        --social-icon-filter: grayscale(100%);
        --social-icon-hover-filter: none;
      }
    }
    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background-color: var(--bg-color);
      color: var(--text-color);
      line-height: 1.6;
      font-size: 17px;
      -webkit-font-smoothing: antialiased;
      -moz-osx-font-smoothing: grayscale;
      transition: background-color 0.4s ease, color 0.4s ease;
    }
    a {
      color: var(--link-color);
      text-decoration: none;
      transition: color 0.3s ease;
      font-weight: 600;
    }
    a:hover, a:focus {
      color: var(--link-hover);
      outline: none;
    }
    h1, h3, h2, h4 {
      color: var(--heading-color);
      margin-top: 0;
      font-weight: 700;
    }
    h1 {
      font-size: 3.5rem;
      font-weight: 800;
    }
    h3 {
      font-size: 1.5rem;
      font-weight: 600;
    }
    h2 {
      font-size: 1.8rem;
      font-weight: 700;
      margin-bottom: 1rem;
    }
    p, li {
      color: var(--body-color);
    }
    .container {
      max-width: 1200px;
      margin: 0 auto;
      padding-left: 1rem;
      padding-right: 1rem;
      padding-top: 6rem;
      padding-bottom: 6rem;
    }
    .center-text {
      text-align: center;
    }
    .typing-svg img {
      margin: 1.5rem auto 3rem;
      display: block;
      max-width: 435px;
      width: 100%;
    }
    .profile-views {
      margin-bottom: 3rem;
    }
    section {
      margin-bottom: 5rem;
    }
    .card {
      background-color: var(--card-bg);
      border-radius: 12px;
      padding: 2rem;
      box-shadow: 0 8px 24px var(--card-shadow);
      transition: box-shadow 0.3s ease, background-color 0.4s ease;
    }
    .card:hover, .card:focus-within {
      box-shadow: 0 12px 40px var(--card-shadow);
    }
    .icons {
      display: flex;
      flex-wrap: wrap;
      gap: 1.25rem;
      justify-content: flex-start;
      align-items: center;
    }
    .icons a {
      display: inline-flex;
      align-items: center;
      justify-content: center;
    }
    .icons img {
      width: 42px;
      height: 42px;
      transition: transform 0.3s ease, filter 0.4s ease;
      filter: var(--social-icon-filter);
    }
    .icons img:hover {
      transform: scale(1.15);
      filter: var(--social-icon-hover-filter);
    }
    .projects-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit,minmax(280px,1fr));
      gap: 2rem;
    }
    .project-img-placeholder {
      width: 100%;
      height: 160px;
      object-fit: cover;
      border-radius: 12px;
      background: linear-gradient(135deg, #60a5fa 0%, #2563eb 100%);
      display: flex;
      align-items: center;
      justify-content: center;
      color: #e0e7ff;
      font-weight: 700;
      font-size: 1.2rem;
      user-select: none;
      transition: background 0.4s ease;
    }
    /* Adjust placeholders in dark */
    @media (prefers-color-scheme: dark) {
      .project-img-placeholder {
        color: #BFDBFE;
      }
      .project-img-placeholder:nth-child(odd) {
        background: linear-gradient(135deg, #34d399, #059669);
      }
      .project-img-placeholder:nth-child(even) {
        background: linear-gradient(135deg, #fbbf24, #ca8a04);
        color: #000;
      }
    }
    .github-stats {
      display: flex;
      flex-direction: column;
      gap: 1.5rem;
      margin-top: 2rem;
    }
    .github-stats img {
      max-width: 100%;
      border-radius: 12px;
      box-shadow: 0 8px 24px var(--card-shadow);
      transition: box-shadow 0.3s ease, filter 0.4s ease;
      filter: var(--social-icon-filter);
    }
    .github-stats img:hover {
      box-shadow: 0 12px 40px var(--card-shadow);
      filter: var(--social-icon-hover-filter);
    }
    .social-icons {
      display: flex;
      gap: 1.5rem;
      justify-content: center;
      margin-bottom: 3rem;
    }
    .social-icons a img {
      filter: var(--social-icon-filter);
      transition: filter 0.3s ease, transform 0.3s ease;
      width: 40px;
      height: 40px;
    }
    .social-icons a:hover img {
      filter: var(--social-icon-hover-filter);
      transform: scale(1.1);
    }
    ul.achievements, ul.certifications {
      padding-left: 1.2rem;
      color: var(--body-color);
    }
    ul.achievements li, ul.certifications li {
      margin-bottom: 0.75rem;
    }
    /* Resume Button */
    .resume-btn {
      display: inline-block;
      background-color: var(--btn-bg);
      color: white;
      font-weight: 600;
      font-size: 1rem;
      padding: 0.75rem 1.75rem;
      border-radius: 0.75rem;
      transition: background-color 0.3s ease, box-shadow 0.3s ease;
      text-decoration: none;
      margin: 1rem auto 3rem;
      cursor: pointer;
      user-select: none;
      box-shadow: 0 4px 14px rgba(37, 99, 235, 0.4);
      text-align: center;
      max-width: 240px;
      display: block;
    }
    .resume-btn:hover, .resume-btn:focus {
      background-color: var(--btn-hover-bg);
      box-shadow: 0 6px 20px rgba(29, 78, 216, 0.5);
      outline: none;
    }
    /* Scroll to top button */
    #scrollToTopBtn {
      position: fixed;
      bottom: 30px;
      right: 30px;
      background-color: var(--btn-bg);
      color: white;
      border: none;
      border-radius: 50%;
      padding: 12px 16px;
      font-size: 20px;
      cursor: pointer;
      box-shadow: 0 4px 8px rgba(0,0,0,0.2);
      z-index: 999;
      display: none;
      transition: background-color 0.3s ease;
    }
    #scrollToTopBtn:hover {
      background-color: var(--btn-hover-bg);
    }
    /* Scroll progress bar */
    #progressBar {
      position: fixed;
      top: 0;
      left: 0;
      height: 5px;
      background-color: var(--progress-bar-bg);
      width: 0%;
      z-index: 999;
      transition: background-color 0.3s ease;
    }
    /* Footer */
    footer {
      text-align: center;
      color: var(--body-color);
      font-size: 0.9rem;
      margin-top: 3rem;
    }
    /* Scrollbar Styles */
    ::-webkit-scrollbar {
      width: 8px;
      background: var(--scrollbar-bg);
    }
    ::-webkit-scrollbar-thumb {
      background: var(--scrollbar-thumb);
      border-radius: 20px;
    }
    ::-webkit-scrollbar-thumb:hover {
      background: var(--btn-hover-bg);
    }
    /* Dark Mode Toggle Styles */
    header#topnav {
      position: fixed;
      top: 0;
      left: 0;
      right: 0;
      backdrop-filter: saturate(180%) blur(10px);
      background-color: var(--card-bg);
      box-shadow: 0 1px 4px var(--card-shadow);
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 0 1.5rem;
      height: 60px;
      z-index: 1000;
      transition: background-color 0.4s ease, box-shadow 0.3s ease;
    }
    header#topnav h1 {
      margin: 0;
      font-size: 1.7rem;
      font-weight: 800;
      color: var(--heading-color);
      user-select: none;
    }
    /* Toggle container replaced with label + input for accessibility */
    .toggle-switch {
      display: inline-flex;
      align-items: center;
      cursor: pointer;
      position: relative;
      width: 52px;
      height: 28px;
      background: #e4e7eb;
      border-radius: 9999px;
      transition: background-color 0.3s ease;
      padding: 4px;
      user-select: none;
    }
    /* Dark mode active state */
    .toggle-switch.dark {
      background: var(--btn-bg);
    }
    /* Hide the default checkbox */
    .toggle-switch input[type="checkbox"] {
      position: absolute;
      opacity: 0;
      width: 0;
      height: 0;
      margin: 0;
      padding: 0;
    }
    .slider {
      position: relative;
      width: 20px;
      height: 20px;
      background: white;
      border-radius: 50%;
      transition: transform 0.3s cubic-bezier(0.4, 0, 0.2, 1);
      box-shadow: 0 1px 4px rgba(0,0,0,0.3);
      will-change: transform;
      z-index: 2;
    }
    /* If checked, shift the slider */
    .toggle-switch input[type="checkbox"]:checked + .slider {
      transform: translateX(24px);
    }
    /* Sun & Moon icons */
    .sun-icon, .moon-icon {
      position: absolute;
      width: 14px;
      height: 14px;
      fill: var(--card-bg);
      pointer-events: none;
      user-select: none;
      top: 7px;
      z-index: 1;
    }
    .sun-icon {
      left: 6px;
    }
    .moon-icon {
      right: 6px;
    }
    /* Responsive */
    @media (max-width: 640px) {
      h1 {
        font-size: 2.7rem;
      }
      h3 {
        font-size: 1.25rem;
      }
      .card {
        padding: 1.5rem;
      }
    }
  </style>
</head>
<body>

  <!-- Scroll progress bar -->
  <div id="progressBar"></div>

  <!-- Top Navigation with Dark Mode Toggle -->
  <header id="topnav" role="banner">
    <h1 tabindex="0">Kapil Rohilla</h1>
    <label for="darkModeToggle" class="toggle-switch" id="toggleSwitch" role="switch" aria-checked="false" aria-label="Toggle Dark Mode" tabindex="0" aria-live="polite">
      <input type="checkbox" id="darkModeToggle" />
      <span class="slider"></span>
      <!-- Sun Icon -->
      <svg class="sun-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" aria-hidden="true" focusable="false">
        <path d="M12 4.5a1 1 0 1 1 0-2 1 1 0 0 1 0 2zM18.364 5.636a1 1 0 1 1 1.415-1.415 1 1 0 0 1-1.415 1.415zM19.5 12a1 1 0 1 1 2 0 1 1 0 0 1-2 0zM18.364 18.364a1 1 0 1 1 1.415 1.415 1 1 0 0 1-1.415-1.415zM12 19.5a1 1 0 1 1 0 2 1 1 0 0 1 0-2zM5.636 18.364a1 1 0 1 1-1.415 1.415 1 1 0 0 1 1.415-1.415zM4.5 12a1 1 0 1 1-2 0 1 1 0 0 1 2 0zM5.636 5.636a1 1 0 1 1-1.415-1.415 1 1 0 0 1 1.415 1.415zM12 8a4 4 0 1 1 0 8a4 4 0 0 1 0-8z"/>
      </svg>
      <!-- Moon Icon -->
      <svg class="moon-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" aria-hidden="true" focusable="false">
        <path d="M21 12.79A9 9 0 0 1 12.21 3c-.12 0-.24 0-.36.01a7 7 0 0 0-7.84 9.45A7 7 0 1 0 21 12.79z"/>
      </svg>
    </label>
  </header>

  <main class="container" role="main" tabindex="-1">

    <header class="center-text" data-aos="fade-down" style="margin-top: 0;">
      <h1>Hi 👋, I'm Kapil Rohilla</h1>
      <h3>Aspiring QA Engineer | Manual & Automation Testing Enthusiast</h3>

      <div class="typing-svg">
        <img src="https://readme-typing-svg.herokuapp.com?font=Poppins&duration=3000&pause=1000&color=00FF6A&center=true&vCenter=true&width=435&lines=Welcome+to+my+GitHub+Profile!;Aspiring+QA+Engineer+from+India;Selenium+%7C+Postman+%7C+Java+%7C+Python" alt="Typing SVG" />
      </div>

      <div class="profile-views">
        <img src="https://komarev.com/ghpvc/?username=kapilrohilla2001&label=Profile%20views&color=0e75b6&style=flat" alt="kapilrohilla2001 Profile views" />
      </div>

      <div>
        <a href="https://github.com/ryo-ma/github-profile-trophy" target="_blank" rel="noreferrer">
          <img src="https://github-profile-trophy.vercel.app/?username=kapilrohilla2001&theme=gruvbox&margin-w=15&margin-h=15&column=3" alt="GitHub Trophies" />
        </a>
      </div>
    </header>

    <section class="card" data-aos="fade-up">
      <h2>👨‍💻 About Me</h2>
      <ul>
        <li><strong>MCA Graduate</strong> from Chandigarh University</li>
        <li>Passionate about <strong>software testing</strong>, <strong>quality assurance</strong>, and <strong>test automation</strong></li>
        <li>Skilled in <strong>Selenium WebDriver</strong>, <strong>Postman</strong>, <strong>Java</strong>, <strong>Python</strong>, and <strong>Manual Testing</strong></li>
        <li>Currently building <strong>automation frameworks</strong> and improving <strong>API testing</strong> skills</li>
        <li>Aiming to contribute to reliable and user-friendly software systems</li>
      </ul>
    </section>

    <section class="center-text" data-aos="fade-up">
      <h2>📫 Connect with Me</h2>
      <div class="social-icons" role="list">
        <a href="https://www.linkedin.com/in/kapil-rohilla/" target="_blank" rel="noreferrer" role="listitem" aria-label="LinkedIn Profile">
          <img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="LinkedIn" />
        </a>
        <a href="https://github.com/kapilrohilla2001" target="_blank" rel="noreferrer" role="listitem" aria-label="GitHub Profile">
          <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/github/github-original.svg" alt="GitHub" />
        </a>
      </div>
      <a href="https://yourdomain.com/resume/Kapil_Rohilla_Resume.pdf" class="resume-btn" target="_blank" rel="noopener noreferrer" aria-label="Download Kapil Rohilla Resume">
        Download Resume
      </a>
    </section>

    <section class="card" data-aos="fade-right">
      <h2>💻 Languages &amp; Tools</h2>
      <div class="icons">
        <a href="https://www.java.com" target="_blank" rel="noreferrer" title="Java">
          <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original.svg" alt="Java" />
        </a>
        <a href="https://www.python.org" target="_blank" rel="noreferrer" title="Python">
          <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="Python" />
        </a>
        <a href="https://www.selenium.dev" target="_blank" rel="noreferrer" title="Selenium">
          <img src="https://www.vectorlogo.zone/logos/selenium/selenium-icon.svg" alt="Selenium" />
        </a>
        <a href="https://postman.com" target="_blank" rel="noreferrer" title="Postman">
          <img src="https://www.vectorlogo.zone/logos/getpostman/getpostman-icon.svg" alt="Postman" />
        </a>
        <a href="https://www.mysql.com/" target="_blank" rel="noreferrer" title="MySQL">
          <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg" alt="MySQL" />
        </a>
        <a href="https://www.w3.org/html/" target="_blank" rel="noreferrer" title="HTML5">
          <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="HTML5" />
        </a>
        <a href="https://www.w3schools.com/css/" target="_blank" rel="noreferrer" title="CSS3">
          <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="CSS3" />
        </a>
        <a href="https://git-scm.com/" target="_blank" rel="noreferrer" title="Git">
          <img src="https://www.vectorlogo.zone/logos/git-scm/git-scm-icon.svg" alt="Git" />
        </a>
      </div>
    </section>

    <section class="card" data-aos="fade-left">
      <h2>📂 Projects</h2>
      <div class="projects-grid">
        <article>
          <div class="project-img-placeholder" aria-label="Covid19 Tracker project image placeholder">
            COVID-19<br />Tracker
          </div>
          <h3 style="color: var(--heading-color); margin-top:1rem;">Covid19 Cases Tracker</h3>
          <p>
            Implemented a real-time global COVID-19 tracking system using Python and data visualization tools.
          </p>
          <p><strong>Technologies:</strong> Python</p>
          <p>
            <a href="https://github.com/kapilrohilla2001/Covid-19-Cases-Tracker.git" target="_blank" rel="noreferrer">View on GitHub</a>
          </p>
        </article>

        <article>
          <div class="project-img-placeholder" aria-label="Face Recognition Attendance System project image placeholder" style="background: linear-gradient(135deg, #34d399, #059669);">
            Face Recognition<br />Attendance
          </div>
          <h3 style="color: var(--heading-color); margin-top:1rem;">Face Recognition Attendance System</h3>
          <p>
            Developed a real-time face recognition attendance system achieving 95% accuracy with Python and OpenCV.
          </p>
          <p><strong>Technologies:</strong> Python, OpenCV</p>
          <p>
            <a href="https://github.com/kapilrohilla2001/Face-Recognition-Attendance-System" target="_blank" rel="noreferrer">View on GitHub</a>
          </p>
        </article>

        <article>
          <div class="project-img-placeholder" aria-label="Mobile App Testing project image placeholder" style="background: linear-gradient(135deg, #fbbf24, #ca8a04); color: #000;">
            Mobile App Testing
          </div>
          <h3 style="color: var(--heading-color); margin-top:1rem;">Mobile App Testing</h3>
          <p>
            Designed 30+ test cases covering UI validation, form inputs, and error handling for Edu Elementary App.
          </p>
          <p><strong>Technologies:</strong> Manual Testing</p>
        </article>
      </div>
    </section>

    <section class="center-text" data-aos="zoom-in-up">
      <h2>🔥 GitHub Stats</h2>
      <div class="github-stats" role="region" aria-label="GitHub statistics and top languages">
        <img
          src="https://github-readme-stats.vercel.app/api?username=kapilrohilla2001&show_icons=true&theme=tokyonight"
          alt="Kapil's GitHub stats"
        />
        <img
          src="https://github-readme-stats.vercel.app/api/top-langs?username=kapilrohilla2001&show_icons=true&locale=en&layout=compact&theme=tokyonight"
          alt="Top Languages"
        />
        <img src="https://github-readme-streak-stats.herokuapp.com/?user=kapilrohilla2001&theme=tokyonight" alt="Streak Stats" />
      </div>
    </section>

    <section class="card" data-aos="fade-up-right">
      <h2>🏆 Achievements</h2>
      <ul class="achievements">
        <li>
          <strong>TPP Class Representative</strong> at Chandigarh University (Jan 2023 - Nov 2024)<br />
          - Addressed disciplinary concerns and maintained professional communication.
        </li>
        <li>
          <strong>Project Expo</strong> at Chandigarh University (Jan 2025 - Apr 2025)<br />
          - Created a fire-fighting robot that successfully passed all phases of the University Project Expo.
        </li>
      </ul>
    </section>

    <section class="card" data-aos="fade-up-left">
      <h2>📜 Certifications</h2>
      <ul class="certifications">
        <li>
          <strong>Python Programming</strong> - Coursera<br />
          Recognized proficiency in Python 3 programming, applicable in data science, machine learning, and data visualization.
        </li>
        <li>
          <strong>Pytest Test Automation</strong> - Test Automation University<br />
          Gained expertise in writing scalable and efficient automated tests using the Pytest framework.
        </li>
        <li>
          <strong>Software Testing Training</strong> - Internshala<br />
          Completed 6-week training covering Java Basics, Selenium WebDriver, Locators, and Automation Testing.
        </li>
      </ul>
    </section>

    <footer>
      <p>© 2025 Kapil Rohilla. All rights reserved.</p>
    </footer>
  </main>

  <!-- Scroll to Top Button -->
  <button id="scrollToTopBtn" title="Go to top">↑</button>

  <!-- AOS Animation Script -->
  <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
  <script>
    AOS.init();
  </script>

  <!-- Scroll Progress Bar and Top Button Logic -->
  <script>
    const scrollToTopBtn = document.getElementById('scrollToTopBtn');
    const progressBar = document.getElementById('progressBar');

    window.onscroll = function () {
      scrollToTopBtn.style.display =
        document.body.scrollTop > 300 || document.documentElement.scrollTop > 300 ? 'block' : 'none';

      let winScroll = document.body.scrollTop || document.documentElement.scrollTop;
      let height = document.documentElement.scrollHeight - document.documentElement.clientHeight;
      let scrolled = (winScroll / height) * 100;
      progressBar.style.width = scrolled + '%';
    };

    scrollToTopBtn.onclick = () => {
      window.scrollTo({ top: 0, behavior: 'smooth' });
    };
  </script>

  <!-- Dark Mode Toggle Logic -->
  <script>
    (function () {
      const toggleCheckbox = document.getElementById('darkModeToggle');
      const toggleLabel = document.getElementById('toggleSwitch');
      const htmlEl = document.documentElement;
      const themeKey = 'kapil-theme';

      // Apply saved theme from localStorage or system preference on load
      function applyTheme(theme) {
        if (theme === 'dark') {
          htmlEl.classList.add('dark');
          toggleCheckbox.checked = true;
          toggleLabel.setAttribute('aria-checked', 'true');
          document.documentElement.style.colorScheme = 'dark';
          toggleLabel.classList.add('dark');
        } else {
          htmlEl.classList.remove('dark');
          toggleCheckbox.checked = false;
          toggleLabel.setAttribute('aria-checked', 'false');
          document.documentElement.style.colorScheme = 'light';
          toggleLabel.classList.remove('dark');
        }
      }

      function getPreferredTheme() {
        if (localStorage.getItem(themeKey)) {
          return localStorage.getItem(themeKey);
        }
        return window.matchMedia('(prefers-color-scheme: dark)').matches ? 'dark' : 'light';
      }

      applyTheme(getPreferredTheme());

      toggleCheckbox.addEventListener('change', () => {
        if (toggleCheckbox.checked) {
          applyTheme('dark');
          localStorage.setItem(themeKey, 'dark');
        } else {
          applyTheme('light');
          localStorage.setItem(themeKey, 'light');
        }
      });

      // Keyboard accessibility handled by label and checkbox natively
    })();
  </script>
</body>
</html>

