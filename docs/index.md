---
hide:
  - header
  - navigation
  - toc
  - footer
---

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kenya School of Artificial Intelligence - KSAI</title>
    <meta name="description" content="Africa's premier AI engineering bootcamp">
    <style>
        /* KSAI Landing Page Styles */
        /* AI Bootcamp Design System - Cutting-edge tech aesthetics */

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            /* Core theme colors */
            --background: hsl(0, 0%, 100%);
            --foreground: hsl(224, 25%, 8%);
            
            /* AI-inspired brand colors */
            --primary: hsl(220, 98%, 61%);
            --primary-foreground: hsl(0, 0%, 100%);
            --primary-glow: hsl(220, 100%, 70%);
            
            --secondary: hsl(215, 25%, 27%);
            --secondary-foreground: hsl(0, 0%, 100%);
            
            --accent: hsl(199, 89%, 48%);
            --accent-foreground: hsl(0, 0%, 100%);
            
            /* Tech gradients */
            --gradient-primary: linear-gradient(135deg, var(--primary), var(--primary-glow));
            --gradient-hero: linear-gradient(135deg, hsl(220, 98%, 61%), hsl(199, 89%, 48%));
            --gradient-cta: linear-gradient(135deg, hsl(220, 98%, 61%), hsl(220, 100%, 70%));
            --gradient-section: linear-gradient(180deg, hsl(220, 13%, 98%), hsl(220, 13%, 96%));
            
            /* Sophisticated neutrals */
            --muted: hsl(220, 13%, 97%);
            --muted-foreground: hsl(215, 16%, 47%);
            --card: hsl(0, 0%, 100%);
            --card-foreground: hsl(224, 25%, 8%);
            
            /* Interactive elements */
            --border: hsl(220, 13%, 91%);
            
            /* Animations & effects */
            --transition-smooth: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            --shadow-glow: 0 0 40px hsl(220, 98%, 61%, 0.3);
            --shadow-elevated: 0 10px 40px -10px hsl(224, 25%, 8%, 0.1);
            --shadow-card: 0 4px 20px hsl(224, 25%, 8%, 0.08);
            
            --radius: 0.75rem;
        }

        body {
            font-family: 'Segoe UI', 'Helvetica Neue', 'Helvetica', Arial, sans-serif;
            line-height: 1.6;
            color: var(--foreground);
            background: var(--background);
            -webkit-font-smoothing: antialiased;
            -moz-osx-font-smoothing: grayscale;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 1rem;
        }

        /* Animations */
        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
        }

        @keyframes glow {
            from { box-shadow: 0 0 20px hsl(220, 98%, 61%, 0.3); }
            to { box-shadow: 0 0 30px hsl(220, 98%, 61%, 0.6); }
        }

        @keyframes slideUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .logo-float {
            animation: float 3s ease-in-out infinite;
        }

        /* Hero Section */
        .hero-section {
            background: var(--gradient-section);
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            padding: 5rem 1rem;
        }

        .hero-container {
            max-width: 1400px;
            margin: 0 auto;
        }

        .hero-logo {
            text-align: center;
            margin-bottom: 3rem;
        }

        .hero-logo img {
            width: 6rem;
            height: 6rem;
            object-fit: contain;
        }

        .hero-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 4rem;
            align-items: center;
        }

        .hero-text {
            text-align: left; /* Changed for better alignment on desktop */
            animation: slideUp 0.6s ease-out;
        }

        .hero-subtitle {
            color: var(--primary);
            font-weight: 600;
            text-transform: uppercase;
            letter-spacing: 1px;
            margin-bottom: 0.75rem;
            font-size: 1rem;
        }

        .hero-title {
            font-size: 3.5rem;
            font-weight: 700;
            color: var(--foreground);
            margin-bottom: 1.5rem;
            line-height: 1.2;
        }

        .gradient-text {
            background: var(--gradient-primary);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            font-weight: 800;
        }

        .hero-description {
            font-size: 1.25rem;
            color: var(--muted-foreground);
            margin-bottom: 2.5rem;
            line-height: 1.6;
            max-width: 600px;
        }

        .highlight {
            color: var(--primary);
            font-weight: 700;
        }

        .hero-buttons {
            display: flex;
            gap: 1rem;
            align-items: center;
        }

        .hero-image {
            text-align: center;
        }

        .hero-img {
            width: 100%;
            max-width: 500px;
            border-radius: var(--radius);
            box-shadow: var(--shadow-elevated);
            transition: var(--transition-smooth);
        }

        .hero-img:hover {
            box-shadow: var(--shadow-glow);
        }

        .hero-caption {
            margin-top: 1.5rem;
            color: var(--muted-foreground);
            font-size: 0.9rem;
        }

        /* Buttons */
        .btn {
            display: inline-block;
            padding: 1rem 2rem;
            border-radius: var(--radius);
            font-weight: 600;
            text-decoration: none;
            transition: var(--transition-smooth);
            border: 2px solid transparent;
            cursor: pointer;
            font-size: 1rem;
        }

        .btn-primary {
            background: var(--gradient-cta);
            color: var(--primary-foreground);
            box-shadow: var(--shadow-glow);
            animation: glow 2s ease-in-out infinite alternate;
        }

        .btn-primary:hover {
            box-shadow: var(--shadow-elevated);
            transform: translateY(-2px);
        }

        .btn-outline {
            border-color: var(--primary);
            color: var(--primary);
            background: transparent;
        }

        .btn-outline:hover {
            background: var(--primary);
            color: var(--primary-foreground);
        }

        .btn-cta {
            background: var(--primary-foreground);
            color: var(--primary);
            font-size: 1.1rem;
            padding: 1.2rem 2.5rem;
        }

        .btn-linkedin {
            background:rgb(61, 149, 238);
            color: white;
        }

        .btn-linkedin:hover {
            background:rgb(56, 146, 236);
        }

        .btn-coffee {
            border: 2px solid #facc15;
            color: #ca8a04;
            background: transparent;
        }

        .btn-coffee:hover {
            background: #facc15;
            color: #1a1a1a;
        }

        /* Generic Section Styles */
        .section-title {
            font-size: 2.5rem;
            font-weight: 700;
            text-align: center;
            margin-bottom: 2rem;
            color: var(--foreground);
        }

        .section-title-white {
            font-size: 2.5rem;
            font-weight: 700;
            text-align: center;
            margin-bottom: 2rem;
            color: var(--secondary-foreground);
        }
        
        .section-img {
            width: 100%;
            max-width: 800px;
            border-radius: var(--radius);
            box-shadow: var(--shadow-elevated);
            transition: var(--transition-smooth);
        }

        .section-img:hover {
            box-shadow: var(--shadow-glow);
        }
        
        /* Mission Section */
        .mission-section {
            padding: 5rem 1rem;
            background: var(--muted);
        }

        .mission-content {
            text-align: center;
            max-width: 900px;
            margin: 0 auto 3rem;
        }

        .mission-text {
            font-size: 1.3rem;
            line-height: 1.8;
            color: var(--card-foreground);
            margin-bottom: 2rem;
        }

        .mission-sub {
            font-size: 1.1rem;
            color: var(--muted-foreground);
            line-height: 1.7;
        }

        .accent-text {
            color: var(--accent);
            font-weight: 700;
        }

        .mission-image {
            text-align: center;
        }

        /* Philosophy Section */
        .philosophy-section {
            padding: 5rem 1rem;
            background: var(--secondary);
            color: var(--secondary-foreground);
        }

        .philosophy-header {
            text-align: center;
            margin-bottom: 4rem;
        }

        .glow-text {
            color: var(--primary-glow);
            text-shadow: 0 0 20px var(--primary-glow);
        }

        .principles-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-bottom: 3rem;
        }

        .principle-card {
            background: rgba(255, 255, 255, 0.1);
            border: 1px solid rgba(59, 130, 246, 0.2);
            border-radius: var(--radius);
            padding: 2rem;
            transition: var(--transition-smooth);
            display: flex;
            gap: 1rem;
        }

        .principle-card:hover {
            border-color: rgba(59, 130, 246, 0.4);
            background: rgba(255, 255, 255, 0.15);
        }

        .principle-icon {
            width: 3rem;
            height: 3rem;
            border-radius: 0.5rem;
            background: rgba(59, 130, 246, 0.2);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5rem;
            flex-shrink: 0;
            transition: var(--transition-smooth);
        }

        .principle-card:hover .principle-icon {
            background: rgba(59, 130, 246, 0.3);
        }

        .principle-title {
            font-size: 1.25rem;
            font-weight: 700;
            color: var(--secondary-foreground);
            margin-bottom: 0.75rem;
        }

        .principle-text {
            color: rgba(255, 255, 255, 0.9);
            line-height: 1.6;
        }

        .philosophy-closing {
            text-align: center;
        }

        .closing-box {
            display: inline-block;
            background: var(--gradient-cta);
            padding: 2rem 3rem;
            border-radius: var(--radius);
            box-shadow: var(--shadow-glow);
        }

        .closing-text {
            font-size: 1.25rem;
            font-weight: 700;
            color: var(--primary-foreground);
            line-height: 1.4;
        }

        /* Pillars Section */
        .pillars-section {
            padding: 5rem 1rem;
            background: var(--background);
        }

        .pillars-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 4rem;
        }

        .pillar-card {
            background: var(--card);
            border: 1px solid var(--border);
            border-radius: var(--radius);
            padding: 2rem;
            text-align: center;
            transition: var(--transition-smooth);
            box-shadow: var(--shadow-card);
        }

        .pillar-card:hover {
            box-shadow: var(--shadow-elevated);
            border-color: rgba(59, 130, 246, 0.2);
            transform: translateY(-4px);
        }

        .pillar-icon {
            width: 4rem;
            height: 4rem;
            margin: 0 auto 1rem;
            background: var(--gradient-section);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 2rem;
            transition: var(--transition-smooth);
        }

        .pillar-card:hover .pillar-icon {
            box-shadow: var(--shadow-glow);
        }

        .pillar-title {
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--foreground);
            margin-bottom: 1rem;
        }

        .pillar-text {
            color: var(--muted-foreground);
            line-height: 1.6;
        }

        /* CTA Section */
        .cta-section {
            background: var(--gradient-cta);
            padding: 5rem 1rem;
            text-align: center;
            color: var(--primary-foreground);
        }

        .cta-title {
            font-size: 2.75rem;
            font-weight: 800;
            margin-bottom: 1.5rem;
        }

        .cta-text {
            font-size: 1.2rem;
            line-height: 1.8;
            margin-bottom: 2.5rem;
            opacity: 0.9;
        }

        /* Community Section */
        .community-section {
            padding: 5rem 1rem;
            background: var(--muted);
            text-align: center;
        }

        .community-text {
            font-size: 1.2rem;
            color: var(--muted-foreground);
            line-height: 1.7;
            margin-bottom: 3rem;
            max-width: 800px;
            margin-left: auto;
            margin-right: auto;
        }

        .social-buttons {
            display: flex;
            flex-wrap: wrap;
            gap: 1rem;
            justify-content: center;
        }

        .social-btn {
            display: inline-block;
            padding: 1rem 2rem;
            border-radius: var(--radius);
            font-weight: 600;
            text-decoration: none;
            color: white;
            transition: var(--transition-smooth);
            box-shadow: var(--shadow-card);
        }

        .social-btn:hover {
            box-shadow: var(--shadow-elevated);
            transform: translateY(-2px);
        }

        .whatsapp { background: #25D366; }
        .whatsapp:hover { background: #128C7E; }

        .telegram { background:rgb(102, 195, 238); }
        .telegram:hover { background: #0088CC; }

        .facebook { background:rgb(113, 168, 241); }
        .facebook:hover { background:rgb(104, 162, 238); }

        /* Instructor Section */
        .instructor-section {
            padding: 5rem 1rem;
            background: var(--background);
        }

        .instructor-card {
            max-width: 800px;
            margin: 0 auto;
            background: var(--card);
            border-radius: var(--radius);
            padding: 3rem;
            text-align: center;
            box-shadow: var(--shadow-elevated);
            border: 1px solid var(--border);
        }

        .instructor-img {
            width: 12rem;
            height: 12rem;
            border-radius: 50%;
            object-fit: cover;
            margin: 0 auto 2rem;
            display: block;
            box-shadow: var(--shadow-card);
            transition: var(--transition-smooth);
        }

        .instructor-img:hover {
            box-shadow: var(--shadow-glow);
        }

        .instructor-name {
            font-size: 2rem;
            font-weight: 700;
            color: var(--primary);
            margin-bottom: 0.5rem;
        }

        .instructor-role {
            font-size: 0.9rem;
            font-weight: 600;
            color: var(--muted-foreground);
            text-transform: uppercase;
            letter-spacing: 1px;
            margin-bottom: 2rem;
        }

        .instructor-bio {
            font-size: 1.1rem;
            color: var(--muted-foreground);
            line-height: 1.7;
            margin-bottom: 2rem;
        }

        .contact-info {
            display: flex;
            flex-wrap: wrap;
            gap: 1rem;
            justify-content: center;
            margin-bottom: 2rem;
        }

        .contact-link {
            color: var(--muted-foreground);
            text-decoration: none;
            transition: var(--transition-smooth);
        }

        .contact-link:hover {
            color: var(--primary);
        }

        /* Contact Section */
        .contact-section {
            padding: 5rem 1rem;
            background: var(--muted);
        }

        .contact-card {
            max-width: 600px;
            margin: 0 auto;
            background: var(--card);
            border-radius: var(--radius);
            padding: 3rem;
            text-align: center;
            box-shadow: var(--shadow-elevated);
            border: 1px solid var(--border);
        }

        .contact-title {
            font-size: 2rem;
            font-weight: 700;
            color: var(--foreground);
            margin-bottom: 2rem;
        }

        .contact-details {
            display: flex;
            flex-wrap: wrap;
            gap: 1rem;
            justify-content: center;
            margin-bottom: 2rem;
        }

        .support-section {
            border-top: 1px solid var(--border);
            margin-top: 3rem;
            padding-top: 2rem;
        }

        .support-title {
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--foreground);
            margin-bottom: 1rem;
        }

        .support-text {
            color: var(--muted-foreground);
            line-height: 1.6;
            margin-bottom: 2rem;
        }

        /* Footer */
        .footer {
            background: var(--secondary);
            color: var(--secondary-foreground);
            padding: 3rem 1rem;
            text-align: center;
        }

        .footer-text {
            margin-bottom: 0.5rem;
            font-size: 1rem;
        }

        .footer-credit {
            margin-top: 1.5rem;
            font-size: 0.9rem;
            opacity: 0.8;
        }

        .credit-name {
            color: var(--primary-glow);
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .hero-grid {
                grid-template-columns: 1fr;
                gap: 2rem;
            }
            
            .hero-text, .hero-image {
                text-align: center;
            }

            .hero-description {
                margin-left: auto;
                margin-right: auto;
            }
            
            .hero-title {
                font-size: 2.5rem;
            }
            
            .hero-buttons {
                flex-direction: column;
                justify-content: center;
            }
            
            .section-title,
            .section-title-white {
                font-size: 2rem;
            }
            
            .principles-grid {
                grid-template-columns: 1fr;
            }
            
            .principle-card {
                flex-direction: column;
                text-align: center;
            }
            
            .social-buttons {
                flex-direction: column;
                align-items: center;
            }
            
            .contact-info,
            .contact-details {
                flex-direction: column;
            }
        }
    </style>
</head>
<body>
    <!-- 
      IMAGE SETUP INSTRUCTIONS
      =========================
      For this page to display correctly, you need to add your images.
      1. Create a folder: `docs/assets/images/`
      2. Place your images inside and name them as follows:
         - `logo.png` (from original: a24b064d-8e2d-4179-b724-1d93c7ecbae8.png)
         - `hero-image.png` (from original: 8061591d-e7b8-4885-9687-7171e5f1bae1.png)
         - `mission-image.jpg` (from original: assets/africa-ai.jpg)
         - `instructor-image.png` (from original: 8061591d-e7b8-4885-9687-7171e5f1bae1.png)
      The paths in this file have been updated to reflect this structure.
    -->

    <!-- Hero Section -->
    <section class="hero-section">
        <div class="hero-container">
            <div style="text-align:center; margin-bottom:2.2rem;">
                <div style="font-size:2.1rem; font-weight:800; background: linear-gradient(90deg, #2563eb 10%, #06b6d4 90%); -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text; color: transparent; letter-spacing:-0.5px; font-family:'Segoe UI', 'Helvetica Neue', Arial, sans-serif; text-shadow:0 2px 8px rgba(38,99,235,0.07); margin-bottom:0.6rem;">FullStack Machine Learning Engineer: Zero to Deployment</div>
                <div style="font-size:1.08rem; color:#2563eb; font-style:normal; margin-top:0.2rem; font-weight:500; background:rgba(6,182,212,0.10); border-radius:1.2rem; display:inline-block; padding:0.7rem 1.5rem; box-shadow:0 2px 12px rgba(38,99,235,0.06); margin-bottom:0.2rem;">
                    From idea to data, pipeline to product, become a full-stack ML engineer the industry respects.<br>
                    <span style="display:inline-block; margin-top:0.7rem; font-size:1.25rem; font-weight:800; background:#22c55e; color:#fff; padding:0.4rem 1.2rem; border-radius:1.2rem; box-shadow:0 2px 8px rgba(34,197,94,0.10);">FREE for all aspiring engineers</span>
                </div>
            </div>
            <!-- Top Logo -->
            <div class="hero-logo">
                <img src="assets\ksai-logo (2).png" alt="KSAI Official Logo" class="logo-float">
            </div>

            <!-- Main Hero Content -->
            <div class="hero-grid">
                <!-- Left: Text Content -->
                <div class="hero-text">
                    <p class="hero-subtitle">Welcome to</p>
                    <h1 class="hero-title" style="font-size:2.2rem; font-weight:800;">
                        Kenya School of<br>
                        <span style="background: linear-gradient(135deg, #3b82f6, #06b6d4); -webkit-background-clip: text; color: transparent; display:inline-block;">Artificial Intelligence</span>
                    </h1>
                    <p class="hero-description">
                        You're not just here to learn you're here to 
                        <strong class="highlight">build, lead, and ship</strong> 
                        Africa's next generation of AI.
                    </p>

                    <div class="hero-buttons">
                        <a href="#cta" class="btn btn-primary" style="background: linear-gradient(135deg,rgb(15, 62, 163), #06b6d4); color: #fff; padding: 0.5rem 1.0rem; font-size: 1rem; border-radius: 0.5rem; font-weight: 400; border: none;">Get Started Free</a>
                        <a href="#mission" class="btn btn-outline" style="border: 2px solid #2563eb; color: #2563eb; padding: 0.5rem 1.0rem; font-size: 1rem; border-radius: 0.5rem; font-weight: 400; background: #fff; margin-left: 0.5rem;">Learn More</a>
                    </div>
                </div>

                <!-- Right: Hero Image -->
                <div class="hero-image">
                    <img src="assets/hero-image-CqORPxMK.jpg" alt="AI Engineers in Africa" class="hero-img" style="max-width:550px; width:100%; display:block; margin:0 auto;">
                    <p class="hero-caption">Empowering AI excellence from Africa to the world.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Mission Section -->
    <section id="mission" class="mission-section">
        <div class="container">
            <h2 class="section-title" style="font-size:2rem; font-weight:800; color:#222;">Why We Exist</h2>
            
            <div class="mission-content">
                <p class="mission-text">
                    Africa has the talent. Africa has the data.<br>
                    Now it needs the <strong class="highlight">courage to build</strong> and the discipline to lead.
                </p>
                <p class="mission-sub">
                    KSAI is not a classroom. It is a builder's lab  a place where young minds learn not to follow, but to 
                    <strong class="accent-text">execute and lead with excellence</strong>.
                </p>
            </div>

            <div class="mission-image">
                <img src="assets\Smart_Africa_africa_business_communities.jpg" alt="AI Innovation Across Africa" class="section-img">
            </div>
        </div>
    </section>

    <!-- Philosophy Section -->
    <section class="philosophy-section">
        <div class="container">
            <div class="philosophy-header">
                <h2 class="section-title-white" style="font-size:2rem; font-weight:800; color:#fff;">Before You Write a Single Line of Code,<br><span style="font-weight:800; color:#3b82f6;">We Need to Rewire Your Brain</span></h2>
            </div>

            <div class="principles-grid">
                <!-- Principle 1 -->
                <div class="principle-card">
                    <div class="principle-icon brain-icon"></div>
                    <div class="principle-content">
                        <h3 class="principle-title" style="font-size:1.2rem; font-weight:700;">First-Principles Thinking</h3>
                        <p class="principle-text">
                            You will not use a tool or a library without understanding the problem it solves and its fundamental trade-offs. 
                            Why Docker over a VM? Why FastAPI over Flask? Why Kubernetes? If your answer is "because a tutorial said so," you're out.
                        </p>
                    </div>
                </div>

                <!-- Principle 2 -->
                <div class="principle-card">
                    <div class="principle-icon cpu-icon"></div>
                    <div class="principle-content">
                        <h3 class="principle-title" style="font-size:1.2rem; font-weight:700;">Systems, Not Models</h3>
                        <p class="principle-text">
                            The model is a small, replaceable gear in a vast machine. You are responsible for the entire machine: 
                            the data ingest, the validation pipeline, the feature store, the training infrastructure, the model registry, 
                            the serving API, the monitoring dashboard, and the feedback loop.
                        </p>
                    </div>
                </div>

                <!-- Principle 3 -->
                <div class="principle-card">
                    <div class="principle-icon code-icon"></div>
                    <div class="principle-content">
                        <h3 class="principle-title" style="font-size:1.2rem; font-weight:700;">Code is a Liability</h3>
                        <p class="principle-text">
                            Every line of code you write is a future bug, a maintenance cost, and a point of failure. 
                            The best engineers don't write more code; they write the least amount of code necessary to build 
                            a robust, scalable, and maintainable system.
                        </p>
                    </div>
                </div>

                <!-- Principle 4 -->
                <div class="principle-card">
                    <div class="principle-icon shield-icon"></div>
                    <div class="principle-content">
                        <h3 class="principle-title" style="font-size:1.2rem; font-weight:700;">Extreme Ownership</h3>
                        <p class="principle-text">
                            The data pipeline broke at 3 AM? That's your problem. The model is drifting in production? Your problem. 
                            The API latency spiked? Your problem. You own the system, end-to-end. No excuses.
                        </p>
                    </div>
                </div>
            </div>

            <div class="philosophy-closing">
                <div class="closing-box">
                    <p class="closing-text">
                        This is your new religion.<br>
                        <span class="glow-text">Burn it into your memory.</span>
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Pillars Section -->
    <section class="pillars-section">
        <div class="container">
            <h2 class="section-title" style="font-size:2rem; font-weight:800; color:#222;">What Makes KSAI Different</h2>
            
            <div class="pillars-grid" style="display:flex; flex-direction:row; justify-content:center; gap:2rem; flex-wrap:nowrap; max-width:1100px; margin:0 auto;">
                <div class="pillar-card" style="min-width:260px; flex:1 1 0;">
                    <div class="pillar-icon"></div>
                    <h3 class="pillar-title" style="font-size:1.2rem; font-weight:700;">Built for Africa</h3>
                    <p class="pillar-text">Real-world problems. Local-first data. Human-centered design.</p>
                </div>

                <div class="pillar-card" style="min-width:260px; flex:1 1 0;">
                    <div class="pillar-icon"></div>
                    <h3 class="pillar-title" style="font-size:1.2rem; font-weight:700;">Engineer-First</h3>
                    <p class="pillar-text">No grades. No lectures. Only code, collaboration, and shipping real projects.</p>
                </div>

                <div class="pillar-card" style="min-width:260px; flex:1 1 0;">
                    <div class="pillar-icon"></div>
                    <h3 class="pillar-title" style="font-size:1.2rem; font-weight:700;">Startup Mindset</h3>
                    <p class="pillar-text">Think like a founder. Build like a product team. Launch like a startup.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- CTA Section -->
    <section id="cta" class="cta-section" style="background: linear-gradient(135deg, #1e293b 0%, #2563eb 100%);">
        <div class="container">
            <h2 class="cta-title" style="font-size:2rem; font-weight:800; color:#fff;">Your Mission Starts Now</h2>
            <p class="cta-text">
                Begin with <strong>Module 0: Foundations of Applied AI Engineering</strong><br>
                This is your environment, mindset, and method — the foundations of all great engineering.
            </p>
            <a href="module0/lesson0.1_workshop/" class="btn btn-cta">Start Building →</a>
        </div>
    </section>

    <!-- Community Section -->
    <section class="community-section">
        <div class="container">
            <h2 class="section-title" style="font-size:2rem; font-weight:800; color:#222;">Join the KSAI Community</h2>
            <p class="community-text">
                Don't learn in isolation. Become part of a growing tribe of AI engineers across Africa. 
                Build together. Share breakthroughs.
            </p>

            <div class="social-buttons">
                <a href="https://chat.whatsapp.com/Hth07uBSP93BukTt0abmMO" class="social-btn whatsapp" target="_blank" rel="noopener noreferrer" style="background:#25D366; color:#fff; padding:0.8rem 2rem; border-radius:0.7rem; font-weight:600; font-size:1.1rem; box-shadow:0 2px 8px rgba(0,0,0,0.08); margin:0 0.3rem 0.7rem 0; display:inline-block;">WhatsApp</a>
                <a href="https://t.me/yourTelegramChannel" class="social-btn telegram" target="_blank" rel="noopener noreferrer" style="background:#229ED9; color:#fff; padding:0.8rem 2rem; border-radius:0.7rem; font-weight:600; font-size:1.1rem; box-shadow:0 2px 8px rgba(0,0,0,0.08); margin:0 0.3rem 0.7rem 0; display:inline-block;">Telegram</a>
                <a href="https://facebook.com/yourFacebookPage" class="social-btn facebook" target="_blank" rel="noopener noreferrer" style="background:#1877F2; color:#fff; padding:0.8rem 2rem; border-radius:0.7rem; font-weight:600; font-size:1.1rem; box-shadow:0 2px 8px rgba(0,0,0,0.08); margin:0 0.3rem 0.7rem 0; display:inline-block;">Facebook</a>
            </div>
        </div>
    </section>

    <!-- Instructor Section -->
    <section class="instructor-section">
        <div class="container">
            <div class="instructor-card">
                <h2 class="section-title" style="font-size:2rem; font-weight:800; color:#222;">Meet Your Instructor</h2>
                
                <img src="assets/founder.jpeg" alt="Alex Mwirigi" class="instructor-img">
                
                <div class="instructor-info">
                    <h3 class="instructor-name">Alex Mwirigi</h3>
                    <p class="instructor-role">Founder @ KSAI | AI Engineer</p>
                    
                    <p class="instructor-bio">
                        I'm building Africa's first AI-powered digital hospital and leading the next generation of engineers 
                        through the Kenya School of Artificial Intelligence.<br><br>
                        My expertise spans Machine Learning, Deep Learning, MLOps, and product-focused startup execution. 
                        I don't teach theory  I deliver real, production-ready solutions to African challenges.
                    </p>
                </div>

                <div class="contact-info">
                    <a href="tel:+254111475368" class="contact-link">📞 +254 111 475 368</a>
                    <a href="mailto:mwirigialex@351@gmail.com" class="contact-link">✉️ mwirigialex351@gmail.com</a>
                </div>

                <a href="https://www.linkedin.com/in/alex-mwirigi-a15b2826b" class="btn btn-linkedin" target="_blank" rel="noopener noreferrer" style="background:#0a66c2; color:#fff; font-weight:600; padding:0.7rem 1.5rem; border-radius:0.5rem; font-size:1rem; box-shadow:0 2px 8px rgba(0,0,0,0.08); border:none; display:inline-block;">Connect on LinkedIn →</a>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="contact-section">
        <div class="container">
            <div class="contact-card">
                <h3 class="contact-title" style="font-size:1.2rem; font-weight:700;">Hire Me or Say Hello</h3>
                
                <div class="contact-details">
                    <a href="tel:+254111475368" class="contact-link">📞 +254 111 475 368</a>
                    <a href="mailto:mwirigialex351@gmail.com" class="contact-link">✉️ mwirigialex351@gmail.com</a>
                </div>

                <a href="https://www.linkedin.com/in/alex-mwirigi-a15b2826b" class="btn btn-linkedin" target="_blank" rel="noopener noreferrer" style="background:#0a66c2; color:#fff; font-weight:600; padding:0.7rem 1.5rem; border-radius:0.5rem; font-size:1rem; box-shadow:0 2px 8px rgba(0,0,0,0.08); border:none; display:inline-block;">View LinkedIn Profile</a>

                <div class="support-section">
                    <h3 class="support-title" style="font-size:1.2rem; font-weight:700;">Support the Mission</h3>
                    <p class="support-text">
                        If this vision inspires you, help us push further. <strong>Buy me a coffee</strong> and be part of the movement.
                    </p>
                    <a href="tel:+254111475368" class="btn btn-coffee">☕ Call: +254 111 475 368</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="footer">
        <div class="container">
            <p class="footer-text">
                © 2025 <strong>Kenya School of Artificial Intelligence</strong>. All rights reserved.
            </p>
            <p class="footer-text">
                Built with vision, discipline, and purpose in 🇰🇪 Kenya for Africa.
            </p>
            <p class="footer-credit">
                Crafted by <strong class="credit-name">Alex Mwirigi</strong> · Founder & AI Engineer
            </p>
        </div>
    </footer>

    <script>
        // KSAI Landing Page JavaScript
        document.addEventListener('DOMContentLoaded', function() {
            // Smooth scrolling for anchor links
            const links = document.querySelectorAll('a[href^="#"]');
            
            links.forEach(link => {
                link.addEventListener('click', function(e) {
                    const href = this.getAttribute('href');
                    // Only prevent default for internal hash links
                    if (href.startsWith('#') && href.length > 1) {
                        e.preventDefault();
                        const targetId = href;
                        const targetSection = document.querySelector(targetId);
                        
                        if (targetSection) {
                            targetSection.scrollIntoView({
                                behavior: 'smooth',
                                block: 'start'
                            });
                        }
                    }
                });
            });

            // Add scroll-triggered animations
            const observerOptions = {
                threshold: 0.1,
                rootMargin: '0px 0px -50px 0px'
            };

            const observer = new IntersectionObserver(function(entries, observer) {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.style.opacity = '1';
                        entry.target.style.transform = 'translateY(0)';
                        observer.unobserve(entry.target); // Stop observing once animated
                    }
                });
            }, observerOptions);

            // Observe elements for animation
            const animateElements = document.querySelectorAll('.pillar-card, .principle-card, .instructor-card, .contact-card, .mission-content, .mission-image');
            
            animateElements.forEach(element => {
                element.style.opacity = '0';
                element.style.transform = 'translateY(30px)';
                element.style.transition = 'opacity 0.6s ease, transform 0.6s ease';
                observer.observe(element);
            });

            // Console welcome message
            console.log(`
             KSAI - Kenya School of Artificial Intelligence
            ===============================================
            
            Welcome to the source code of Africa's premier AI bootcamp!
            
            Built with:
            • Vanilla HTML, CSS, and JavaScript
            • Modern CSS Grid and Flexbox
            • Mobile-first responsive design
            
            Ready to build the future of AI in Africa? 🇰🇪
            `);
        });
    </script>
</body>
</html>