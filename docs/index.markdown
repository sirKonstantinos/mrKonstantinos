<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Name - Portfolio</title>
    <style>
        /* CSS Variables for consistent theming */
        :root {
            --bg-color: #0f172a;
            --text-main: #f8fafc;
            --text-muted: #94a3b8;
            --accent-color: #38bdf8;
            --card-bg: #1e293b;
            --font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        /* Base Styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: var(--font-family);
            background-color: var(--bg-color);
            color: var(--text-main);
            line-height: 1.6;
        }

        a {
            color: var(--accent-color);
            text-decoration: none;
            transition: color 0.3s ease;
        }

        a:hover {
            color: #7dd3fc;
        }

        /* Navigation */
        nav {
            display: flex;
            justify-content: space-between;
            padding: 1.5rem 5%;
            background-color: rgba(15, 23, 42, 0.9);
            position: fixed;
            width: 100%;
            top: 0;
            backdrop-filter: blur(10px);
            z-index: 1000;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: var(--accent-color);
        }

        .nav-links {
            display: flex;
            gap: 2rem;
            list-style: none;
        }

        /* Sections General */
        section {
            padding: 6rem 5% 4rem;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
        }

        h2 {
            font-size: 2.5rem;
            margin-bottom: 2rem;
            border-bottom: 2px solid var(--accent-color);
            display: inline-block;
            padding-bottom: 0.5rem;
        }

        /* Hero Section */
        #hero {
            align-items: flex-start;
        }

        .greeting {
            color: var(--accent-color);
            font-size: 1.2rem;
            font-weight: 600;
            margin-bottom: 1rem;
            display: block;
        }

        .title {
            font-size: 4rem;
            line-height: 1.1;
            margin-bottom: 1rem;
        }

        .subtitle {
            font-size: 2.5rem;
            color: var(--text-muted);
            margin-bottom: 1.5rem;
        }

        .hero-text {
            max-width: 600px;
            color: var(--text-muted);
            font-size: 1.1rem;
            margin-bottom: 2rem;
        }

        .btn {
            display: inline-block;
            padding: 0.8rem 1.5rem;
            background-color: transparent;
            color: var(--accent-color);
            border: 1px solid var(--accent-color);
            border-radius: 5px;
            font-weight: bold;
            transition: all 0.3s ease;
        }

        .btn:hover {
            background-color: rgba(56, 189, 248, 0.1);
            transform: translateY(-3px);
        }

        /* About Section */
        .about-content {
            display: flex;
            gap: 2rem;
            flex-wrap: wrap;
        }

        .about-text {
            flex: 1;
            min-width: 300px;
            color: var(--text-muted);
            font-size: 1.1rem;
        }

        .about-text p {
            margin-bottom: 1rem;
        }

        /* Skills Section */
        .skills-grid {
            display: flex;
            flex-wrap: wrap;
            gap: 1.5rem;
        }

        .skill-badge {
            background-color: var(--card-bg);
            padding: 1rem 2rem;
            border-radius: 8px;
            font-weight: bold;
            letter-spacing: 1px;
            border-bottom: 3px solid transparent;
            transition: all 0.3s ease;
        }

        .skill-badge:hover {
            transform: translateY(-5px);
            border-bottom: 3px solid var(--accent-color);
            box-shadow: 0 10px 20px rgba(0,0,0,0.2);
        }

        /* Projects Section */
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .project-card {
            background-color: var(--card-bg);
            border-radius: 8px;
            padding: 2rem;
            transition: transform 0.3s ease;
        }

        .project-card:hover {
            transform: translateY(-10px);
        }

        .project-title {
            font-size: 1.5rem;
            margin-bottom: 1rem;
            color: var(--text-main);
        }

        .project-desc {
            color: var(--text-muted);
            margin-bottom: 1.5rem;
        }

        .project-tech {
            display: flex;
            gap: 1rem;
            font-size: 0.9rem;
            color: var(--accent-color);
            font-family: monospace;
        }

        /* Contact Section */
        #contact {
            text-align: center;
            align-items: center;
            min-height: 60vh;
        }

        #contact p {
            max-width: 600px;
            color: var(--text-muted);
            margin-bottom: 2rem;
            font-size: 1.1rem;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 2rem;
            color: var(--text-muted);
            font-size: 0.9rem;
            background-color: var(--bg-color);
        }
    </style>
</head>
<body>

    <!-- Navigation -->
    <nav>
        <div class="logo">Portfolio.</div>
        <ul class="nav-links">
            <li><a href="#about">About</a></li>
            <li><a href="#skills">Skills</a></li>
            <li><a href="#projects">Projects</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <!-- Hero Section -->
    <section id="hero">
        <span class="greeting">Hi, my name is</span>
        <h1 class="title">Your Name.</h1>
        <h2 class="subtitle">I build things for the web.</h2>
        <p class="hero-text">
            I'm a Junior Software Developer and a 5th-year Informatics & Electronic Systems Engineering student. 
            I specialize in building exceptional digital experiences using modern web technologies and Java.
        </p>
        <a href="#projects" class="btn">Check out my work</a>
    </section>

    <!-- About Section -->
    <section id="about">
        <h2>About Me</h2>
        <div class="about-content">
            <div class="about-text">
                <p>Hello! My name is [Your Name] and I enjoy creating things that live on the internet. My interest in software development started back when I began my academic journey, and it has evolved into a true passion.</p>
                <p>Currently, I am in my <strong>5th year</strong> studying Informatics and Electronic Systems Engineering. Alongside my studies, I have gained <strong>6 months of professional experience</strong> working at a software company. This role taught me how to collaborate effectively in a team, write clean code, and tackle real-world problems.</p>
                <p>My main focus these days is building accessible, inclusive products and improving my backend architecture skills with Java.</p>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills">
        <h2>Tech Stack</h2>
        <p style="color: var(--text-muted); margin-bottom: 2rem;">Here are a few technologies I've been working with recently:</p>
        <div class="skills-grid">
            <div class="skill-badge">HTML5</div>
            <div class="skill-badge">CSS3</div>
            <div class="skill-badge">JavaScript (ES6+)</div>
            <div class="skill-badge">Java</div>
            <div class="skill-badge">Git & GitHub</div>
            <div class="skill-badge">Responsive Design</div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects">
        <h2>Some Things I've Built</h2>
        <div class="projects-grid">
            <!-- Project 1 -->
            <div class="project-card">
                <h3 class="project-title">Project Name One</h3>
                <p class="project-desc">A brief description of what this project does, the problem it solves, and your specific role in building it.</p>
                <div class="project-tech">
                    <span>HTML</span>
                    <span>CSS</span>
                    <span>JS</span>
                </div>
            </div>
            <!-- Project 2 -->
            <div class="project-card">
                <h3 class="project-title">Java Application Two</h3>
                <p class="project-desc">A backend system or desktop application demonstrating object-oriented programming principles and clean architecture.</p>
                <div class="project-tech">
                    <span>Java</span>
                    <span>OOP</span>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact">
        <h2>Get In Touch</h2>
        <p>I'm currently looking for new opportunities. Whether you have a question, a project idea, or just want to say hi, my inbox is always open. I'll try my best to get back to you!</p>
        <a href="mailto:your.email@example.com" class="btn">Say Hello</a>
        <br><br>
        <div style="margin-top: 2rem;">
            <a href="https://github.com/YOUR_USERNAME" target="_blank" style="margin-right: 1.5rem; font-size: 1.2rem;">GitHub</a>
            <a href="https://linkedin.com/in/YOUR_LINKEDIN" target="_blank" style="font-size: 1.2rem;">LinkedIn</a>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <p>Designed & Built by [Your Name]</p>
    </footer>

</body>
</html>