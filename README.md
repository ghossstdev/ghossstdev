<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Component</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="container">
        <div class="content-wrapper">
            <div class="profile-section">
                <div class="avatar-wrapper">
                    <img src="https://avatars.githubusercontent.com/u/111188920" alt="Avatar" class="avatar">
                </div>
                <div class="info-wrapper">
                    <div class="text-wrapper">
                        <h1 class="name">John Doe</h1>
                        <p class="role">Frontend Developer</p>
                    </div>
                    <div class="links-wrapper">
                        <a href="#" class="social-link">
                            <svg class="icon"><!-- GithubIcon --></svg>
                            <span>johndoe</span>
                        </a>
                        <a href="#" class="social-link">
                            <svg class="icon"><!-- TwitterIcon --></svg>
                            <span>@johndoe</span>
                        </a>
                        <a href="#" class="social-link">
                            <svg class="icon"><!-- LinkedinIcon --></svg>
                            <span>johndoe</span>
                        </a>
                    </div>
                </div>
            </div>
            <div class="section">
                <h2 class="section-title">About Me</h2>
                <p class="section-content">
                    I am a frontend developer with a passion for creating beautiful and functional user interfaces. I have
                    experience working with HTML, CSS, JavaScript, React, Next.js, Astro, and Linux.
                </p>
            </div>
            <div class="section">
                <h2 class="section-title">Skills</h2>
                <div class="skills-grid">
                    <div class="skill">
                        <svg class="icon"><!-- HashIcon --></svg>
                        <span>HTML</span>
                    </div>
                    <div class="skill">
                        <svg class="icon"><!-- CodepenIcon --></svg>
                        <span>CSS</span>
                    </div>
                    <div class="skill">
                        <svg class="icon"><!-- CodepenIcon --></svg>
                        <span>JavaScript</span>
                    </div>
                    <div class="skill">
                        <svg class="icon"><!-- CodepenIcon --></svg>
                        <span>React</span>
                    </div>
                    <div class="skill">
                        <svg class="icon"><!-- CodepenIcon --></svg>
                        <span>Next.js</span>
                    </div>
                    <div class="skill">
                        <svg class="icon"><!-- SpaceIcon --></svg>
                        <span>Astro</span>
                    </div>
                    <div class="skill">
                        <svg class="icon"><!-- LaptopIcon --></svg>
                        <span>Linux</span>
                    </div>
                </div>
            </div>
            <div class="section">
                <h2 class="section-title">Projects</h2>
                <div class="projects-grid">
                    <div class="card">
                        <div class="card-header">
                            <h3 class="card-title">Project 1</h3>
                            <p class="card-description">A web application built with React and Next.js.</p>
                        </div>
                        <div class="card-content">
                            <svg class="icon"><!-- GithubIcon --></svg>
                            <a href="#" class="card-link">View on GitHub</a>
                        </div>
                    </div>
                    <div class="card">
                        <div class="card-header">
                            <h3 class="card-title">Project 2</h3>
                            <p class="card-description">A static website built with Astro.</p>
                        </div>
                        <div class="card-content">
                            <svg class="icon"><!-- GithubIcon --></svg>
                            <a href="#" class="card-link">View on GitHub</a>
                        </div>
                    </div>
                </div>
            </div>
            <div class="section">
                <h2 class="section-title">Contact</h2>
                <div class="contact-wrapper">
                    <div class="contact-item">
                        <svg class="icon"><!-- MailOpenIcon --></svg>
                        <span>johndoe@example.com</span>
                    </div>
                    <div class="contact-item">
                        <svg class="icon"><!-- PhoneIcon --></svg>
                        <span>+1 (555) 555-5555</span>
                    </div>
                </div>
            </div>
        </div>
    </div>
</body>
</html>

<style>
  * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    background-color: var(--background-color);
    color: var(--foreground-color);
    font-family: Arial, sans-serif;
}

.container {
    max-width: 768px;
    width: 100%;
    padding: 16px;
}

.content-wrapper {
    display: flex;
    flex-direction: column;
    gap: 32px;
}

.profile-section {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 16px;
}

@media (min-width: 768px) {
    .profile-section {
        flex-direction: row;
        align-items: flex-start;
    }
}

.avatar-wrapper {
    flex-shrink: 0;
}

.avatar {
    width: 128px;
    height: 128px;
    border-radius: 50%;
}

.info-wrapper {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 16px;
}

@media (min-width: 768px) {
    .info-wrapper {
        align-items: flex-start;
    }
}

.text-wrapper {
    text-align: center;
}

@media (min-width: 768px) {
    .text-wrapper {
        text-align: left;
    }
}

.name {
    font-size: 2rem;
    font-weight: bold;
}

.role {
    color: var(--muted-foreground-color);
}

.links-wrapper {
    display: flex;
    flex-direction: column;
    gap: 8px;
}

@media (min-width: 768px) {
    .links-wrapper {
        flex-direction: row;
    }
}

.social-link {
    display: flex;
    align-items: center;
    gap: 8px;
    text-decoration: none;
    color: inherit;
}

.section {
    margin-top: 32px;
}

.section-title {
    font-size: 1.5rem;
    font-weight: bold;
}

.section-content {
    margin-top: 16px;
    color: var(--muted-foreground-color);
}

.skills-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 16px;
    margin-top: 16px;
}

@media (min-width: 768px) {
    .skills-grid {
        grid-template-columns: repeat(3, 1fr);
    }
}

.skill {
    display: flex;
    align-items: center;
    gap: 8px;
    background-color: var(--muted-background-color);
    border-radius: 8px;
    padding: 8px;
}

.projects-grid {
    display: grid;
    grid-template-columns: 1fr;
    gap: 16px;
    margin-top: 16px;
}

@media (min-width: 768px) {
    .projects-grid {
        grid-template-columns: 1fr 1fr;
    }
}

.card {
    border: 1px solid var(--muted-background-color);
    border-radius: 8px;
    padding: 16px;
}

.card-header {
    margin-bottom: 16px;
}

.card-title {
    font-size: 1.25rem;
    font-weight: bold;
}

.card-description {
    color: var(--muted-foreground-color);
}

.card-content {
    display: flex;
    align-items: center;
    gap: 8px;
}

.card-link {
    color: var(--primary-color);
    text-decoration: none;
}

.card-link:hover {
    text-decoration: underline;
}

.contact-wrapper {
    display: flex;
    flex-direction: column;
    gap: 16px;
}

@media (min-width: 768px) {
    .contact-wrapper {
        flex-direction: row;
    }
}

.contact-item {
    display: flex;
    align-items: center;
    gap: 8px;
}

</style>
