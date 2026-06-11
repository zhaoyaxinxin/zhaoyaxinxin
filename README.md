<div align="center">

<!-- ⭐ COSMIC DEVELOPER — 星空宇宙主题 GitHub Profile ⭐ -->

<svg width="100%" viewBox="0 0 1200 700" xmlns="http://www.w3.org/2000/svg">
  <defs>

    <!-- ===== 深空背景渐变 ===== -->
    <radialGradient id="deepSpace" cx="50%" cy="40%" r="70%" fx="50%" fy="40%">
      <stop offset="0%" stop-color="#0d0d3f"/>
      <stop offset="25%" stop-color="#080828"/>
      <stop offset="55%" stop-color="#040418"/>
      <stop offset="85%" stop-color="#010108"/>
      <stop offset="100%" stop-color="#000005"/>
    </radialGradient>

    <radialGradient id="nebulaCore" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stop-color="#2a1a5e" stop-opacity="0.9"/>
      <stop offset="40%" stop-color="#1a0a4e" stop-opacity="0.5"/>
      <stop offset="70%" stop-color="#0a0530" stop-opacity="0.2"/>
      <stop offset="100%" stop-color="transparent" stop-opacity="0"/>
    </radialGradient>

    <!-- ===== 恒星发光渐变 ===== -->
    <radialGradient id="starCore" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stop-color="#ffffff"/>
      <stop offset="8%" stop-color="#fffde8"/>
      <stop offset="20%" stop-color="#fff9c4"/>
      <stop offset="40%" stop-color="#ffcc02"/>
      <stop offset="65%" stop-color="#ff8c00"/>
      <stop offset="85%" stop-color="#e64a00" stop-opacity="0.4"/>
      <stop offset="100%" stop-color="#cc3300" stop-opacity="0"/>
    </radialGradient>

    <radialGradient id="starOuterGlow" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stop-color="#ffcc00" stop-opacity="0.6"/>
      <stop offset="30%" stop-color="#ff9900" stop-opacity="0.3"/>
      <stop offset="60%" stop-color="#ff6600" stop-opacity="0.1"/>
      <stop offset="100%" stop-color="#ff4400" stop-opacity="0"/>
    </radialGradient>

    <radialGradient id="starInnerGlow" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stop-color="#ffffff" stop-opacity="1"/>
      <stop offset="40%" stop-color="#fffde0" stop-opacity="0.8"/>
      <stop offset="100%" stop-color="#ffcc00" stop-opacity="0"/>
    </radialGradient>

    <!-- ===== 行星渐变 ===== -->
    <!-- 近轨行星：红褐色岩石 -->
    <radialGradient id="planet1Grad" cx="35%" cy="35%" r="60%">
      <stop offset="0%" stop-color="#e8a87c"/>
      <stop offset="30%" stop-color="#d4744a"/>
      <stop offset="60%" stop-color="#8b3a2a"/>
      <stop offset="100%" stop-color="#3d1208"/>
    </radialGradient>

    <!-- 中轨行星：蓝绿类地 -->
    <radialGradient id="planet2Grad" cx="35%" cy="35%" r="60%">
      <stop offset="0%" stop-color="#7ec8e3"/>
      <stop offset="25%" stop-color="#4a90d9"/>
      <stop offset="55%" stop-color="#1a5276"/>
      <stop offset="80%" stop-color="#0d3b2e"/>
      <stop offset="100%" stop-color="#051a10"/>
    </radialGradient>

    <!-- 中远轨行星：土黄带环 -->
    <radialGradient id="planet3Grad" cx="35%" cy="35%" r="60%">
      <stop offset="0%" stop-color="#f5deb3"/>
      <stop offset="30%" stop-color="#daa520"/>
      <stop offset="60%" stop-color="#b8860b"/>
      <stop offset="100%" stop-color="#5c3a00"/>
    </radialGradient>

    <!-- 远轨行星：青蓝气态巨行星 -->
    <radialGradient id="planet4Grad" cx="35%" cy="35%" r="60%">
      <stop offset="0%" stop-color="#a8d8ea"/>
      <stop offset="25%" stop-color="#6bb5d0"/>
      <stop offset="50%" stop-color="#3a7ca5"/>
      <stop offset="75%" stop-color="#1a4a6e"/>
      <stop offset="100%" stop-color="#0a1a30"/>
    </radialGradient>

    <!-- 气态巨行星条纹滤镜 -->
    <pattern id="gasStripes" x="0" y="0" width="100%" height="15%" patternUnits="userSpaceOnUse">
      <rect width="100%" height="50%" fill="none" stroke="#ffffff22" stroke-width="3"/>
    </pattern>

    <!-- ===== 流体星云滤镜 ===== -->
    <filter id="nebulaFluid1" x="-30%" y="-30%" width="160%" height="160%">
      <feTurbulence type="fractalNoise" baseFrequency="0.012" numOctaves="5" seed="42" result="noise">
        <animate attributeName="baseFrequency"
          values="0.012;0.016;0.009;0.014;0.012"
          dur="28s" repeatCount="indefinite"
          calcMode="spline"
          keySplines="0.45 0 0.55 1; 0.45 0 0.55 1; 0.45 0 0.55 1; 0.45 0 0.55 1"/>
        <animate attributeName="seed"
          values="42;55;38;46;42"
          dur="28s" repeatCount="indefinite"/>
      </feTurbulence>
      <feDisplacementMap in="SourceGraphic" in2="noise" scale="70" xChannelSelector="R" yChannelSelector="G" result="displaced"/>
      <feGaussianBlur in="displaced" stdDeviation="6" result="blurred"/>
    </filter>

    <filter id="nebulaFluid2" x="-30%" y="-30%" width="160%" height="160%">
      <feTurbulence type="fractalNoise" baseFrequency="0.008" numOctaves="4" seed="77" result="noise">
        <animate attributeName="baseFrequency"
          values="0.008;0.011;0.006;0.009;0.008"
          dur="35s" repeatCount="indefinite"
          calcMode="spline"
          keySplines="0.35 0 0.65 1; 0.35 0 0.65 1; 0.35 0 0.65 1; 0.35 0 0.65 1"/>
      </feTurbulence>
      <feDisplacementMap in="SourceGraphic" in2="noise" scale="90" xChannelSelector="R" yChannelSelector="B" result="displaced"/>
      <feGaussianBlur in="displaced" stdDeviation="10" result="blurred"/>
    </filter>

    <filter id="nebulaFluid3" x="-40%" y="-40%" width="180%" height="180%">
      <feTurbulence type="fractalNoise" baseFrequency="0.006" numOctaves="3" seed="13" result="noise">
        <animate attributeName="baseFrequency"
          values="0.006;0.009;0.004;0.007;0.006"
          dur="42s" repeatCount="indefinite"
          calcMode="spline"
          keySplines="0.5 0 0.5 1; 0.5 0 0.5 1; 0.5 0 0.5 1; 0.5 0 0.5 1"/>
      </feTurbulence>
      <feDisplacementMap in="SourceGraphic" in2="noise" scale="120" xChannelSelector="B" yChannelSelector="G" result="displaced"/>
      <feGaussianBlur in="displaced" stdDeviation="16" result="blurred"/>
    </filter>

    <!-- ===== 光晕滤镜 ===== -->
    <filter id="glowStar" x="-80%" y="-80%" width="260%" height="260%">
      <feGaussianBlur stdDeviation="12" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <filter id="glowSoft" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="4" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <filter id="glowText" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="3" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <filter id="glowIntense" x="-100%" y="-100%" width="300%" height="300%">
      <feGaussianBlur stdDeviation="20" result="blur1"/>
      <feGaussianBlur stdDeviation="8" result="blur2"/>
      <feMerge>
        <feMergeNode in="blur1"/>
        <feMergeNode in="blur2"/>
        <feMergeNode in="blur2"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <!-- ===== 行星阴影滤镜 ===== -->
    <filter id="planetShadow" x="-20%" y="-20%" width="140%" height="140%">
      <feGaussianBlur stdDeviation="2"/>
    </filter>

    <!-- ===== 流星拖尾渐变 ===== -->
    <linearGradient id="shootingStarTrail" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#ffffff" stop-opacity="1"/>
      <stop offset="30%" stop-color="#ffffff" stop-opacity="0.6"/>
      <stop offset="60%" stop-color="#aaccff" stop-opacity="0.15"/>
      <stop offset="100%" stop-color="#aaccff" stop-opacity="0"/>
    </linearGradient>

    <!-- ===== 恒星光线 mask ===== -->
    <radialGradient id="rayFade" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stop-color="#ffffff" stop-opacity="1"/>
      <stop offset="60%" stop-color="#ffffff" stop-opacity="0.5"/>
      <stop offset="100%" stop-color="#ffffff" stop-opacity="0"/>
    </radialGradient>

    <!-- ===== 星空闪烁动画 ===== -->
    <style>
      @keyframes twinkle1 { 0%,100%{opacity:0.3} 50%{opacity:1} }
      @keyframes twinkle2 { 0%,100%{opacity:0.8} 40%{opacity:0.2} 75%{opacity:0.9} }
      @keyframes twinkle3 { 0%,100%{opacity:0.5} 30%{opacity:0.1} 60%{opacity:1} 85%{opacity:0.3} }
      @keyframes twinkle4 { 0%,100%{opacity:0.7} 20%{opacity:0.15} 55%{opacity:0.95} 80%{opacity:0.25} }

      @keyframes starRotate { 100%{transform:rotate(360deg)} }
      @keyframes starPulse { 0%,100%{opacity:0.6;transform:scale(1)} 50%{opacity:1;transform:scale(1.08)} }
      @keyframes starPulseOuter { 0%,100%{opacity:0.3;transform:scale(1)} 50%{opacity:0.7;transform:scale(1.15)} }

      @keyframes orbit1 { 100%{transform:rotate(360deg)} }
      @keyframes orbit2 { 100%{transform:rotate(-360deg)} }
      @keyframes orbit3 { 100%{transform:rotate(360deg)} }
      @keyframes orbit4 { 100%{transform:rotate(-360deg)} }

      @keyframes selfSpin1 { 100%{transform:rotate(720deg)} }
      @keyframes selfSpin2 { 100%{transform:rotate(-540deg)} }
      @keyframes selfSpin3 { 100%{transform:rotate(600deg)} }
      @keyframes selfSpin4 { 100%{transform:rotate(-300deg)} }

      @keyframes moonOrbit { 100%{transform:rotate(360deg)} }

      @keyframes shoot1 {
        0%{transform:translate(0,0) scale(0);opacity:0}
        5%{transform:translate(30,-15) scale(0.4);opacity:0.3}
        10%{transform:translate(60,-30) scale(0.8);opacity:0.7}
        15%{transform:translate(120,-60) scale(1);opacity:1}
        25%{transform:translate(200,-100) scale(1);opacity:0.9}
        40%{transform:translate(320,-160) scale(0.7);opacity:0.4}
        60%{transform:translate(480,-240) scale(0.3);opacity:0.1}
        100%{transform:translate(800,-400) scale(0);opacity:0}
      }
      @keyframes shoot2 {
        0%{transform:translate(0,0) scale(0);opacity:0}
        3%{transform:translate(15,-8) scale(0.3);opacity:0.2}
        8%{transform:translate(45,-23) scale(0.7);opacity:0.6}
        12%{transform:translate(90,-45) scale(1);opacity:1}
        20%{transform:translate(180,-90) scale(0.9);opacity:0.7}
        35%{transform:translate(300,-150) scale(0.5);opacity:0.2}
        100%{transform:translate(600,-300) scale(0);opacity:0}
      }
      @keyframes shoot3 {
        0%{transform:translate(0,0) scale(0);opacity:0}
        6%{transform:translate(20,-10) scale(0.5);opacity:0.4}
        12%{transform:translate(70,-35) scale(0.9);opacity:0.8}
        18%{transform:translate(130,-65) scale(1);opacity:1}
        30%{transform:translate(240,-120) scale(0.8);opacity:0.5}
        50%{transform:translate(400,-200) scale(0.3);opacity:0.1}
        100%{transform:translate(700,-350) scale(0);opacity:0}
      }

      @keyframes textGlow {
        0%,100%{filter:drop-shadow(0 0 6px rgba(100,200,255,0.5)) drop-shadow(0 0 12px rgba(80,180,255,0.3))}
        50%{filter:drop-shadow(0 0 10px rgba(120,220,255,0.8)) drop-shadow(0 0 20px rgba(100,200,255,0.5)) drop-shadow(0 0 40px rgba(60,160,255,0.2))}
      }

      @keyframes floatParticle1 {
        0%{transform:translate(0,0) rotate(0deg)}
        25%{transform:translate(30,-20) rotate(90deg)}
        50%{transform:translate(10,-35) rotate(180deg)}
        75%{transform:translate(-25,-15) rotate(270deg)}
        100%{transform:translate(0,0) rotate(360deg)}
      }
      @keyframes floatParticle2 {
        0%{transform:translate(0,0) rotate(0deg)}
        33%{transform:translate(-20,-25) rotate(120deg)}
        66%{transform:translate(-5,-10) rotate(240deg)}
        100%{transform:translate(0,0) rotate(360deg)}
      }

      @keyframes asteroidFloat {
        0%{transform:translate(0,0) rotate(0deg)}
        20%{transform:translate(60,10) rotate(70deg)}
        45%{transform:translate(100,-20) rotate(160deg)}
        65%{transform:translate(40,-30) rotate(230deg)}
        85%{transform:translate(-20,-10) rotate(300deg)}
        100%{transform:translate(0,0) rotate(360deg)}
      }

      @keyframes auraSpin1 { 100%{transform:rotate(360deg)} }
      @keyframes auraSpin2 { 100%{transform:rotate(-360deg)} }

      .star-particle { animation: twinkle1 3s ease-in-out infinite; }
      .star-particle-fast { animation: twinkle2 1.8s ease-in-out infinite; }
      .star-particle-slow { animation: twinkle3 5s ease-in-out infinite; }
      .star-particle-var { animation: twinkle4 4.2s ease-in-out infinite; }
    </style>
  </defs>

  <!-- ════════════════ L1: 深空背景 ════════════════ -->
  <rect width="1200" height="700" fill="url(#deepSpace)"/>

  <!-- ════════════════ L2: 流体星云 ════════════════ -->
  <!-- 星云1：紫色大范围 -->
  <ellipse cx="400" cy="280" rx="280" ry="200" fill="#6a0dad" opacity="0.35" filter="url(#nebulaFluid1)">
    <animate attributeName="opacity" values="0.3;0.4;0.28;0.35;0.3" dur="30s" repeatCount="indefinite"/>
  </ellipse>
  <ellipse cx="500" cy="240" rx="200" ry="150" fill="#4a0080" opacity="0.25" filter="url(#nebulaFluid2)"/>

  <!-- 星云2：蓝紫区域 -->
  <ellipse cx="750" cy="320" rx="250" ry="180" fill="#1a3a8a" opacity="0.3" filter="url(#nebulaFluid2)">
    <animate attributeName="opacity" values="0.25;0.35;0.22;0.3;0.25" dur="36s" repeatCount="indefinite"/>
  </ellipse>

  <!-- 星云3：粉紫色点缀 -->
  <ellipse cx="550" cy="350" rx="180" ry="120" fill="#8a2a6a" opacity="0.2" filter="url(#nebulaFluid3)">
    <animate attributeName="opacity" values="0.15;0.25;0.18;0.22;0.15" dur="40s" repeatCount="indefinite"/>
  </ellipse>

  <!-- 星云4：深蓝扩散 -->
  <ellipse cx="650" cy="200" rx="320" ry="160" fill="#0a2a6a" opacity="0.25" filter="url(#nebulaFluid1)"/>

  <!-- 星云5：中心附近暖色 -->
  <ellipse cx="600" cy="300" rx="150" ry="100" fill="#cc4400" opacity="0.08" filter="url(#nebulaFluid3)">
    <animate attributeName="opacity" values="0.06;0.1;0.05;0.08;0.06" dur="20s" repeatCount="indefinite"/>
  </ellipse>

  <!-- ════════════════ L3: 远景星空 ════════════════ -->
  <g id="starfield">
    <circle cx="45" cy="30" r="1.2" fill="#fff" class="star-particle" style="animation-delay:0s"/>
    <circle cx="120" cy="85" r="0.7" fill="#aaccff" class="star-particle-fast" style="animation-delay:0.3s"/>
    <circle cx="200" cy="15" r="1.5" fill="#fff" class="star-particle-slow" style="animation-delay:0.8s"/>
    <circle cx="280" cy="55" r="0.5" fill="#ffddcc" class="star-particle" style="animation-delay:1.2s"/>
    <circle cx="340" cy="120" r="1.8" fill="#ffffff" class="star-particle-var" style="animation-delay:0.5s"/>
    <circle cx="50" cy="180" r="0.8" fill="#aaddff" class="star-particle-fast" style="animation-delay:1.7s"/>
    <circle cx="160" cy="150" r="1.0" fill="#ffffff" class="star-particle-slow" style="animation-delay:2.1s"/>
    <circle cx="90" cy="250" r="0.6" fill="#ffccaa" class="star-particle" style="animation-delay:0.9s"/>
    <circle cx="250" cy="200" r="1.4" fill="#ffffff" class="star-particle-var" style="animation-delay:2.5s"/>

    <circle cx="850" cy="40" r="1.1" fill="#ffffff" class="star-particle-fast" style="animation-delay:0.2s"/>
    <circle cx="950" cy="90" r="1.6" fill="#ccddff" class="star-particle-slow" style="animation-delay:1.1s"/>
    <circle cx="1020" cy="25" r="0.7" fill="#ffffff" class="star-particle" style="animation-delay:1.8s"/>
    <circle cx="1100" cy="70" r="1.3" fill="#ffddaa" class="star-particle-var" style="animation-delay:0.7s"/>
    <circle cx="1150" cy="140" r="0.5" fill="#aaddff" class="star-particle-fast" style="animation-delay:2.2s"/>
    <circle cx="780" cy="130" r="0.9" fill="#ffffff" class="star-particle-slow" style="animation-delay:3.0s"/>
    <circle cx="900" cy="170" r="1.7" fill="#ffffff" class="star-particle" style="animation-delay:1.4s"/>
    <circle cx="1050" cy="200" r="0.6" fill="#eeccff" class="star-particle-fast" style="animation-delay:2.8s"/>
    <circle cx="1120" cy="250" r="1.0" fill="#ffffff" class="star-particle-var" style="animation-delay:0.4s"/>

    <circle cx="30" cy="400" r="0.8" fill="#ffffff" class="star-particle-slow" style="animation-delay:1.5s"/>
    <circle cx="100" cy="350" r="1.5" fill="#bbddff" class="star-particle-fast" style="animation-delay:2.0s"/>
    <circle cx="180" cy="420" r="0.5" fill="#ffffff" class="star-particle" style="animation-delay:3.2s"/>
    <circle cx="80" cy="500" r="1.2" fill="#ffccdd" class="star-particle-var" style="animation-delay:1.9s"/>
    <circle cx="220" cy="380" r="0.7" fill="#ffffff" class="star-particle-fast" style="animation-delay:0.6s"/>

    <circle cx="1080" cy="380" r="1.4" fill="#ffffff" class="star-particle" style="animation-delay:2.4s"/>
    <circle cx="1150" cy="450" r="0.8" fill="#ccddff" class="star-particle-slow" style="animation-delay:1.3s"/>
    <circle cx="980" cy="500" r="1.1" fill="#ffffff" class="star-particle-var" style="animation-delay:3.1s"/>
    <circle cx="1100" cy="550" r="0.6" fill="#ffddbb" class="star-particle-fast" style="animation-delay:0.8s"/>
    <circle cx="1050" cy="620" r="1.8" fill="#ffffff" class="star-particle-slow" style="animation-delay:2.6s"/>

    <circle cx="350" cy="580" r="0.7" fill="#ffffff" class="star-particle" style="animation-delay:1.6s"/>
    <circle cx="450" cy="620" r="1.3" fill="#aaccee" class="star-particle-fast" style="animation-delay:2.9s"/>
    <circle cx="550" cy="550" r="0.5" fill="#ffffff" class="star-particle-var" style="animation-delay:0.2s"/>
    <circle cx="650" cy="590" r="1.0" fill="#ffffff" class="star-particle-slow" style="animation-delay:3.3s"/>
    <circle cx="750" cy="630" r="0.9" fill="#eeddff" class="star-particle-fast" style="animation-delay:1.0s"/>
    <circle cx="850" cy="560" r="1.6" fill="#ffffff" class="star-particle" style="animation-delay:2.1s"/>

    <circle cx="300" cy="50" r="0.4" fill="#ffffff" class="star-particle-fast" style="animation-delay:3.5s"/>
    <circle cx="500" cy="80" r="0.6" fill="#ddeeff" class="star-particle-slow" style="animation-delay:1.1s"/>
    <circle cx="700" cy="60" r="1.1" fill="#ffffff" class="star-particle-var" style="animation-delay:2.7s"/>
    <circle cx="1000" cy="110" r="0.4" fill="#ffffff" class="star-particle" style="animation-delay:0.1s"/>
    <circle cx="400" cy="160" r="0.5" fill="#ffeedd" class="star-particle-fast" style="animation-delay:1.9s"/>
  </g>

  <!-- ════════════════ L4: 轨道参考线 ════════════════ -->
  <g opacity="0.08">
    <ellipse cx="600" cy="300" rx="170" ry="100" fill="none" stroke="#88aacc" stroke-width="1" stroke-dasharray="6,8"/>
    <ellipse cx="600" cy="300" rx="270" ry="160" fill="none" stroke="#88aacc" stroke-width="0.8" stroke-dasharray="4,12"/>
    <ellipse cx="600" cy="300" rx="370" ry="220" fill="none" stroke="#88aacc" stroke-width="0.7" stroke-dasharray="3,15"/>
    <ellipse cx="600" cy="300" rx="470" ry="280" fill="none" stroke="#88aacc" stroke-width="0.6" stroke-dasharray="2,18"/>
  </g>

  <!-- ════════════════ L5: 中央恒星 ════════════════ -->
  <g transform="translate(600,300)">

    <!-- 外脉冲光晕 -->
    <circle cx="0" cy="0" r="130" fill="url(#starOuterGlow)" style="animation:starPulseOuter 3.5s ease-in-out infinite"/>

    <!-- 光线束旋转 -->
    <g style="animation:starRotate 16s cubic-bezier(0.45,0,0.55,1) infinite">
      <!-- 16道光线 -->
      <g opacity="0.5">
        <polygon points="0,-180 -8,-20 0,-25 8,-20" fill="#ffcc00" opacity="0.7" mask="url(#rayMask)"/>
        <polygon points="0,-180 -8,-20 0,-25 8,-20" fill="#ffcc00" opacity="0.7" transform="rotate(22.5)" mask="url(#rayMask)"/>
        <polygon points="0,-180 -7,-20 0,-25 7,-20" fill="#ffaa00" opacity="0.5" transform="rotate(45)" mask="url(#rayMask)"/>
        <polygon points="0,-180 -9,-20 0,-25 9,-20" fill="#ffcc00" opacity="0.7" transform="rotate(67.5)" mask="url(#rayMask)"/>
        <polygon points="0,-180 -8,-20 0,-25 8,-20" fill="#ffaa00" opacity="0.5" transform="rotate(90)" mask="url(#rayMask)"/>
        <polygon points="0,-180 -7,-20 0,-25 7,-20" fill="#ffcc00" opacity="0.7" transform="rotate(112.5)" mask="url(#rayMask)"/>
        <polygon points="0,-180 -9,-20 0,-25 9,-20" fill="#ffaa00" opacity="0.5" transform="rotate(135)" mask="url(#rayMask)"/>
        <polygon points="0,-180 -8,-20 0,-25 8,-20" fill="#ffcc00" opacity="0.7" transform="rotate(157.5)" mask="url(#rayMask)"/>
        <polygon points="0,-180 -7,-20 0,-25 7,-20" fill="#ffaa00" opacity="0.5" transform="rotate(180)" mask="url(#rayMask)"/>
        <polygon points="0,-180 -9,-20 0,-25 9,-20" fill="#ffcc00" opacity="0.7" transform="rotate(202.5)" mask="url(#rayMask)"/>
        <polygon points="0,-180 -8,-20 0,-25 8,-20" fill="#ffaa00" opacity="0.5" transform="rotate(225)" mask="url(#rayMask)"/>
        <polygon points="0,-180 -7,-20 0,-25 7,-20" fill="#ffcc00" opacity="0.7" transform="rotate(247.5)" mask="url(#rayMask)"/>
        <polygon points="0,-180 -9,-20 0,-25 9,-20" fill="#ffaa00" opacity="0.5" transform="rotate(270)" mask="url(#rayMask)"/>
        <polygon points="0,-180 -8,-20 0,-25 8,-20" fill="#ffcc00" opacity="0.7" transform="rotate(292.5)" mask="url(#rayMask)"/>
        <polygon points="0,-180 -7,-20 0,-25 7,-20" fill="#ffaa00" opacity="0.5" transform="rotate(315)" mask="url(#rayMask)"/>
        <polygon points="0,-180 -9,-20 0,-25 9,-20" fill="#ffcc00" opacity="0.7" transform="rotate(337.5)" mask="url(#rayMask)"/>
      </g>
    </g>

    <!-- 光线束 mask -->
    <mask id="rayMask">
      <rect x="-200" y="-200" width="400" height="400" fill="black"/>
      <circle cx="0" cy="0" r="180" fill="url(#rayFade)"/>
    </mask>

    <!-- 内发光层 -->
    <circle cx="0" cy="0" r="70" fill="url(#starInnerGlow)" style="animation:starPulse 3s ease-in-out infinite"/>

    <!-- 恒星核心 -->
    <circle cx="0" cy="0" r="35" fill="url(#starCore)" filter="url(#glowIntense)"/>

    <!-- 极亮白核 -->
    <circle cx="0" cy="0" r="12" fill="#ffffff" filter="url(#glowSoft)"/>

  </g>

  <!-- ════════════════ L6: 公转行星 ════════════════ -->

  <!-- 行星1：近轨岩石行星（半径170，周期8s） -->
  <g transform="translate(600,300)" style="animation:orbit1 8s linear infinite">
    <g transform="translate(170,0)">
      <g style="animation:selfSpin1 12s linear infinite">
        <circle cx="0" cy="0" r="8" fill="url(#planet1Grad)" filter="url(#planetShadow)"/>
        <!-- 行星表面纹理 -->
        <circle cx="-2" cy="-2" r="2.5" fill="#c47a5a" opacity="0.4"/>
        <circle cx="3" cy="1" r="1.5" fill="#6b2a1a" opacity="0.3"/>
      </g>
    </g>
  </g>

  <!-- 行星2：中轨蓝绿类地行星（半径270，周期15s）+ 小卫星 -->
  <g transform="translate(600,300)" style="animation:orbit2 15s linear infinite">
    <g transform="translate(270,0)">
      <g style="animation:selfSpin2 18s linear infinite">
        <!-- 行星主体 -->
        <circle cx="0" cy="0" r="14" fill="url(#planet2Grad)" filter="url(#planetShadow)"/>
        <!-- 大陆斑块 -->
        <ellipse cx="3" cy="-4" rx="5" ry="3.5" fill="#4a9a5a" opacity="0.35"/>
        <ellipse cx="-2" cy="5" rx="4" ry="2.5" fill="#3a8a4a" opacity="0.3"/>
        <!-- 极地冰盖 -->
        <ellipse cx="0" cy="-12" rx="6" ry="2" fill="#cceeff" opacity="0.3"/>
        <!-- 大气光晕 -->
        <circle cx="0" cy="0" r="16" fill="none" stroke="#88ccff" stroke-width="1.5" opacity="0.25"/>
      </g>
      <!-- 小卫星 -->
      <g style="animation:moonOrbit 3s linear infinite">
        <circle cx="22" cy="0" r="3" fill="#aaa" opacity="0.7"/>
      </g>
    </g>
  </g>

  <!-- 行星3：中远轨带环行星（半径370，周期25s） -->
  <g transform="translate(600,300)" style="animation:orbit3 25s linear infinite">
    <g transform="translate(370,0)">
      <!-- 行星环（倾斜） -->
      <g transform="rotate(-20)">
        <ellipse cx="0" cy="0" rx="24" ry="7" fill="none" stroke="#daa520" stroke-width="3" opacity="0.5"/>
        <ellipse cx="0" cy="0" rx="20" ry="5.5" fill="none" stroke="#eedd88" stroke-width="1.5" opacity="0.35"/>
        <ellipse cx="0" cy="0" rx="28" ry="8.5" fill="none" stroke="#b8860b" stroke-width="2" opacity="0.3"/>
      </g>
      <!-- 行星主体 -->
      <g style="animation:selfSpin3 22s linear infinite">
        <circle cx="0" cy="0" r="12" fill="url(#planet3Grad)" filter="url(#planetShadow)"/>
        <!-- 云带 -->
        <ellipse cx="0" cy="-3" rx="11" ry="2.5" fill="#eedd88" opacity="0.2"/>
        <ellipse cx="0" cy="4" rx="10" ry="2" fill="#b8860b" opacity="0.25"/>
      </g>
    </g>
  </g>

  <!-- 行星4：远轨气态巨行星（半径470，周期38s） -->
  <g transform="translate(600,300)" style="animation:orbit4 38s linear infinite">
    <g transform="translate(470,0)">
      <g style="animation:selfSpin4 28s linear infinite">
        <!-- 主体 -->
        <ellipse cx="0" cy="0" rx="22" ry="18" fill="url(#planet4Grad)" filter="url(#planetShadow)"/>
        <!-- 气态条纹 -->
        <ellipse cx="0" cy="-6" rx="20" ry="4" fill="#aaddff33"/>
        <ellipse cx="0" cy="0" rx="21" ry="3.5" fill="#4488bb33"/>
        <ellipse cx="0" cy="6" rx="18" ry="4" fill="#22669933"/>
        <ellipse cx="0" cy="-2" rx="19" ry="2" fill="#ffffff15"/>
        <!-- 大气光晕 -->
        <ellipse cx="0" cy="0" rx="25" ry="21" fill="none" stroke="#88ccff" stroke-width="1" opacity="0.2"/>
        <!-- 大红斑 -->
        <ellipse cx="5" cy="4" rx="5" ry="3" fill="#ff6644" opacity="0.4"/>
      </g>
    </g>
  </g>

  <!-- ════════════════ L7: 流星 ════════════════ -->
  <!-- 流星1 -->
  <g style="animation:shoot1 8s cubic-bezier(0.4,0,0.2,1) infinite">
    <line x1="0" y1="0" x2="-60" y2="30" stroke="url(#shootingStarTrail)" stroke-width="2" stroke-linecap="round"/>
    <circle cx="0" cy="0" r="1.5" fill="#ffffff" filter="url(#glowSoft)"/>
  </g>

  <!-- 流星2 -->
  <g style="animation:shoot2 11s cubic-bezier(0.4,0,0.2,1) infinite; animation-delay:4s">
    <line x1="0" y1="0" x2="-45" y2="22" stroke="url(#shootingStarTrail)" stroke-width="1.5" stroke-linecap="round"/>
    <circle cx="0" cy="0" r="1" fill="#ffffff" filter="url(#glowSoft)"/>
  </g>

  <!-- 流星3 -->
  <g style="animation:shoot3 13s cubic-bezier(0.4,0,0.2,1) infinite; animation-delay:7s">
    <line x1="0" y1="0" x2="-55" y2="28" stroke="url(#shootingStarTrail)" stroke-width="1.8" stroke-linecap="round"/>
    <circle cx="0" cy="0" r="1.3" fill="#ffffff" filter="url(#glowSoft)"/>
  </g>

  <!-- ════════════════ L8: 文字叠加层 ════════════════ -->
  <g transform="translate(600,580)">
    <!-- 半透明背景面板 -->
    <rect x="-280" y="-55" width="560" height="110" rx="16" fill="#000820aa" stroke="#33446666" stroke-width="1"/>
    <rect x="-280" y="-55" width="560" height="110" rx="16" fill="none" stroke="#66779933" stroke-width="0.5"/>

    <!-- 装饰线 -->
    <line x1="-240" y1="-45" x2="240" y2="-45" stroke="url(#starOuterGlow)" stroke-width="0.5" opacity="0.4"/>

    <!-- 姓名 -->
    <text x="0" y="-8" text-anchor="middle" font-family="Arial,Helvetica,sans-serif" font-size="26" font-weight="bold" fill="#e8eeff" filter="url(#glowText)">
      Yaxin Zhao ·· 赵雅欣
    </text>

    <!-- 身份定位 -->
    <text x="0" y="24" text-anchor="middle" font-family="Arial,Helvetica,sans-serif" font-size="14" fill="#88aacc">
      CS @ Nankai University ·· AI Agent Developer ·· Information Security
    </text>

    <!-- 副标题 -->
    <text x="0" y="44" text-anchor="middle" font-family="Arial,Helvetica,sans-serif" font-size="11" fill="#556688">
      Building the future ·· one star at a time ✦
    </text>

    <!-- 装饰线 -->
    <line x1="-240" y1="52" x2="240" y2="52" stroke="url(#starOuterGlow)" stroke-width="0.5" opacity="0.4"/>
  </g>

  <!-- ════════════════ L9: 前景漂浮粒子 ════════════════ -->
  <!-- 大颗粒漂浮物，增加景深感 -->
  <g>
    <circle cx="180" cy="150" r="3" fill="#4488ff" opacity="0.25" filter="url(#glowSoft)" style="animation:floatParticle1 18s ease-in-out infinite"/>
    <circle cx="950" cy="480" r="2.5" fill="#ff66aa" opacity="0.2" filter="url(#glowSoft)" style="animation:floatParticle2 22s ease-in-out infinite"/>
    <circle cx="300" cy="500" r="2" fill="#44ddff" opacity="0.2" filter="url(#glowSoft)" style="animation:asteroidFloat 26s ease-in-out infinite"/>
    <circle cx="880" cy="120" r="1.8" fill="#cc88ff" opacity="0.2" filter="url(#glowSoft)" style="animation:floatParticle1 20s ease-in-out infinite; animation-delay:5s"/>
  </g>

</svg>

<br/>

<!-- ═══════════════════════════════════════════════ -->
<!--          PROJECT SHOWCASE（项目展示）           -->
<!-- ═══════════════════════════════════════════════ -->

| 🚀 Featured Projects | |
|---|---|
| **[Mouse-Select-Translator](https://github.com/zhaoyaxinxin/Mouse-Select-Translator)**<br/>Windows 划词翻译，集成 DeepSeek + OCR ·· C# | **[PsyAI](https://github.com/zhaoyaxinxin/PsyAI)**<br/>AI心理Coding创新大赛作品 ·· TypeScript |
| **[Deep-Research](https://github.com/zhaoyaxinxin/Deep-Research)**<br/>深度研究工具 ·· Python | **[MiroFish](https://github.com/zhaoyaxinxin/MiroFish)**<br/>群体智能引擎，预测万物 ·· Swarm Intelligence |
| **[ai-music-generator](https://github.com/zhaoyaxinxin/ai-music-generator)**<br/>基于 Suno + DeepSeek 的 AI 音乐生成 ·· JavaScript | **[NKU_Course_Note](https://github.com/zhaoyaxinxin/NKU_Course_Note)**<br/>📚 南开大学 信息安全课程笔记 |

<br/>

<div align="center">

### 🛠️ Tech Constellation

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![C#](https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=csharp&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![DeepSeek](https://img.shields.io/badge/DeepSeek-4F46E5?style=flat-square&logo=data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjQiIGhlaWdodD0iMjQiIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0id2hpdGUiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+PGNpcmNsZSBjeD0iMTIiIGN5PSIxMiIgcj0iMTAiLz48L3N2Zz4=&logoColor=white)
![Suno](https://img.shields.io/badge/Suno-FF4F00?style=flat-square&logo=data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjQiIGhlaWdodD0iMjQiIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0id2hpdGUiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+PGNpcmNsZSBjeD0iMTIiIGN5PSIxMiIgcj0iMTAiLz48L3N2Zz4=&logoColor=white)
![Transformer](https://img.shields.io/badge/Transformer-FF6F00?style=flat-square&logo=transformers&logoColor=white)

![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white)
![Windows](https://img.shields.io/badge/Windows-0078D4?style=flat-square&logo=windows&logoColor=white)

<br/>

<img src="https://komarev.com/ghpvc/?username=zhaoyaxinxin&style=flat-square&color=4a4a8a" alt="visitors"/>

<p style="color:#445566;font-size:11px;margin-top:20px">
✦ Exploring the cosmos of code ·· one commit at a time ✦
</p>

</div>

</div>
