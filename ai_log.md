# AI log for SITE 1101 individual Project 3
Author: Yusif Musayev
---



## Step 1 - Asking about basic HTML structure for index.html 

**My prompt**
How can I create a basic HTML5 structure for the homepage (index.html) of my portfolio website?

**AI response**
I'll help you create a basic HTML5 structure for your portfolio homepage.
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="My professional portfolio showcasing my projects and skills">
    <title>My Portfolio</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section id="home">
            <h1>Welcome to My Portfolio</h1>
            <p>Your professional introduction goes here</p>
        </section>

        <section id="about">
            <h2>About Me</h2>
            <p>Tell your story and background here</p>
        </section>

        <section id="projects">
            <h2>My Projects</h2>
            <article>
                <h3>Project 1</h3>
                <p>Project description</p>
            </article>
        </section>

        <section id="contact">
            <h2>Contact</h2>
            <p>Your contact information goes here</p>
        </section>
    </main>

    <footer>
        <p>&copy; 2025 My Portfolio. All rights reserved.</p>
    </footer>
</body>
</html>



## Step 2 - Asking about navigation bar and hero section

**My prompt:**
How can I create a navigation bar and hero section for the homepage (index.html) of my portfolio website?

**Ai response:**
I'll help you create a styled navigation bar and hero section for your portfolio homepage.



<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="My professional portfolio showcasing my projects and skills">
    <title>My Portfolio</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header class="navbar">
        <nav class="nav-container">
            <div class="logo">MyPortfolio</div>
            <ul class="nav-menu">
                <li class="nav-item"><a href="#home" class="nav-link">Home</a></li>
                <li class="nav-item"><a href="#about" class="nav-link">About</a></li>
                <li class="nav-item"><a href="#projects" class="nav-link">Projects</a></li>
                <li class="nav-item"><a href="#contact" class="nav-link">Contact</a></li>
            </ul>
            <div class="hamburger">
                <span></span>
                <span></span>
                <span></span>
            </div>
        </nav>
    </header>

    <main>
        <section id="home" class="hero">
            <div class="hero-content">
                <h1>Hi, I'm Your Name</h1>
                <p class="hero-subtitle">Full Stack Developer | Creative Designer | Problem Solver</p>
                <button class="cta-button">View My Work</button>
            </div>
            <div class="hero-image">
                <img src="profile.jpg" alt="Profile Picture">
            </div>
        </section>

        <section id="about">
            <h2>About Me</h2>
            <p>Tell your story and background here</p>
        </section>

        <section id="projects">
            <h2>My Projects</h2>
            <article>
                <h3>Project 1</h3>
                <p>Project description</p>
            </article>
        </section>

        <section id="contact">
            <h2>Contact</h2>
            <p>Your contact information goes here</p>
        </section>
    </main>

    <footer>
        <p>&copy; 2025 My Portfolio. All rights reserved.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>

Now create a styles.css file with styling:

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    line-height: 1.6;
    color: #333;
}

/* Navigation Bar */
.navbar {
    background-color: #fff;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    position: sticky;
    top: 0;
    z-index: 100;
}

.nav-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    max-width: 1200px;
    margin: 0 auto;
    padding: 1rem 2rem;
}

.logo {
    font-size: 1.5rem;
    font-weight: bold;
    color: #007bff;
}

.nav-menu {
    display: flex;
    list-style: none;
    gap: 2rem;
}

.nav-link {
    text-decoration: none;
    color: #333;
    font-weight: 500;
    transition: color 0.3s ease;
}

.nav-link:hover {
    color: #007bff;
}

.hamburger {
    display: none;
    flex-direction: column;
    cursor: pointer;
}

.hamburger span {
    width: 25px;
    height: 3px;
    background-color: #333;
    margin: 5px 0;
    transition: 0.3s;
}

/* Hero Section */
.hero {
    display: flex;
    align-items: center;
    justify-content: space-between;
    max-width: 1200px;
    margin: 0 auto;
    padding: 4rem 2rem;
    gap: 3rem;
    min-height: 600px;
}

.hero-content {
    flex: 1;
}

.hero h1 {
    font-size: 3rem;
    margin-bottom: 1rem;
    color: #222;
}

.hero-subtitle {
    font-size: 1.25rem;
    color: #666;
    margin-bottom: 2rem;
}

.cta-button {
    padding: 0.75rem 2rem;
    font-size: 1rem;
    background-color: #007bff;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    transition: background-color 0.3s ease;
}

.cta-button:hover {
    background-color: #0056b3;
}

.hero-image {
    flex: 1;
    text-align: center;
}

.hero-image img {
    max-width: 100%;
    height: auto;
    border-radius: 10px;
}

/* Responsive Design */
@media (max-width: 768px) {
    .nav-menu {
        display: none;
    }

    .hamburger {
        display: flex;
    }

    .hero {
        flex-direction: column;
        padding: 2rem 1rem;
        min-height: auto;
    }

    .hero h1 {
        font-size: 2rem;
    }

    .hero-subtitle {
        font-size: 1rem;
    }
}


## Step 3 - Asking AI about CSS styling for the homepage 

**My prompt** 
How can I style the navigation bar, hero section, buttons, and layout for my portfolio homepage (index.html) using CSS?

**AI response** 
I'll provide you with comprehensive CSS styling for your portfolio homepage covering the navigation bar, hero section, buttons, and overall layout.

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

:root {
    --primary-color: #007bff;
    --primary-dark: #0056b3;
    --text-color: #333;
    --light-bg: #f8f9fa;
    --white: #fff;
    --shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    line-height: 1.6;
    color: var(--text-color);
    background-color: var(--white);
}

/* ==================== NAVIGATION BAR ==================== */
.navbar {
    background-color: var(--white);
    box-shadow: var(--shadow);
    position: sticky;
    top: 0;
    z-index: 100;
}

.nav-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    max-width: 1200px;
    margin: 0 auto;
    padding: 1rem 2rem;
}

.logo {
    font-size: 1.8rem;
    font-weight: 700;
    color: var(--primary-color);
    text-decoration: none;
    letter-spacing: -0.5px;
}

.logo:hover {
    color: var(--primary-dark);
}

.nav-menu {
    display: flex;
    list-style: none;
    gap: 2.5rem;
}

.nav-item {
    position: relative;
}

.nav-link {
    text-decoration: none;
    color: var(--text-color);
    font-weight: 500;
    font-size: 0.95rem;
    transition: color 0.3s ease;
    padding-bottom: 0.5rem;
}

.nav-link:hover,
.nav-link.active {
    color: var(--primary-color);
    border-bottom: 2px solid var(--primary-color);
}

.hamburger {
    display: none;
    flex-direction: column;
    cursor: pointer;
    gap: 6px;
}

.hamburger span {
    width: 25px;
    height: 3px;
    background-color: var(--text-color);
    transition: all 0.3s ease;
    border-radius: 2px;
}

/* ==================== HERO SECTION ==================== */
.hero {
    display: flex;
    align-items: center;
    justify-content: space-between;
    max-width: 1200px;
    margin: 0 auto;
    padding: 5rem 2rem;
    gap: 4rem;
    min-height: 600px;
}

.hero-content {
    flex: 1;
    animation: fadeInLeft 0.8s ease-in;
}

.hero h1 {
    font-size: 3.5rem;
    font-weight: 700;
    margin-bottom: 1rem;
    color: var(--text-color);
    line-height: 1.2;
}

.hero h1 span {
    color: var(--primary-color);
}

.hero-subtitle {
    font-size: 1.25rem;
    color: #666;
    margin-bottom: 2rem;
    font-weight: 400;
}

.cta-button {
    padding: 0.875rem 2.5rem;
    font-size: 1rem;
    background-color: var(--primary-color);
    color: var(--white);
    border: none;
    border-radius: 5px;
    cursor: pointer;
    font-weight: 600;
    transition: all 0.3s ease;
    box-shadow: 0 4px 15px rgba(0, 123, 255, 0.3);
    margin-right: 1rem;
    margin-bottom: 2rem;
    display: inline-block;
}

.cta-button:hover {
    background-color: var(--primary-dark);
    transform: translateY(-2px);
    box-shadow: 0 6px 20px rgba(0, 123, 255, 0.4);
}

.cta-button.secondary {
    background-color: transparent;
    color: var(--primary-color);
    border: 2px solid var(--primary-color);
    box-shadow: none;
}

.cta-button.secondary:hover {
    background-color: var(--primary-color);
    color: var(--white);
}

.hero-image {
    flex: 1;
    text-align: center;
    animation: fadeInRight 0.8s ease-in;
}

.hero-image img {
    max-width: 100%;
    height: auto;
    border-radius: 10px;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
    transition: transform 0.3s ease;
}

.hero-image img:hover {
    transform: scale(1.05);
}

.social-links {
    display: flex;
    gap: 1.5rem;
    margin-top: 2rem;
}

.social-links a {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    width: 45px;
    height: 45px;
    border-radius: 50%;
    background-color: var(--light-bg);
    color: var(--primary-color);
    text-decoration: none;
    font-size: 1.2rem;
    transition: all 0.3s ease;
}

.social-links a:hover {
    background-color: var(--primary-color);
    color: var(--white);
    transform: translateY(-3px);
}

/* ==================== GENERAL LAYOUT ==================== */
main section {
    max-width: 1200px;
    margin: 0 auto;
    padding: 4rem 2rem;
}

main section h2 {
    font-size: 2.5rem;
    margin-bottom: 1.5rem;
    color: var(--text-color);
}

footer {
    background-color: var(--light-bg);
    text-align: center;
    padding: 2rem;
    margin-top: 3rem;
    border-top: 1px solid #ddd;
}

footer p {
    margin: 0.5rem 0;
    color: #666;
}

footer a {
    color: var(--primary-color);
    text-decoration: none;
}

footer a:hover {
    text-decoration: underline;
}

/* ==================== ANIMATIONS ==================== */
@keyframes fadeInLeft {
    from {
        opacity: 0;
        transform: translateX(-30px);
    }
    to {
        opacity: 1;
        transform: translateX(0);
    }
}

@keyframes fadeInRight {
    from {
        opacity: 0;
        transform: translateX(30px);
    }
    to {
        opacity: 1;
        transform: translateX(0);
    }
}

/* ==================== RESPONSIVE DESIGN ==================== */
@media (max-width: 768px) {
    .nav-menu {
        display: none;
    }

    .hamburger {
        display: flex;
    }

    .hero {
        flex-direction: column;
        padding: 2rem 1rem;
        min-height: auto;
        gap: 2rem;
    }

    .hero h1 {
        font-size: 2.2rem;
    }

    .hero-subtitle {
        font-size: 1rem;
    }

    .cta-button {
        padding: 0.75rem 1.5rem;
        font-size: 0.9rem;
        margin-right: 0.5rem;
        margin-bottom: 1rem;
    }

    main section {
        padding: 2rem 1rem;
    }

    main section h2 {
        font-size: 1.8rem;
    }
}

@media (max-width: 480px) {
    .nav-container {
        padding: 1rem;
    }

    .logo {
        font-size: 1.5rem;
    }

    .hero h1 {
        font-size: 1.8rem;
    }

    .hero-subtitle {
        font-size: 0.9rem;
    }

    .cta-button {
        display: block;
        width: 100%;
        margin-bottom: 1rem;
        text-align: center;
    }
}


## Step 4 - HTML multi-page structure

**My prompt** 
How can I extend my website to have multiple pages such as about.html, projects.html, and extra.html while keeping the same navigation bar and footer across all pages?


**AI response** 
I'll help you create a multi-page portfolio website with consistent navigation and footer across all pages.

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="About Yusif Musayev - Computer Science Student">
    <title>About | Yusif Musayev Portfolio</title>
    <link rel="stylesheet" href="css/style.css">
</head>
<body>
    <!-- NAVBAR -->
    <header class="navbar">
        <div class="nav-container">
            <a href="index.html" class="logo">Yusif<span>.</span></a>
            <nav id="nav-menu" class="nav-menu">
                <a href="index.html" class="nav-link">Home</a>
                <a href="about.html" class="nav-link active">About</a>
                <a href="projects.html" class="nav-link">Projects</a>
                <a href="extra.html" class="nav-link">More</a>
            </nav>
            <button class="hamburger" id="burger-btn">
                <span></span><span></span><span></span>
            </button>
        </div>
    </header>

    <main>
        <section class="about-section container">
            <h1>About Me</h1>
            <div class="about-content">
                <div class="about-text">
                    <h2>Who I Am</h2>
                    <p>I'm a first-year Computer Science student at ADA University with a passion for technology and software development.</p>
                    <p>My journey in tech started with curiosity about how things work. I love solving problems through code and creating solutions that make a difference.</p>
                </div>
                <div class="about-text">
                    <h2>Skills & Expertise</h2>
                    <ul class="skills-list">
                        <li>HTML5 & CSS3</li>
                        <li>JavaScript</li>
                        <li>Web Development</li>
                        <li>Problem Solving</li>
                        <li>Version Control (Git)</li>
                    </ul>
                </div>
            </div>
        </section>
    </main>

    <!-- FOOTER -->
    <footer class="footer">
        <div class="container footer-content">
            <p>&copy; 2025 Yusif Musayev. All rights reserved.</p>
            <p>Website repository: 
                <a href="https://github.com/USERNAME/site-portfolio" target="_blank">GitHub Repo</a>
            </p>
        </div>
    </footer>

    <script src="js/main.js"></script>
</body>
</html>

create projects.html:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="My Projects - Yusif Musayev Portfolio">
    <title>Projects | Yusif Musayev Portfolio</title>
    <link rel="stylesheet" href="css/style.css">
</head>
<body>
    <!-- NAVBAR -->
    <header class="navbar">
        <div class="nav-container">
            <a href="index.html" class="logo">Yusif<span>.</span></a>
            <nav id="nav-menu" class="nav-menu">
                <a href="index.html" class="nav-link">Home</a>
                <a href="about.html" class="nav-link">About</a>
                <a href="projects.html" class="nav-link active">Projects</a>
                <a href="extra.html" class="nav-link">More</a>
            </nav>
            <button class="hamburger" id="burger-btn">
                <span></span><span></span><span></span>
            </button>
        </div>
    </header>

    <main>
        <section class="projects-section container">
            <h1>My Projects</h1>
            <div class="projects-grid">
                <article class="project-card">
                    <div class="project-image">
                        <img src="assets/project1.jpg" alt="Project 1">
                    </div>
                    <div class="project-content">
                        <h3>Project Title 1</h3>
                        <p>Description of your first project. Include technologies used and what you learned.</p>
                        <div class="project-tags">
                            <span class="tag">HTML</span>
                            <span class="tag">CSS</span>
                            <span class="tag">JavaScript</span>
                        </div>
                        <a href="#" class="project-link">View Project →</a>
                    </div>
                </article>

                <article class="project-card">
                    <div class="project-image">
                        <img src="assets/project2.jpg" alt="Project 2">
                    </div>
                    <div class="project-content">
                        <h3>Project Title 2</h3>
                        <p>Description of your second project. Highlight key features and your role.</p>
                        <div class="project-tags">
                            <span class="tag">Python</span>
                            <span class="tag">Database</span>
                        </div>
                        <a href="#" class="project-link">View Project →</a>
                    </div>
                </article>

                <article class="project-card">
                    <div class="project-image">
                        <img src="assets/project3.jpg" alt="Project 3">
                    </div>
                    <div class="project-content">
                        <h3>Project Title 3</h3>
                        <p>Description of your third project. Explain the problem it solves.</p>
                        <div class="project-tags">
                            <span class="tag">JavaScript</span>
                            <span class="tag">API</span>
                        </div>
                        <a href="#" class="project-link">View Project →</a>
                    </div>
                </article>
            </div>
        </section>
    </main>

    <!-- FOOTER -->
    <footer class="footer">
        <div class="container footer-content">
            <p>&copy; 2025 Yusif Musayev. All rights reserved.</p>
            <p>Website repository: 
                <a href="https://github.com/USERNAME/site-portfolio" target="_blank">GitHub Repo</a>
            </p>
        </div>
    </footer>

    <script src="js/main.js"></script>
</body>
</html>

Create extra.html:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="More About Me - Yusif Musayev Portfolio">
    <title>More | Yusif Musayev Portfolio</title>
    <link rel="stylesheet" href="css/style.css">
</head>
<body>
    <!-- NAVBAR -->
    <header class="navbar">
        <div class="nav-container">
            <a href="index.html" class="logo">Yusif<span>.</span></a>
            <nav id="nav-menu" class="nav-menu">
                <a href="index.html" class="nav-link">Home</a>
                <a href="about.html" class="nav-link">About</a>
                <a href="projects.html" class="nav-link">Projects</a>
                <a href="extra.html" class="nav-link active">More</a>
            </nav>
            <button class="hamburger" id="burger-btn">
                <span></span><span></span><span></span>
            </button>
        </div>
    </header>

    <main>
        <section class="extra-section container">
            <h1>More About Me</h1>
            
            <div class="extra-content">
                <div class="card">
                    <h2>Education</h2>
                    <p><strong>ADA University</strong></p>
                    <p>Computer Science (First Year)</p>
                    <p>Currently pursuing knowledge in software development and computer science fundamentals.</p>
                </div>

                <div class="card">
                    <h2>Interests</h2>
                    <ul>
                        <li>Web Development</li>
                        <li>Problem Solving</li>
                        <li>Open Source Contribution</li>
                        <li>Continuous Learning</li>
                    </ul>
                </div>

                <div class="card">
                    <h2>Get In Touch</h2>
                    <p>I'm always interested in hearing about new opportunities and projects.</p>
                    <a href="mailto:your.email@example.com" class="btn primary">Send Me an Email</a>
                </div>
            </div>
        </section>
    </main>

    <!-- FOOTER -->
    <footer class="footer">
        <div class="container footer-content">
            <p>&copy; 2025 Yusif Musayev. All rights reserved.</p>
            <p>Website repository: 
                <a href="https://github.com/USERNAME/site-portfolio" target="_blank">GitHub Repo</a>
            </p>
        </div>
    </footer>

    <script src="js/main.js"></script>
</body>
</html>

Now add CSS for the new page sections to your style.css:
// ...existing code...

/* ==================== ABOUT PAGE ==================== */
.about-section {
    padding: 4rem 2rem;
}

.about-section h1 {
    font-size: 2.5rem;
    margin-bottom: 2rem;
    text-align: center;
}

.about-content {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 3rem;
    max-width: 1000px;
    margin: 0 auto;
}

.about-text h2 {
    font-size: 1.8rem;
    margin-bottom: 1rem;
    color: var(--primary-color);
}

.about-text p {
    margin-bottom: 1rem;
    line-height: 1.8;
    color: #555;
}

.skills-list {
    list-style: none;
    padding: 0;
}

.skills-list li {
    padding: 0.5rem 0;
    padding-left: 1.5rem;
    position: relative;
}

.skills-list li:before {
    content: "✓";
    position: absolute;
    left: 0;
    color: var(--primary-color);
    font-weight: bold;
}

/* ==================== PROJECTS PAGE ==================== */
.projects-section {
    padding: 4rem 2rem;
}

.projects-section h1 {
    font-size: 2.5rem;
    margin-bottom: 3rem;
    text-align: center;
}

.projects-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 2rem;
    max-width: 1200px;
    margin: 0 auto;
}

.project-card {
    background: white;
    border-radius: 10px;
    overflow: hidden;
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.project-card:hover {
    transform: translateY(-10px);
    box-shadow: 0 8px 25px rgba(0, 0, 0, 0.15);
}

.project-image {
    width: 100%;
    height: 200px;
    overflow: hidden;
}

.project-image img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: transform 0.3s ease;
}

.project-card:hover .project-image img {
    transform: scale(1.1);
}

.project-content {
    padding: 1.5rem;
}

.project-content h3 {
    font-size: 1.3rem;
    margin-bottom: 0.5rem;
    color: var(--text-color);
}

.project-content p {
    color: #666;
    margin-bottom: 1rem;
    font-size: 0.95rem;
}

.project-tags {
    display: flex;
    gap: 0.5rem;
    flex-wrap: wrap;
    margin-bottom: 1rem;
}

.tag {
    background-color: var(--light-bg);
    color: var(--primary-color);
    padding: 0.25rem 0.75rem;
    border-radius: 20px;
    font-size: 0.8rem;
    font-weight: 500;
}

.project-link {
    color: var(--primary-color);
    text-decoration: none;
    font-weight: 600;
    transition: color 0.3s ease;
}

.project-link:hover {
    color: var(--primary-dark);
}

/* ==================== EXTRA PAGE ==================== */
.extra-section {
    padding: 4rem 2rem;
}

.extra-section h1 {
    font-size: 2.5rem;
    margin-bottom: 3rem;
    text-align: center;
}

.extra-content {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 2rem;
    max-width: 1200px;
    margin: 0 auto;
}

.card {
    background: white;
    padding: 2rem;
    border-radius: 10px;
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s ease;
}

.card:hover {
    transform: translateY(-5px);
}

.card h2 {
    color: var(--primary-color);
    margin-bottom: 1rem;
    font-size: 1.5rem;
}

.card p {
    color: #555;
    margin-bottom: 0.8rem;
    line-height: 1.6;
}

.card ul {
    list-style-position: inside;
    color: #555;
}

.card ul li {
    margin-bottom: 0.5rem;
}

/* ==================== RESPONSIVE MULTI-PAGE ==================== */
@media (max-width: 768px) {
    .about-content {
        grid-template-columns: 1fr;
    }

    .projects-grid {
        grid-template-columns: 1fr;
    }

    .extra-content {
        grid-template-columns: 1fr;
    }

    .projects-section h1,
    .about-section h1,
    .extra-section h1 {
        font-size: 1.8rem;
    }
}

Key features of this multi-page structure:

✅ Consistent Navigation - Same navbar across all pages
✅ Consistent Footer - Same footer on every page
✅ Active Link Highlighting - Current page is highlighted in navbar
✅ Responsive Design - Works on all devices
✅ Semantic HTML - Proper page structure
✅ Shared CSS - Single stylesheet for all pages
✅ Easy Navigation - Links between pages work seamlessly
Replace placeholder content and image paths with your actual information!

## Step 5 - Dark theme CSS

**My prompt** 
I want to create a dark theme for my website that works for all pages. Can you help me write CSS for the layout, navigation bar, text, hero section, and general styling?


**AI response**
I'll help you create a comprehensive dark theme CSS that works across all your portfolio pages.
// ...existing code...

/* ==================== DARK THEME ==================== */
:root {
    --primary-color: #007bff;
    --primary-dark: #0056b3;
    --primary-light: #4da3ff;
    --text-color: #333;
    --text-light: #666;
    --light-bg: #f8f9fa;
    --white: #fff;
    --shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    
    /* Dark theme colors */
    --dark-bg: #1a1a1a;
    --dark-surface: #2d2d2d;
    --dark-text: #e0e0e0;
    --dark-text-secondary: #a0a0a0;
    --dark-border: #404040;
}

body.dark-mode {
    background-color: var(--dark-bg);
    color: var(--dark-text);
}

/* ==================== DARK MODE NAVBAR ==================== */
body.dark-mode .navbar {
    background-color: var(--dark-surface);
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.5);
}

body.dark-mode .logo {
    color: var(--primary-light);
}

body.dark-mode .logo:hover {
    color: var(--primary-color);
}

body.dark-mode .nav-link {
    color: var(--dark-text);
}

body.dark-mode .nav-link:hover,
body.dark-mode .nav-link.active {
    color: var(--primary-light);
    border-bottom-color: var(--primary-light);
}

body.dark-mode .hamburger span {
    background-color: var(--dark-text);
}

/* ==================== DARK MODE HERO SECTION ==================== */
body.dark-mode .hero h1 {
    color: var(--dark-text);
}

body.dark-mode .hero h1 span {
    color: var(--primary-light);
}

body.dark-mode .hero-subtitle {
    color: var(--dark-text-secondary);
}

body.dark-mode .cta-button {
    background-color: var(--primary-light);
    color: var(--dark-bg);
    box-shadow: 0 4px 15px rgba(77, 163, 255, 0.3);
}

body.dark-mode .cta-button:hover {
    background-color: var(--primary-color);
    box-shadow: 0 6px 20px rgba(77, 163, 255, 0.4);
}

body.dark-mode .cta-button.secondary {
    color: var(--primary-light);
    border-color: var(--primary-light);
}

body.dark-mode .cta-button.secondary:hover {
    background-color: var(--primary-light);
    color: var(--dark-bg);
}

body.dark-mode .hero-image img {
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.5);
}

/* ==================== DARK MODE SOCIAL LINKS ==================== */
body.dark-mode .social-links a {
    background-color: var(--dark-border);
    color: var(--primary-light);
}

body.dark-mode .social-links a:hover {
    background-color: var(--primary-light);
    color: var(--dark-bg);
}

/* ==================== DARK MODE GENERAL SECTIONS ==================== */
body.dark-mode main section {
    background-color: transparent;
}

body.dark-mode main section h2 {
    color: var(--dark-text);
}

body.dark-mode main section h1 {
    color: var(--dark-text);
}

/* ==================== DARK MODE ABOUT PAGE ==================== */
body.dark-mode .about-text h2 {
    color: var(--primary-light);
}

body.dark-mode .about-text p {
    color: var(--dark-text-secondary);
}

body.dark-mode .skills-list li {
    color: var(--dark-text-secondary);
}

body.dark-mode .skills-list li:before {
    color: var(--primary-light);
}

/* ==================== DARK MODE PROJECTS PAGE ==================== */
body.dark-mode .project-card {
    background-color: var(--dark-surface);
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.3);
}

body.dark-mode .project-card:hover {
    box-shadow: 0 8px 25px rgba(77, 163, 255, 0.2);
}

body.dark-mode .project-content h3 {
    color: var(--dark-text);
}

body.dark-mode .project-content p {
    color: var(--dark-text-secondary);
}

body.dark-mode .tag {
    background-color: var(--dark-border);
    color: var(--primary-light);
}

body.dark-mode .project-link {
    color: var(--primary-light);
}

body.dark-mode .project-link:hover {
    color: var(--primary-color);
}

/* ==================== DARK MODE EXTRA PAGE ==================== */
body.dark-mode .card {
    background-color: var(--dark-surface);
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.3);
}

body.dark-mode .card h2 {
    color: var(--primary-light);
}

body.dark-mode .card p {
    color: var(--dark-text-secondary);
}

body.dark-mode .card ul {
    color: var(--dark-text-secondary);
}

body.dark-mode .card a {
    background-color: var(--primary-light);
    color: var(--dark-bg);
}

body.dark-mode .card a:hover {
    background-color: var(--primary-color);
}

/* ==================== DARK MODE FOOTER ==================== */
body.dark-mode .footer {
    background-color: var(--dark-surface);
    border-top-color: var(--dark-border);
}

body.dark-mode footer p {
    color: var(--dark-text-secondary);
}

body.dark-mode footer a {
    color: var(--primary-light);
}

body.dark-mode footer a:hover {
    color: var(--primary-color);
}

/* ==================== THEME TOGGLE BUTTON ==================== */
.theme-toggle {
    position: fixed;
    bottom: 2rem;
    right: 2rem;
    width: 60px;
    height: 60px;
    border-radius: 50%;
    background-color: var(--primary-color);
    color: white;
    border: none;
    cursor: pointer;
    font-size: 1.5rem;
    display: flex;
    align-items: center;
    justify-content: center;
    transition: all 0.3s ease;
    box-shadow: 0 4px 15px rgba(0, 123, 255, 0.3);
    z-index: 999;
}

.theme-toggle:hover {
    background-color: var(--primary-dark);
    transform: scale(1.1);
    box-shadow: 0 6px 20px rgba(0, 123, 255, 0.4);
}

body.dark-mode .theme-toggle {
    background-color: var(--primary-light);
    box-shadow: 0 4px 15px rgba(77, 163, 255, 0.3);
}

body.dark-mode .theme-toggle:hover {
    background-color: var(--primary-color);
    box-shadow: 0 6px 20px rgba(77, 163, 255, 0.4);
}

/* ==================== DARK MODE ANIMATIONS ==================== */
body {
    transition: background-color 0.3s ease, color 0.3s ease;
}

body.dark-mode * {
    transition: background-color 0.3s ease, color 0.3s ease, border-color 0.3s ease;
}

/* ==================== RESPONSIVE DARK MODE ==================== */
@media (max-width: 768px) {
    .theme-toggle {
        width: 50px;
        height: 50px;
        font-size: 1.2rem;
        bottom: 1.5rem;
        right: 1.5rem;
    }
}

@media (max-width: 480px) {
    .theme-toggle {
        width: 45px;
        height: 45px;
        font-size: 1rem;
        bottom: 1rem;
        right: 1rem;
    }
}

/* ==================== PREFERS DARK MODE ==================== */
@media (prefers-color-scheme: dark) {
    body {
        background-color: var(--dark-bg);
        color: var(--dark-text);
    }

    body:not(.light-mode) {
        background-color: var(--dark-bg);
        color: var(--dark-text);
    }
}

Now create a js/theme.js file to handle dark mode toggling:
document.addEventListener('DOMContentLoaded', function() {
    const themeToggle = document.querySelector('.theme-toggle');
    const htmlElement = document.documentElement;
    const body = document.body;

    // Check for saved theme preference or default to light mode
    const currentTheme = localStorage.getItem('theme') || 'light';
    
    // Apply saved theme on page load
    if (currentTheme === 'dark') {
        body.classList.add('dark-mode');
        htmlElement.setAttribute('data-theme', 'dark');
        updateToggleIcon('light');
    } else {
        body.classList.remove('dark-mode');
        htmlElement.setAttribute('data-theme', 'light');
        updateToggleIcon('dark');
    }

    // Theme toggle button click handler
    if (themeToggle) {
        themeToggle.addEventListener('click', function() {
            body.classList.toggle('dark-mode');
            
            const theme = body.classList.contains('dark-mode') ? 'dark' : 'light';
            localStorage.setItem('theme', theme);
            htmlElement.setAttribute('data-theme', theme);
            
            // Update icon
            updateToggleIcon(theme === 'dark' ? 'light' : 'dark');
        });
    }
});

function updateToggleIcon(nextTheme) {
    const themeToggle = document.querySelector('.theme-toggle');
    if (!themeToggle) return;
    
    if (nextTheme === 'dark') {
        themeToggle.innerHTML = '🌙'; // Moon icon for dark mode
        themeToggle.title = 'Switch to Dark Mode';
    } else {
        themeToggle.innerHTML = '☀️'; // Sun icon for light mode
        themeToggle.title = 'Switch to Light Mode';
    }
}


Update your index.html to include the theme toggle button and JavaScript:
// ...existing navbar code...

    </main>

    <!-- THEME TOGGLE BUTTON -->
    <button class="theme-toggle" title="Toggle Dark Mode">☀️</button>

    <!-- FOOTER -->
    <footer class="footer">
        <div class="container footer-content">
            <p>&copy; 2025 Yusif Musayev. All rights reserved.</p>
            <p>Website repository: 
                <a href="https://github.com/USERNAME/site-portfolio" target="_blank">GitHub Repo</a>
            </p>
        </div>
    </footer>

    <script src="js/main.js"></script>
    <script src="js/theme.js"></script>
</body>
</html>

Add the theme toggle button to all pages (about.html, projects.html, extra.html) before the closing </main> tag:
<!-- THEME TOGGLE BUTTON -->
<button class="theme-toggle" title="Toggle Dark Mode">☀️</button>

Key features of this dark theme:

✅ Full Dark Mode Support across all pages
✅ Persistent Theme - Remembers user preference using localStorage
✅ Smooth Transitions between light and dark modes
✅ Accessible Colors - High contrast for readability
✅ System Preference Detection - Respects user's OS dark mode preference
✅ Floating Toggle Button - Easy access from any page
✅ All Elements Styled - Navigation, hero, cards, footer, buttons
✅ Mobile Responsive - Toggle button adapts to screen size
Users can now toggle between light and dark themes, and their preference will be saved!

## Step 6 - JavaScript burger menu

**My prompt**
Can you help me write JavaScript code that makes the navigation menu open and close when the burger button is clicked on mobile screens?

**AI response**
I'll help you create JavaScript code for a responsive hamburger menu that opens and closes on mobile screens.

Create a main.js file:
document.addEventListener('DOMContentLoaded', function() {
    const burgerBtn = document.getElementById('burger-btn');
    const navMenu = document.getElementById('nav-menu');
    const navLinks = document.querySelectorAll('.nav-link');

    // Toggle menu when burger button is clicked
    burgerBtn.addEventListener('click', function() {
        navMenu.classList.toggle('active');
        burgerBtn.classList.toggle('active');
    });

    // Close menu when a nav link is clicked
    navLinks.forEach(link => {
        link.addEventListener('click', function() {
            navMenu.classList.remove('active');
            burgerBtn.classList.remove('active');
        });
    });

    // Close menu when clicking outside of it
    document.addEventListener('click', function(event) {
        const isClickInsideNav = navMenu.contains(event.target);
        const isClickOnBurger = burgerBtn.contains(event.target);

        if (!isClickInsideNav && !isClickOnBurger && navMenu.classList.contains('active')) {
            navMenu.classList.remove('active');
            burgerBtn.classList.remove('active');
        }
    });

    // Close menu on window resize if screen is larger than mobile breakpoint
    window.addEventListener('resize', function() {
        if (window.innerWidth > 768) {
            navMenu.classList.remove('active');
            burgerBtn.classList.remove('active');
        }
    });
});

Now add CSS styles for the mobile menu to your style.css:
// ...existing code...

/* ==================== MOBILE MENU STYLES ==================== */
@media (max-width: 768px) {
    .nav-menu {
        position: fixed;
        left: -100%;
        top: 70px;
        flex-direction: column;
        background-color: var(--white);
        width: 100%;
        text-align: center;
        transition: 0.3s;
        box-shadow: 0 10px 27px rgba(0, 0, 0, 0.05);
        padding: 2rem 0;
        gap: 0;
    }

    .nav-menu.active {
        left: 0;
    }

    .nav-item {
        margin: 1rem 0;
    }

    .nav-link {
        display: block;
        padding: 1rem;
        font-size: 1.1rem;
    }

    .hamburger {
        display: flex !important;
        position: relative;
        z-index: 999;
    }

    .hamburger.active span:nth-child(1) {
        transform: rotate(-45deg) translate(-5px, 6px);
    }

    .hamburger.active span:nth-child(2) {
        opacity: 0;
    }

    .hamburger.active span:nth-child(3) {
        transform: rotate(45deg) translate(-5px, -6px);
    }
}

/* ==================== DARK MODE MOBILE MENU ==================== */
@media (max-width: 768px) {
    body.dark-mode .nav-menu {
        background-color: var(--dark-surface);
        box-shadow: 0 10px 27px rgba(0, 0, 0, 0.3);
    }

    body.dark-mode .nav-link {
        color: var(--dark-text);
        border-bottom: 1px solid var(--dark-border);
    }

    body.dark-mode .nav-link:hover,
    body.dark-mode .nav-link.active {
        background-color: var(--dark-border);
        color: var(--primary-light);
    }
}

/* ==================== SMOOTH TRANSITIONS ==================== */
.hamburger span {
    transition: all 0.3s ease;
}

.nav-menu {
    transition: left 0.3s ease;
}

Update your HTML files to ensure the burger button has the correct ID. Here's the navbar structure for index.html, about.html, projects.html, and extra.html:
<!-- NAVBAR -->
<header class="navbar">
    <div class="nav-container">
        <a href="index.html" class="logo">Yusif<span>.</span></a>
        <nav id="nav-menu" class="nav-menu">
            <a href="index.html" class="nav-link active">Home</a>
            <a href="about.html" class="nav-link">About</a>
            <a href="projects.html" class="nav-link">Projects</a>
            <a href="extra.html" class="nav-link">More</a>
        </nav>
        <button class="hamburger" id="burger-btn">
            <span></span>
            <span></span>
            <span></span>
        </button>
    </div>
</header>

Make sure your index.html includes both JavaScript files at the end before the closing </body> tag:
<!-- ...existing code... -->

    <script src="js/main.js"></script>
    <script src="js/theme.js"></script>
</body>
</html>

<!-- ...existing code... -->

    <script src="js/main.js"></script>
    <script src="js/theme.js"></script>
</body>
</html>

Key features of this hamburger menu:

✅ Click to Toggle - Burger button opens/closes menu
✅ Close on Link Click - Menu closes when you click a navigation link
✅ Close on Outside Click - Menu closes when clicking outside
✅ Auto Close on Resize - Menu closes when window resizes to desktop size
✅ Animated Icon - Burger icon transforms into an X when active
✅ Dark Mode Support - Menu works in both light and dark themes
✅ Smooth Transitions - Animated opening and closing
✅ Mobile Optimized - Full-width menu on mobile devices

## Step 7 - Project 1 description and screenshot structure

**My prompt**
Can you help me write a clear academic description for my Project 1? 
We built NOT, AND, and OR logic gates on a breadboard using transistors, resistors, LEDs, and buttons. 
We also tested all input combinations and took photos for each state. 
Please also show me an example of how to organize these photos in HTML.

**AI response** 
I'll help you write a clear academic description for your logic gates project and show you how to organize the photos in HTML.

First, here's an academic description for your project:

Project 1: Digital Logic Gates Implementation Using Discrete Components

This project demonstrates the fundamental principles of digital logic by constructing NOT, AND, and OR logic gates using discrete electronic components on a breadboard. The implementation utilizes transistors as switching elements, resistors for current limiting and pull-up/pull-down configurations, LEDs as visual output indicators, and push buttons for user input. Each gate was thoroughly tested across all possible input combinations (truth table states), with photographic documentation of each configuration. This hands-on approach provides practical understanding of how digital logic is implemented at the circuit level, forming the foundation for understanding more complex digital systems.

Now, create a detailed project page structure. Update your projects.html:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="My Projects - Yusif Musayev Portfolio">
    <title>Projects | Yusif Musayev Portfolio</title>
    <link rel="stylesheet" href="css/style.css">
</head>
<body>
    <!-- NAVBAR -->
    <header class="navbar">
        <div class="nav-container">
            <a href="index.html" class="logo">Yusif<span>.</span></a>
            <nav id="nav-menu" class="nav-menu">
                <a href="index.html" class="nav-link">Home</a>
                <a href="about.html" class="nav-link">About</a>
                <a href="projects.html" class="nav-link active">Projects</a>
                <a href="extra.html" class="nav-link">More</a>
            </nav>
            <button class="hamburger" id="burger-btn">
                <span></span><span></span><span></span>
            </button>
        </div>
    </header>

    <main>
        <section class="projects-section container">
            <h1>My Projects</h1>
            
            <!-- PROJECT 1: LOGIC GATES -->
            <article class="project-detail">
                <div class="project-header">
                    <h2>Digital Logic Gates Implementation</h2>
                    <div class="project-meta">
                        <span class="project-date">2025</span>
                        <span class="project-category">Electronics</span>
                    </div>
                </div>

                <div class="project-description">
                    <h3>Project Overview</h3>
                    <p>
                        This project demonstrates the fundamental principles of digital logic by constructing NOT, AND, and OR logic gates using discrete electronic components on a breadboard. The implementation utilizes transistors as switching elements, resistors for current limiting and pull-up/pull-down configurations, LEDs as visual output indicators, and push buttons for user input. Each gate was thoroughly tested across all possible input combinations (truth table states), with photographic documentation of each configuration.
                    </p>
                    
                    <h3>Objectives</h3>
                    <ul>
                        <li>Understand the fundamental operation of logic gates</li>
                        <li>Implement digital logic using discrete components</li>
                        <li>Test circuits and verify truth tables experimentally</li>
                        <li>Document findings with photographic evidence</li>
                    </ul>

                    <h3>Components Used</h3>
                    <div class="components-grid">
                        <div class="component-item">
                            <strong>Transistors</strong>
                            <p>Switching elements for logic operations</p>
                        </div>
                        <div class="component-item">
                            <strong>Resistors</strong>
                            <p>Pull-up, pull-down, and current limiting</p>
                        </div>
                        <div class="component-item">
                            <strong>LEDs</strong>
                            <p>Visual output indicators</p>
                        </div>
                        <div class="component-item">
                            <strong>Push Buttons</strong>
                            <p>User input controls</p>
                        </div>
                    </div>

                    <h3>Project Photos</h3>
                    <div class="photos-container">
                        <!-- NOT GATE PHOTOS -->
                        <div class="gate-section">
                            <h4>NOT Gate</h4>
                            <div class="photo-grid">
                                <div class="photo-item">
                                    <img src="assets/logic-gates/not-gate-0.jpg" alt="NOT Gate - Input 0">
                                    <p class="photo-caption">NOT Gate: Input = 0, Output = 1 (LED ON)</p>
                                </div>
                                <div class="photo-item">
                                    <img src="assets/logic-gates/not-gate-1.jpg" alt="NOT Gate - Input 1">
                                    <p class="photo-caption">NOT Gate: Input = 1, Output = 0 (LED OFF)</p>
                                </div>
                            </div>
                        </div>

                        <!-- AND GATE PHOTOS -->
                        <div class="gate-section">
                            <h4>AND Gate</h4>
                            <div class="photo-grid">
                                <div class="photo-item">
                                    <img src="assets/logic-gates/and-gate-00.jpg" alt="AND Gate - 0,0">
                                    <p class="photo-caption">AND Gate: A=0, B=0, Output = 0 (LED OFF)</p>
                                </div>
                                <div class="photo-item">
                                    <img src="assets/logic-gates/and-gate-01.jpg" alt="AND Gate - 0,1">
                                    <p class="photo-caption">AND Gate: A=0, B=1, Output = 0 (LED OFF)</p>
                                </div>
                                <div class="photo-item">
                                    <img src="assets/logic-gates/and-gate-10.jpg" alt="AND Gate - 1,0">
                                    <p class="photo-caption">AND Gate: A=1, B=0, Output = 0 (LED OFF)</p>
                                </div>
                                <div class="photo-item">
                                    <img src="assets/logic-gates/and-gate-11.jpg" alt="AND Gate - 1,1">
                                    <p class="photo-caption">AND Gate: A=1, B=1, Output = 1 (LED ON)</p>
                                </div>
                            </div>
                        </div>

                        <!-- OR GATE PHOTOS -->
                        <div class="gate-section">
                            <h4>OR Gate</h4>
                            <div class="photo-grid">
                                <div class="photo-item">
                                    <img src="assets/logic-gates/or-gate-00.jpg" alt="OR Gate - 0,0">
                                    <p class="photo-caption">OR Gate: A=0, B=0, Output = 0 (LED OFF)</p>
                                </div>
                                <div class="photo-item">
                                    <img src="assets/logic-gates/or-gate-01.jpg" alt="OR Gate - 0,1">
                                    <p class="photo-caption">OR Gate: A=0, B=1, Output = 1 (LED ON)</p>
                                </div>
                                <div class="photo-item">
                                    <img src="assets/logic-gates/or-gate-10.jpg" alt="OR Gate - 1,0">
                                    <p class="photo-caption">OR Gate: A=1, B=0, Output = 1 (LED ON)</p>
                                </div>
                                <div class="photo-item">
                                    <img src="assets/logic-gates/or-gate-11.jpg" alt="OR Gate - 1,1">
                                    <p class="photo-caption">OR Gate: A=1, B=1, Output = 1 (LED ON)</p>
                                </div>
                            </div>
                        </div>
                    </div>

                    <h3>Truth Tables</h3>
                    <div class="truth-tables">
                        <div class="table-container">
                            <h4>NOT Gate Truth Table</h4>
                            <table>
                                <thead>
                                    <tr>
                                        <th>Input A</th>
                                        <th>Output</th>
                                    </tr>
                                </thead>
                                <tbody>
                                    <tr>
                                        <td>0</td>
                                        <td>1</td>
                                    </tr>
                                    <tr>
                                        <td>1</td>
                                        <td>0</td>
                                    </tr>
                                </tbody>
                            </table>
                        </div>

                        <div class="table-container">
                            <h4>AND Gate Truth Table</h4>
                            <table>
                                <thead>
                                    <tr>
                                        <th>Input A</th>
                                        <th>Input B</th>
                                        <th>Output</th>
                                    </tr>
                                </thead>
                                <tbody>
                                    <tr>
                                        <td>0</td>
                                        <td>0</td>
                                        <td>0</td>
                                    </tr>
                                    <tr>
                                        <td>0</td>
                                        <td>1</td>
                                        <td>0</td>
                                    </tr>
                                    <tr>
                                        <td>1</td>
                                        <td>0</td>
                                        <td>0</td>
                                    </tr>
                                    <tr>
                                        <td>1</td>
                                        <td>1</td>
                                        <td>1</td>
                                    </tr>
                                </tbody>
                            </table>
                        </div>

                        <div class="table-container">
                            <h4>OR Gate Truth Table</h4>
                            <table>
                                <thead>
                                    <tr>
                                        <th>Input A</th>
                                        <th>Input B</th>
                                        <th>Output</th>
                                    </tr>
                                </thead>
                                <tbody>
                                    <tr>
                                        <td>0</td>
                                        <td>0</td>
                                        <td>0</td>
                                    </tr>
                                    <tr>
                                        <td>0</td>
                                        <td>1</td>
                                        <td>1</td>
                                    </tr>
                                    <tr>
                                        <td>1</td>
                                        <td>0</td>
                                        <td>1</td>
                                    </tr>
                                    <tr>
                                        <td>1</td>
                                        <td>1</td>
                                        <td>1</td>
                                    </tr>
                                </tbody>
                            </table>
                        </div>
                    </div>

                    <h3>Key Findings</h3>
                    <ul>
                        <li>Successfully implemented all three gate types using discrete components</li>
                        <li>All experimental results matched theoretical truth tables</li>
                        <li>Transistor switching behavior was consistent across all test cases</li>
                        <li>Proper biasing and component selection crucial for reliable operation</li>
                    </ul>

                    <h3>Technologies & Skills</h3>
                    <div class="skills-tags">
                        <span class="skill-tag">Digital Logic</span>
                        <span class="skill-tag">Circuit Design</span>
                        <span class="skill-tag">Breadboarding</span>
                        <span class="skill-tag">Testing & Verification</span>
                        <span class="skill-tag">Electronics</span>
                    </div>
                </div>
            </article>

            <hr class="project-divider">

            <!-- You can add more projects here following the same structure -->

        </section>
    </main>

    <!-- THEME TOGGLE BUTTON -->
    <button class="theme-toggle" title="Toggle Dark Mode">☀️</button>

    <!-- FOOTER -->
    <footer class="footer">
        <div class="container footer-content">
            <p>&copy; 2025 Yusif Musayev. All rights reserved.</p>
            <p>Website repository: 
                <a href="https://github.com/USERNAME/site-portfolio" target="_blank">GitHub Repo</a>
            </p>
        </div>
    </footer>

    <script src="js/main.js"></script>
    <script src="js/theme.js"></script>
</body>
</html>

Now add CSS for the project detail page to your style.css:
// ...existing code...

/* ==================== PROJECT DETAIL PAGE ==================== */
.project-detail {
    background: white;
    padding: 3rem;
    border-radius: 10px;
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
    margin-bottom: 3rem;
}

.project-header {
    margin-bottom: 2rem;
    border-bottom: 2px solid var(--light-bg);
    padding-bottom: 1.5rem;
}

.project-header h2 {
    font-size: 2.2rem;
    color: var(--text-color);
    margin-bottom: 0.5rem;
}

.project-meta {
    display: flex;
    gap: 1rem;
    font-size: 0.9rem;
}

.project-date,
.project-category {
    background-color: var(--light-bg);
    padding: 0.5rem 1rem;
    border-radius: 20px;
    color: var(--primary-color);
    font-weight: 500;
}

.project-description {
    line-height: 1.8;
}

.project-description h3 {
    font-size: 1.5rem;
    color: var(--primary-color);
    margin-top: 2rem;
    margin-bottom: 1rem;
}

.project-description p {
    color: #555;
    margin-bottom: 1rem;
}

.project-description ul {
    margin-left: 1.5rem;
    margin-bottom: 1rem;
    color: #555;
}

.project-description ul li {
    margin-bottom: 0.5rem;
}

/* ==================== COMPONENTS GRID ==================== */
.components-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 1.5rem;
    margin-bottom: 2rem;
}

.component-item {
    background-color: var(--light-bg);
    padding: 1.5rem;
    border-radius: 8px;
    border-left: 4px solid var(--primary-color);
}

.component-item strong {
    color: var(--primary-color);
    font-size: 1.1rem;
    display: block;
    margin-bottom: 0.5rem;
}

.component-item p {
    color: #666;
    font-size: 0.9rem;
}

/* ==================== PHOTOS CONTAINER ==================== */
.photos-container {
    margin: 2rem 0;
}

.gate-section {
    margin-bottom: 3rem;
}

.gate-section h4 {
    font-size: 1.3rem;
    color: var(--primary-color);
    margin-bottom: 1.5rem;
    padding-bottom: 0.5rem;
    border-bottom: 2px solid var(--light-bg);
}

.photo-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 2rem;
}

.photo-item {
    background-color: #f9f9f9;
    border-radius: 8px;
    overflow: hidden;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    border: 1px solid #eee;
}

.photo-item:hover {
    transform: translateY(-5px);
    box-shadow: 0 6px 20px rgba(0, 123, 255, 0.15);
}

.photo-item img {
    width: 100%;
    height: 250px;
    object-fit: cover;
    display: block;
}

.photo-caption {
    padding: 1rem;
    font-size: 0.9rem;
    color: #555;
    text-align: center;
    background-color: white;
}

/* ==================== TRUTH TABLES ==================== */
.truth-tables {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 2rem;
    margin: 2rem 0;
}

.table-container {
    background-color: var(--light-bg);
    padding: 1.5rem;
    border-radius: 8px;
}

.table-container h4 {
    color: var(--primary-color);
    margin-bottom: 1rem;
    font-size: 1.1rem;
}

table {
    width: 100%;
    border-collapse: collapse;
}

table thead {
    background-color: var(--primary-color);
    color: white;
}

table th,
table td {
    padding: 1rem;
    text-align: center;
    border-bottom: 1px solid #ddd;
}

table tbody tr:hover {
    background-color: rgba(0, 123, 255, 0.1);
}

/* ==================== SKILLS TAGS ==================== */
.skills-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.8rem;
    margin-top: 1.5rem;
}

.skill-tag {
    background-color: var(--primary-color);
    color: white;
    padding: 0.5rem 1rem;
    border-radius: 20px;
    font-size: 0.9rem;
    font-weight: 500;
}

/* ==================== PROJECT DIVIDER ==================== */
.project-divider {
    border: none;
    border-top: 2px solid var(--light-bg);
    margin: 3rem 0;
}

/* ==================== DARK MODE PROJECT DETAIL ==================== */
body.dark-mode .project-detail {
    background-color: var(--dark-surface);
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.3);
}

body.dark-mode .project-header {
    border-bottom-color: var(--dark-border);
}

body.dark-mode .project-header h2 {
    color: var(--dark-text);
}

body.dark-mode .project-date,
body.dark-mode .project-category {
    background-color: var(--dark-border);
    color: var(--primary-light);
}

body.dark-mode .project-description h3 {
    color: var(--primary-light);
}

body.dark-mode .project-description p,
body.dark-mode .project-description ul {
    color: var(--dark-text-secondary);
}

body.dark-mode .component-item {
    background-color: var(--dark-border);
    border-left-color: var(--primary-light);
}

body.dark-mode .component-item strong {
    color: var(--primary-light);
}

body.dark-mode .component-item p {
    color: var(--dark-text-secondary);
}

body.dark-mode .gate-section h4 {
    color: var(--primary-light);
    border-bottom-color: var(--dark-border);
}

body.dark-mode .photo-item {
    background-color: var(--dark-border);
    border-color: var(--dark-border);
}

body.dark-mode .photo-caption {
    background-color: var(--dark-surface);
    color: var(--dark-text-secondary);
}

body.dark-mode .table-container {
    background-color: var(--dark-border);
}

body.dark-mode .table-container h4 {
    color: var(--primary-light);
}

body.dark-mode table thead {
    background-color: var(--primary-light);
    color: var(--dark-bg);
}

body.dark-mode table tbody tr:hover {
    background-color: rgba(77, 163, 255, 0.1);
}

body.dark-mode .skill-tag {
    background-color: var(--primary-light);
    color: var(--dark-bg);
}

body.dark-mode .project-divider {
    border-top-color: var(--dark-border);
}

/* ==================== RESPONSIVE PROJECT DETAIL ==================== */
@media (max-width: 768px) {
    .project-detail {
        padding: 1.5rem;
    }

    .project-header h2 {
        font-size: 1.6rem;
    }

    .photo-grid {
        grid-template-columns: 1fr;
    }

    .truth-tables {
        grid-template-columns: 1fr;
    }

    .components-grid {
        grid-template-columns: 1fr;
    }
}
    
    Key features of this structure:

✅ Academic Description - Professional project overview
✅ Organized Photo Gallery - Photos grouped by gate type
✅ Truth Tables - Visual representation of logic
✅ Component Details - Clear component descriptions
✅ Responsive Grid Layout - Works on all devices
✅ Dark Mode Support - Fully styled for both themes
✅ Photo Captions - Descriptive labels for each image
✅ Skills & Tags - Technology highlights
Replace the asset paths with your actual project photos!

