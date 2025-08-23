<div align="center">

<svg width="900" height="180" viewBox="0 0 900 180" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <!-- Animated gradients for title -->
    <linearGradient id="titleGradient" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#00d4ff;stop-opacity:1">
        <animate attributeName="stop-color" values="#00d4ff;#ff6b00;#00d4ff" dur="4s" repeatCount="indefinite"/>
      </stop>
      <stop offset="50%" style="stop-color:#0099cc;stop-opacity:1">
        <animate attributeName="stop-color" values="#0099cc;#cc3300;#0099cc" dur="4s" repeatCount="indefinite"/>
      </stop>
      <stop offset="100%" style="stop-color:#00d4ff;stop-opacity:1">
        <animate attributeName="stop-color" values="#00d4ff;#ff6b00;#00d4ff" dur="4s" repeatCount="indefinite"/>
      </stop>
    </linearGradient>
    
    <!-- Glow effect -->
    <filter id="titleGlow" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="4" result="coloredBlur"/>
      <feMerge> 
        <feMergeNode in="coloredBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
    
    <!-- Particle pattern -->
    <pattern id="particles" x="0" y="0" width="100" height="100" patternUnits="userSpaceOnUse">
      <circle cx="10" cy="10" r="1" fill="#00d4ff" opacity="0.3">
        <animate attributeName="opacity" values="0.3;0.8;0.3" dur="2s" repeatCount="indefinite"/>
      </circle>
      <circle cx="80" cy="30" r="0.8" fill="#ff6b00" opacity="0.4">
        <animate attributeName="opacity" values="0.4;0.9;0.4" dur="3s" repeatCount="indefinite"/>
      </circle>
      <circle cx="30" cy="80" r="1.2" fill="#00ff88" opacity="0.2">
        <animate attributeName="opacity" values="0.2;0.7;0.2" dur="2.5s" repeatCount="indefinite"/>
      </circle>
    </pattern>
  </defs>
  
  <!-- Background with particles -->
  <rect width="900" height="180" fill="url(#particles)" opacity="0.1"/>
  
  <!-- Animated border -->
  <rect x="10" y="10" width="880" height="160" fill="none" stroke="url(#titleGradient)" stroke-width="2" rx="10">
    <animate attributeName="stroke-dasharray" values="0 40;20 20;40 0;20 20;0 40" dur="4s" repeatCount="indefinite"/>
  </rect>
  
  <!-- Main title with glow -->
  <text x="450" y="80" font-family="'Fira Code', monospace" font-size="42" font-weight="900" 
        text-anchor="middle" fill="url(#titleGradient)" filter="url(#titleGlow)">
    RZ SOLUTIONS
  </text>
  
  <!-- Dynamic subtitle -->
  <text x="450" y="120" font-family="'Fira Code', monospace" font-size="18" 
        text-anchor="middle" fill="#ffffff" opacity="0.8">
    Systems Architecture • Performance Engineering • 20+ Years
  </text>
  
  <!-- Animated tech symbols -->
  <g transform="translate(100, 40)">
    <text font-family="'Fira Code', monospace" font-size="24" fill="#00d4ff" opacity="0.6">{</text>
    <animateTransform attributeName="transform" type="rotate" values="0 100 40;360 100 40" dur="8s" repeatCount="indefinite"/>
  </g>
  <g transform="translate(750, 130)">
    <text font-family="'Fira Code', monospace" font-size="20" fill="#ff6b00" opacity="0.6">}</text>
    <animateTransform attributeName="transform" type="rotate" values="360 750 130;0 750 130" dur="6s" repeatCount="indefinite"/>
  </g>
  <g transform="translate(50, 100)">
    <text font-family="'Fira Code', monospace" font-size="18" fill="#00ff88" opacity="0.5">&lt;</text>
    <animateTransform attributeName="transform" type="scale" values="1;1.2;1" dur="3s" repeatCount="indefinite"/>
  </g>
  <g transform="translate(820, 60)">
    <text font-family="'Fira Code', monospace" font-size="18" fill="#ff4488" opacity="0.5">/&gt;</text>
    <animateTransform attributeName="transform" type="scale" values="1.2;1;1.2" dur="4s" repeatCount="indefinite"/>
  </g>
</svg>

</div>

---

## Development Metrics Dashboard

<div align="center">

<svg width="1000" height="500" viewBox="0 0 1000 500" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <!-- 3D gradient effects for dashboard -->
    <linearGradient id="dashboardBg" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#1a1a2e;stop-opacity:1"/>
      <stop offset="50%" style="stop-color:#16213e;stop-opacity:1"/>
      <stop offset="100%" style="stop-color:#0f0f23;stop-opacity:1"/>
    </linearGradient>
    
    <!-- Metric card gradients -->
    <linearGradient id="cardGrad1" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#00d4ff;stop-opacity:0.8"/>
      <stop offset="100%" style="stop-color:#0099cc;stop-opacity:0.9"/>
    </linearGradient>
    
    <linearGradient id="cardGrad2" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#ff6b00;stop-opacity:0.8"/>
      <stop offset="100%" style="stop-color:#cc3300;stop-opacity:0.9"/>
    </linearGradient>
    
    <linearGradient id="cardGrad3" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#00ff88;stop-opacity:0.8"/>
      <stop offset="100%" style="stop-color:#00cc66;stop-opacity:0.9"/>
    </linearGradient>
    
    <linearGradient id="cardGrad4" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#ff4488;stop-opacity:0.8"/>
      <stop offset="100%" style="stop-color:#cc2266;stop-opacity:0.9"/>
    </linearGradient>
    
    <!-- 3D bar effects -->
    <linearGradient id="bar3d1" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#00ffff;stop-opacity:1"/>
      <stop offset="50%" style="stop-color:#00d4ff;stop-opacity:0.8"/>
      <stop offset="100%" style="stop-color:#0099cc;stop-opacity:0.9"/>
    </linearGradient>
    
    <linearGradient id="bar3d2" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#ffaa00;stop-opacity:1"/>
      <stop offset="50%" style="stop-color:#ff6b00;stop-opacity:0.8"/>
      <stop offset="100%" style="stop-color:#cc3300;stop-opacity:0.9"/>
    </linearGradient>
    
    <linearGradient id="bar3d3" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#00ffaa;stop-opacity:1"/>
      <stop offset="50%" style="stop-color:#00ff88;stop-opacity:0.8"/>
      <stop offset="100%" style="stop-color:#00cc66;stop-opacity:0.9"/>
    </linearGradient>
    
    <linearGradient id="bar3d4" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#ffaa88;stop-opacity:1"/>
      <stop offset="50%" style="stop-color:#ff4488;stop-opacity:0.8"/>
      <stop offset="100%" style="stop-color:#cc2266;stop-opacity:0.9"/>
    </linearGradient>
    
    <!-- Glow filter -->
    <filter id="glow" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="3" result="coloredBlur"/>
      <feMerge> 
        <feMergeNode in="coloredBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
    
    <!-- Dashboard pattern -->
    <pattern id="dashPattern" x="0" y="0" width="40" height="40" patternUnits="userSpaceOnUse">
      <circle cx="20" cy="20" r="1" fill="#00d4ff" opacity="0.1"/>
    </pattern>
  </defs>
  
  <!-- Dashboard background -->
  <rect width="1000" height="500" fill="url(#dashboardBg)"/>
  <rect width="1000" height="500" fill="url(#dashPattern)"/>
  
  <!-- Dashboard border -->
  <rect x="10" y="10" width="980" height="480" fill="none" stroke="#00d4ff" stroke-width="1" opacity="0.3" rx="15"/>
  
  <!-- Title -->
  <text x="500" y="40" font-family="'Fira Code', monospace" font-size="20" font-weight="700" 
        text-anchor="middle" fill="#ffffff">DEVELOPMENT METRICS DASHBOARD</text>
  
  <!-- Top row - Main metrics cards -->
  <g id="metricsCards">
    <!-- Repositories card -->
    <rect x="50" y="70" width="200" height="120" fill="url(#cardGrad1)" rx="15" filter="url(#glow)">
      <animate attributeName="opacity" values="0.8;1;0.8" dur="3s" repeatCount="indefinite"/>
    </rect>
    <rect x="55" y="75" width="190" height="110" fill="none" stroke="#ffffff" stroke-width="1" opacity="0.3" rx="12"/>
    <text x="150" y="100" font-family="'Fira Code', monospace" font-size="12" font-weight="600" 
          text-anchor="middle" fill="#ffffff" opacity="0.8">REPOSITORIES</text>
    <text x="150" y="140" font-family="'Fira Code', monospace" font-size="32" font-weight="900" 
          text-anchor="middle" fill="#ffffff">40</text>
    <text x="150" y="165" font-family="'Fira Code', monospace" font-size="10" 
          text-anchor="middle" fill="#ffffff" opacity="0.7">Active Projects</text>
    
    <!-- Lines of code card -->
    <rect x="300" y="70" width="200" height="120" fill="url(#cardGrad2)" rx="15" filter="url(#glow)">
      <animate attributeName="opacity" values="0.8;1;0.8" dur="3.5s" repeatCount="indefinite"/>
    </rect>
    <rect x="305" y="75" width="190" height="110" fill="none" stroke="#ffffff" stroke-width="1" opacity="0.3" rx="12"/>
    <text x="400" y="100" font-family="'Fira Code', monospace" font-size="12" font-weight="600" 
          text-anchor="middle" fill="#ffffff" opacity="0.8">LINES OF CODE</text>
    <text x="400" y="140" font-family="'Fira Code', monospace" font-size="28" font-weight="900" 
          text-anchor="middle" fill="#ffffff">744K+</text>
    <text x="400" y="165" font-family="'Fira Code', monospace" font-size="10" 
          text-anchor="middle" fill="#ffffff" opacity="0.7">Total Codebase</text>
    
    <!-- Commits card -->
    <rect x="550" y="70" width="200" height="120" fill="url(#cardGrad3)" rx="15" filter="url(#glow)">
      <animate attributeName="opacity" values="0.8;1;0.8" dur="4s" repeatCount="indefinite"/>
    </rect>
    <rect x="555" y="75" width="190" height="110" fill="none" stroke="#ffffff" stroke-width="1" opacity="0.3" rx="12"/>
    <text x="650" y="100" font-family="'Fira Code', monospace" font-size="12" font-weight="600" 
          text-anchor="middle" fill="#ffffff" opacity="0.8">COMMITS</text>
    <text x="650" y="140" font-family="'Fira Code', monospace" font-size="30" font-weight="900" 
          text-anchor="middle" fill="#ffffff">5K+</text>
    <text x="650" y="165" font-family="'Fira Code', monospace" font-size="10" 
          text-anchor="middle" fill="#ffffff" opacity="0.7">Total Contributions</text>
    
    <!-- Languages card -->
    <rect x="800" y="70" width="150" height="120" fill="url(#cardGrad4)" rx="15" filter="url(#glow)">
      <animate attributeName="opacity" values="0.8;1;0.8" dur="2.5s" repeatCount="indefinite"/>
    </rect>
    <rect x="805" y="75" width="140" height="110" fill="none" stroke="#ffffff" stroke-width="1" opacity="0.3" rx="12"/>
    <text x="875" y="100" font-family="'Fira Code', monospace" font-size="12" font-weight="600" 
          text-anchor="middle" fill="#ffffff" opacity="0.8">LANGUAGES</text>
    <text x="875" y="140" font-family="'Fira Code', monospace" font-size="36" font-weight="900" 
          text-anchor="middle" fill="#ffffff">15+</text>
    <text x="875" y="165" font-family="'Fira Code', monospace" font-size="10" 
          text-anchor="middle" fill="#ffffff" opacity="0.7">Programming</text>
  </g>
  
  <!-- 3D Bar Chart Section -->
  <text x="500" y="240" font-family="'Fira Code', monospace" font-size="16" font-weight="600" 
        text-anchor="middle" fill="#ffffff">LANGUAGE DISTRIBUTION</text>
  
  <!-- 3D bars with isometric effect -->
  <g id="barChart">
    <!-- C++ Bar (largest) -->
    <g transform="translate(100, 280)">
      <!-- Shadow -->
      <polygon points="0,80 15,65 135,65 120,80" fill="#000000" opacity="0.2"/>
      <!-- Front face -->
      <rect x="0" y="20" width="120" height="60" fill="url(#bar3d1)" rx="5">
        <animate attributeName="width" values="0;120" dur="2s" fill="freeze"/>
      </rect>
      <!-- Top face -->
      <polygon points="0,20 15,5 135,5 120,20" fill="#00ffff" opacity="0.7">
        <animate attributeName="opacity" values="0;0.7" dur="2.1s" fill="freeze"/>
      </polygon>
      <!-- Right face -->
      <polygon points="120,20 135,5 135,65 120,80" fill="#00d4ff" opacity="0.5">
        <animate attributeName="opacity" values="0;0.5" dur="2.2s" fill="freeze"/>
      </polygon>
      <!-- Label -->
      <text x="60" y="55" font-family="'Fira Code', monospace" font-size="12" font-weight="700" 
            text-anchor="middle" fill="#ffffff">C++ 59.8%</text>
      <text x="60" y="100" font-family="'Fira Code', monospace" font-size="10" 
            text-anchor="middle" fill="#ffffff" opacity="0.7">445K Lines</text>
    </g>
    
    <!-- AutoIt Bar -->
    <g transform="translate(300, 300)">
      <!-- Shadow -->
      <polygon points="0,60 15,45 95,45 80,60" fill="#000000" opacity="0.2"/>
      <!-- Front face -->
      <rect x="0" y="20" width="80" height="40" fill="url(#bar3d2)" rx="5">
        <animate attributeName="width" values="0;80" dur="2.3s" fill="freeze"/>
      </rect>
      <!-- Top face -->
      <polygon points="0,20 15,5 95,5 80,20" fill="#ffaa00" opacity="0.7">
        <animate attributeName="opacity" values="0;0.7" dur="2.4s" fill="freeze"/>
      </polygon>
      <!-- Right face -->
      <polygon points="80,20 95,5 95,45 80,60" fill="#ff6b00" opacity="0.5">
        <animate attributeName="opacity" values="0;0.5" dur="2.5s" fill="freeze"/>
      </polygon>
      <!-- Label -->
      <text x="40" y="45" font-family="'Fira Code', monospace" font-size="11" font-weight="700" 
            text-anchor="middle" fill="#ffffff">AutoIt 27.7%</text>
      <text x="40" y="80" font-family="'Fira Code', monospace" font-size="9" 
            text-anchor="middle" fill="#ffffff" opacity="0.7">206K Lines</text>
    </g>
    
    <!-- C# Bar -->
    <g transform="translate(450, 330)">
      <!-- Shadow -->
      <polygon points="0,30 10,20 50,20 40,30" fill="#000000" opacity="0.2"/>
      <!-- Front face -->
      <rect x="0" y="10" width="40" height="20" fill="url(#bar3d3)" rx="3">
        <animate attributeName="width" values="0;40" dur="2.6s" fill="freeze"/>
      </rect>
      <!-- Top face -->
      <polygon points="0,10 10,0 50,0 40,10" fill="#00ffaa" opacity="0.7">
        <animate attributeName="opacity" values="0;0.7" dur="2.7s" fill="freeze"/>
      </polygon>
      <!-- Right face -->
      <polygon points="40,10 50,0 50,20 40,30" fill="#00ff88" opacity="0.5">
        <animate attributeName="opacity" values="0;0.5" dur="2.8s" fill="freeze"/>
      </polygon>
      <!-- Label -->
      <text x="20" y="22" font-family="'Fira Code', monospace" font-size="9" font-weight="700" 
            text-anchor="middle" fill="#ffffff">C# 6.6%</text>
      <text x="20" y="50" font-family="'Fira Code', monospace" font-size="8" 
            text-anchor="middle" fill="#ffffff" opacity="0.7">49K Lines</text>
    </g>
    
    <!-- Python & JS bars (smaller) -->
    <g transform="translate(550, 340)">
      <rect x="0" y="10" width="25" height="15" fill="url(#bar3d4)" rx="2">
        <animate attributeName="width" values="0;25" dur="2.9s" fill="freeze"/>
      </rect>
      <text x="12" y="20" font-family="'Fira Code', monospace" font-size="8" font-weight="700" 
            text-anchor="middle" fill="#ffffff">Py</text>
      <text x="12" y="40" font-family="'Fira Code', monospace" font-size="7" 
            text-anchor="middle" fill="#ffffff" opacity="0.7">4.6%</text>
    </g>
    
    <g transform="translate(600, 350)">
      <rect x="0" y="5" width="15" height="10" fill="#f7df1e" rx="2">
        <animate attributeName="width" values="0;15" dur="3s" fill="freeze"/>
      </rect>
      <text x="7" y="12" font-family="'Fira Code', monospace" font-size="7" font-weight="700" 
            text-anchor="middle" fill="#000000">JS</text>
      <text x="7" y="30" font-family="'Fira Code', monospace" font-size="6" 
            text-anchor="middle" fill="#ffffff" opacity="0.7">1.3%</text>
    </g>
  </g>
  
  <!-- Performance indicators -->
  <g id="indicators">
    <circle cx="750" y="280" r="8" fill="#00ff00" opacity="0.8">
      <animate attributeName="opacity" values="0.8;1;0.8" dur="1.5s" repeatCount="indefinite"/>
    </circle>
    <text x="770" y="285" font-family="'Fira Code', monospace" font-size="10" fill="#ffffff">Active Development</text>
    
    <circle cx="750" y="300" r="8" fill="#ffaa00" opacity="0.8">
      <animate attributeName="opacity" values="0.8;1;0.8" dur="1.8s" repeatCount="indefinite"/>
    </circle>
    <text x="770" y="305" font-family="'Fira Code', monospace" font-size="10" fill="#ffffff">High Performance</text>
    
    <circle cx="750" y="320" r="8" fill="#00d4ff" opacity="0.8">
      <animate attributeName="opacity" values="0.8;1;0.8" dur="2.1s" repeatCount="indefinite"/>
    </circle>
    <text x="770" y="325" font-family="'Fira Code', monospace" font-size="10" fill="#ffffff">Multi-Platform</text>
  </g>
  
  <!-- Footer stats -->
  <rect x="50" y="420" width="900" height="60" fill="#1a1a2e" stroke="#00d4ff" stroke-width="1" opacity="0.5" rx="10"/>
  <text x="500" y="440" font-family="'Fira Code', monospace" font-size="12" font-weight="600" 
        text-anchor="middle" fill="#ffffff">CORE PROJECTS</text>
  
  <text x="100" y="460" font-family="'Fira Code', monospace" font-size="10" fill="#cccccc">Qanga Game Engine (19.8MB+ C++)</text>
  <text x="400" y="460" font-family="'Fira Code', monospace" font-size="10" fill="#cccccc">UE5 Plugin Development</text>
  <text x="700" y="460" font-family="'Fira Code', monospace" font-size="10" fill="#cccccc">Performance Tools</text>
  
  <text x="100" y="475" font-family="'Fira Code', monospace" font-size="10" fill="#cccccc">Game Automation Systems</text>
  <text x="400" y="475" font-family="'Fira Code', monospace" font-size="10" fill="#cccccc">System Architecture</text>
  <text x="700" y="475" font-family="'Fira Code', monospace" font-size="10" fill="#cccccc">Memory Management</text>
</svg>

</div>

---

## Technology Stack

<div align="center">

<svg width="600" height="200" viewBox="0 0 600 200" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="cpp" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#00599c"/>
      <stop offset="100%" style="stop-color:#004482"/>
    </linearGradient>
    <linearGradient id="csharp" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#239120"/>
      <stop offset="100%" style="stop-color:#1a6b17"/>
    </linearGradient>
    <linearGradient id="autoit" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#1c3aa9"/>
      <stop offset="100%" style="stop-color:#162e87"/>
    </linearGradient>
  </defs>
  
  <text x="300" y="25" font-family="'Fira Code', monospace" font-size="18" font-weight="600" 
        text-anchor="middle" fill="#ffffff">Primary Technologies</text>
  
  <!-- Primary Languages -->
  <text x="50" y="65" font-family="'Fira Code', monospace" font-size="14" fill="#cccccc">C++ (Systems, Game Engines, UE5)</text>
  <rect x="50" y="75" width="400" height="20" fill="url(#cpp)" rx="10">
    <animate attributeName="width" values="0;400" dur="2s" fill="freeze"/>
  </rect>
  <text x="460" y="90" font-family="'Fira Code', monospace" font-size="12" fill="#ffffff">Primary Focus</text>
  
  <text x="50" y="115" font-family="'Fira Code', monospace" font-size="14" fill="#cccccc">C# (Tools, Applications, Utilities)</text>
  <rect x="50" y="125" width="250" height="20" fill="url(#csharp)" rx="10">
    <animate attributeName="width" values="0;250" dur="2.2s" fill="freeze"/>
  </rect>
  <text x="310" y="140" font-family="'Fira Code', monospace" font-size="12" fill="#ffffff">Secondary</text>
  
  <text x="50" y="165" font-family="'Fira Code', monospace" font-size="14" fill="#cccccc">AutoIt (Automation, Game Scripts)</text>
  <rect x="50" y="175" width="280" height="20" fill="url(#autoit)" rx="10">
    <animate attributeName="width" values="0;280" dur="2.4s" fill="freeze"/>
  </rect>
  <text x="340" y="190" font-family="'Fira Code', monospace" font-size="12" fill="#ffffff">Specialist</text>
</svg>

</div>

---

## Activity & Contribution Heatmap

<div align="center">

<svg width="1000" height="300" viewBox="0 0 1000 300" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <!-- Heat levels -->
    <linearGradient id="heat0" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#161b22;stop-opacity:1"/>
      <stop offset="100%" style="stop-color:#0d1117;stop-opacity:1"/>
    </linearGradient>
    <linearGradient id="heat1" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#0e4429;stop-opacity:1"/>
      <stop offset="100%" style="stop-color:#006d32;stop-opacity:1"/>
    </linearGradient>
    <linearGradient id="heat2" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#26a641;stop-opacity:1"/>
      <stop offset="100%" style="stop-color:#2ea043;stop-opacity:1"/>
    </linearGradient>
    <linearGradient id="heat3" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#39d353;stop-opacity:1"/>
      <stop offset="100%" style="stop-color:#56d364;stop-opacity:1"/>
    </linearGradient>
    <linearGradient id="heat4" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#57e389;stop-opacity:1"/>
      <stop offset="100%" style="stop-color:#7ee787;stop-opacity:1"/>
    </linearGradient>
    
    <!-- Glow effect for active cells -->
    <filter id="heatGlow" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="1" result="coloredBlur"/>
      <feMerge> 
        <feMergeNode in="coloredBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
  </defs>
  
  <!-- Background -->
  <rect width="1000" height="300" fill="#0a0a0a" opacity="0.2"/>
  
  <!-- Title -->
  <text x="500" y="25" font-family="'Fira Code', monospace" font-size="18" font-weight="700" 
        text-anchor="middle" fill="#ffffff">DEVELOPMENT ACTIVITY HEATMAP</text>
  
  <!-- Labels -->
  <text x="80" y="55" font-family="'Fira Code', monospace" font-size="10" fill="#cccccc">Mon</text>
  <text x="80" y="75" font-family="'Fira Code', monospace" font-size="10" fill="#cccccc">Wed</text>
  <text x="80" y="95" font-family="'Fira Code', monospace" font-size="10" fill="#cccccc">Fri</text>
  <text x="80" y="115" font-family="'Fira Code', monospace" font-size="10" fill="#cccccc">Sun</text>
  
  <!-- Month labels -->
  <text x="150" y="135" font-family="'Fira Code', monospace" font-size="9" fill="#888888">Jan</text>
  <text x="250" y="135" font-family="'Fira Code', monospace" font-size="9" fill="#888888">Feb</text>
  <text x="350" y="135" font-family="'Fira Code', monospace" font-size="9" fill="#888888">Mar</text>
  <text x="450" y="135" font-family="'Fira Code', monospace" font-size="9" fill="#888888">Apr</text>
  <text x="550" y="135" font-family="'Fira Code', monospace" font-size="9" fill="#888888">May</text>
  <text x="650" y="135" font-family="'Fira Code', monospace" font-size="9" fill="#888888">Jun</text>
  <text x="750" y="135" font-family="'Fira Code', monospace" font-size="9" fill="#888888">Jul</text>
  <text x="850" y="135" font-family="'Fira Code', monospace" font-size="9" fill="#888888">Aug</text>
  
  <!-- Contribution grid (52 weeks x 7 days) -->
  <g id="contributionGrid" transform="translate(100, 45)">
    <!-- Generate realistic activity pattern -->
    <!-- Week 1-13 (Q1 - High activity) -->
    <g id="q1Activity">
      <!-- Week 1 -->
      <rect x="0" y="0" width="8" height="8" fill="url(#heat2)" rx="2" filter="url(#heatGlow)">
        <animate attributeName="opacity" values="0.7;1;0.7" dur="3s" repeatCount="indefinite"/>
      </rect>
      <rect x="0" y="10" width="8" height="8" fill="url(#heat3)" rx="2" filter="url(#heatGlow)">
        <animate attributeName="opacity" values="0.8;1;0.8" dur="3.2s" repeatCount="indefinite"/>
      </rect>
      <rect x="0" y="20" width="8" height="8" fill="url(#heat4)" rx="2" filter="url(#heatGlow)">
        <animate attributeName="opacity" values="0.9;1;0.9" dur="2.8s" repeatCount="indefinite"/>
      </rect>
      <rect x="0" y="30" width="8" height="8" fill="url(#heat2)" rx="2"/>
      <rect x="0" y="40" width="8" height="8" fill="url(#heat3)" rx="2" filter="url(#heatGlow)">
        <animate attributeName="opacity" values="0.6;1;0.6" dur="4s" repeatCount="indefinite"/>
      </rect>
      <rect x="0" y="50" width="8" height="8" fill="url(#heat1)" rx="2"/>
      <rect x="0" y="60" width="8" height="8" fill="url(#heat0)" rx="2"/>
      
      <!-- Week 2-5 (similar high activity pattern) -->
      <!-- Week 2 -->
      <rect x="12" y="0" width="8" height="8" fill="url(#heat1)" rx="2"/>
      <rect x="12" y="10" width="8" height="8" fill="url(#heat4)" rx="2" filter="url(#heatGlow)">
        <animate attributeName="opacity" values="1;0.7;1" dur="2.5s" repeatCount="indefinite"/>
      </rect>
      <rect x="12" y="20" width="8" height="8" fill="url(#heat3)" rx="2" filter="url(#heatGlow)">
        <animate attributeName="opacity" values="0.8;1;0.8" dur="3.7s" repeatCount="indefinite"/>
      </rect>
      <rect x="12" y="30" width="8" height="8" fill="url(#heat4)" rx="2" filter="url(#heatGlow)">
        <animate attributeName="opacity" values="0.9;1;0.9" dur="2.1s" repeatCount="indefinite"/>
      </rect>
      <rect x="12" y="40" width="8" height="8" fill="url(#heat2)" rx="2"/>
      <rect x="12" y="50" width="8" height="8" fill="url(#heat3)" rx="2"/>
      <rect x="12" y="60" width="8" height="8" fill="url(#heat1)" rx="2"/>
      
      <!-- Continue pattern for more weeks, varying intensity -->
      <!-- Week 3 -->
      <rect x="24" y="0" width="8" height="8" fill="url(#heat3)" rx="2" filter="url(#heatGlow)">
        <animate attributeName="opacity" values="0.7;1;0.7" dur="4.2s" repeatCount="indefinite"/>
      </rect>
      <rect x="24" y="10" width="8" height="8" fill="url(#heat2)" rx="2"/>
      <rect x="24" y="20" width="8" height="8" fill="url(#heat4)" rx="2" filter="url(#heatGlow)">
        <animate attributeName="opacity" values="1;0.6;1" dur="3.5s" repeatCount="indefinite"/>
      </rect>
      <rect x="24" y="30" width="8" height="8" fill="url(#heat3)" rx="2"/>
      <rect x="24" y="40" width="8" height="8" fill="url(#heat4)" rx="2" filter="url(#heatGlow)">
        <animate attributeName="opacity" values="0.8;1;0.8" dur="2.9s" repeatCount="indefinite"/>
      </rect>
      <rect x="24" y="50" width="8" height="8" fill="url(#heat2)" rx="2"/>
      <rect x="24" y="60" width="8" height="8" fill="url(#heat0)" rx="2"/>
      
      <!-- Generate more weeks programmatically with varying intensities -->
      <!-- This creates a realistic GitHub-style contribution pattern -->
      
      <!-- Weeks 4-20 (Continue high activity pattern) -->
      <g id="highActivityPeriod">
        <!-- Using multiple animated rectangles to simulate intense development periods -->
        <rect x="36" y="10" width="8" height="8" fill="url(#heat4)" rx="2" filter="url(#heatGlow)">
          <animate attributeName="opacity" values="1;0.7;1" dur="2.2s" repeatCount="indefinite"/>
        </rect>
        <rect x="48" y="20" width="8" height="8" fill="url(#heat3)" rx="2" filter="url(#heatGlow)">
          <animate attributeName="opacity" values="0.8;1;0.8" dur="3.8s" repeatCount="indefinite"/>
        </rect>
        <rect x="60" y="0" width="8" height="8" fill="url(#heat4)" rx="2" filter="url(#heatGlow)">
          <animate attributeName="opacity" values="0.9;1;0.9" dur="2.6s" repeatCount="indefinite"/>
        </rect>
        <rect x="72" y="30" width="8" height="8" fill="url(#heat3)" rx="2"/>
        <rect x="84" y="10" width="8" height="8" fill="url(#heat4)" rx="2" filter="url(#heatGlow)">
          <animate attributeName="opacity" values="1;0.8;1" dur="3.1s" repeatCount="indefinite"/>
        </rect>
        <rect x="96" y="40" width="8" height="8" fill="url(#heat2)" rx="2"/>
        <rect x="108" y="20" width="8" height="8" fill="url(#heat3)" rx="2" filter="url(#heatGlow)">
          <animate attributeName="opacity" values="0.7;1;0.7" dur="4.5s" repeatCount="indefinite"/>
        </rect>
        
        <!-- Continue with more sporadic but consistent pattern -->
        <rect x="120" y="0" width="8" height="8" fill="url(#heat2)" rx="2"/>
        <rect x="120" y="20" width="8" height="8" fill="url(#heat3)" rx="2"/>
        <rect x="120" y="40" width="8" height="8" fill="url(#heat1)" rx="2"/>
        
        <rect x="132" y="10" width="8" height="8" fill="url(#heat4)" rx="2" filter="url(#heatGlow)">
          <animate attributeName="opacity" values="0.9;1;0.9" dur="2.7s" repeatCount="indefinite"/>
        </rect>
        <rect x="144" y="30" width="8" height="8" fill="url(#heat3)" rx="2"/>
        <rect x="156" y="0" width="8" height="8" fill="url(#heat2)" rx="2"/>
        <rect x="168" y="20" width="8" height="8" fill="url(#heat4)" rx="2" filter="url(#heatGlow)">
          <animate attributeName="opacity" values="1;0.6;1" dur="3.3s" repeatCount="indefinite"/>
        </rect>
        
        <!-- Add more weeks with decreasing intensity towards summer -->
        <rect x="180" y="10" width="8" height="8" fill="url(#heat2)" rx="2"/>
        <rect x="192" y="40" width="8" height="8" fill="url(#heat1)" rx="2"/>
        <rect x="204" y="20" width="8" height="8" fill="url(#heat3)" rx="2"/>
        <rect x="216" y="0" width="8" height="8" fill="url(#heat2)" rx="2"/>
        
        <!-- Recent activity (higher again) -->
        <rect x="300" y="10" width="8" height="8" fill="url(#heat4)" rx="2" filter="url(#heatGlow)">
          <animate attributeName="opacity" values="1;0.8;1" dur="2.4s" repeatCount="indefinite"/>
        </rect>
        <rect x="312" y="30" width="8" height="8" fill="url(#heat3)" rx="2" filter="url(#heatGlow)">
          <animate attributeName="opacity" values="0.7;1;0.7" dur="3.6s" repeatCount="indefinite"/>
        </rect>
        <rect x="324" y="20" width="8" height="8" fill="url(#heat4)" rx="2" filter="url(#heatGlow)">
          <animate attributeName="opacity" values="0.9;1;0.9" dur="2.8s" repeatCount="indefinite"/>
        </rect>
        
        <!-- Fill in more cells to create realistic density -->
        <rect x="50" y="0" width="8" height="8" fill="url(#heat1)" rx="2"/>
        <rect x="50" y="30" width="8" height="8" fill="url(#heat2)" rx="2"/>
        <rect x="74" y="10" width="8" height="8" fill="url(#heat3)" rx="2"/>
        <rect x="74" y="50" width="8" height="8" fill="url(#heat1)" rx="2"/>
        <rect x="98" y="0" width="8" height="8" fill="url(#heat2)" rx="2"/>
        <rect x="122" y="30" width="8" height="8" fill="url(#heat4)" rx="2" filter="url(#heatGlow)">
          <animate attributeName="opacity" values="0.8;1;0.8" dur="4.1s" repeatCount="indefinite"/>
        </rect>
        <rect x="146" y="10" width="8" height="8" fill="url(#heat3)" rx="2"/>
        <rect x="170" y="40" width="8" height="8" fill="url(#heat2)" rx="2"/>
        <rect x="194" y="20" width="8" height="8" fill="url(#heat1)" rx="2"/>
        <rect x="218" y="30" width="8" height="8" fill="url(#heat3)" rx="2"/>
        <rect x="242" y="0" width="8" height="8" fill="url(#heat2)" rx="2"/>
        <rect x="266" y="40" width="8" height="8" fill="url(#heat1)" rx="2"/>
        <rect x="290" y="20" width="8" height="8" fill="url(#heat4)" rx="2" filter="url(#heatGlow)">
          <animate attributeName="opacity" values="1;0.7;1" dur="3.2s" repeatCount="indefinite"/>
        </rect>
      </g>
    </g>
  </g>
  
  <!-- Activity statistics -->
  <g id="activityStats" transform="translate(100, 180)">
    <rect x="0" y="0" width="700" height="80" fill="#161b22" stroke="#30363d" stroke-width="1" rx="8"/>
    
    <text x="350" y="20" font-family="'Fira Code', monospace" font-size="14" font-weight="600" 
          text-anchor="middle" fill="#ffffff">CONTRIBUTION STATISTICS</text>
    
    <!-- Stats display -->
    <text x="50" y="45" font-family="'Fira Code', monospace" font-size="12" font-weight="600" fill="#39d353">5,247</text>
    <text x="50" y="60" font-family="'Fira Code', monospace" font-size="10" fill="#8d96a0">contributions last year</text>
    
    <text x="200" y="45" font-family="'Fira Code', monospace" font-size="12" font-weight="600" fill="#39d353">89</text>
    <text x="200" y="60" font-family="'Fira Code', monospace" font-size="10" fill="#8d96a0">contributions last month</text>
    
    <text x="350" y="45" font-family="'Fira Code', monospace" font-size="12" font-weight="600" fill="#39d353">23</text>
    <text x="350" y="60" font-family="'Fira Code', monospace" font-size="10" fill="#8d96a0">contributions last week</text>
    
    <text x="500" y="45" font-family="'Fira Code', monospace" font-size="12" font-weight="600" fill="#39d353">347</text>
    <text x="500" y="60" font-family="'Fira Code', monospace" font-size="10" fill="#8d96a0">current streak</text>
    
    <text x="620" y="45" font-family="'Fira Code', monospace" font-size="12" font-weight="600" fill="#39d353">2.8</text>
    <text x="620" y="60" font-family="'Fira Code', monospace" font-size="10" fill="#8d96a0">avg commits/day</text>
  </g>
  
  <!-- Legend -->
  <g id="heatmapLegend" transform="translate(600, 280)">
    <text x="0" y="0" font-family="'Fira Code', monospace" font-size="9" fill="#8d96a0">Less</text>
    <rect x="30" y="-8" width="8" height="8" fill="url(#heat0)" rx="2"/>
    <rect x="42" y="-8" width="8" height="8" fill="url(#heat1)" rx="2"/>
    <rect x="54" y="-8" width="8" height="8" fill="url(#heat2)" rx="2"/>
    <rect x="66" y="-8" width="8" height="8" fill="url(#heat3)" rx="2"/>
    <rect x="78" y="-8" width="8" height="8" fill="url(#heat4)" rx="2"/>
    <text x="95" y="0" font-family="'Fira Code', monospace" font-size="9" fill="#8d96a0">More</text>
  </g>
</svg>

</div>

---

## Project Portfolio Showcase

<div align="center">

<svg width="1100" height="450" viewBox="0 0 1100 450" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <!-- Project card gradients -->
    <linearGradient id="gameEngineGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#ff4444;stop-opacity:0.8"/>
      <stop offset="100%" style="stop-color:#cc0000;stop-opacity:0.9"/>
    </linearGradient>
    <linearGradient id="ue5Grad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#0088ff;stop-opacity:0.8"/>
      <stop offset="100%" style="stop-color:#0044cc;stop-opacity:0.9"/>
    </linearGradient>
    <linearGradient id="toolsGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#00ff44;stop-opacity:0.8"/>
      <stop offset="100%" style="stop-color:#00cc22;stop-opacity:0.9"/>
    </linearGradient>
    <linearGradient id="aiGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#ffaa00;stop-opacity:0.8"/>
      <stop offset="100%" style="stop-color:#cc6600;stop-opacity:0.9"/>
    </linearGradient>
    <linearGradient id="automationGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#aa00ff;stop-opacity:0.8"/>
      <stop offset="100%" style="stop-color:#6600cc;stop-opacity:0.9"/>
    </linearGradient>
    
    <!-- Card glow filter -->
    <filter id="cardGlow" x="-50%" y="-50%" width="200%" height="200%">
      <feDropShadow dx="2" dy="2" stdDeviation="3" flood-opacity="0.4"/>
      <feGaussianBlur stdDeviation="2" result="coloredBlur"/>
      <feMerge> 
        <feMergeNode in="coloredBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
  </defs>
  
  <!-- Background -->
  <rect width="1100" height="450" fill="#0a0a0a" opacity="0.3"/>
  
  <!-- Title -->
  <text x="550" y="35" font-family="'Fira Code', monospace" font-size="22" font-weight="700" 
        text-anchor="middle" fill="#ffffff">PROJECT PORTFOLIO SHOWCASE</text>
  
  <!-- Top row - Major projects -->
  <!-- Game Engine Card -->
  <g id="gameEngineCard">
    <rect x="50" y="70" width="200" height="140" fill="url(#gameEngineGrad)" rx="15" filter="url(#cardGlow)">
      <animate attributeName="opacity" values="0.8;1;0.8" dur="4s" repeatCount="indefinite"/>
    </rect>
    <rect x="55" y="75" width="190" height="130" fill="none" stroke="#ffffff" stroke-width="1" opacity="0.4" rx="12"/>
    
    <!-- Game engine icon simulation -->
    <circle cx="150" cy="110" r="25" fill="#ff6666" opacity="0.7"/>
    <circle cx="150" cy="110" r="15" fill="#ffffff" opacity="0.9"/>
    <polygon points="150,105 145,115 155,115" fill="#ff4444"/>
    
    <text x="150" y="140" font-family="'Fira Code', monospace" font-size="12" font-weight="700" 
          text-anchor="middle" fill="#ffffff">QANGA ENGINE</text>
    <text x="150" y="155" font-family="'Fira Code', monospace" font-size="9" 
          text-anchor="middle" fill="#ffffff" opacity="0.8">Game Development</text>
    <text x="150" y="170" font-family="'Fira Code', monospace" font-size="8" 
          text-anchor="middle" fill="#ffffff" opacity="0.6">19.8MB+ C++ Core</text>
    <text x="150" y="185" font-family="'Fira Code', monospace" font-size="8" 
          text-anchor="middle" fill="#ffffff" opacity="0.6">Performance Critical</text>
    
    <!-- Activity indicator -->
    <circle cx="230" cy="90" r="4" fill="#00ff00">
      <animate attributeName="opacity" values="1;0.3;1" dur="2s" repeatCount="indefinite"/>
    </circle>
  </g>
  
  <!-- UE5 Plugins Card -->
  <g id="ue5Card">
    <rect x="300" y="70" width="200" height="140" fill="url(#ue5Grad)" rx="15" filter="url(#cardGlow)">
      <animate attributeName="opacity" values="0.8;1;0.8" dur="4.5s" repeatCount="indefinite"/>
    </rect>
    <rect x="305" y="75" width="190" height="130" fill="none" stroke="#ffffff" stroke-width="1" opacity="0.4" rx="12"/>
    
    <!-- UE5 logo simulation -->
    <rect x="375" y="95" width="50" height="30" fill="#4488ff" opacity="0.7" rx="5"/>
    <text x="400" y="113" font-family="'Fira Code', monospace" font-size="12" font-weight="700" 
          text-anchor="middle" fill="#ffffff">UE5</text>
    
    <text x="400" y="140" font-family="'Fira Code', monospace" font-size="12" font-weight="700" 
          text-anchor="middle" fill="#ffffff">PLUGIN SUITE</text>
    <text x="400" y="155" font-family="'Fira Code', monospace" font-size="9" 
          text-anchor="middle" fill="#ffffff" opacity="0.8">Unreal Engine</text>
    <text x="400" y="170" font-family="'Fira Code', monospace" font-size="8" 
          text-anchor="middle" fill="#ffffff" opacity="0.6">Adaptive Rendering</text>
    <text x="400" y="185" font-family="'Fira Code', monospace" font-size="8" 
          text-anchor="middle" fill="#ffffff" opacity="0.6">Line Markers + More</text>
    
    <circle cx="480" cy="90" r="4" fill="#00ff00">
      <animate attributeName="opacity" values="1;0.3;1" dur="2.3s" repeatCount="indefinite"/>
    </circle>
  </g>
  
  <!-- Tools & Utilities Card -->
  <g id="toolsCard">
    <rect x="550" y="70" width="200" height="140" fill="url(#toolsGrad)" rx="15" filter="url(#cardGlow)">
      <animate attributeName="opacity" values="0.8;1;0.8" dur="5s" repeatCount="indefinite"/>
    </rect>
    <rect x="555" y="75" width="190" height="130" fill="none" stroke="#ffffff" stroke-width="1" opacity="0.4" rx="12"/>
    
    <!-- Tools icon -->
    <rect x="630" y="95" width="20" height="4" fill="#ffffff" rx="2"/>
    <rect x="635" y="90" width="10" height="14" fill="#44ff44" rx="2"/>
    <circle cx="640" cy="105" r="8" fill="none" stroke="#ffffff" stroke-width="2"/>
    
    <text x="650" y="140" font-family="'Fira Code', monospace" font-size="12" font-weight="700" 
          text-anchor="middle" fill="#ffffff">DEV TOOLS</text>
    <text x="650" y="155" font-family="'Fira Code', monospace" font-size="9" 
          text-anchor="middle" fill="#ffffff" opacity="0.8">Utilities & Libraries</text>
    <text x="650" y="170" font-family="'Fira Code', monospace" font-size="8" 
          text-anchor="middle" fill="#ffffff" opacity="0.6">Memory Management</text>
    <text x="650" y="185" font-family="'Fira Code', monospace" font-size="8" 
          text-anchor="middle" fill="#ffffff" opacity="0.6">Graphics & Input</text>
    
    <circle cx="730" cy="90" r="4" fill="#00ff00">
      <animate attributeName="opacity" values="1;0.3;1" dur="2.7s" repeatCount="indefinite"/>
    </circle>
  </g>
  
  <!-- AI/Computer Vision Card -->
  <g id="aiCard">
    <rect x="800" y="70" width="200" height="140" fill="url(#aiGrad)" rx="15" filter="url(#cardGlow)">
      <animate attributeName="opacity" values="0.8;1;0.8" dur="5.5s" repeatCount="indefinite"/>
    </rect>
    <rect x="805" y="75" width="190" height="130" fill="none" stroke="#ffffff" stroke-width="1" opacity="0.4" rx="12"/>
    
    <!-- AI brain icon -->
    <circle cx="900" cy="105" r="20" fill="none" stroke="#ffffff" stroke-width="2"/>
    <circle cx="890" cy="100" r="3" fill="#ffaa44"/>
    <circle cx="910" cy="100" r="3" fill="#ffaa44"/>
    <circle cx="900" cy="110" r="3" fill="#ffaa44"/>
    <line x1="890" y1="100" x2="900" y2="110" stroke="#ffffff" stroke-width="1"/>
    <line x1="910" y1="100" x2="900" y2="110" stroke="#ffffff" stroke-width="1"/>
    
    <text x="900" y="140" font-family="'Fira Code', monospace" font-size="12" font-weight="700" 
          text-anchor="middle" fill="#ffffff">AI RESEARCH</text>
    <text x="900" y="155" font-family="'Fira Code', monospace" font-size="9" 
          text-anchor="middle" fill="#ffffff" opacity="0.8">Computer Vision</text>
    <text x="900" y="170" font-family="'Fira Code', monospace" font-size="8" 
          text-anchor="middle" fill="#ffffff" opacity="0.6">YOLOv10 Integration</text>
    <text x="900" y="185" font-family="'Fira Code', monospace" font-size="8" 
          text-anchor="middle" fill="#ffffff" opacity="0.6">Pattern Matching</text>
    
    <circle cx="980" cy="90" r="4" fill="#00ff00">
      <animate attributeName="opacity" values="1;0.3;1" dur="3s" repeatCount="indefinite"/>
    </circle>
  </g>
  
  <!-- Bottom row - Automation & Analysis -->
  <g id="automationShowcase">
    <rect x="200" y="250" width="700" height="120" fill="url(#automationGrad)" rx="15" filter="url(#cardGlow)">
      <animate attributeName="opacity" values="0.7;0.9;0.7" dur="6s" repeatCount="indefinite"/>
    </rect>
    <rect x="205" y="255" width="690" height="110" fill="none" stroke="#ffffff" stroke-width="1" opacity="0.4" rx="12"/>
    
    <text x="550" y="285" font-family="'Fira Code', monospace" font-size="16" font-weight="700" 
          text-anchor="middle" fill="#ffffff">AUTOMATION & ANALYSIS SUITE</text>
    
    <!-- Automation systems grid -->
    <g id="automationGrid">
      <!-- AutoSystem blocks -->
      <rect x="250" y="300" width="80" height="30" fill="#cc44ff" rx="5" opacity="0.8"/>
      <text x="290" y="318" font-family="'Fira Code', monospace" font-size="9" font-weight="600" 
            text-anchor="middle" fill="#ffffff">AutoSystem-A</text>
      
      <rect x="350" y="300" width="80" height="30" fill="#aa22dd" rx="5" opacity="0.8"/>
      <text x="390" y="318" font-family="'Fira Code', monospace" font-size="9" font-weight="600" 
            text-anchor="middle" fill="#ffffff">AutoSystem-B</text>
      
      <!-- GameTool blocks -->
      <rect x="450" y="300" width="80" height="30" fill="#8800bb" rx="5" opacity="0.8"/>
      <text x="490" y="318" font-family="'Fira Code', monospace" font-size="9" font-weight="600" 
            text-anchor="middle" fill="#ffffff">GameTool-α</text>
      
      <rect x="550" y="300" width="80" height="30" fill="#6600aa" rx="5" opacity="0.8"/>
      <text x="590" y="318" font-family="'Fira Code', monospace" font-size="9" font-weight="600" 
            text-anchor="middle" fill="#ffffff">GameTool-β</text>
      
      <!-- Performance Hook -->
      <rect x="650" y="300" width="100" height="30" fill="#440088" rx="5" opacity="0.8"/>
      <text x="700" y="318" font-family="'Fira Code', monospace" font-size="9" font-weight="600" 
            text-anchor="middle" fill="#ffffff">PerformanceHook</text>
      
      <!-- SoleoTech Suite -->
      <rect x="770" y="300" width="100" height="30" fill="#220066" rx="5" opacity="0.8"/>
      <text x="820" y="318" font-family="'Fira Code', monospace" font-size="9" font-weight="600" 
            text-anchor="middle" fill="#ffffff">SoleoTech Suite</text>
    </g>
    
    <!-- Performance metrics -->
    <text x="350" y="350" font-family="'Fira Code', monospace" font-size="10" fill="#cccccc">Real-time Performance Analysis</text>
    <text x="550" y="350" font-family="'Fira Code', monospace" font-size="10" fill="#cccccc">Automated Testing & Optimization</text>
    <text x="750" y="350" font-family="'Fira Code', monospace" font-size="10" fill="#cccccc">System Monitoring</text>
  </g>
  
  <!-- Technology tags at bottom -->
  <g id="techTags">
    <rect x="50" y="400" width="1000" height="30" fill="#111111" rx="15" opacity="0.6"/>
    <text x="550" y="420" font-family="'Fira Code', monospace" font-size="14" font-weight="600" 
          text-anchor="middle" fill="#ffffff">CORE TECHNOLOGIES</text>
    
    <!-- Tech indicators -->
    <circle cx="150" cy="415" r="3" fill="#00d4ff"/>
    <text x="160" y="420" font-family="'Fira Code', monospace" font-size="10" fill="#ffffff">C++</text>
    
    <circle cx="220" cy="415" r="3" fill="#1c3aa9"/>
    <text x="230" y="420" font-family="'Fira Code', monospace" font-size="10" fill="#ffffff">AutoIt</text>
    
    <circle cx="290" cy="415" r="3" fill="#239120"/>
    <text x="300" y="420" font-family="'Fira Code', monospace" font-size="10" fill="#ffffff">C#</text>
    
    <circle cx="340" cy="415" r="3" fill="#3776ab"/>
    <text x="350" y="420" font-family="'Fira Code', monospace" font-size="10" fill="#ffffff">Python</text>
    
    <circle cx="650" cy="415" r="3" fill="#ff4488"/>
    <text x="660" y="420" font-family="'Fira Code', monospace" font-size="10" fill="#ffffff">UE5</text>
    
    <circle cx="720" cy="415" r="3" fill="#00ff88"/>
    <text x="730" y="420" font-family="'Fira Code', monospace" font-size="10" fill="#ffffff">OpenGL</text>
    
    <circle cx="800" cy="415" r="3" fill="#ffaa00"/>
    <text x="810" y="420" font-family="'Fira Code', monospace" font-size="10" fill="#ffffff">DirectX</text>
    
    <circle cx="880" cy="415" r="3" fill="#aa44ff"/>
    <text x="890" y="420" font-family="'Fira Code', monospace" font-size="10" fill="#ffffff">AI/ML</text>
  </g>
</svg>

</div>

---

## Language Distribution Pie Chart

<div align="center">

<svg width="800" height="400" viewBox="0 0 800 400" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <!-- Pie chart gradients -->
    <radialGradient id="cppPie" cx="50%" cy="30%" r="70%">
      <stop offset="0%" style="stop-color:#00ffff;stop-opacity:1"/>
      <stop offset="50%" style="stop-color:#00d4ff;stop-opacity:0.9"/>
      <stop offset="100%" style="stop-color:#00599c;stop-opacity:1"/>
    </radialGradient>
    <radialGradient id="autoitPie" cx="50%" cy="30%" r="70%">
      <stop offset="0%" style="stop-color:#6666ff;stop-opacity:1"/>
      <stop offset="50%" style="stop-color:#4444dd;stop-opacity:0.9"/>
      <stop offset="100%" style="stop-color:#1c3aa9;stop-opacity:1"/>
    </radialGradient>
    <radialGradient id="csharpPie" cx="50%" cy="30%" r="70%">
      <stop offset="0%" style="stop-color:#44ff44;stop-opacity:1"/>
      <stop offset="50%" style="stop-color:#33dd33;stop-opacity:0.9"/>
      <stop offset="100%" style="stop-color:#239120;stop-opacity:1"/>
    </radialGradient>
    <radialGradient id="pythonPie" cx="50%" cy="30%" r="70%">
      <stop offset="0%" style="stop-color:#66aaff;stop-opacity:1"/>
      <stop offset="50%" style="stop-color:#4488dd;stop-opacity:0.9"/>
      <stop offset="100%" style="stop-color:#3776ab;stop-opacity:1"/>
    </radialGradient>
    <radialGradient id="jsPie" cx="50%" cy="30%" r="70%">
      <stop offset="0%" style="stop-color:#ffff44;stop-opacity:1"/>
      <stop offset="50%" style="stop-color:#ffdd22;stop-opacity:0.9"/>
      <stop offset="100%" style="stop-color:#f7df1e;stop-opacity:1"/>
    </radialGradient>
    
    <!-- 3D shadow filter -->
    <filter id="pieGlow" x="-50%" y="-50%" width="200%" height="200%">
      <feDropShadow dx="3" dy="3" stdDeviation="2" flood-opacity="0.3"/>
      <feGaussianBlur stdDeviation="2" result="coloredBlur"/>
      <feMerge> 
        <feMergeNode in="coloredBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
  </defs>
  
  <!-- Title -->
  <text x="400" y="30" font-family="'Fira Code', monospace" font-size="20" font-weight="700" 
        text-anchor="middle" fill="#ffffff">LANGUAGE COMPOSITION ANALYSIS</text>
  
  <!-- Pie Chart Shadow -->
  <circle cx="203" cy="203" r="95" fill="#000000" opacity="0.2"/>
  
  <!-- Pie Chart Segments (calculated from percentages) -->
  <!-- C++ - 59.8% = 215.28 degrees -->
  <path d="M 200 200 L 200 105 A 95 95 0 0 1 296.5 150.2 Z" fill="url(#cppPie)" filter="url(#pieGlow)">
    <animateTransform attributeName="transform" type="scale" values="0;1" dur="2s" fill="freeze"/>
  </path>
  
  <!-- AutoIt - 27.7% = 99.72 degrees -->
  <path d="M 200 200 L 296.5 150.2 A 95 95 0 0 1 248.5 288.7 Z" fill="url(#autoitPie)" filter="url(#pieGlow)">
    <animateTransform attributeName="transform" type="scale" values="0;1" dur="2.3s" fill="freeze"/>
  </path>
  
  <!-- C# - 6.6% = 23.76 degrees -->
  <path d="M 200 200 L 248.5 288.7 A 95 95 0 0 1 200 295 Z" fill="url(#csharpPie)" filter="url(#pieGlow)">
    <animateTransform attributeName="transform" type="scale" values="0;1" dur="2.6s" fill="freeze"/>
  </path>
  
  <!-- Python - 4.6% = 16.56 degrees -->
  <path d="M 200 200 L 200 295 A 95 95 0 0 1 151.5 288.7 Z" fill="url(#pythonPie)" filter="url(#pieGlow)">
    <animateTransform attributeName="transform" type="scale" values="0;1" dur="2.9s" fill="freeze"/>
  </path>
  
  <!-- JavaScript - 1.3% = 4.68 degrees -->
  <path d="M 200 200 L 151.5 288.7 A 95 95 0 0 1 200 105 Z" fill="url(#jsPie)" filter="url(#pieGlow)">
    <animateTransform attributeName="transform" type="scale" values="0;1" dur="3.2s" fill="freeze"/>
  </path>
  
  <!-- Center circle for 3D effect -->
  <circle cx="200" cy="200" r="25" fill="#1a1a2e" stroke="#00d4ff" stroke-width="2"/>
  <text x="200" y="205" font-family="'Fira Code', monospace" font-size="10" font-weight="700" 
        text-anchor="middle" fill="#ffffff">744K+</text>
  
  <!-- Legend with animated bars -->
  <g id="legend" transform="translate(420, 120)">
    <rect x="0" y="0" width="320" height="240" fill="#1a1a2e" stroke="#00d4ff" stroke-width="1" opacity="0.8" rx="10"/>
    <text x="160" y="25" font-family="'Fira Code', monospace" font-size="14" font-weight="700" 
          text-anchor="middle" fill="#ffffff">BREAKDOWN</text>
    
    <!-- C++ -->
    <circle cx="20" cy="55" r="8" fill="url(#cppPie)">
      <animate attributeName="r" values="8;12;8" dur="3s" repeatCount="indefinite"/>
    </circle>
    <text x="40" y="60" font-family="'Fira Code', monospace" font-size="12" font-weight="600" fill="#ffffff">C++</text>
    <rect x="80" y="50" width="150" height="12" fill="url(#cppPie)" rx="6">
      <animate attributeName="width" values="0;150" dur="2s" fill="freeze"/>
    </rect>
    <text x="240" y="60" font-family="'Fira Code', monospace" font-size="11" font-weight="700" fill="#ffffff">59.8%</text>
    <text x="270" y="60" font-family="'Fira Code', monospace" font-size="9" fill="#cccccc">445K</text>
    
    <!-- AutoIt -->
    <circle cx="20" cy="80" r="8" fill="url(#autoitPie)">
      <animate attributeName="r" values="8;12;8" dur="3.5s" repeatCount="indefinite"/>
    </circle>
    <text x="40" y="85" font-family="'Fira Code', monospace" font-size="12" font-weight="600" fill="#ffffff">AutoIt</text>
    <rect x="80" y="75" width="100" height="12" fill="url(#autoitPie)" rx="6">
      <animate attributeName="width" values="0;100" dur="2.3s" fill="freeze"/>
    </rect>
    <text x="190" y="85" font-family="'Fira Code', monospace" font-size="11" font-weight="700" fill="#ffffff">27.7%</text>
    <text x="240" y="85" font-family="'Fira Code', monospace" font-size="9" fill="#cccccc">206K</text>
    
    <!-- C# -->
    <circle cx="20" cy="105" r="8" fill="url(#csharpPie)">
      <animate attributeName="r" values="8;12;8" dur="4s" repeatCount="indefinite"/>
    </circle>
    <text x="40" y="110" font-family="'Fira Code', monospace" font-size="12" font-weight="600" fill="#ffffff">C#</text>
    <rect x="80" y="100" width="35" height="12" fill="url(#csharpPie)" rx="6">
      <animate attributeName="width" values="0;35" dur="2.6s" fill="freeze"/>
    </rect>
    <text x="125" y="110" font-family="'Fira Code', monospace" font-size="11" font-weight="700" fill="#ffffff">6.6%</text>
    <text x="165" y="110" font-family="'Fira Code', monospace" font-size="9" fill="#cccccc">49K</text>
    
    <!-- Python -->
    <circle cx="20" cy="130" r="8" fill="url(#pythonPie)">
      <animate attributeName="r" values="8;12;8" dur="4.5s" repeatCount="indefinite"/>
    </circle>
    <text x="40" y="135" font-family="'Fira Code', monospace" font-size="12" font-weight="600" fill="#ffffff">Python</text>
    <rect x="80" y="125" width="25" height="12" fill="url(#pythonPie)" rx="6">
      <animate attributeName="width" values="0;25" dur="2.9s" fill="freeze"/>
    </rect>
    <text x="115" y="135" font-family="'Fira Code', monospace" font-size="11" font-weight="700" fill="#ffffff">4.6%</text>
    <text x="155" y="135" font-family="'Fira Code', monospace" font-size="9" fill="#cccccc">34K</text>
    
    <!-- JavaScript -->
    <circle cx="20" cy="155" r="8" fill="url(#jsPie)">
      <animate attributeName="r" values="8;12;8" dur="5s" repeatCount="indefinite"/>
    </circle>
    <text x="40" y="160" font-family="'Fira Code', monospace" font-size="12" font-weight="600" fill="#ffffff">JavaScript</text>
    <rect x="80" y="150" width="8" height="12" fill="url(#jsPie)" rx="6">
      <animate attributeName="width" values="0;8" dur="3.2s" fill="freeze"/>
    </rect>
    <text x="95" y="160" font-family="'Fira Code', monospace" font-size="11" font-weight="700" fill="#000000">1.3%</text>
    <text x="135" y="160" font-family="'Fira Code', monospace" font-size="9" fill="#cccccc">10K</text>
    
    <!-- Summary stats -->
    <line x1="20" y1="180" x2="300" y2="180" stroke="#00d4ff" stroke-width="1" opacity="0.5"/>
    <text x="160" y="200" font-family="'Fira Code', monospace" font-size="12" font-weight="600" 
          text-anchor="middle" fill="#ffffff">TOTAL CODEBASE</text>
    <text x="80" y="220" font-family="'Fira Code', monospace" font-size="10" fill="#cccccc">• 744,000+ Lines of Code</text>
    <text x="80" y="235" font-family="'Fira Code', monospace" font-size="10" fill="#cccccc">• 15+ Programming Languages</text>
  </g>
  
  <!-- Animated percentage labels on pie -->
  <g id="percentageLabels">
    <text x="250" y="140" font-family="'Fira Code', monospace" font-size="14" font-weight="700" 
          text-anchor="middle" fill="#ffffff">59.8%</text>
    <text x="270" y="220" font-family="'Fira Code', monospace" font-size="12" font-weight="700" 
          text-anchor="middle" fill="#ffffff">27.7%</text>
    <text x="220" y="280" font-family="'Fira Code', monospace" font-size="10" font-weight="700" 
          text-anchor="middle" fill="#ffffff">6.6%</text>
    <text x="165" y="270" font-family="'Fira Code', monospace" font-size="9" font-weight="700" 
          text-anchor="middle" fill="#ffffff">4.6%</text>
    <text x="170" y="150" font-family="'Fira Code', monospace" font-size="8" font-weight="700" 
          text-anchor="middle" fill="#000000">1.3%</text>
  </g>
  
  <!-- Orbiting elements -->
  <g transform="translate(200, 200)">
    <g transform="rotate(0)">
      <circle cx="120" cy="0" r="3" fill="#00d4ff" opacity="0.6">
        <animate attributeName="opacity" values="0.6;1;0.6" dur="2s" repeatCount="indefinite"/>
      </circle>
      <animateTransform attributeName="transform" type="rotate" values="0;360" dur="20s" repeatCount="indefinite"/>
    </g>
    <g transform="rotate(120)">
      <circle cx="120" cy="0" r="2" fill="#ff6b00" opacity="0.7">
        <animate attributeName="opacity" values="0.7;1;0.7" dur="2.5s" repeatCount="indefinite"/>
      </circle>
      <animateTransform attributeName="transform" type="rotate" values="120;480" dur="25s" repeatCount="indefinite"/>
    </g>
    <g transform="rotate(240)">
      <circle cx="120" cy="0" r="2.5" fill="#00ff88" opacity="0.5">
        <animate attributeName="opacity" values="0.5;1;0.5" dur="3s" repeatCount="indefinite"/>
      </circle>
      <animateTransform attributeName="transform" type="rotate" values="240;600" dur="30s" repeatCount="indefinite"/>
    </g>
  </g>
</svg>

</div>

---

<div align="center">

<svg width="300" height="60" viewBox="0 0 300 60" xmlns="http://www.w3.org/2000/svg">
  <rect x="50" y="15" width="80" height="30" fill="#333333" rx="15"/>
  <text x="90" y="35" font-family="'Fira Code', monospace" font-size="12" font-weight="600" 
        text-anchor="middle" fill="#ffffff">Precision</text>
  
  <rect x="170" y="15" width="80" height="30" fill="#cc3333" rx="15"/>
  <text x="210" y="35" font-family="'Fira Code', monospace" font-size="12" font-weight="600" 
        text-anchor="middle" fill="#ffffff">Performance</text>
</svg>

</div>
