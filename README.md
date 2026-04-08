<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Personal Portfolio</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            background-color: #f8f9fa;
            color: #333;
            line-height: 1.6;
        }

        
        nav {
            display: flex;
            justify-content: flex-end;
            align-items: center;
            padding: 20px 8%;
            background: #ffffff;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }

        nav a {
            margin-left: 30px;
            text-decoration: none;
            color: #444;
            font-weight: 600;
            font-size: 0.9rem;
            text-transform: uppercase;
            letter-spacing: 1px;
            transition: color 0.3s;
        }

        nav a:hover {
            color: #6366f1;
        }

    
        header.hero {
            height: 90vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            background: linear-gradient(135deg, #6366f1 0%, #a855f7 100%);
            color: white;
            text-align: center;
            padding-top: 60px;
        }

        .profile-pic {
            width: 180px;
            height: 180px;
            border-radius: 50%;
            border: 6px solid rgba(255, 255, 255, 0.3);
            object-fit: cover;
            margin-bottom: 20px;
        }

        
        section {
            padding: 100px 10%;
            max-width: 1200px;
            margin: 0 auto;
        }

        h2 {
            font-size: 2rem;
            margin-bottom: 30px;
            color: #1f2937;
            position: relative;
            display: inline-block;
        }

        h2::after {
            content: '';
            position: absolute;
            width: 50%;
            height: 4px;
            background: #6366f1;
            bottom: -10px;
            left: 0;
            border-radius: 2px;
        }

        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }

        .card {
            background: white;
            padding: 25px;
            border-radius: 12px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
        }

        
        .video-container {
            position: relative;
            padding-bottom: 56.25%;
            height: 0;
            overflow: hidden;
            border-radius: 8px;
            margin-bottom: 15px;
        }

        .video-container iframe {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
        }

        
        .contact-table {
            width: 100%;
            border-collapse: collapse;
            background: white;
            border-radius: 12px;
            overflow: hidden;
            box-shadow: 0 4px 15px rgba(0,0,0,0.05);
        }

        .contact-table td {
            padding: 20px;
            border-bottom: 1px solid #eee;
        }

        .label-cell {
            background-color: #f3f4f6;
            font-weight: 600;
            width: 30%;
            color: #4b5563;
        }

        input[type="text"], 
        input[type="email"], 
        textarea {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 6px;
            outline: none;
            transition: border 0.3s;
        }

        input:focus, textarea:focus {
            border-color: #6366f1;
        }

        .submit-btn {
            background: #6366f1;
            color: white;
            border: none;
            padding: 12px 30px;
            border-radius: 6px;
            cursor: pointer;
            font-weight: 600;
            transition: background 0.3s;
        }

        .submit-btn:hover {
            background: #4f46e5;
        }

        footer {
            background: #1f2937;
            color: #9ca3af;
            text-align: center;
            padding: 50px 20px;
        }
    </style>
</head>
<body>

    <nav>
        <a href="#about">About</a>
        <a href="#skills">Skills</a>
        <a href="#tutorials">Tutorials</a>
        <a href="#contact">Contact</a>
    </nav>

    <header class="hero">
        <img src="/FB_IMG_17160401108825296.jpg " alt="Profile Picture" class="profile-pic">
        <h1>JERO ESTEBAN</h1>
        <p>I.T STUDENT</p>
    </header>

    <section id="about">
 <h2>About Me</h2>
        <p>I am a creative developer passionate about building clean, functional, and user-friendly websites. I enjoy learning new technologies and sharing my knowledge through tutorials.</p>
    </section>

    <section id="skills">
        <h2>My Skills</h2>
        <div class="grid">
            <div class="card"><h3>Design</h3><p>UI/UX Design, Figma, Canva.</p></div>
            <div class="card"><h3>Development</h3><p>HTML5, CSS3, JavaScript.</p></div>
            <div class="card"><h3>Other</h3><p>Video Editing, SEO Optimization.</p></div>
        </div>
    </section>

    <section id="tutorials">
        <h2>Video Tutorials</h2>
        <div class="grid">
            <div class="card">
                <div class="video-container">
                    <iframe src="https://www.youtube.com/embed/dQw4w9WgXcQ" frameborder="0" allowfullscreen></iframe>
                </div>
                <h3>Tutorial #1</h3>
                <p>Getting started with the basics.</p>
            </div>
            <div class="card">
                <div class="video-container">
                    <iframe src="https://www.youtube.com/embed/dQw4w9WgXcQ" frameborder="0" allowfullscreen></iframe>
                </div>
                <h3>Tutorial #2</h3>
                <p>Mastering the design phase.</p>
            </div>
            <div class="card">
                <div class="video-container">
                    <iframe src="https://www.youtube.com/embed/dQw4w9WgXcQ" frameborder="0" allowfullscreen></iframe>
                </div>
                <h3>Tutorial #3</h3>
                <p>Advanced tips and tricks.</p>
            </div>
        </div>
    </section>

    <section id="contact">
        <h2>Contact Me</h2>
        <p style="margin-bottom: 20px;">Have a question? Fill out the form below and I'll get back to you!</p>
        
        <form action="#">
            <table class="contact-table">
                <tr>
                    <td class="label-cell">Full Name</td>
                    <td><input type="text" placeholder="Your Name" required></td>
                </tr>
                <tr>
                    <td class="label-cell">Email Address</td>
                    <td><input type="email" placeholder="email@example.com" required></td>
                </tr>
                <tr>
                    <td class="label-cell">Message</td>
                    <td><textarea rows="5" placeholder="How can I help you?" required></textarea></td>
                </tr>
                <tr>
                    <td class="label-cell"></td>
                    <td><button type="submit" class="submit-btn">Send Message</button></td>
                </tr>
            </table>
        </form>
    </section>

    <footer>
        <p>&copy; 2026 Esteban, Jero Portfolio.</p>
    </footer>

</body>
</html>
