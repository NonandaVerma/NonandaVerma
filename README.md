<svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 920 2220" width="100%" height="2220">
  <defs>
    <!-- Master Brochure Cyan-Blue Canvas Gradient -->
    <linearGradient id="brochureBg" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="#1489CA" />
      <stop offset="45%" stop-color="#117EBA" />
      <stop offset="100%" stop-color="#0E6B9E" />
    </linearGradient>

    <!-- Animated Outer Border Flow Gradient -->
    <linearGradient id="borderFlow" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#FF7704">
        <animate attributeName="stop-color" values="#FF7704;#FFFFFF;#1489CA;#FF7704" dur="7s" repeatCount="indefinite" />
      </stop>
      <stop offset="50%" stop-color="#FFFFFF">
        <animate attributeName="stop-color" values="#FFFFFF;#FF7704;#1489CA;#FFFFFF" dur="7s" repeatCount="indefinite" />
      </stop>
      <stop offset="100%" stop-color="#1489CA">
        <animate attributeName="stop-color" values="#1489CA;#F6530F;#FF7704;#1489CA" dur="7s" repeatCount="indefinite" />
      </stop>
    </linearGradient>

    <!-- Card Soft Drop Shadow Filter -->
    <filter id="cardShadow" x="-10%" y="-10%" width="120%" height="125%">
      <feDropShadow dx="0" dy="14" stdDeviation="18" flood-color="#000000" flood-opacity="0.22" />
    </filter>

    <!-- Clip Paths for Cards (Rounded corners + Bottom callout bar) -->
    <clipPath id="cardClip1"><rect x="35" y="320" width="850" height="505" rx="26" /></clipPath>
    <clipPath id="cardClip2"><rect x="35" y="895" width="850" height="525" rx="26" /></clipPath>
    <clipPath id="cardClip3"><rect x="35" y="1495" width="850" height="525" rx="26" /></clipPath>

    <!-- Master Clip for Rounded Canvas & Animated Waves -->
    <clipPath id="masterClip"><rect x="0" y="0" width="920" height="2220" rx="28" /></clipPath>
    <clipPath id="waveClip"><rect x="0" y="2060" width="920" height="160" rx="28" /></clipPath>
  </defs>

  <style>
    @keyframes panelBreathe {
      0%, 100% {
        stroke-opacity: 0.65;
        stroke-width: 2.2;
      }
      50% {
        stroke-opacity: 1;
        stroke-width: 3.8;
      }
    }
    .panel-container {
      animation: panelBreathe 5s ease-in-out infinite;
    }
    .main-title {
      font-family: -apple-system, BlinkMacSystemFont, 'Montserrat', 'Segoe UI', Roboto, sans-serif;
      font-size: 50px;
      font-weight: 900;
      letter-spacing: 2.5px;
      text-transform: uppercase;
      fill: #FFFFFF;
      filter: drop-shadow(0 4px 10px rgba(0, 0, 0, 0.25));
    }
    .btn-text {
      font-family: -apple-system, BlinkMacSystemFont, 'Montserrat', 'Segoe UI', Roboto, sans-serif;
      font-size: 13px;
      font-weight: 800;
      letter-spacing: 1.4px;
      fill: #FFFFFF;
    }
    .card-title {
      font-family: -apple-system, BlinkMacSystemFont, 'Montserrat', 'Segoe UI', Roboto, sans-serif;
      font-size: 25px;
      font-weight: 900;
      letter-spacing: 1px;
      text-transform: uppercase;
      fill: #FF7704;
    }
    .body-lead {
      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
      font-size: 15px;
      line-height: 1.7;
      font-weight: 500;
      fill: #334155;
    }
    .bullet-bold {
      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
      font-size: 14px;
      font-weight: 700;
      fill: #0F172A;
    }
    .bullet-desc {
      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
      font-size: 14px;
      font-weight: 400;
      fill: #475569;
    }
    .quote-text {
      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
      font-size: 15px;
      font-weight: 600;
      fill: #FFFFFF;
    }
    .quad-title {
      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
      font-size: 15.5px;
      font-weight: 800;
      letter-spacing: 0.5px;
      text-transform: uppercase;
      fill: #0F172A;
    }
    .quad-sub {
      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
      font-size: 13px;
      font-style: italic;
      fill: #64748B;
    }
    .badge-text {
      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
      font-size: 12px;
      font-weight: 700;
      letter-spacing: 0.3px;
      fill: #FFFFFF;
    }
    .proj-title {
      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
      font-size: 15.5px;
      font-weight: 800;
      fill: #0F172A;
    }
    .proj-tags {
      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
      font-size: 12px;
      font-weight: 700;
      letter-spacing: 0.6px;
      fill: #1489CA;
    }
    .proj-desc {
      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
      font-size: 13.5px;
      font-weight: 400;
      line-height: 1.6;
      fill: #475569;
    }
  </style>

  <g clip-path="url(#masterClip)">
    <!-- 1. FULL BROCHURE BLUE CANVAS WITH BREATHING BORDER -->
    <rect x="0" y="0" width="920" height="2220" fill="url(#brochureBg)" />
    <rect class="panel-container" x="3" y="3" width="914" height="2214" rx="26" fill="none" stroke="url(#borderFlow)" stroke-width="2.5" />

    <!-- ==================================================== -->
    <!-- TOP HERO SECTION (Spacious, Centered & Animated)    -->
    <!-- ==================================================== -->
    <g transform="translate(0, 48)">
      <!-- Main Title: Nonanda Verma (Crisp, Solid Pure White - ZERO orange haze!) -->
      <text x="50%" y="45" text-anchor="middle" class="main-title">NONANDA VERMA</text>

      <!-- True Typewriter Character-by-Character TextPath Animation -->
      <g transform="translate(110, 65)">
        <!-- Line 1: DESIGNER BY EYE. DEVELOPER BY CODE. -->
        <path id="typePath0">
          <animate id="anim0" attributeName="d" begin="0s;anim2.end" dur="4000ms" fill="remove"
            values="m0,22 h0 ; m0,22 h700 ; m0,22 h700 ; m0,22 h0" keyTimes="0;0.52;0.88;1" />
        </path>
        <text font-family="-apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif" fill="#FFFFFF" font-size="15.5" font-weight="700" letter-spacing="3.2px" dominant-baseline="middle" x="50%" text-anchor="middle">
          <textPath href="#typePath0" xlink:href="#typePath0">
            DESIGNER BY EYE. DEVELOPER BY CODE.
          </textPath>
        </text>

        <!-- Line 2: FULL-STACK ARCHITECT + AI SYSTEMS ENGINEER -->
        <path id="typePath1">
          <animate id="anim1" attributeName="d" begin="anim0.end" dur="4000ms" fill="remove"
            values="m0,22 h0 ; m0,22 h700 ; m0,22 h700 ; m0,22 h0" keyTimes="0;0.52;0.88;1" />
        </path>
        <text font-family="-apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif" fill="#FFFFFF" font-size="15.5" font-weight="700" letter-spacing="3.2px" dominant-baseline="middle" x="50%" text-anchor="middle">
          <textPath href="#typePath1" xlink:href="#typePath1">
            FULL-STACK ARCHITECT + AI SYSTEMS ENGINEER
          </textPath>
        </text>

        <!-- Line 3: RESILIENT ARCHITECTURES WITH BESPOKE AESTHETICS -->
        <path id="typePath2">
          <animate id="anim2" attributeName="d" begin="anim1.end" dur="4000ms" fill="remove"
            values="m0,22 h0 ; m0,22 h700 ; m0,22 h700 ; m0,22 h0" keyTimes="0;0.52;0.88;1" />
        </path>
        <text font-family="-apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif" fill="#FFFFFF" font-size="15.5" font-weight="700" letter-spacing="3.2px" dominant-baseline="middle" x="50%" text-anchor="middle">
          <textPath href="#typePath2" xlink:href="#typePath2">
            RESILIENT ARCHITECTURES WITH BESPOKE AESTHETICS
          </textPath>
        </text>
      </g>

      <!-- Centered Divider Line with Breathing Opacity -->
      <line x1="220" y1="104" x2="700" y2="104" stroke="#FFFFFF" stroke-width="1.5" stroke-opacity="0.8">
        <animate attributeName="stroke-opacity" values="0.4; 0.9; 0.4" dur="4s" repeatCount="indefinite" />
      </line>

      <!-- 3 Spacious Pill Buttons (Centered with generous gaps) -->
      <g transform="translate(225, 130)">
        <!-- LinkedIn -->
        <rect x="0" y="0" width="135" height="42" rx="21" fill="#0A5B9E" stroke="#FFFFFF" stroke-width="1.8" />
        <text x="67.5" y="26" text-anchor="middle" class="btn-text">LINKEDIN</text>

        <!-- Let's Connect -->
        <rect x="155" y="0" width="160" height="42" rx="21" fill="#070A12" stroke="#FFFFFF" stroke-width="1.8" />
        <text x="235" y="26" text-anchor="middle" class="btn-text">LET'S CONNECT</text>

        <!-- Portfolio -->
        <rect x="335" y="0" width="135" height="42" rx="21" fill="#FF7704" stroke="#FFFFFF" stroke-width="1.8" />
        <text x="402.5" y="26" text-anchor="middle" class="btn-text">PORTFOLIO</text>
      </g>
    </g>

    <!-- ==================================================== -->
    <!-- CARD 1: THE 30-SECOND DOWNLOAD (Generous 70px Gap)   -->
    <!-- ==================================================== -->
    <g clip-path="url(#cardClip1)">
      <!-- White Card Container (Expanded to 505px height) -->
      <rect x="35" y="320" width="850" height="505" rx="26" fill="#FFFFFF" filter="url(#cardShadow)" />

      <!-- Card Header: Animated Ticking Timer Icon & Bold Title -->
      <g transform="translate(90, 370)">
        <g stroke="#FF7704" stroke-width="3" fill="none" stroke-linecap="round" stroke-linejoin="round">
          <circle cx="16" cy="18" r="13">
            <animate attributeName="r" values="13; 14.5; 13" dur="2s" repeatCount="indefinite" />
          </circle>
          <line x1="16" y1="2" x2="16" y2="5" />
          <line x1="12" y1="2" x2="20" y2="2" />
          <line x1="16" y1="18" x2="22" y2="13" />
        </g>
        <text x="46" y="25" class="card-title">THE 30-SECOND DOWNLOAD</text>
      </g>

      <!-- Lead Paragraph with Generous White Space -->
      <text x="90" y="432" class="body-lead">
        <tspan x="90" dy="0">I engineer resilient full-stack systems, custom cryptographic identity protocols, and autonomous AI agent workflows — then</tspan>
        <tspan x="90" dy="26">wrap them in high-converting, pixel-perfect design systems. Zero boilerplate fluff, zero sloppy layouts.</tspan>
      </text>

      <!-- Bullet Points (Spaced by generous 55px gaps) -->
      <g transform="translate(90, 502)">
        <circle cx="7" cy="7" r="5.5" fill="#1489CA" />
        <text x="25" y="11">
          <tspan class="bullet-bold">Architectural Depth: </tspan>
          <tspan class="bullet-desc">From engineering in-house enterprise OAuth2 Identity Providers (IdP) with cryptographic JWT/JWE lifecycles,</tspan>
        </text>
        <text x="25" y="29" class="bullet-desc">to orchestrating local AI agent CLI execution environments with real-time WebSocket pipelines.</text>
      </g>

      <g transform="translate(90, 558)">
        <circle cx="7" cy="7" r="5.5" fill="#FF7704" />
        <text x="25" y="11">
          <tspan class="bullet-bold">Agentic AI &amp; RAG: </tspan>
          <tspan class="bullet-desc">Creator of ENVI, an autonomous AI portfolio command center featuring 5-tier zero-downtime failover,</tspan>
        </text>
        <text x="25" y="29" class="bullet-desc">Python FastAPI, LangGraph StateGraphs, and ChromaDB 768-dimensional vector retrieval.</text>
      </g>

      <g transform="translate(90, 614)">
        <circle cx="7" cy="7" r="5.5" fill="#0A5B9E" />
        <text x="25" y="11">
          <tspan class="bullet-bold">Visual Instincts: </tspan>
          <tspan class="bullet-desc">3rd Runner-Up nationwide in the Government of India / MyGov IHRC National Logo Design Competition.</tspan>
        </text>
        <text x="25" y="29" class="bullet-desc">Every layout I ship is disciplined, responsive, and performance-tuned.</text>
      </g>

      <g transform="translate(90, 670)">
        <circle cx="7" cy="7" r="5.5" fill="#070A12" />
        <text x="25" y="11">
          <tspan class="bullet-bold">Academic Rigor: </tspan>
          <tspan class="bullet-desc">Master of Computer Applications (75% First Class Distinction) &amp; BSc Biotechnology (92% Distinction Honours).</tspan>
        </text>
      </g>

      <!-- Bottom Orange Quote Bar (Generous 65px Height & Padding) -->
      <g transform="translate(35, 740)">
        <rect x="0" y="0" width="850" height="65" fill="#FF7704" />
        <text x="50%" y="40" text-anchor="middle" class="quote-text" font-style="italic">"Most developers either dread CSS or run away from distributed backend logic. I live comfortably in the middle."</text>
      </g>
    </g>

    <!-- ==================================================== -->
    <!-- CARD 2: PRODUCTION ARCHITECTURE & STACK (Gap: 75px)  -->
    <!-- ==================================================== -->
    <g clip-path="url(#cardClip2)">
      <rect x="35" y="895" width="850" height="525" rx="26" fill="#FFFFFF" filter="url(#cardShadow)" />

      <!-- Card Header -->
      <g transform="translate(90, 942)">
        <g stroke="#FF7704" stroke-width="2.8" fill="none" stroke-linecap="round" stroke-linejoin="round">
          <path d="M14.7 6.3a1 1 0 0 0 0 1.4l1.6 1.6a1 1 0 0 0 1.4 0l3.77-3.77a6 6 0 0 1-7.94 7.94l-6.91 6.91a2.12 2.12 0 0 1-3-3l6.91-6.91a6 6 0 0 1 7.94-7.94l-3.76 3.76z"/>
        </g>
        <text x="46" y="24" class="card-title">PRODUCTION ARCHITECTURE &amp; STACK</text>
      </g>

      <!-- Quadrant 1: Frontend & Edge Delivery -->
      <g transform="translate(90, 1005)">
        <text x="0" y="16" class="quad-title">⚡ Frontend &amp; Edge Delivery</text>
        <text x="0" y="38" class="quad-sub">Pixel-perfect, accessible, 60fps edge rendering</text>
        <g transform="translate(0, 54)">
          <rect x="0" y="0" width="94" height="28" rx="14" fill="#070A12" /><text x="47" y="18" text-anchor="middle" class="badge-text">Next.js 16</text>
          <rect x="102" y="0" width="84" height="28" rx="14" fill="#1489CA" /><text x="144" y="18" text-anchor="middle" class="badge-text">React 19</text>
          <rect x="194" y="0" width="88" height="28" rx="14" fill="#D97706" /><text x="238" y="18" text-anchor="middle" class="badge-text">JavaScript</text>
          <rect x="290" y="0" width="96" height="28" rx="14" fill="#0284C7" /><text x="338" y="18" text-anchor="middle" class="badge-text">Tailwind v4</text>
        </g>
      </g>

      <!-- Quadrant 2: Backend, Systems & APIs -->
      <g transform="translate(500, 1005)">
        <text x="0" y="16" class="quad-title">⚙️ Backend, Systems &amp; APIs</text>
        <text x="0" y="38" class="quad-sub">Distributed microservices &amp; cryptographic security</text>
        <g transform="translate(0, 54)">
          <rect x="0" y="0" width="118" height="28" rx="14" fill="#059669" /><text x="59" y="18" text-anchor="middle" class="badge-text">Python FastAPI</text>
          <rect x="126" y="0" width="76" height="28" rx="14" fill="#16A34A" /><text x="164" y="18" text-anchor="middle" class="badge-text">Node.js</text>
          <rect x="210" y="0" width="78" height="28" rx="14" fill="#070A12" /><text x="249" y="18" text-anchor="middle" class="badge-text">ColdBox</text>
          <rect x="296" y="0" width="78" height="28" rx="14" fill="#EA580C" /><text x="335" y="18" text-anchor="middle" class="badge-text">OAuth2</text>
        </g>
      </g>

      <!-- Quadrant 3: Agentic AI & Vector Intelligence (68px row gap) -->
      <g transform="translate(90, 1155)">
        <text x="0" y="16" class="quad-title">🤖 Agentic AI &amp; Vector Intelligence</text>
        <text x="0" y="38" class="quad-sub">Multi-agent graphs, persistent memory &amp; LLM failover</text>
        <g transform="translate(0, 54)">
          <rect x="0" y="0" width="94" height="28" rx="14" fill="#FF7704" /><text x="47" y="18" text-anchor="middle" class="badge-text">LangGraph</text>
          <rect x="102" y="0" width="94" height="28" rx="14" fill="#DC2626" /><text x="149" y="18" text-anchor="middle" class="badge-text">ChromaDB</text>
          <rect x="204" y="0" width="96" height="28" rx="14" fill="#4D7C0F" /><text x="252" y="18" text-anchor="middle" class="badge-text">NVIDIA NIM</text>
          <rect x="308" y="0" width="70" height="28" rx="14" fill="#070A12" /><text x="343" y="18" text-anchor="middle" class="badge-text">Ollama</text>
        </g>
      </g>

      <!-- Quadrant 4: Cloud, DevOps & UI Systems -->
      <g transform="translate(500, 1155)">
        <text x="0" y="16" class="quad-title">☁️ Cloud, DevOps &amp; UI Systems</text>
        <text x="0" y="38" class="quad-sub">Containers, edge infrastructure &amp; brand design</text>
        <g transform="translate(0, 54)">
          <rect x="0" y="0" width="76" height="28" rx="14" fill="#0284C7" /><text x="38" y="18" text-anchor="middle" class="badge-text">Docker</text>
          <rect x="84" y="0" width="88" height="28" rx="14" fill="#15803D" /><text x="128" y="18" text-anchor="middle" class="badge-text">MongoDB</text>
          <rect x="180" y="0" width="96" height="28" rx="14" fill="#070A12" /><text x="228" y="18" text-anchor="middle" class="badge-text">Vercel Edge</text>
          <rect x="284" y="0" width="96" height="28" rx="14" fill="#0A5B9E" /><text x="332" y="18" text-anchor="middle" class="badge-text">UI Systems</text>
        </g>
      </g>

      <!-- Bottom Blue Callout Bar -->
      <g transform="translate(35, 1265)">
        <rect x="0" y="0" width="850" height="65" fill="#1489CA" />
        <text x="50%" y="40" text-anchor="middle" class="quote-text">Production-hardened architectures paired with pixel-perfect visual discipline.</text>
      </g>
    </g>

    <!-- ==================================================== -->
    <!-- CARD 3: FEATURED ENGINEERING SHOWCASE (Gap: 75px)    -->
    <!-- ==================================================== -->
    <g clip-path="url(#cardClip3)">
      <rect x="35" y="1495" width="850" height="525" rx="26" fill="#FFFFFF" filter="url(#cardShadow)" />

      <!-- Card Header -->
      <g transform="translate(90, 1542)">
        <g stroke="#FF7704" stroke-width="2.8" fill="none" stroke-linecap="round" stroke-linejoin="round">
          <path d="M4.5 16.5c-1.5 1.26-2 5-2 5s3.74-.5 5-2c.71-.84.7-2.13-.09-2.91a2.18 2.18 0 0 0-2.91-.09z"/>
          <path d="M12 15l-3-3a22 22 0 0 1 2-3.95A12.88 12.88 0 0 1 22 2c0 2.72-.78 7.5-6 11a22.35 22.35 0 0 1-4 2z"/>
        </g>
        <text x="46" y="24" class="card-title">FEATURED ENGINEERING SHOWCASE</text>
      </g>

      <!-- Project 1 -->
      <g transform="translate(90, 1605)">
        <text x="0" y="16" class="proj-title">🚀 Portfolio &amp; ENVI AI Command Center</text>
        <text x="0" y="38" class="proj-tags">NEXT.JS 16 • FASTAPI • LANGGRAPH • CHROMADB</text>
        <text x="0" y="60" class="proj-desc">5-tier zero-downtime LLM failover, 768-dim vector RAG memory,</text>
        <text x="0" y="80" class="proj-desc">and Cloudinary edge asset compression (f_auto, q_auto).</text>
      </g>

      <!-- Project 2 -->
      <g transform="translate(500, 1605)">
        <text x="0" y="16" class="proj-title">🔐 Custom OAuth2 Identity Provider (IdP)</text>
        <text x="0" y="38" class="proj-tags">COLDBOX • JWT / JWE • RSA-256 ROTATION • MSSQL</text>
        <text x="0" y="60" class="proj-desc">RFC 6749 compliant PKCE auth server with automated PEM key</text>
        <text x="0" y="80" class="proj-desc">rotation, eliminating recurring commercial identity SaaS costs.</text>
      </g>

      <!-- Project 3 (68px row gap) -->
      <g transform="translate(90, 1755)">
        <text x="0" y="16" class="proj-title">⚡ Agentic SSH Terminal Orchestrator</text>
        <text x="0" y="38" class="proj-tags">NODE.JS • EXPRESS • XTERM.JS • LOCAL OLLAMA</text>
        <text x="0" y="60" class="proj-desc">Sub-10ms bi-directional WebSocket ANSI streaming bridge routing</text>
        <text x="0" y="80" class="proj-desc">autonomous CLI agent workflows with persistent Tmux sessions.</text>
      </g>

      <!-- Project 4 -->
      <g transform="translate(500, 1755)">
        <text x="0" y="16" class="proj-title">📊 Schema-Driven Dynamic Dashboard</text>
        <text x="0" y="38" class="proj-tags">REACT • PLOTLY.JS • RECHARTS • MONGODB ATLAS</text>
        <text x="0" y="60" class="proj-desc">Low-code data analytics engine dynamically transforming raw JSON</text>
        <text x="0" y="80" class="proj-desc">and Mongo schemas into multi-axis charts with zero frontend rebuilds.</text>
      </g>

      <!-- Bottom Dark Callout Bar -->
      <g transform="translate(35, 1865)">
        <rect x="0" y="0" width="850" height="65" fill="#070A12" />
        <text x="50%" y="40" text-anchor="middle" class="quote-text">Engineered for fault-tolerance, sub-second latency, and measurable impact.</text>
      </g>
    </g>

    <!-- ==================================================== -->
    <!-- DYNAMIC UNDULATING WAVE FOOTER (NO BROKEN EDGES!)    -->
    <!-- ==================================================== -->
    <g clip-path="url(#waveClip)">
      <rect x="0" y="2060" width="920" height="160" fill="#1489CA" />

      <!-- Layer 1: White Undulating Rolling Wave (Seamless Morphing) -->
      <path fill="#FFFFFF" opacity="0.95">
        <animate attributeName="d" dur="8s" repeatCount="indefinite"
          values="M 0 2110 Q 230 2160 460 2110 T 920 2110 L 920 2220 L 0 2220 Z; M 0 2130 Q 230 2085 460 2130 T 920 2130 L 920 2220 L 0 2220 Z; M 0 2110 Q 230 2160 460 2110 T 920 2110 L 920 2220 L 0 2220 Z" />
      </path>

      <!-- Layer 2: Deep Navy Rolling Wave (Seamless Morphing - ZERO CUTOFF!) -->
      <path fill="#070A12" opacity="0.95">
        <animate attributeName="d" dur="6s" repeatCount="indefinite"
          values="M 0 2135 Q 230 2095 460 2145 T 920 2135 L 920 2220 L 0 2220 Z; M 0 2150 Q 230 2185 460 2125 T 920 2150 L 920 2220 L 0 2220 Z; M 0 2135 Q 230 2095 460 2145 T 920 2135 L 920 2220 L 0 2220 Z" />
      </path>

      <!-- Layer 3: Vibrant Orange Swoosh Wave (Seamless Morphing) -->
      <path fill="#FF7704">
        <animate attributeName="d" dur="5s" repeatCount="indefinite"
          values="M 0 2158 Q 230 2200 460 2158 T 920 2168 L 920 2220 L 0 2220 Z; M 0 2172 Q 230 2135 460 2180 T 920 2162 L 920 2220 L 0 2220 Z; M 0 2158 Q 230 2200 460 2158 T 920 2168 L 920 2220 L 0 2220 Z" />
      </path>
    </g>
  </g>
</svg>
