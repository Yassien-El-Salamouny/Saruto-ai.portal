# Saruto-ai.portal
SARUTO's Cloud AI Landing Portal

<img width="150" height="150" alt="Boundless" src="https://github.com/user-attachments/assets/494fce43-6450-47e8-be0e-d4fc9d0f3184" />
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 500 500" width="100%" height="100%">
    <defs>
        <!-- Glow / Optical Bloom Filters -->
        <filter id="hyper-glow" x="-50%" y="-50%" width="200%" height="200%">
            <feGaussianBlur stdDeviation="8" result="blur1"/>
            <feGaussianBlur stdDeviation="20" result="blur2"/>
            <feMerge>
                <feMergeNode in="blur2"/>
                <feMergeNode in="blur1"/>
                <feMergeNode in="SourceGraphic"/>
            </feMerge>
        </filter>

<filter id="soft-blur">
            <feGaussianBlur stdDeviation="3"/>
        </filter>
 <!-- Deep Space Outer Glare -->
        <radialGradient id="space-glare" cx="50%" cy="40%" r="50%">
            <stop offset="0%" stop-color="#ffffff" stop-opacity="0.35"/>
            <stop offset="25%" stop-color="#fef3c7" stop-opacity="0.18"/>
            <stop offset="55%" stop-color="#3b82f6" stop-opacity="0.06"/>
            <stop offset="100%" stop-color="#000000" stop-opacity="0"/>
        </radialGradient>
 <!-- Accretion Light / Gravitational Lensing Halo Gradient -->
        <linearGradient id="lens-halo" x1="0%" y1="0%" x2="100%" y2="0%">
            <stop offset="0%" stop-color="#ffffff" stop-opacity="0.95"/>
            <stop offset="30%" stop-color="#fef3c7" stop-opacity="0.85"/>
            <stop offset="65%" stop-color="#f97316" stop-opacity="0.5"/>
            <stop offset="100%" stop-color="#3b82f6" stop-opacity="0.1"/>
        </linearGradient>
 <!-- Main Accretion Disk (Doppler-beamed: Bright left, dim right) -->
        <linearGradient id="accretion-beam" x1="0%" y1="0%" x2="100%" y2="0%">
            <stop offset="0%" stop-color="#ffffff" stop-opacity="0.1"/>
            <stop offset="18%" stop-color="#ffffff" stop-opacity="1"/>
            <stop offset="40%" stop-color="#ffedd5" stop-opacity="0.95"/>
            <stop offset="70%" stop-color="#fdba74" stop-opacity="0.6"/>
            <stop offset="100%" stop-color="#ea580c" stop-opacity="0"/>
        </linearGradient>
    </defs>
<!-- Outer Ambient Energy Halo -->
    <circle cx="250" cy="200" r="210" fill="url(#space-glare)"/>
 <!-- Tilted Black Hole Assembly (~14deg Clockwise) -->
    <g transform="rotate(14 250 200)">
 <!-- 1. GRAVITATIONAL LENSING: Upper Halo Arch -->
        <path d="M 80,200 C 80,80 320,80 320,200 C 295,120 105,120 80,200 Z" 
              fill="url(#lens-halo)" 
              filter="url(#hyper-glow)"/>
        <path d="M 110,200 C 110,115 290,115 290,200 C 275,140 125,140 110,200 Z" 
              fill="#ffffff" 
              opacity="0.7" 
              filter="url(#soft-blur)"/>
 <!-- 2. GRAVITATIONAL LENSING: Lower Halo Arch -->
        <path d="M 90,200 C 90,305 310,305 310,200 C 285,255 115,255 90,200 Z" 
              fill="url(#lens-halo)" 
              opacity="0.75" 
              filter="url(#hyper-glow)"/>
  <!-- 3. ACCRETION DISK: Main Horizontal Beam Across Center -->
        <ellipse cx="250" cy="200" rx="220" ry="11" 
                 fill="url(#accretion-beam)" 
                 filter="url(#hyper-glow)"/>
        <ellipse cx="250" cy="200" rx="210" ry="4" 
                 fill="#ffffff" 
                 opacity="0.9"/>
 <!-- 4. PITCH BLACK EVENT HORIZON CORE -->
        <circle cx="250" cy="200" r="58" fill="#020305"/>
<!-- 5. PHOTON RING (Sharp Luminescent Border around Horizon) -->
        <circle cx="250" cy="200" r="59.5" 
                fill="none" 
                stroke="#ffffff" 
                stroke-width="2" 
                filter="url(#hyper-glow)"/>
        <circle cx="250" cy="200" r="59" 
                fill="none" 
                stroke="#ffffff" 
                stroke-width="1"/>

 </g>
 <!-- TYPOGRAPHY: SARUTO AI -->
                                                           <text x="250" y="425" 
          font-family="-apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif" 
          font-size="32" 
          font-weight="900" 
          fill="#ffffff" 
          text-anchor="middle" 
          letter-spacing="0.32em" 
          filter="url(#soft-blur)" 
          opacity="0.4">SARUTO AI</text>

    <text x="250" y="425" 
          font-family="-apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif" 
          font-size="32" 
          font-weight="900" 
          fill="#ffffff" 
          text-anchor="middle" 
          letter-spacing="0.32em">SARUTO AI</text>
</svg>
