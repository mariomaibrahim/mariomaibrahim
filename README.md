<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Mariam Ibrahim - GitHub Profile</title>
  <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css">
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      line-height: 1.6;
      color: #333;
      background: linear-gradient(to right, #1a1a2e, #16213e, #0f3460);
      color: #e6e6e6;
      padding: 20px;
    }
    
    .container {
      max-width: 900px;
      margin: 0 auto;
      padding: 20px;
      background-color: rgba(255, 255, 255, 0.1);
      border-radius: 10px;
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.5);
      backdrop-filter: blur(5px);
    }
    
    h1, h2, h3, h4 {
      color: #ff9a8b;
      text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
    }
    
    .intro-text {
      font-size: 1.1em;
      color: #d8d8d8;
      margin-bottom: 20px;
      text-align: justify;
    }
    
    .section {
      margin-bottom: 30px;
      border-bottom: 1px solid rgba(255, 255, 255, 0.1);
      padding-bottom: 20px;
    }
    
    .skills-container {
      display: flex;
      flex-wrap: wrap;
      gap: 15px;
      margin-top: 20px;
    }
    
    .skill-badge {
      background: rgba(255, 255, 255, 0.1);
      padding: 8px 15px;
      border-radius: 20px;
      display: inline-flex;
      align-items: center;
      gap: 8px;
      transition: all 0.3s ease;
      cursor: pointer;
    }
    
    .skill-badge:hover {
      background: rgba(255, 255, 255, 0.2);
      transform: translateY(-3px);
      box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
    }
    
    .tools-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(70px, 1fr));
      gap: 20px;
      margin-top: 20px;
    }
    
    .tool-item {
      display: flex;
      flex-direction: column;
      align-items: center;
      text-align: center;
    }
    
    .tool-icon {
      width: 50px;
      height: 50px;
      padding: 10px;
      border-radius: 12px;
      background: rgba(255, 255, 255, 0.1);
      margin-bottom: 8px;
      transition: all 0.3s ease;
      display: flex;
      align-items: center;
      justify-content: center;
    }
    
    .tool-icon:hover {
      transform: scale(1.15);
      background: rgba(255, 255, 255, 0.2);
    }
    
    .tool-name {
      font-size: 0.8em;
      color: #d8d8d8;
    }
    
    table {
      width: 100%;
      border-collapse: collapse;
      margin: 20px 0;
      background-color: rgba(255, 255, 255, 0.05);
      border-radius: 8px;
      overflow: hidden;
    }
    
    th, td {
      padding: 12px 15px;
      text-align: left;
      border-bottom: 1px solid rgba(255, 255, 255, 0.1);
    }
    
    th {
      background-color: rgba(255, 255, 255, 0.1);
      color: #ff9a8b;
    }
    
    tr:hover {
      background-color: rgba(255, 255, 255, 0.1);
    }
    
    .connect-links {
      display: flex;
      gap: 15px;
      flex-wrap: wrap;
      margin-top: 20px;
    }
    
    .connect-button {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      padding: 10px 15px;
      border-radius: 8px;
      background: linear-gradient(45deg, #ff9a8b, #ff6a88);
      color: white;
      text-decoration: none;
      transition: all 0.3s ease;
      font-weight: 600;
    }
    
    .connect-button:hover {
      transform: translateY(-3px);
      box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
      background: linear-gradient(45deg, #ff6a88, #ff9a8b);
    }
    
    blockquote {
      border-left: 4px solid #ff9a8b;
      padding: 15px;
      margin: 20px 0;
      background-color: rgba(255, 255, 255, 0.05);
      border-radius: 0 8px 8px 0;
      font-style: italic;
    }
    
    .stats-container {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 20px;
      margin-top: 20px;
    }
    
    @media (max-width: 768px) {
      .stats-container {
        grid-template-columns: 1fr;
      }
    }
    
    .typing-animation {
      border-right: 2px solid #ff9a8b;
      white-space: nowrap;
      overflow: hidden;
      animation: typing 3.5s steps(40, end), blink-caret 0.75s step-end infinite;
    }
    
    @keyframes typing {
      from { width: 0 }
      to { width: 100% }
    }
    
    @keyframes blink-caret {
      from, to { border-color: transparent }
      50% { border-color: #ff9a8b }
    }
    
    .floating {
      animation: floating 3s ease-in-out infinite;
    }
    
    @keyframes floating {
      0% { transform: translateY(0px); }
      50% { transform: translateY(-10px); }
      100% { transform: translateY(0px); }
    }
    
    .cyber-badge {
      position: relative;
      overflow: hidden;
      padding: 10px 20px;
      background: linear-gradient(45deg, #0f3460, #162447);
      border-radius: 8px;
      box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
      margin: 10px 0;
    }
    
    .cyber-badge::before {
      content: '';
      position: absolute;
      top: -50%;
      left: -50%;
      width: 200%;
      height: 200%;
      background: linear-gradient(
        45deg, 
        transparent 0%, 
        rgba(255, 255, 255, 0.1) 50%, 
        transparent 100%
      );
      transform: rotate(45deg);
      animation: shine 3s infinite;
    }
    
    @keyframes shine {
      0% { left: -100%; top: -100%; }
      100% { left: 100%; top: 100%; }
    }
    
    .glass-card {
      background: rgba(255, 255, 255, 0.1);
      backdrop-filter: blur(10px);
      border-radius: 10px;
      padding: 20px;
      box-shadow: 0 8px 32px rgba(0, 0, 0, 0.2);
      border: 1px solid rgba(255, 255, 255, 0.1);
      margin: 20px 0;
    }
    
    .neon-text {
      color: #fff;
      text-shadow: 
        0 0 5px #fff, 
        0 0 10px #fff, 
        0 0 15px #0073e6, 
        0 0 20px #0073e6, 
        0 0 25px #0073e6;
      animation: neon 1.5s ease-in-out infinite alternate;
    }
    
    @keyframes neon {
      from {
        text-shadow: 
          0 0 5px #fff, 
          0 0 10px #fff, 
          0 0 15px #0073e6, 
          0 0 20px #0073e6;
      }
      to {
        text-shadow: 
          0 0 5px #fff, 
          0 0 10px #0073e6, 
          0 0 15px #0073e6, 
          0 0 20px #0073e6, 
          0 0 25px #0073e6;
      }
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="section">
      <div class="animate__animated animate__fadeIn">
        <img src="https://media0.giphy.com/media/jTNG3RF6EwbkpD4LZx/giphy.gif?cid=6c09b952jtz228wqwtg6r73qf9lt18kn6wcej9cym19oitkk&ep=v1_internal_gif_by_id&rid=giphy.gif&ct=g" alt="welcome gif" style="max-width: 100%; border-radius: 10px; margin-bottom: 20px;">
        
        <h1 class="typing-animation neon-text">Hello! 🫡 I'm Mariam ✨</h1>
        
        <div class="cyber-badge animate__animated animate__fadeInLeft">
          <p>Student at <strong>Borg El Arab University of Technology</strong>, Department of <strong>Information Technology</strong></p>
        </div>
        
        <p class="intro-text animate__animated animate__fadeIn">
          I have a deep passion for <strong>Cybersecurity</strong> and a growing interest in <strong>Digital Forensics</strong>. 
          My dream is to become a <strong>Digital Forensic Analyst</strong>, helping uncover the truth behind digital evidence and cyber incidents. 🕵️‍♀️💻
        </p>
      </div>
    </div>
    
    <div class="section">
      <h2 class="animate__animated animate__fadeInDown">🧠 Currently Learning</h2>
      <div class="skills-container">
        <div class="skill-badge animate__animated animate__fadeInRight">
          <i class="fas fa-search"></i> Digital Forensics & Evidence Handling
        </div>
        <div class="skill-badge animate__animated animate__fadeInRight" style="animation-delay: 0.1s;">
          <i class="fas fa-toolbox"></i> Tools like Autopsy, FTK, Wireshark
        </div>
        <div class="skill-badge animate__animated animate__fadeInRight" style="animation-delay: 0.2s;">
          <i class="fas fa-bomb"></i> Ethical Hacking & Penetration Testing
        </div>
        <div class="skill-badge animate__animated animate__fadeInRight" style="animation-delay: 0.3s;">
          <i class="fas fa-scroll"></i> Cryptography & Secure Communication
        </div>
        <div class="skill-badge animate__animated animate__fadeInRight" style="animation-delay: 0.4s;">
          <i class="fas fa-shield-alt"></i> Incident Response and Threat Analysis
        </div>
        <div class="skill-badge animate__animated animate__fadeInRight" style="animation-delay: 0.5s;">
          <i class="fas fa-laptop-code"></i> Working with Kali Linux and Windows
        </div>
      </div>
    </div>
    
    <div class="section">
      <h2 class="animate__animated animate__fadeInDown">🛠️ Skills</h2>
      <div class="glass-card animate__animated animate__fadeIn">
        <table>
          <tr>
            <th>Area</th>
            <th>Skills & Tools</th>
          </tr>
          <tr>
            <td>Cybersecurity</td>
            <td>Vulnerability Assessment, Forensics, SOC Basics</td>
          </tr>
          <tr>
            <td>Programming</td>
            <td>Python, Bash, C++, C</td>
          </tr>
          <tr>
            <td>Networking</td>
            <td>TCP/IP, OSI Model, VPN, Firewalls, CCNA</td>
          </tr>
          <tr>
            <td>Tools & Platforms</td>
            <td>Kali Linux, Autopsy, Wireshark, Metasploit, FTK</td>
          </tr>
          <tr>
            <td>Soft Skills</td>
            <td>Analytical Thinking, Detail-Oriented, Teamwork</td>
          </tr>
        </table>
      </div>
    </div>
    
    <div class="section">
      <h3 class="animate__animated animate__fadeInLeft">🧰 Languages and Tools:</h3>
      <div class="tools-grid">
        <!-- Original Icons -->
        <div class="tool-item animate__animated animate__bounce">
          <div class="tool-icon">
            <img src="https://www.vectorlogo.zone/logos/gnu_bash/gnu_bash-icon.svg" alt="bash" width="40" height="40"/>
          </div>
          <div class="tool-name">Bash</div>
        </div>
        <div class="tool-item animate__animated animate__bounce" style="animation-delay: 0.1s">
          <div class="tool-icon">
            <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/cplusplus/cplusplus-original.svg" alt="cplusplus" width="40" height="40"/>
          </div>
          <div class="tool-name">C++</div>
        </div>
        <div class="tool-item animate__animated animate__bounce" style="animation-delay: 0.2s">
          <div class="tool-icon">
            <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="css3" width="40" height="40"/>
          </div>
          <div class="tool-name">CSS3</div>
        </div>
        <div class="tool-item animate__animated animate__bounce" style="animation-delay: 0.3s">
          <div class="tool-icon">
            <img src="https://www.vectorlogo.zone/logos/figma/figma-icon.svg" alt="figma" width="40" height="40"/>
          </div>
          <div class="tool-name">Figma</div>
        </div>
        <div class="tool-item animate__animated animate__bounce" style="animation-delay: 0.4s">
          <div class="tool-icon">
            <img src="https://www.vectorlogo.zone/logos/git-scm/git-scm-icon.svg" alt="git" width="40" height="40"/>
          </div>
          <div class="tool-name">Git</div>
        </div>
        <div class="tool-item animate__animated animate__bounce" style="animation-delay: 0.5s">
          <div class="tool-icon">
            <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="40" height="40"/>
          </div>
          <div class="tool-name">HTML5</div>
        </div>
        <div class="tool-item animate__animated animate__bounce" style="animation-delay: 0.6s">
          <div class="tool-icon">
            <img src="https://www.vectorlogo.zone/logos/adobe_illustrator/adobe_illustrator-icon.svg" alt="illustrator" width="40" height="40"/>
          </div>
          <div class="tool-name">Illustrator</div>
        </div>
        <div class="tool-item animate__animated animate__bounce" style="animation-delay: 0.7s">
          <div class="tool-icon">
            <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original.svg" alt="java" width="40" height="40"/>
          </div>
          <div class="tool-name">Java</div>
        </div>
        <div class="tool-item animate__animated animate__bounce" style="animation-delay: 0.8s">
          <div class="tool-icon">
            <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/linux/linux-original.svg" alt="linux" width="40" height="40"/>
          </div>
          <div class="tool-name">Linux</div>
        </div>
        <div class="tool-item animate__animated animate__bounce" style="animation-delay: 0.9s">
          <div class="tool-icon">
            <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg" alt="mysql" width="40" height="40"/>
          </div>
          <div class="tool-name">MySQL</div>
        </div>
        <div class="tool-item animate__animated animate__bounce" style="animation-delay: 1.0s">
          <div class="tool-icon">
            <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/photoshop/photoshop-line.svg" alt="photoshop" width="40" height="40"/>
          </div>
          <div class="tool-name">Photoshop</div>
        </div>
        <div class="tool-item animate__animated animate__bounce" style="animation-delay: 1.1s">
          <div class="tool-icon">
            <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/php/php-original.svg" alt="php" width="40" height="40"/>
          </div>
          <div class="tool-name">PHP</div>
        </div>
        <div class="tool-item animate__animated animate__bounce" style="animation-delay: 1.2s">
          <div class="tool-icon">
            <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/>
          </div>
          <div class="tool-name">Python</div>
        </div>
        <div class="tool-item animate__animated animate__bounce" style="animation-delay: 1.3s">
          <div class="tool-icon">
            <img src="https://upload.wikimedia.org/wikipedia/commons/e/e4/Cisco_CCNA_logo.svg" alt="ccna" width="40" height="40"/>
          </div>
          <div class="tool-name">CCNA</div>
        </div>
        
        <!-- Added Icons -->
        <div class="tool-item animate__animated animate__bounce" style="animation-delay: 1.4s">
          <div class="tool-icon">
            <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/c/c-original.svg" alt="c" width="40" height="40"/>
          </div>
          <div class="tool-name">C</div>
        </div>
        <div class="tool-item animate__animated animate__bounce" style="animation-delay: 1.5s">
          <div class="tool-icon">
            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/wireshark/wireshark-original.svg" alt="wireshark" width="40" height="40"/>
          </div>
          <div class="tool-name">Wireshark</div>
        </div>
        <div class="tool-item animate__animated animate__bounce" style="animation-delay: 1.6s">
          <div class="tool-icon floating">
            <img src="https://upload.wikimedia.org/wikipedia/commons/2/2b/Kali-dragon-icon.svg" alt="kali" width="40" height="40"/>
          </div>
          <div class="tool-name">Kali Linux</div>
        </div>
        <div class="tool-item animate__animated animate__bounce" style="animation-delay: 1.7s">
          <div class="tool-icon">
            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/bash/bash-original.svg" alt="bash scripting" width="40" height="40"/>
          </div>
          <div class="tool-name">Bash Script</div>
        </div>
      </div>
    </div>
    
    <div class="section">
      <h2 class="animate__animated animate__fadeInDown">📫 Connect with Me</h2>
      <div class="connect-links">
        <a href="mailto:mariamibrahim2355@gmail.com" class="connect-button animate__animated animate__fadeInUp">
          <i class="fas fa-envelope"></i> Email
        </a>
        <a href="https://www.linkedin.com/in/mariam-ibrahim-b95743307?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app" class="connect-button animate__animated animate__fadeInUp" style="animation-delay: 0.2s">
          <i class="fab fa-linkedin"></i> LinkedIn
        </a>
        <a href="https://github.com/mariomaibrahim" class="connect-button animate__animated animate__fadeInUp" style="animation-delay: 0.4s">
          <i class="fab fa-github"></i> GitHub
        </a>
      </div>
    </div>
    
    <div class="section">
      <h2 class="animate__animated animate__fadeInDown">📊 GitHub Stats</h2>
      <div class="stats-container">
        <div class="animate__animated animate__fadeInLeft">
          <img src="https://github-readme-stats.vercel.app/api?username=mariomaibrahim&show_icons=true&theme=radical" alt="My GitHub Stats" style="width: 100%; border-radius: 10px; box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);">
        </div>
        <div class="animate__animated animate__fadeInRight">
          <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=mariomaibrahim&layout=compact&theme=radical" alt="Top Langs" style="width: 100%; border-radius: 10px; box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);">
        </div>
      </div>
    </div>
    
    <div class="section" style="border-bottom: none;">
      <blockquote class="animate__animated animate__fadeIn">
        <p class="neon-text" style="text-align: center; font-size: 1.2em;">
          🛡️ "Digital forensics is not just about tools, it's about asking the right questions."
        </p>
      </blockquote>
      
      <div class="cyber-badge animate__animated animate__pulse animate__infinite" style="text-align: center; margin-top: 30px;">
        <i class="fas fa-shield-alt" style="margin-right: 10px;"></i>
        <span>Future Digital Forensic Analyst</span>
        <i class="fas fa-laptop-code" style="margin-left: 10px;"></i>
      </div>
    </div>
  </div>
</body>
</html>
