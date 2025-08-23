<div align="center">

<svg width="800" height="120" viewBox="0 0 800 120" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="titleGradient" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#00d4ff;stop-opacity:1" />
      <stop offset="50%" style="stop-color:#0099cc;stop-opacity:1" />
      <stop offset="100%" style="stop-color:#00d4ff;stop-opacity:1" />
    </linearGradient>
    <linearGradient id="glowGradient" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#00d4ff;stop-opacity:0.3" />
      <stop offset="50%" style="stop-color:#00d4ff;stop-opacity:0.8" />
      <stop offset="100%" style="stop-color:#00d4ff;stop-opacity:0.3" />
    </linearGradient>
  </defs>
  
  <!-- Background pulse effect -->
  <rect width="800" height="120" fill="url(#glowGradient)" opacity="0.1">
    <animate attributeName="opacity" values="0.1;0.3;0.1" dur="3s" repeatCount="indefinite"/>
  </rect>
  
  <!-- Main title -->
  <text x="400" y="45" font-family="'Fira Code', monospace" font-size="36" font-weight="700" 
        text-anchor="middle" fill="url(#titleGradient)">
    Rz Solutions
    <animate attributeName="opacity" values="1;0.7;1" dur="2s" repeatCount="indefinite"/>
  </text>
  
  <!-- Subtitle with typewriter effect -->
  <text x="400" y="75" font-family="'Fira Code', monospace" font-size="16" 
        text-anchor="middle" fill="#888888">
    Systems Architecture • Performance Engineering
  </text>
  
  <!-- Animated underline -->
  <line x1="250" y1="85" x2="550" y2="85" stroke="url(#titleGradient)" stroke-width="2">
    <animate attributeName="stroke-dasharray" values="0,300;300,0;0,300" dur="4s" repeatCount="indefinite"/>
    <animate attributeName="stroke-dashoffset" values="0;-300;-600" dur="4s" repeatCount="indefinite"/>
  </line>
</svg>

</div>

---

<div align="center">

<svg width="700" height="300" viewBox="0 0 700 300" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="barGradient" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#00d4ff"/>
      <stop offset="100%" style="stop-color:#0099cc"/>
    </linearGradient>
    <filter id="glow">
      <feGaussianBlur stdDeviation="3" result="coloredBlur"/>
      <feMerge> 
        <feMergeNode in="coloredBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
  </defs>
  
  <!-- Background grid -->
  <defs>
    <pattern id="grid" width="20" height="20" patternUnits="userSpaceOnUse">
      <path d="M 20 0 L 0 0 0 20" fill="none" stroke="#333" stroke-width="0.5" opacity="0.3"/>
    </pattern>
  </defs>
  <rect width="700" height="300" fill="url(#grid)"/>
  
  <!-- Repository Statistics -->
  <text x="350" y="30" font-family="'Fira Code', monospace" font-size="18" font-weight="600" 
        text-anchor="middle" fill="#00d4ff">Repository Analytics</text>
  
  <!-- Total Repos -->
  <text x="50" y="70" font-family="'Fira Code', monospace" font-size="12" fill="#cccccc">Total Repositories</text>
  <rect x="50" y="80" width="200" height="25" fill="url(#barGradient)" rx="12" filter="url(#glow)">
    <animate attributeName="width" values="0;200" dur="2s" fill="freeze"/>
  </rect>
  <text x="260" y="97" font-family="'Fira Code', monospace" font-size="14" font-weight="700" fill="#ffffff">40</text>
  
  <!-- C++ Dominance -->
  <text x="50" y="130" font-family="'Fira Code', monospace" font-size="12" fill="#cccccc">C++ Codebase (Qanga)</text>
  <rect x="50" y="140" width="350" height="25" fill="#f34b7d" rx="12" filter="url(#glow)">
    <animate attributeName="width" values="0;350" dur="2.5s" fill="freeze"/>
  </rect>
  <text x="410" y="157" font-family="'Fira Code', monospace" font-size="14" font-weight="700" fill="#ffffff">19.8M+ bytes</text>
  
  <!-- Languages -->
  <text x="50" y="190" font-family="'Fira Code', monospace" font-size="12" fill="#cccccc">Languages Mastered</text>
  <rect x="50" y="200" width="150" height="25" fill="#4ecdc4" rx="12" filter="url(#glow)">
    <animate attributeName="width" values="0;150" dur="1.8s" fill="freeze"/>
  </rect>
  <text x="210" y="217" font-family="'Fira Code', monospace" font-size="14" font-weight="700" fill="#ffffff">15+</text>
  
  <!-- Experience -->
  <text x="50" y="250" font-family="'Fira Code', monospace" font-size="12" fill="#cccccc">Years of Engineering</text>
  <rect x="50" y="260" width="240" height="25" fill="#ffd93d" rx="12" filter="url(#glow)">
    <animate attributeName="width" values="0;240" dur="2.2s" fill="freeze"/>
  </rect>
  <text x="300" y="277" font-family="'Fira Code', monospace" font-size="14" font-weight="700" fill="#000000">20+</text>
  
  <!-- Performance indicators -->
  <g transform="translate(450, 70)">
    <circle cx="30" cy="30" r="25" fill="none" stroke="#00d4ff" stroke-width="3">
      <animate attributeName="stroke-dasharray" values="0,157;78,79;157,0" dur="3s" repeatCount="indefinite"/>
    </circle>
    <text x="30" y="36" font-family="'Fira Code', monospace" font-size="12" font-weight="700" 
          text-anchor="middle" fill="#00d4ff">PERF</text>
  </g>
  
  <g transform="translate(550, 70)">
    <polygon points="30,10 50,50 10,50" fill="#4ecdc4" filter="url(#glow)">
      <animateTransform attributeName="transform" type="rotate" 
                        values="0 30 30;360 30 30" dur="4s" repeatCount="indefinite"/>
    </polygon>
    <text x="30" y="75" font-family="'Fira Code', monospace" font-size="10" font-weight="600" 
          text-anchor="middle" fill="#4ecdc4">ARCH</text>
  </g>
</svg>

</div>

---

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
    <linearGradient id="js" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#f7df1e"/>
      <stop offset="100%" style="stop-color:#e5c700"/>
    </linearGradient>
    <linearGradient id="python" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#3776ab"/>
      <stop offset="100%" style="stop-color:#306998"/>
    </linearGradient>
  </defs>
  
  <text x="300" y="25" font-family="'Fira Code', monospace" font-size="16" font-weight="600" 
        text-anchor="middle" fill="#ffffff">Technology Stack</text>
  
  <!-- Language bars with labels -->
  <text x="50" y="55" font-family="'Fira Code', monospace" font-size="12" fill="#cccccc">C++</text>
  <rect x="100" y="45" width="400" height="15" fill="url(#cpp)" rx="7">
    <animate attributeName="width" values="0;400" dur="2s" fill="freeze"/>
  </rect>
  
  <text x="50" y="80" font-family="'Fira Code', monospace" font-size="12" fill="#cccccc">C#</text>
  <rect x="100" y="70" width="250" height="15" fill="url(#csharp)" rx="7">
    <animate attributeName="width" values="0;250" dur="2.2s" fill="freeze"/>
  </rect>
  
  <text x="50" y="105" font-family="'Fira Code', monospace" font-size="12" fill="#cccccc">AutoIt</text>
  <rect x="100" y="95" width="200" height="15" fill="url(#autoit)" rx="7">
    <animate attributeName="width" values="0;200" dur="2.4s" fill="freeze"/>
  </rect>
  
  <text x="50" y="130" font-family="'Fira Code', monospace" font-size="12" fill="#cccccc">JavaScript</text>
  <rect x="100" y="120" width="180" height="15" fill="url(#js)" rx="7">
    <animate attributeName="width" values="0;180" dur="2.6s" fill="freeze"/>
  </rect>
  
  <text x="50" y="155" font-family="'Fira Code', monospace" font-size="12" fill="#cccccc">Python</text>
  <rect x="100" y="145" width="160" height="15" fill="url(#python)" rx="7">
    <animate attributeName="width" values="0;160" dur="2.8s" fill="freeze"/>
  </rect>
  
  <!-- Floating code symbols -->
  <g opacity="0.6">
    <text x="520" y="60" font-family="'Fira Code', monospace" font-size="20" fill="#00599c">{}</text>
    <text x="520" y="85" font-family="'Fira Code', monospace" font-size="18" fill="#239120">()</text>
    <text x="520" y="110" font-family="'Fira Code', monospace" font-size="16" fill="#1c3aa9">[]</text>
    <text x="520" y="135" font-family="'Fira Code', monospace" font-size="14" fill="#f7df1e">&lt;&gt;</text>
    <text x="520" y="160" font-family="'Fira Code', monospace" font-size="12" fill="#3776ab">::</text>
    
    <animateTransform attributeName="transform" type="translate" 
                      values="0,0; 5,0; 0,0; -5,0; 0,0" dur="4s" repeatCount="indefinite"/>
  </g>
</svg>

</div>

---

<div align="center">

<svg width="500" height="150" viewBox="0 0 500 150" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="pathGradient" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#ff6b6b"/>
      <stop offset="33%" style="stop-color:#4ecdc4"/>
      <stop offset="66%" style="stop-color:#45b7d1"/>
      <stop offset="100%" style="stop-color:#96ceb4"/>
    </linearGradient>
  </defs>
  
  <text x="250" y="25" font-family="'Fira Code', monospace" font-size="16" font-weight="600" 
        text-anchor="middle" fill="#ffffff">Core Focus Areas</text>
  
  <!-- Animated connection path -->
  <path d="M50,50 Q150,30 250,50 Q350,70 450,50" stroke="url(#pathGradient)" stroke-width="3" fill="none">
    <animate attributeName="stroke-dasharray" values="0,400;200,200;400,0" dur="3s" repeatCount="indefinite"/>
  </path>
  
  <!-- Focus area nodes -->
  <circle cx="50" cy="50" r="8" fill="#ff6b6b">
    <animate attributeName="r" values="8;12;8" dur="2s" repeatCount="indefinite"/>
  </circle>
  <text x="50" y="75" font-family="'Fira Code', monospace" font-size="10" font-weight="600" 
        text-anchor="middle" fill="#ff6b6b">Game Dev</text>
  
  <circle cx="150" cy="30" r="8" fill="#4ecdc4">
    <animate attributeName="r" values="8;12;8" dur="2s" begin="0.5s" repeatCount="indefinite"/>
  </circle>
  <text x="150" y="20" font-family="'Fira Code', monospace" font-size="10" font-weight="600" 
        text-anchor="middle" fill="#4ecdc4">UE5 Plugins</text>
  
  <circle cx="250" cy="50" r="8" fill="#45b7d1">
    <animate attributeName="r" values="8;12;8" dur="2s" begin="1s" repeatCount="indefinite"/>
  </circle>
  <text x="250" y="75" font-family="'Fira Code', monospace" font-size="10" font-weight="600" 
        text-anchor="middle" fill="#45b7d1">Performance</text>
  
  <circle cx="350" cy="70" r="8" fill="#96ceb4">
    <animate attributeName="r" values="8;12;8" dur="2s" begin="1.5s" repeatCount="indefinite"/>
  </circle>
  <text x="350" y="90" font-family="'Fira Code', monospace" font-size="10" font-weight="600" 
        text-anchor="middle" fill="#96ceb4">Automation</text>
  
  <circle cx="450" cy="50" r="8" fill="#ffd93d">
    <animate attributeName="r" values="8;12;8" dur="2s" begin="2s" repeatCount="indefinite"/>
  </circle>
  <text x="450" y="75" font-family="'Fira Code', monospace" font-size="10" font-weight="600" 
        text-anchor="middle" fill="#ffd93d">Systems</text>
  
  <!-- Central processing indicator -->
  <g transform="translate(250, 110)">
    <rect x="-15" y="-8" width="30" height="16" fill="#333" rx="8"/>
    <rect x="-12" y="-5" width="24" height="10" fill="#00d4ff" rx="5" opacity="0.8">
      <animate attributeName="opacity" values="0.8;0.3;0.8" dur="1s" repeatCount="indefinite"/>
    </rect>
    <text x="0" y="3" font-family="'Fira Code', monospace" font-size="8" font-weight="600" 
          text-anchor="middle" fill="#000">CPU</text>
  </g>
</svg>

</div>

---

<div align="center">

<table style="border: none; background: transparent;">
<tr>
<td align="center" style="border: none; background: transparent;">

<svg width="200" height="120" viewBox="0 0 200 120" xmlns="http://www.w3.org/2000/svg">
  <text x="100" y="20" font-family="'Fira Code', monospace" font-size="12" font-weight="600" 
        text-anchor="middle" fill="#cccccc">neXuz-dev</text>
  
  <rect x="20" y="30" width="160" height="60" fill="#0d1117" stroke="#00d4ff" stroke-width="2" rx="8"/>
  
  <!-- Activity graph simulation -->
  <g transform="translate(30, 40)">
    <rect x="0" y="30" width="8" height="10" fill="#196127">
      <animate attributeName="height" values="10;20;15;10" dur="3s" repeatCount="indefinite"/>
      <animate attributeName="y" values="30;20;25;30" dur="3s" repeatCount="indefinite"/>
    </rect>
    <rect x="12" y="25" width="8" height="15" fill="#239a3b">
      <animate attributeName="height" values="15;25;20;15" dur="3s" begin="0.5s" repeatCount="indefinite"/>
      <animate attributeName="y" values="25;15;20;25" dur="3s" begin="0.5s" repeatCount="indefinite"/>
    </rect>
    <rect x="24" y="20" width="8" height="20" fill="#26a641">
      <animate attributeName="height" values="20;30;25;20" dur="3s" begin="1s" repeatCount="indefinite"/>
      <animate attributeName="y" values="20;10;15;20" dur="3s" begin="1s" repeatCount="indefinite"/>
    </rect>
    <rect x="36" y="15" width="8" height="25" fill="#39d353">
      <animate attributeName="height" values="25;35;30;25" dur="3s" begin="1.5s" repeatCount="indefinite"/>
      <animate attributeName="y" values="15;5;10;15" dur="3s" begin="1.5s" repeatCount="indefinite"/>
    </rect>
    <!-- More bars... -->
    <rect x="48" y="10" width="8" height="30" fill="#39d353">
      <animate attributeName="height" values="30;40;35;30" dur="3s" begin="2s" repeatCount="indefinite"/>
      <animate attributeName="y" values="10;0;5;10" dur="3s" begin="2s" repeatCount="indefinite"/>
    </rect>
  </g>
  
  <text x="100" y="110" font-family="'Fira Code', monospace" font-size="10" fill="#00d4ff">Systems Architecture</text>
</svg>

</td>
<td align="center" style="border: none; background: transparent;">

<svg width="200" height="120" viewBox="0 0 200 120" xmlns="http://www.w3.org/2000/svg">
  <text x="100" y="20" font-family="'Fira Code', monospace" font-size="12" font-weight="600" 
        text-anchor="middle" fill="#cccccc">Rz-Software</text>
  
  <rect x="20" y="30" width="160" height="60" fill="#0d1117" stroke="#7c3aed" stroke-width="2" rx="8"/>
  
  <!-- Activity graph simulation -->
  <g transform="translate(30, 40)">
    <rect x="0" y="25" width="8" height="15" fill="#196127">
      <animate attributeName="height" values="15;25;20;15" dur="3s" begin="0.3s" repeatCount="indefinite"/>
      <animate attributeName="y" values="25;15;20;25" dur="3s" begin="0.3s" repeatCount="indefinite"/>
    </rect>
    <rect x="12" y="20" width="8" height="20" fill="#239a3b">
      <animate attributeName="height" values="20;30;25;20" dur="3s" begin="0.8s" repeatCount="indefinite"/>
      <animate attributeName="y" values="20;10;15;20" dur="3s" begin="0.8s" repeatCount="indefinite"/>
    </rect>
    <rect x="24" y="15" width="8" height="25" fill="#26a641">
      <animate attributeName="height" values="25;35;30;25" dur="3s" begin="1.3s" repeatCount="indefinite"/>
      <animate attributeName="y" values="15;5;10;15" dur="3s" begin="1.3s" repeatCount="indefinite"/>
    </rect>
    <rect x="36" y="12" width="8" height="28" fill="#39d353">
      <animate attributeName="height" values="28;38;33;28" dur="3s" begin="1.8s" repeatCount="indefinite"/>
      <animate attributeName="y" values="12;2;7;12" dur="3s" begin="1.8s" repeatCount="indefinite"/>
    </rect>
    <rect x="48" y="8" width="8" height="32" fill="#39d353">
      <animate attributeName="height" values="32;42;37;32" dur="3s" begin="2.3s" repeatCount="indefinite"/>
      <animate attributeName="y" values="8;-2;3;8" dur="3s" begin="2.3s" repeatCount="indefinite"/>
    </rect>
  </g>
  
  <text x="100" y="110" font-family="'Fira Code', monospace" font-size="10" fill="#7c3aed">Performance Engineering</text>
</svg>

</td>
</tr>
</table>

</div>

---

<div align="center">

<svg width="400" height="80" viewBox="0 0 400 80" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="finalGradient" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#333333"/>
      <stop offset="50%" style="stop-color:#666666"/>
      <stop offset="100%" style="stop-color:#333333"/>
    </linearGradient>
  </defs>
  
  <rect x="50" y="25" width="120" height="30" fill="url(#finalGradient)" rx="15"/>
  <text x="110" y="45" font-family="'Fira Code', monospace" font-size="12" font-weight="600" 
        text-anchor="middle" fill="#ffffff">Precision</text>
  
  <rect x="230" y="25" width="120" height="30" fill="#cc3333" rx="15"/>
  <text x="290" y="45" font-family="'Fira Code', monospace" font-size="12" font-weight="600" 
        text-anchor="middle" fill="#ffffff">Performance</text>
  
  <!-- Subtle animation -->
  <circle cx="200" cy="40" r="3" fill="#00d4ff" opacity="0.7">
    <animate attributeName="opacity" values="0.7;1;0.7" dur="2s" repeatCount="indefinite"/>
    <animate attributeName="r" values="3;5;3" dur="2s" repeatCount="indefinite"/>
  </circle>
</svg>

</div>
