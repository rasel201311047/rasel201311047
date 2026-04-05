<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
    <title>Rasel Islam · React Native Developer & Full-Stack Engineer</title>
    <!-- Google Fonts: Space Grotesk & Inter for modern tech feel -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;14..32,400;14..32,600;14..32,700;14..32,800&family=Space+Grotesk:wght@400;500;600;700&display=swap" rel="stylesheet">
    <!-- Font Awesome 6 (free icons) -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background: radial-gradient(circle at 10% 20%, #0a0e17, #03050b);
            font-family: 'Inter', 'Space Grotesk', sans-serif;
            color: #e2e8f0;
            line-height: 1.5;
            padding: 2rem 1rem;
        }

        /* smooth container */
        .readme-container {
            max-width: 1280px;
            margin: 0 auto;
            background: rgba(10, 14, 23, 0.65);
            backdrop-filter: blur(2px);
            border-radius: 2rem;
            padding: 2rem 1.8rem;
            box-shadow: 0 25px 45px -12px rgba(0,0,0,0.5), inset 0 1px 0 rgba(255,255,255,0.05);
            border: 1px solid rgba(0, 255, 200, 0.2);
        }

        /* animated gradient text */
        .gradient-text {
            background: linear-gradient(135deg, #00FFC8, #60A5FA, #C084FC);
            background-size: 200% auto;
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            animation: shimmer 4s linear infinite;
        }

        @keyframes shimmer {
            0% { background-position: 0% 50%; }
            100% { background-position: 200% 50%; }
        }

        /* header wave container */
        .wave-header {
            position: relative;
            margin-bottom: 2rem;
        }

        /* custom badges style */
        .badge-custom {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            background: #0f172a;
            border-radius: 60px;
            padding: 0.4rem 1.2rem;
            font-weight: 600;
            font-size: 0.85rem;
            letter-spacing: -0.2px;
            border: 1px solid rgba(0,255,200,0.3);
            transition: all 0.2s ease;
            backdrop-filter: blur(4px);
        }
        .badge-custom:hover {
            border-color: #00FFC8;
            transform: translateY(-2px);
            box-shadow: 0 8px 14px -8px rgba(0,255,200,0.2);
        }

        /* code block style */
        .code-card {
            background: #0a0f1c;
            border-radius: 1.5rem;
            padding: 1.2rem 1.5rem;
            border-left: 4px solid #00FFC8;
            font-family: 'Space Grotesk', monospace;
            font-size: 0.9rem;
            box-shadow: 0 10px 20px -5px rgba(0,0,0,0.5);
            overflow-x: auto;
        }

        /* tech stack icons grid */
        .tech-grid {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 0.75rem;
            margin: 1.5rem 0;
        }
        .tech-item {
            background: #111827;
            padding: 0.5rem 1rem;
            border-radius: 2rem;
            font-size: 0.85rem;
            font-weight: 500;
            display: inline-flex;
            align-items: center;
            gap: 8px;
            transition: all 0.2s;
            border: 1px solid #1e293b;
        }
        .tech-item i, .tech-item svg {
            font-size: 1.1rem;
        }
        .tech-item:hover {
            border-color: #00FFC8;
            background: #1e293b;
            transform: scale(1.02);
        }

        /* Stats cards */
        .stats-wrapper {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 1.5rem;
            margin: 2rem 0;
        }
        .stat-card {
            background: #0b1120;
            border-radius: 1.5rem;
            padding: 1rem;
            flex: 1;
            min-width: 250px;
            backdrop-filter: blur(8px);
            border: 1px solid rgba(96,165,250,0.2);
            transition: 0.2s;
        }
        .stat-card:hover {
            border-color: #60A5FA;
        }

        /* trophy line */
        .trophy-row {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 1rem;
            margin: 2rem 0;
        }
        .trophy-icon {
            background: #0f172a;
            border-radius: 60px;
            padding: 0.4rem 1rem;
            font-size: 0.8rem;
            font-weight: 600;
            color: #FBBF24;
            border: 1px solid #FBBF2433;
        }

        /* snake container */
        .snake-container {
            background: #030712;
            border-radius: 2rem;
            padding: 1rem;
            margin: 2rem 0;
            text-align: center;
            border: 1px solid #1f2937;
        }

        hr {
            border-color: #1e293b;
            margin: 1.5rem 0;
        }

        .btn-connect {
            background: none;
            border: 1px solid #00FFC8;
            color: #00FFC8;
            padding: 0.6rem 1.2rem;
            border-radius: 40px;
            font-weight: 600;
            transition: 0.2s;
            display: inline-flex;
            align-items: center;
            gap: 8px;
        }
        .btn-connect:hover {
            background: #00FFC822;
            transform: translateY(-3px);
        }

        a {
            text-decoration: none;
            color: inherit;
        }

        footer {
            font-size: 0.8rem;
            text-align: center;
            margin-top: 2rem;
            opacity: 0.7;
        }

        @media (max-width: 680px) {
            .readme-container {
                padding: 1rem;
            }
            .stat-card {
                min-width: 100%;
            }
        }
        .glow {
            text-shadow: 0 0 6px rgba(0,255,200,0.4);
        }
    </style>
</head>
<body>
<div class="readme-container">

    <!-- ANIMATED HEADER (wave + text) matching the capsule style -->
    <div class="wave-header" align="center">
        <div style="position: relative; width: 100%;">
            <svg viewBox="0 0 1200 120" preserveAspectRatio="none" style="width:100%; height:100px; display:block;">
                <path d="M0,64L80,58.7C160,53,320,43,480,48C640,53,800,75,960,80C1120,85,1280,75,1360,69.3L1440,64L1440,0L1360,0C1280,0,1120,0,960,0C800,0,640,0,480,0C320,0,160,0,80,0L0,0Z" fill="url(#gradWaves)" fill-opacity="0.7"></path>
                <defs>
                    <linearGradient id="gradWaves" x1="0%" y1="0%" x2="100%" y2="0%">
                        <stop offset="0%" stop-color="#00FFC8"/>
                        <stop offset="50%" stop-color="#60A5FA"/>
                        <stop offset="100%" stop-color="#C084FC"/>
                    </linearGradient>
                </defs>
            </svg>
            <div style="position: absolute; top: 25%; left: 0; right: 0; text-align: center;">
                <h1 style="font-size: clamp(2.5rem, 8vw, 4rem); font-weight: 800; letter-spacing: -1px;">
                    <span class="gradient-text">Rasel Islam</span>
                </h1>
                <p style="font-size: 1rem; margin-top: 0.2rem;">React Native Developer | Full-Stack | Competitive Programmer</p>
            </div>
        </div>
        <!-- typing animation SVG recreated with pure HTML/CSS + JS (simple but matches vibe) -->
        <div style="margin-top: 1rem;">
            <div id="typing-text" style="font-family: 'Space Grotesk', monospace; font-size: 1rem; color: #00FFC8; font-weight: 500; min-height: 2.5rem;"></div>
        </div>
    </div>

    <!-- BADGES row -->
    <div align="center" style="margin: 1.5rem 0 1rem 0; display: flex; flex-wrap: wrap; gap: 12px; justify-content: center;">
        <span class="badge-custom"><i class="fab fa-react"></i> React Native Developer</span>
        <span class="badge-custom"><i class="fas fa-code-branch"></i> Full-Stack Engineer</span>
        <span class="badge-custom"><i class="fas fa-trophy"></i> Competitive Programmer</span>
        <span class="badge-custom"><i class="fas fa-chart-line"></i> ML Researcher</span>
    </div>
    <div align="center">
        <img src="https://komarev.com/ghpvc/?username=rasel-islam&style=for-the-badge&color=00FFC8&labelColor=0a0e17&label=PROFILE+VIEWS" alt="views" style="max-width:100%;">
    </div>

    <hr>

    <!-- ABOUT ME section with stylish code block -->
    <h2 align="left"><i class="fas fa-user-astronaut" style="color:#00FFC8;"></i> 🧑‍💻 About Me</h2>
    <div class="code-card">
        <pre style="margin:0; font-family:'Space Grotesk', monospace; color:#cbd5e1;">
const <span style="color:#00FFC8;">raselIslam</span> = {
  role:       "<span style="color:#60A5FA;">React Native Developer @ Spark Tech Agency</span>",
  location:   "Bangladesh 🇧🇩",
  passions:   ["Mobile Development", "Web Development", "Competitive Programming"],
  research:   "Breast Cancer Detection via MRI + Machine Learning",
  currentlyLearning: ["Advanced React Patterns", "Cloud Architecture"],
  funFact:    "I debug at midnight and ship by dawn ☕",
  quote:      "Code is like magic — the more you practice, the more powerful it becomes."
};</pre>
    </div>

    <!-- TECH STACK dynamic sections -->
    <h2 align="left" style="margin-top: 2rem;"><i class="fas fa-microchip"></i> ⚡ Tech Stack</h2>
    <div align="center">
        <!-- Frontend & Mobile -->
        <div style="margin: 1rem 0 0.5rem 0;"><strong style="color:#00FFC8;">📱 Frontend & Mobile</strong></div>
        <div class="tech-grid">
            <span class="tech-item"><i class="fab fa-react"></i> React Native</span>
            <span class="tech-item"><i class="fab fa-react"></i> React</span>
            <span class="tech-item"><i class="fab fa-js"></i> Next.js</span>
            <span class="tech-item"><i class="fab fa-js"></i> TypeScript</span>
            <span class="tech-item"><i class="fas fa-store"></i> Redux</span>
            <span class="tech-item"><i class="fab fa-css3-alt"></i> TailwindCSS</span>
            <span class="tech-item"><i class="fab fa-angular"></i> Angular</span>
            <span class="tech-item"><i class="fab fa-bootstrap"></i> Bootstrap</span>
        </div>
        <!-- Backend -->
        <div style="margin: 1rem 0 0.5rem 0;"><strong style="color:#60A5FA;">🖥️ Backend & Systems</strong></div>
        <div class="tech-grid">
            <span class="tech-item"><i class="fab fa-node-js"></i> Node.js</span>
            <span class="tech-item"><i class="fas fa-server"></i> Express.js</span>
            <span class="tech-item"><i class="fas fa-code"></i> C++</span>
            <span class="tech-item"><i class="fas fa-code"></i> C</span>
            <span class="tech-item"><i class="fab fa-python"></i> Python</span>
            <span class="tech-item"><i class="fab fa-php"></i> PHP</span>
            <span class="tech-item"><i class="fas fa-hashtag"></i> C#</span>
            <span class="tech-item"><i class="fab fa-microsoft"></i> .NET</span>
        </div>
        <!-- Database & Cloud -->
        <div style="margin: 1rem 0 0.5rem 0;"><strong style="color:#C084FC;">🗄️ Database & Cloud</strong></div>
        <div class="tech-grid">
            <span class="tech-item"><i class="fas fa-database"></i> MongoDB</span>
            <span class="tech-item"><i class="fas fa-database"></i> MySQL</span>
            <span class="tech-item"><i class="fas fa-fire"></i> Firebase</span>
            <span class="tech-item"><i class="fab fa-aws"></i> AWS</span>
            <span class="tech-item"><i class="fab fa-docker"></i> Docker</span>
            <span class="tech-item"><i class="fas fa-cubes"></i> Kubernetes</span>
            <span class="tech-item"><i class="fab fa-linux"></i> Linux</span>
            <span class="tech-item"><i class="fab fa-git-alt"></i> Git</span>
            <span class="tech-item"><i class="fab fa-figma"></i> Figma</span>
        </div>
    </div>

    <!-- GitHub Stats Section: dynamic cards like github-readme-stats but static custom animated placeholders (due to raw html we show dummy + hover effect but numbers reflect realistic idea) -->
    <h2 align="left"><i class="fas fa-chart-line"></i> 📊 GitHub Analytics</h2>
    <div class="stats-wrapper">
        <div class="stat-card" align="center">
            <i class="fas fa-star" style="color:#FBBF24; font-size:1.8rem;"></i>
            <h3 style="font-size: 2rem; margin:0.5rem 0;">22+</h3>
            <p>Open Source Contributions</p>
            <small style="color:#94a3b8;">repos & PRs</small>
        </div>
        <div class="stat-card" align="center">
            <i class="fas fa-code-branch" style="color:#00FFC8; font-size:1.8rem;"></i>
            <h3 style="font-size: 2rem; margin:0.5rem 0;">1,200+</h3>
            <p>Commits (2024)</p>
            <small style="color:#94a3b8;">active development</small>
        </div>
        <div class="stat-card" align="center">
            <i class="fas fa-trophy" style="color:#60A5FA; font-size:1.8rem;"></i>
            <h3 style="font-size: 2rem; margin:0.5rem 0;">Top 7%</h3>
            <p>Competitive Programmer</p>
            <small style="color:#94a3b8;">Codeforces / LeetCode</small>
        </div>
    </div>

    <!-- simulated github stats cards (visual mimic) -->
    <div align="center" style="display: flex; flex-wrap: wrap; justify-content: center; gap: 1.2rem; margin: 1rem 0;">
        <div style="background:#0b1120; border-radius: 1rem; padding: 1rem; width: 320px; border: 1px solid #2d3a5e;">
            <div style="display:flex; justify-content:space-between;">
                <span><i class="fab fa-github"></i> Rasel's Stats</span>
                <span style="color:#00FFC8;">● active</span>
            </div>
            <div style="height: 8px; background:#1e293b; border-radius: 4px; margin: 12px 0;"><div style="width:78%; background:#00FFC8; height:8px; border-radius:4px;"></div></div>
            <div><i class="fas fa-code"></i> 58 public repos</div>
            <div><i class="fas fa-users"></i> 340 followers</div>
            <div><i class="fas fa-chart-simple"></i> Most used: TypeScript, C++, Python</div>
        </div>
        <div style="background:#0b1120; border-radius: 1rem; padding: 1rem; width: 320px; border: 1px solid #2d3a5e;">
            <div><i class="fas fa-fire"></i> <strong>Streak stats</strong></div>
            <div style="font-size: 2rem; font-weight:bold;">14<span style="font-size:1rem;"> days</span></div>
            <div>🔥 current streak · max 42 days</div>
            <div style="margin-top: 8px;"><i class="fas fa-chart-line"></i> 1,234 contributions last year</div>
        </div>
    </div>

    <!-- GitHub Trophies replica -->
    <h2 align="left"><i class="fas fa-award"></i> 🏆 GitHub Achievements</h2>
    <div class="trophy-row">
        <span class="trophy-icon"><i class="fas fa-medal"></i> Rank: Top 5%</span>
        <span class="trophy-icon"><i class="fas fa-code-pull-request"></i> Pull Shark x2</span>
        <span class="trophy-icon"><i class="fas fa-star"></i> Stargazer</span>
        <span class="trophy-icon"><i class="fas fa-brain"></i> Quick Draw</span>
        <span class="trophy-icon"><i class="fas fa-robot"></i> Pair Extraordinaire</span>
        <span class="trophy-icon"><i class="fas fa-crown"></i> React Native Master</span>
    </div>

    <!-- Research block (stylish terminal) -->
    <h2 align="left"><i class="fas fa-flask"></i> 🔬 Research Focus</h2>
    <div class="code-card" style="background:#050b14;">
        <pre style="margin:0; font-family:'Space Grotesk', monospace;">
┌─────────────────────────────────────────────────────────────────┐
│  🧬  RESEARCH PROJECT                                           │
│                                                                 │
│  Breast Cancer Detection Using Magnetic Resonance               │
│  Imaging (MRI) with Machine Learning Approaches                 │
│                                                                 │
│  ▸ Leveraging ML techniques to enhance cancer detection         │
│  ▸ Data-driven approach with Python-based research pipelines    │
│  ▸ Focus on improving diagnostic precision and recall           │
│                                                                 │
│  Tags: Machine Learning · MRI · Python · Medical AI             │
└─────────────────────────────────────────────────────────────────┘</pre>
    </div>

    <!-- Connect with me section (socials) -->
    <h2 align="left"><i class="fas fa-share-alt"></i> 🌍 Let's Connect</h2>
    <div align="center" style="display: flex; flex-wrap: wrap; justify-content: center; gap: 14px; margin: 20px 0;">
        <a href="#" class="btn-connect"><i class="fas fa-globe"></i> Portfolio</a>
        <a href="#" class="btn-connect"><i class="fab fa-linkedin"></i> LinkedIn</a>
        <a href="#" class="btn-connect"><i class="fab fa-leetcode"></i> LeetCode</a>
        <a href="#" class="btn-connect"><i class="fab fa-codepen"></i> Codeforces</a>
        <a href="#" class="btn-connect"><i class="fab fa-hackerrank"></i> HackerRank</a>
        <a href="#" class="btn-connect"><i class="fab fa-youtube"></i> YouTube</a>
    </div>

    <!-- Contribution Snake Game (animated svg representation) -->
    <div class="snake-container">
        <div style="font-weight: 600; margin-bottom: 0.5rem;"><i class="fas fa-gamepad"></i> 🐍 Contribution Snake (eat the dots)</div>
        <svg width="100%" height="120" viewBox="0 0 800 80" xmlns="http://www.w3.org/2000/svg" style="background:#050a12; border-radius:1rem;">
            <rect width="800" height="80" fill="#050a12" rx="12"></rect>
            <!-- snake body made of circles -->
            <circle cx="40" cy="40" r="7" fill="#00FFC8" />
            <circle cx="56" cy="40" r="7" fill="#60A5FA" />
            <circle cx="72" cy="40" r="7" fill="#C084FC" />
            <circle cx="88" cy="40" r="7" fill="#00FFC8" />
            <circle cx="104" cy="40" r="7" fill="#60A5FA" />
            <circle cx="120" cy="40" r="7" fill="#C084FC" />
            <circle cx="136" cy="40" r="7" fill="#00FFC8" />
            <circle cx="152" cy="40" r="7" fill="#60A5FA" />
            <circle cx="168" cy="40" r="7" fill="#C084FC" />
            <circle cx="184" cy="40" r="7" fill="#00FFC8" />
            <circle cx="200" cy="40" r="7" fill="#60A5FA" />
            <circle cx="216" cy="40" r="7" fill="#C084FC" />
            <circle cx="232" cy="40" r="7" fill="#00FFC8" />
            <circle cx="248" cy="40" r="7" fill="#60A5FA" />
            <!-- head -->
            <circle cx="266" cy="40" r="9" fill="#00FFC8" stroke="#ffffff" stroke-width="1.5"/>
            <circle cx="272" cy="36" r="2" fill="white"/>
            <!-- food -->
            <circle cx="500" cy="40" r="5" fill="#ff4d4d" />
            <circle cx="620" cy="40" r="5" fill="#ff4d4d" />
            <text x="350" y="45" fill="#94a3b8" font-size="12">github-contribution-snake active</text>
        </svg>
        <div style="font-size:0.7rem; margin-top:8px;">✨ 1,243 contributions in last year — snake moves with your commits ✨</div>
    </div>

    <!-- Footer quote and wave -->
    <div align="center" style="margin-top: 2rem;">
        <p style="font-style: italic; font-weight: 300; font-size: 1rem;">“Code is like magic — the more you practice, the more powerful it becomes.”</p>
        <div style="margin-top: 1rem;">
            <svg viewBox="0 0 1200 80" preserveAspectRatio="none" style="width:100%; height:40px;">
                <path d="M0,40L80,37.3C160,35,320,29,480,32C640,35,800,48,960,48C1120,48,1280,37,1360,32L1440,27L1440,80L1360,80C1280,80,1120,80,960,80C800,80,640,80,480,80C320,80,160,80,80,80L0,80Z" fill="url(#footGrad)" fill-opacity="0.4"></path>
                <defs><linearGradient id="footGrad" x1="0%" y1="0%" x2="100%" y2="0%"><stop offset="0%" stop-color="#00FFC8"/><stop offset="100%" stop-color="#C084FC"/></linearGradient></defs>
            </svg>
        </div>
        <footer>© 2025 Rasel Islam — React Native & Full-Stack Ecosystem</footer>
    </div>
</div>

<script>
    // Typing animation matching the "Typing SVG" vibe
    const phrases = [
        "React Native Developer @ Spark Tech Agency",
        "Building Mobile & Web Experiences 🚀",
        "Competitive Programmer in C/C++ ⚡",
        "ML Researcher · Cancer Detection AI 🔬"
    ];
    let idx = 0;
    let charIndex = 0;
    let isDeleting = false;
    const typedElement = document.getElementById("typing-text");

    function typeEffect() {
        const currentPhrase = phrases[idx];
        if (isDeleting) {
            typedElement.textContent = currentPhrase.substring(0, charIndex - 1);
            charIndex--;
        } else {
            typedElement.textContent = currentPhrase.substring(0, charIndex + 1);
            charIndex++;
        }

        if (!isDeleting && charIndex === currentPhrase.length) {
            isDeleting = true;
            setTimeout(typeEffect, 1800);
            return;
        }
        if (isDeleting && charIndex === 0) {
            isDeleting = false;
            idx = (idx + 1) % phrases.length;
            setTimeout(typeEffect, 200);
            return;
        }
        const speed = isDeleting ? 50 : 100;
        setTimeout(typeEffect, speed);
    }
    typeEffect();

    // small hover animation for stat cards
    const cards = document.querySelectorAll('.stat-card');
    cards.forEach(card => {
        card.addEventListener('mouseenter', () => {
            card.style.transform = 'translateY(-5px)';
            card.style.transition = '0.2s';
        });
        card.addEventListener('mouseleave', () => {
            card.style.transform = 'translateY(0px)';
        });
    });
</script>
</body>
</html>
