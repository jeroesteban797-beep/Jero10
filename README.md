<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Portfolio</title>
  <style>
    body {font-family: Arial, sans-serif; margin:0; background:#fff; color:#333;}
    header {background:#111; color:#fff; padding:20px; text-align:center;}
    nav {display:flex; justify-content:center; background:#333; flex-wrap:wrap;}
    nav a, nav button {color:#fff; text-decoration:none; padding:14px 20px; font-size:16px; border:none; background:none; cursor:pointer;}
    nav a:hover, nav button:hover {background:#555;}
    section {padding:60px 20px;}
    h2 {margin-top:0; text-align:center;}
    html {scroll-behavior:smooth;}
    /* Hero */
    #home {display:flex; align-items:center; justify-content:space-between; flex-wrap:wrap;}
    #home .intro {flex:1; padding:20px;}
    #home img {flex:1; max-width:400px; border-radius:10px;}
    /* Services cards */
    .services {display:grid; grid-template-columns:repeat(auto-fit,minmax(200px,1fr)); gap:20px;}
    .service-card {padding:20px; border:1px solid #ddd; border-radius:8px; text-align:center; background:#f9f9f9;}
    /* Gallery */
    .gallery {display:flex; flex-wrap:wrap; gap:20px; justify-content:center;}
    .gallery-item {flex:1; min-width:250px; text-align:center;}
    .gallery-item img {max-width:100%; border-radius:8px; box-shadow:0 2px 6px rgba(0,0,0,0.2);}
    /* Contact form */
    form {max-width:500px; margin:auto; display:flex; flex-direction:column;}
    form input, form textarea {margin:10px 0; padding:10px; font-size:14px; border:1px solid #ccc; border-radius:4px;}
    form button {padding:12px; background:#333; color:#fff; border:none; cursor:pointer; font-size:16px;}
    form button:hover {background:#555;}
    /* Stats */
    .stats {display:flex; justify-content:center; gap:40px; flex-wrap:wrap; text-align:center;}
    .stat {font-size:20px; font-weight:bold;}
 
    #chatbot {
    position: fixed;
    bottom: 20px;
    right: 20px;
    width: 300px;
    background: #1e1e1e;
    border: 1px solid #333;
    border-radius: 10px;
    transition: all 0.3s ease;
    z-index: 1000;
}

#chatbot.minimized {
    height: 40px;
    width: 150px;
    overflow: hidden;
}

#chat-window {
    height: 300px;
    overflow-y: auto;
    padding: 10px;
    color: white;
    font-size: 14px;
}

#chat-input {
    width: 100%;
    padding: 10px;
    border: none;
    background: #2d2d2d;
    color: white;
}

  </style>
</head>
<body>

<header>
  <h1>My Portfolio</h1>
  <p>Showcasing my skills, projects, and achievements</p>
</header>

<nav>
  <a href="#home">Home</a>
  <a href="#about">About</a>
  <a href="#skills">Skills</a>
  <a href="#projects">Projects</a>
  <a href="#certificates">Certificates</a>
  <a href="#contact">Contact</a>
  <button onclick="downloadCV()">Download CV</button>
</nav>

<!-- Hero -->
<section id="home">
  <div class="intro">
    <h1>Hello, I’m Jero Esteban</h1>
    <p>A Second Year College Student of Central Philippines State University-Moises Padilla Campus.Taking up the Bachelor of Science in Information Technology.</p>
  </div>
  <img src="/Messenger_creation_D7004EDB-C243-4CE4-A2F5-599EBDA34F21.jpeg" alt="My Portrait">
</section>


<section id="about">
  <h1>About Me</h1>
  <p>I am a passionate developer and designer, focused on creating modern, user-friendly digital experiences.</p>
  <div class="stats">
    <div class="stat">2+ Years</div>
    <div class="stat">10+ Projects</div>
    <div class="stat">10+ Certificates</div>
  </div>
</section>


<section id="skills">
  <h1>Skills</h1>
  <ul>
    <li>Web Development (HTML, CSS, JavaScript)</li>
    <li>UI/UX Design</li>
    <li>WordPress Customization</li>
    <li>Graphic Design (Canva, Photoshop)</li>
  </ul>
</section>

<section id="projects">
  <h1>Projects</h1>
  <div class="gallery">
    <div class="gallery-item">
      <img src="/Messenger_creation_F171150B-9DBD-4A25-8C2A-08BFB811119A.jpeg" alt="Certificate 1">
      <p>Artificial Intelligence</p>
    </div>
    <div class="gallery-item">
      <img src="/Messenger_creation_88DDEBB8-06A8-48FE-8C49-A1B9B34FF890.jpeg" alt="Certificate 2">
      <p>IT SEMINAR</p>
    </div>

<section id="certificates">
  <h1>Certificates</h1>
  <div class="gallery">
    <div class="gallery-item">
      <img src="/Messenger_creation_59EECDCE-C501-405F-9190-65829671D23C.jpeg" alt="Certificate 1">
      <p>Cisco Networking Fundamentals</p>
    </div>
    <div class="gallery-item">
      <img src="/Messenger_creation_B7E4A3F8-C60C-4A9E-8110-1ADACE32B8AF.jpeg" alt="Certificate 2">
      <p>IT SEMINAR</p>
    </div>

  </div>
</section>

<section id="contact">
  <h1>Contact</h1>
  <p>Reach out to me directly using the form below:</p>
  <form action="mailto:yourname@example.com" method="post" enctype="text/plain">
    <input type="text" name="name" placeholder="Your Name" required>
    <input type="email" name="email" placeholder="Your Email" required>
    <textarea name="message" rows="5" placeholder="Your Message" required></textarea>
    <button type="submit">Send Message</button>
  </form>
</section>

<div id="chatbot">
    <div onclick="toggleChat()" style="background: #333; padding: 10px; cursor: pointer; border-radius: 10px 10px 0 0;">
        <span>🤖 Portfolio AI</span>
    </div>
    <div id="chat-window"></div>
    <input id="chat-input" type="text" placeholder="Ask me about my portfolio...">
</div>


<script>
  function downloadCV() {
    const link = document.createElement('a');
    link.href = 'https://sg.docworkspace.com/d/sbCaie7EbDP9VEam_iz85afwpa7cxibg96n?sa=601.1245';
    link.download = 'My_CV.pdf';
    link.click();
  }

  const chatWindow = document.getElementById('chat-window');
  const chatInput = document.getElementById('chat-input');

  chatInput.addEventListener('keypress', function (e) {
    if (e.key === 'Enter' && chatInput.value.trim() !== "") {
        const userMessage = chatInput.value;
        
        
        appendMessage('User', userMessage);
        chatInput.value = ''; 

        
        setTimeout(() => {
            const botResponse = getBotResponse(userMessage);
            appendMessage('AI', botResponse);
        }, 600);
    }
});

function appendMessage(sender, text) {
    const msgDiv = document.createElement('div');
    msgDiv.innerHTML = `<strong>${sender}:</strong> ${text}`;
    msgDiv.style.margin = "5px 0";
    chatWindow.appendChild(msgDiv);
    chatWindow.scrollTop = chatWindow.scrollHeight; 
}

function getBotResponse(input) {
    const query = input.toLowerCase();
    if (query.includes("skills")) return "I am proficient in HTML, CSS, JS, and React!";
    if (query.includes("contact")) return "You can reach me via the contact form above.";
    if (query.includes("projects")) return "Check out my 'Work' section for my latest projects!";
    return "That's a great question! I'm still learning, but feel free to browse my resume.";
}


function toggleChat() {
    const bot = document.getElementById('chatbot');
    bot.classList.toggle('minimized');
}
