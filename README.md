<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Personal Portfolio of Sheel Patel">
    <title>Sheel Patel - Portfolio</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <img src="Sheel_Headshot.png" alt="Sheel Patel Headshot" class="profile-img">
        <h1>Sheel Patel</h1>
        <p>Bioengineering, Neuroscience, Cognitive Science | University of Pennsylvania</p>
    </header>
    <main>
        <section id="about">
            <h2>About Me</h2>
            <p>
                I am passionate about improving adolescent mental health, advancing TBI research, 
                and exploring the intersection of climate and neurological health. I am also pursuing 
                an accelerated Master's in Bioengineering, with minors in Healthcare Management, 
                Data Science, and Chemistry.
            </p>
        </section>
        <section id="projects">
            <h2>Projects</h2>
            <ul>
                <li>
                    <a href="https://github.com/sheelpatel/project1" target="_blank">
                        Project 1
                    </a> - Developing deep learning algorithms for traumatic brain injury research.
                </li>
                <li>
                    <a href="https://github.com/sheelpatel/project2" target="_blank">
                        Project 2
                    </a> - Exploring climate and neurological health through computational models.
                </li>
            </ul>
        </section>
        <section id="contact">
            <h2>Contact</h2>
            <p>
                Email: <a href="mailto:sheelp@sas.upenn.edu">sheelp@sas.upenn.edu</a>
            </p>
        </section>
    </main>
    <footer>
        <p>&copy; 2025 Sheel Patel. All rights reserved.</p>
    </footer>
</body>
</html>

/* General Styles */
body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
    color: #333;
}

/* Header Section */
header {
    text-align: center;
    padding: 2em;
    background-color: #0077b6;
    color: white;
}

.profile-img {
    width: 150px;
    height: 150px;
    border-radius: 50%;
    margin-bottom: 1em;
    border: 3px solid white;
}

/* Main Content */
main {
    padding: 2em;
    max-width: 800px;
    margin: 0 auto;
}

section {
    margin-bottom: 2em;
}

h2 {
    color: #0077b6;
    border-bottom: 2px solid #0077b6;
    display: inline-block;
    padding-bottom: 0.3em;
    margin-bottom: 1em;
}

a {
    color: #0077b6;
    text-decoration: none;
}

a:hover {
    text-decoration: underline;
}

/* Footer */
footer {
    text-align: center;
    padding: 1em;
    background-color: #333;
    color: white;
    margin-top: 2em;
}


