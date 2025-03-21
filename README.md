<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio</title>
    <style>
        /* General Styles */
        body {
            font-family: 'Poppins', sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(to bottom, #1e1e2f, #2b2b40);
            color: #f4f4f9;
            overflow-x: hidden;
        }

        header {
            background-color: #ff6f61;
            color: white;
            text-align: center;
            padding: 1rem;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.4);
            animation: fadeDown 1s ease-in-out;
        }

        nav ul {
            list-style: none;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
        }
        .profile-photo {
    display: block; /* Centers the image */
    margin: 20px auto; /* Adds spacing and centers */
    width: 150px; /* Adjust width as needed */
    height: 150px; /* Adjust height as needed */
    border-radius: 50%; /* Makes it a circular image */
    border: 3px solid #fff; /* Optional: Add a border */
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2); /* Optional: Adds a shadow effect */
}



        nav ul li {
            margin: 0 15px;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            font-size: 1.1rem;
            transition: color 0.3s ease-in-out, transform 0.3s;
        }

        nav ul li a:hover {
            color: #ffe67d;
            transform: scale(1.1);
        }

        section {
            display: none;
            padding: 50px;
            text-align: center;
            min-height: 80vh;
            animation: fadeIn 1s ease-in-out;
        }

        section.active {
            display: block;
        }

        .section-background {
            border-radius: 15px;
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.4);
            padding: 40px;
            color: white;
        }

        h2 {
            font-size: 2rem;
            margin-bottom: 20px;
            color: #76c7c0;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .project, .skill, .qualification, .certification {
            background: #34344a;
            margin: 20px auto;
            padding: 20px;
            border-radius: 10px;
            width: 60%;
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.3);
        }
    </style>
</head>
<body>
    <header>
        <h1>My Portfolio</h1>
        <nav>
            <ul>
                <li><a id="home-link">Home</a></li>
                <li><a id="about-link">About</a></li>
                <li><a id="skills-link">Technical Skills</a></li>
                <li><a id="education-link">Education</a></li>
                <li><a id="certifications-link">Certifications</a></li>
                <li><a id="projects-link">Projects</a></li>
                <li><a id="contact-link">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section id="home" class="active section-background">
        <h2>Welcome to My Portfolio</h2>
        <img src="photo.jpg"  class="profile-photo">
        <p>Discover my projects, skills, and passions as you navigate through my website.</p>
    </section>

    <section id="about" class="section-background">
        <h2>About Me</h2>
        <p>"Hi, I'm Nivshini from Sivakasi! I'm currently pursuing a degree in Artificial Intelligence and Machine Learning at M.Kumarasamy College of Engineering, Karur.
            I am passionate about exploring new technologies, front-end development, AI, and machine learning. With a strong sense of adaptability, teamwork, and problem-solving skills, I love taking on challenges and continuously improving my skills. 
            Let's connect and innovate together!"</p>
    </section>

    <section id="skills" class="section-background">
        <h2>Technical Skills</h2>
        <div class="skill"><p>Programming Languages: Java, Python, C, C++</p></div>
        <div class="skill"><p>Web Development: HTML, CSS, JavaScript</p></div>
        <div class="skill"><p>Machine Learning: Scikit-Learn, Pandas</p></div>
    </section>

    <section id="education" class="section-background">
        <h2>Educational Qualification</h2>
        <div class="qualification"><p>Bachelor of Engineering in Artificial Intelligence and Machine Learning - M.Kumarasamy College of Engineering, Karur</p></div>
        <div class="qualification"><p>Higher Secondary Certificate - Vinayakar Matriculation Higher Secondary School, Sivakasi(84%)
        </p></div>
        <div class="qualification"><p>Secondary School Certificate - Vinayakar Matriculation Higher Secondary School, Sivakasi(Pass)
        </p></div>
    </section>

    <section id="certifications" class="section-background">
        <h2>Certifications</h2>
        <div class="certification"><p>Data Analytics Essentials - Cisco</p></div>
        <div class="certification"><p>Machine Learning With Python - Cognitive Class</p></div>
        <div class="certification"><p>Full Stack Development - Novi Tech</p></div>
        <div class="certification"><p>Introductio to Industry 4.0 and Internet of Things - NPTEL</p></div>
    </section>

    <section id="projects" class="section-background">
        <h2>My Projects</h2>
        <div class="project">
            <h3>Chat Application</h3>
            <p>A Java-based application that allows users to send and receive messages in real time.</p>
        </div>
        <div class="project">
            <h3>Connected vehicle Fleet Management</h3>
            <p>A fleet management system that analyzes past data to optimize routes, monitor vehicle performance, and improve operational efficiency.</p>
        </div>
    </section>

    <section id="contact" class="section-background">
        <h2>Contact Me</h2>
        <p>📞 Phone: 9342320566</p>
        <p>If you have any questions or queries, feel free to get in touch:</p>
        <form id="contact-form">
            <label for="name">Your Name:</label><br>
            <input type="text" id="name" name="name" placeholder="Enter your name" required><br><br>
    
            <label for="email">Your Email:</label><br>
            <input type="email" id="email" name="email" placeholder="Enter your email" required><br><br>
    
            <label for="message">Your Message:</label><br>
            <textarea id="message" name="message" rows="4" placeholder="Enter your message or query" required></textarea><br><br>
    
        </form>
        <button onclick="alert('Thanks for reaching out!')">submit</button>
    </section>

    <footer>
        &copy; 2025 My Portfolio. Made with ❤.
    </footer>

    <script>
        document.addEventListener("DOMContentLoaded", function () {
            const links = {
                home: document.getElementById("home-link"),
                about: document.getElementById("about-link"),
                skills: document.getElementById("skills-link"),
                education: document.getElementById("education-link"),
                certifications: document.getElementById("certifications-link"),
                projects: document.getElementById("projects-link"),
                contact: document.getElementById("contact-link"),
            };

            const sections = {
                home: document.getElementById("home"),
                about: document.getElementById("about"),
                skills: document.getElementById("skills"),
                education: document.getElementById("education"),
                certifications: document.getElementById("certifications"),
                projects: document.getElementById("projects"),
                contact: document.getElementById("contact"),
            };

            Object.keys(links).forEach((key) => {
                links[key].addEventListener("click", () => {
                    Object.values(sections).forEach((section) => {
                        section.classList.remove("active");
                    });
                    sections[key].classList.add("active");
                });
            });
        });
    </script>
</body>
</html>
