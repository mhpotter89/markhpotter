# markhpotter.com
/* --- Variables --- */
:root {
    --primary-color: #1a365d; /* Deep Navy Blue */
    --secondary-color: #2b6cb0; /* Professional Mid-Blue */
    --accent-color: #4a5568; /* Slate Grey */
    --text-color: #2d3748; /* Dark Grey for primary text */
    --text-light: #718096; /* Medium Grey for secondary text */
    --bg-color: #ffffff; /* Clean White */
    --bg-light: #edf2f7; /* Soft Cool Grey for alternating sections */
    --border-color: #e2e8f0; /* Crisp Light Grey for borders */
    --font-main: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
    --transition: all 0.3s ease;
}

/* --- Global Styles --- */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: var(--font-main);
    color: var(--text-color);
    line-height: 1.6;
    background-color: var(--bg-color);
}

a {
    text-decoration: none;
    color: var(--secondary-color);
    transition: var(--transition);
}

a:hover {
    color: var(--primary-color);
}

.container {
    max-width: 1100px;
    margin: 0 auto;
    padding: 0 20px;
}

.section-title {
    font-size: 2.5rem;
    color: var(--primary-color);
    margin-bottom: 3rem;
    text-align: center;
    font-weight: 700;
    letter-spacing: -0.5px;
}

.mt-2 { margin-top: 2rem; }

/* --- Buttons --- */
.btn {
    display: inline-block;
    padding: 12px 28px;
    border-radius: 4px; /* Sharper corners for a corporate look */
    font-weight: 600;
    cursor: pointer;
    transition: var(--transition);
    text-align: center;
}

.btn-primary {
    background-color: var(--secondary-color);
    color: #fff;
    border: 1px solid var(--secondary-color);
}

.btn-primary:hover {
    background-color: var(--primary-color);
    border-color: var(--primary-color);
    color: #fff;
}

.btn-outline {
    background-color: transparent;
    color: var(--secondary-color);
    border: 2px solid var(--secondary-color);
}

.btn-outline:hover {
    background-color: var(--bg-light);
    color: var(--primary-color);
    border-color: var(--primary-color);
}

/* --- Navigation --- */
.navbar {
    background-color: #ffffff;
    box-shadow: 0 1px 3px rgba(0,0,0,0.05); /* Softer, highly professional shadow */
    position: fixed;
    width: 100%;
    top: 0;
    z-index: 1000;
    border-bottom: 1px solid var(--border-color);
}

.nav-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 18px 20px;
    max-width: 1100px;
    margin: 0 auto;
}

.logo {
    font-size: 1.4rem;
    font-weight: 700;
    color: var(--primary-color);
    letter-spacing: -0.5px;
}

.nav-links {
    list-style: none;
    display: flex;
    align-items: center;
    gap: 32px;
}

.nav-links a {
    color: var(--accent-color);
    font-weight: 600;
    font-size: 0.95rem;
}

.nav-links a:hover {
    color: var(--secondary-color);
}

/* --- Hero Section --- */
.hero {
    padding: 200px 0 120px;
    background: linear-gradient(to bottom, var(--bg-light), #ffffff); /* Subtle gradient */
    text-align: center;
    border-bottom: 1px solid var(--border-color);
}

.hero h1 {
    font-size: 3.2rem;
    color: var(--primary-color);
    line-height: 1.25;
    margin-bottom: 24px;
    font-weight: 700;
    letter-spacing: -1px;
}

.hero-subtitle {
    font-size: 1.2rem;
    color: var(--text-light);
    max-width: 800px;
    margin: 0 auto 40px;
    line-height: 1.7;
}

/* --- Portfolio Section --- */
.portfolio {
    padding: 100px 0;
}

.grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 30px;
}

.card {
    background: #fff;
    padding: 35px 30px;
    border-radius: 6px;
    box-shadow: 0 4px 6px rgba(0,0,0,0.02);
    border: 1px solid var(--border-color);
    transition: var(--transition);
}

.card:hover {
    transform: translateY(-4px);
    box-shadow: 0 12px 20px rgba(0,0,0,0.06);
    border-color: var(--secondary-color); /* Highlight border on hover */
}

.card h3 {
    color: var(--primary-color);
    margin-bottom: 15px;
    font-size: 1.3rem;
    font-weight: 600;
}

.card p {
    color: var(--text-light);
    margin-bottom: 12px;
    font-size: 0.95rem;
}

.card strong {
    color: var(--text-color);
}

/* --- Experience Section --- */
.experience {
    padding: 100px 0;
}

.bg-light {
    background-color: var(--bg-light);
    border-top: 1px solid var(--border-color);
    border-bottom: 1px solid var(--border-color);
}

.timeline {
    max-width: 800px;
    margin: 0 auto;
}

.timeline-item {
    margin-bottom: 45px;
    padding-left: 25px;
    border-left: 3px solid var(--secondary-color);
}

.timeline-item h3 {
    color: var(--primary-color);
    margin-bottom: 12px;
    font-size: 1.4rem;
}

.timeline-item p {
    color: var(--text-light);
    font-size: 1.05rem;
}

.resume-download {
    text-align: center;
    margin-top: 60px;
}

/* --- About Section --- */
.about {
    padding: 100px 0;
}

.about-content {
    max-width: 800px;
    margin: 0 auto;
}

.about-text h3 {
    color: var(--primary-color);
    margin-bottom: 15px;
    font-size: 1.4rem;
    border-bottom: 2px solid var(--bg-light);
    padding-bottom: 8px;
    display: inline-block;
}

.about-text p {
    margin-bottom: 24px;
    font-size: 1.05rem;
    color: var(--text-light);
}

/* --- Footer --- */
.footer {
    background-color: var(--primary-color);
    color: #fff;
    padding: 70px 0 40px;
    text-align: center;
}

.footer h2 {
    margin-bottom: 20px;
    color: #fff;
}

.footer p {
    color: var(--accent-color);
}

.contact-links {
    margin: 35px 0;
    display: flex;
    justify-content: center;
    gap: 35px;
}

.contact-links a, .contact-links span {
    color: #fff;
    font-weight: 500;
    font-size: 1.05rem;
}

.contact-links a:hover {
    color: var(--secondary-color);
}

.copyright {
    margin-top: 50px;
    font-size: 0.9rem;
    border-top: 1px solid rgba(255,255,255,0.05);
    padding-top: 25px;
    color: #718096;
}

/* --- Responsive --- */
@media (max-width: 768px) {
    .hero h1 { font-size: 2.4rem; }
    .nav-links { display: none; }
    .contact-links { flex-direction: column; gap: 15px; }
}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mark Potter | Learning Architecture & Product</title>
    <link rel="stylesheet" href="style.css">
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">
</head>
<body>

    <nav class="navbar">
        <div class="nav-container">
            <a href="#home" class="logo">Mark Potter</a>
            <ul class="nav-links">
                <li><a href="#portfolio">Portfolio</a></li>
                <li><a href="#experience">Experience</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact" class="btn btn-outline">Let's Connect</a></li>
            </ul>
        </div>
    </nav>

    <header id="home" class="hero">
        <div class="container">
            <h1>Leading Diverse Learning Experiences to Support Diverse Learners.</h1>
            <p class="hero-subtitle">My career has centered on one driving question: How do we design learning experiences that help people grow faster, more confidently, and with greater engagement? By merging strong pedagogy with AI-driven efficiency and insight, I build large-scale instructional ecosystems that scale expertise and transform organizations.</p>
            <div class="hero-actions">
                <a href="#portfolio" class="btn btn-primary">View My Work</a>
            </div>
        </div>
    </header>

    <section id="portfolio" class="portfolio">
        <div class="container">
            <h2 class="section-title">Case Studies & Projects</h2>
            <div class="grid">
                
                <div class="card">
                    <h3>AI Transformation in EdTech</h3>
                    <p><strong>Context:</strong> Flagship platforms across McGraw Hill, ETS, and Pearson.</p>
                    <p><strong>Impact:</strong> Led cross-functional teams to define strategic visions for impactful learning experiences. Streamlined operations by redesigning processes and integrating AI tools that preserve consistency while increasing velocity and improving learning effectiveness through personalized mastery pathways.</p>
                </div>

                <div class="card">
                    <h3>LAPIS Framework</h3>
                    <p><strong>Context:</strong> Learning Architecture & Personalized Infrastructure Stack.</p>
                    <p><strong>Impact:</strong> Developed modular educational frameworks and UI concepts for a "Contextual Creative Studio," supporting highly tailored learning environments and data-informed structural design.</p>
                </div>

                <div class="card">
                    <h3>Procedural Generation Systems</h3>
                    <p><strong>Context:</strong> Technical prototyping and systems-thinking.</p>
                    <p><strong>Impact:</strong> Developed a Python and web-based solar system generator modeling complex civilization mechanics and precursor structures, translating complex systems architecture into mapping expansive learning ecosystems.</p>
                </div>

            </div>
        </div>
    </section>

    <section id="experience" class="experience bg-light">
        <div class="container">
            <h2 class="section-title">Experience & Philosophy</h2>
            
            <div class="timeline">
                <div class="timeline-item">
                    <h3>Product Leadership</h3>
                    <p>Leading the long-term vision, discovery, prioritization, and delivery for flagship platforms like McGraw Hill's Connect and Lazuli at the Learning Design Alliance. Grounding strategy in user research with educators and learners to architect intuitive, workflow-aligned experiences.</p>
                </div>
                <div class="timeline-item">
                    <h3>Learning Science Strategy</h3>
                    <p>Designing robust experiences grounded in evidence-based educational design. Translating complex research into scalable product features and AI-supported workflows that maintain pedagogical integrity and transparency.</p>
                </div>
                <div class="timeline-item">
                    <h3>Mentorship & Culture</h3>
                    <p>Fostering continuous improvement and psychological safety. Coaching teams and subject matter experts to adopt new methodologies, navigate change management, and build confidence in emerging learning technologies.</p>
                </div>
            </div>

            <div class="resume-download">
                <a href="#" class="btn btn-primary">Download Full Resume (PDF)</a>
            </div>
        </div>
    </section>

    <section id="about" class="about">
        <div class="container">
            <h2 class="section-title">About Me</h2>
            <div class="about-content">
                <div class="about-text">
                    <h3>The Professional</h3>
                    <p>I hold a Master’s degree in Educational Technology and Applied Learning Science from Carnegie Mellon University. I remain deeply connected to the program, serving as a Graduate Student Industry Mentor to coach students in product and course design projects.</p>
                    
                    <h3 class="mt-2">The Personal</h3>
                    <p>Based in Bethel Park, PA, my systems-thinking approach extends well beyond the screen. I am an active Game Master for tabletop role-playing games, focusing heavily on narrative world-building and precise visual character design—whether that means ensuring a generated character has featureless white wraps instead of a traditional face, or correcting the mechanics of a single-ended polearm kopesh.</p>
                    <p>Whether I'm propagating spider plants for my indoor garden, managing complex rule systems, or out exploring with my wife, kids, and our three dogs—Luna, Monty, and Shadow—I am always looking for ways to build, refine, and improve the environments around me.</p>
                </div>
            </div>
        </div>
    </section>

    <footer id="contact" class="footer">
        <div class="container">
            <h2>Let's Connect</h2>
            <p>I am always open to discussing new opportunities, learning architecture, or systems design.</p>
            <div class="contact-links">
                <a href="mailto:mark.h.potter@gmail.com">mark.h.potter@gmail.com</a>
                <a href="https://www.linkedin.com/in/markhpotter" target="_blank">LinkedIn Profile</a>
                <span>Bethel Park, PA</span>
            </div>
            <p class="copyright">&copy; 2026 Mark Potter. All rights reserved.</p>
        </div>
    </footer>

</body>
</html>
