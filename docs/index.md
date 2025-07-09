<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Kenya School of Artificial Intelligence</title>

  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, sans-serif;
      background-color: #ffffff;
      color: #222;
    }

    h1, h2, h3 {
      font-weight: 700;
      line-height: 1.3;
    }

    p {
      line-height: 1.8;
      font-size: 1.1rem;
      color: #333;
    }

    .ksai-section {
      max-width: 1200px;
      margin: 0 auto;
      padding: 3rem 2rem;
    }

    .ksai-logo {
      max-width: 240px;
      margin-bottom: 2rem;
      filter: drop-shadow(0 2px 4px rgba(0, 0, 0, 0.2));
    }

    .ksai-img {
      border-radius: 12px;
      box-shadow: 0 4px 16px rgba(0, 0, 0, 0.15);
      width: 100%;
      max-width: 700px;
    }

    .ksai-card {
      background-color: #ffffff;
      padding: 2rem;
      border-radius: 12px;
      transition: all 0.2s ease;
      box-shadow: 0 2px 8px rgba(0,0,0,0.05);
      flex: 1 1 300px;
      max-width: 340px;
    }

    .ksai-card:hover {
      transform: translateY(-4px);
      box-shadow: 0 8px 20px rgba(0, 0, 0, 0.08);
    }

    .cta-button, .social-buttons a, .contact-button {
      display: inline-block;
      font-weight: bold;
      text-decoration: none;
      border-radius: 8px;
      transition: all 0.3s ease;
    }

    .cta-button {
      background: #ffd700;
      color: black;
      padding: 1rem 2rem;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
    }

    .cta-button:hover {
      background: #ffcc00;
      box-shadow: 0 6px 16px rgba(0,0,0,0.15);
    }

    .social-buttons a {
      margin: 0.5rem;
      padding: 0.6rem 1.2rem;
      color: white;
    }

    footer {
      background-color: rgb(179, 196, 223);
      color: rgb(2, 7, 12);
      text-align: center;
      padding: 3rem 1rem;
      font-size: 0.95rem;
    }

    /* Responsive Styles */
    @media (max-width: 768px) {
      .hero-grid {
        display: block !important;
        padding: 0 1rem;
      }

      .ksai-logo {
        width: 180px !important;
      }

      h1 {
        font-size: 2.2rem !important;
      }

      .ksai-card {
        max-width: 100%;
      }

      .social-buttons {
        display: flex;
        flex-direction: column;
        gap: 1rem;
      }
    }
  </style>
</head>

<section style="background: linear-gradient(135deg, #f9fafb, #e9f0f8); padding: 6rem 2rem; font-family: 'Segoe UI', 'Helvetica Neue', 'Helvetica', sans-serif;">

  <!-- 🚀 Top Centered Hero Logo -->
  <div style="text-align: center; margin-bottom: 3rem;">
    <img src="assets/ksai-logo (2).png" alt="KSAI Top Logo" style="width: 380px; height: auto; object-fit: contain;">
  </div>

  <!-- Main Grid Layout -->
  <div style="max-width: 1200px; margin: 0 auto; display: grid; grid-template-columns: 1fr 1fr; gap: 4rem; align-items: center;">

    <!-- LEFT: Text Column -->
    <div>
      <p style="font-size: 1rem; font-weight: 600; color: #2563eb; text-transform: uppercase; letter-spacing: 1px; margin-bottom: 0.75rem;">
        Welcome to
      </p>
      <h1 style="font-size: 3.8rem; font-weight: 500; color: #1e293b; margin-bottom: 1rem; line-height: 1.2;">
        Kenya School of<br><span style="color: #2563eb; font-weight: 700;">Artificial Intelligence</span>
      </h1>
      <p style="font-size: 1.25rem; color: #475569; margin-bottom: 2.5rem; font-weight: 400; line-height: 1.6;">
        You’re not just here to learn — you're here to <strong style="color: #1d4ed8;">build, lead, and ship</strong> Africa’s next generation of AI.
      </p>

      <!-- ✅ Centered Button -->
   <div style="text-align: center;">
        <a href="module0/lesson0.1_workshop/" style="display: inline-block; background-color: #1d4ed8; color: white; padding: 1rem 2.5rem; font-size: 1rem; border-radius: 0.75rem; font-weight: 600; text-decoration: none; box-shadow: 0 6px 20px rgba(0, 0, 0, 0.08); transition: background 0.3s ease;">
           Get Started Free
        </a>
      </div>
    </div>

    <!-- RIGHT: Full Logo Showpiece -->
    <div style="text-align: center;">
      <img src="assets/images (1).jpeg" alt="KSAI Full Logo" style="width: 100%; max-width: 500px; height: auto; object-fit: contain;">
      <p style="margin-top: 1.5rem; color: #6b7280; font-size: 0.9rem;">Empowering AI excellence from Africa to the world.</p>
    </div>

  </div>
</section>






<!-- Mission Section -->
<section style="background-color: #f9fafb; padding: 5rem 2rem; text-align: center; font-family: 'Segoe UI', 'Helvetica Neue', sans-serif;">
  <div style="max-width: 960px; margin: 0 auto;">
    
    <!-- Section Title -->
    <h2 style="font-size: 2.5rem; font-weight: 700; color: #1e293b; margin-bottom: 1.5rem;">
      Why We Exist
    </h2>

    <!-- Mission Statement -->
    <p style="font-size: 1.2rem; line-height: 1.8; color: #374151; margin-bottom: 3rem;">
      Africa has the talent. Africa has the data. <br>
      Now it needs the <strong style="color: #1d4ed8;">courage to build</strong> — and the discipline to lead.
      <br><br>
      <span style="color: #4b5563;">
        KSAI is not a classroom. It is a builder’s lab — a place where young minds learn not to follow, but to
        <strong style="color: #2563eb;">execute and lead with excellence</strong>.
      </span>
    </p>

    <!-- Image -->
    <div>
      <img src="assets/image.png" alt="AI in Africa" style="width: 100%; max-width: 640px; height: auto; border-radius: 1rem; box-shadow: 0 12px 30px rgba(0, 0, 0, 0.08);">
    </div>
    
  </div>
</section>


  <!-- Core Pillars -->
<section style="background-color: #f9f9f9; padding: 5rem 2rem; font-family: 'Segoe UI', 'Helvetica Neue', sans-serif;">
  <div style="text-align: center; max-width: 1100px; margin: 0 auto;">

    <!-- Section Title -->
    <h2 style="font-size: 2.5rem; font-weight: 700; color: #1e293b; margin-bottom: 2rem;">
      What Makes KSAI Different
    </h2>

    <!-- Pillars Grid -->
    <div style="display: flex; flex-wrap: wrap; gap: 2rem; justify-content: center;">

      <!-- Pillar 1 -->
      <div style="flex: 1 1 300px; background: white; border-radius: 1rem; padding: 2rem; box-shadow: 0 8px 24px rgba(0, 0, 0, 0.05); max-width: 340px;">
        <h3 style="font-size: 1.5rem; font-weight: 700; color: #2563eb; margin-bottom: 1rem;">Built for Africa</h3>
        <p style="font-size: 1rem; color: #4b5563; line-height: 1.6;">
          Real-world problems. Local-first data. Human-centered design.
        </p>
      </div>

      <!-- Pillar 2 -->
      <div style="flex: 1 1 300px; background: white; border-radius: 1rem; padding: 2rem; box-shadow: 0 8px 24px rgba(0, 0, 0, 0.05); max-width: 340px;">
        <h3 style="font-size: 1.5rem; font-weight: 700; color: #2563eb; margin-bottom: 1rem;">Engineer-First</h3>
        <p style="font-size: 1rem; color: #4b5563; line-height: 1.6;">
          No grades. No lectures. Only code, collaboration, and shipping real projects.
        </p>
      </div>

      <!-- Pillar 3 -->
      <div style="flex: 1 1 300px; background: white; border-radius: 1rem; padding: 2rem; box-shadow: 0 8px 24px rgba(0, 0, 0, 0.05); max-width: 340px;">
        <h3 style="font-size: 1.5rem; font-weight: 700; color: #2563eb; margin-bottom: 1rem;">Startup Mindset</h3>
        <p style="font-size: 1rem; color: #4b5563; line-height: 1.6;">
          Think like a founder. Build like a product team. Launch like a startup.
        </p>
      </div>

    </div>
  </div>
</section>


  <!-- Call to Action -->
<section style="background-color:rgb(178, 194, 224); color: white; text-align: center; padding: 5rem 2rem; font-family: 'Segoe UI', 'Helvetica Neue', sans-serif;">
  <div style="max-width: 800px; margin: 0 auto;">
    
    <!-- CTA Heading -->
    <h2 style="font-size: 2.75rem; font-weight: 800; margin-bottom: 1rem;">
      Your Mission Starts Now
    </h2>

    <!-- CTA Text -->
    <p style="font-size: 1.2rem; line-height: 1.8; margin-bottom: 2.5rem;">
      Begin with <strong>Module 0: Foundations of Applied AI Engineering</strong><br>
      This is your environment, mindset, and method — the foundations of all great engineering.
    </p>

    <!-- CTA Button -->
    <a href="module0/lesson0.1_workshop/" style="
      display: inline-block;
      background-color: white;
      color: #1d4ed8;
      padding: 1rem 2.5rem;
      font-size: 1rem;
      font-weight: 600;
      border-radius: 0.75rem;
      text-decoration: none;
      box-shadow: 0 6px 20px rgba(0, 0, 0, 0.1);
      transition: background-color 0.3s ease, color 0.3s ease;
    ">
      Start Building →
    </a>
  </div>
</section>

  <!-- Community Section -->
<section style="background-color: #f9fafb; padding: 5rem 2rem; text-align: center; font-family: 'Segoe UI', 'Helvetica Neue', sans-serif;">
  <div style="max-width: 800px; margin: 0 auto;">

    <!-- Title -->
    <h2 style="font-size: 2.5rem; font-weight: 700; color: #1e293b; margin-bottom: 1rem;">
      Join the KSAI Community
    </h2>

    <!-- Subtext -->
    <p style="font-size: 1.2rem; color: #4b5563; line-height: 1.7; margin-bottom: 3rem;">
      Don’t learn in isolation. Become part of a growing tribe of AI engineers across Africa.
      Build together. Share breakthroughs.
    </p>

    <!-- Social Buttons -->
    <div style="display: flex; gap: 1rem; justify-content: center; flex-wrap: wrap;">

      <a href="https://chat.whatsapp.com/Hth07uBSP93BukTt0abmMO" style="
        background-color: #25D366;
        color: white;
        padding: 0.85rem 1.75rem;
        border-radius: 0.75rem;
        font-size: 1rem;
        font-weight: 600;
        text-decoration: none;
        transition: background-color 0.3s ease;
        box-shadow: 0 6px 14px rgba(0,0,0,0.08);
      ">
        WhatsApp
      </a>

      <a href="https://t.me/yourTelegramChannel" style="
        background-color: #229ED9;
        color: white;
        padding: 0.85rem 1.75rem;
        border-radius: 0.75rem;
        font-size: 1rem;
        font-weight: 600;
        text-decoration: none;
        transition: background-color 0.3s ease;
        box-shadow: 0 6px 14px rgba(0,0,0,0.08);
      ">
        Telegram
      </a>

      <a href="https://facebook.com/yourFacebookPage" style="
        background-color: #1877F2;
        color: white;
        padding: 0.85rem 1.75rem;
        border-radius: 0.75rem;
        font-size: 1rem;
        font-weight: 600;
        text-decoration: none;
        transition: background-color 0.3s ease;
        box-shadow: 0 6px 14px rgba(0,0,0,0.08);
      ">
        Facebook
      </a>

    </div>

  </div>
</section>


<!-- Instructor Section -->
<section style="background-color: #f9f9f9; padding: 5rem 2rem; text-align: center; font-family: 'Segoe UI', 'Helvetica Neue', sans-serif;">
  <div style="max-width: 820px; margin: 0 auto;">

    <!-- Section Title -->
    <h2 style="font-size: 2.5rem; font-weight: 800; color: #1a1a1a; margin-bottom: 2.5rem;">
      Meet Your Instructor
    </h2>

    <!-- Profile Image -->
    <img src="assets/founder.jpeg" alt="Alex Mwirigi"
         style="width: 180px; height: 180px; border-radius: 50%; object-fit: cover; box-shadow: 0 12px 28px rgba(0,0,0,0.1); margin-bottom: 2rem;">

    <!-- Instructor Bio -->
    <p style="font-size: 1.2rem; color: #374151; line-height: 1.8; margin-bottom: 2rem;">
      <strong style="font-size: 1.4rem; color: #1d4ed8;">Alex Mwirigi</strong> — Founder @ KSAI | AI Engineer
      <br><br>
      I’m building Africa’s first AI-powered digital hospital and leading the next generation of engineers through the Kenya School of Artificial Intelligence.
      <br><br>
      My expertise spans Machine Learning, Deep Learning, MLOps, and product-focused startup execution. I don’t teach theory  I deliver real, production-ready solutions to African challenges.
    </p>

    <!-- Contact & LinkedIn -->
    <div style="margin-top: 2.5rem; font-size: 1rem;">
      <p style="color: #555; margin-bottom: 1rem;">
        <strong>Phone:</strong> <a href="tel:+254111475368" style="color: #1d4ed8; text-decoration: none;">+254 111 475 368</a> &nbsp; | &nbsp;
        <strong>Email:</strong> <a href="mailto:mwirigialex@351@gmail.com" style="color: #1d4ed8; text-decoration: none;">mwirigialex@351@gmail.com</a>
      </p>

      <a href="https://www.linkedin.com/in/alex-mwirigi-a15b2826b" target="_blank"
         style="display: inline-block; background-color: #0a66c2; color: white; padding: 1rem 2rem; border-radius: 0.75rem; font-weight: 600; text-decoration: none; box-shadow: 0 6px 20px rgba(0,0,0,0.1); transition: background 0.3s ease;">
        Connect on LinkedIn →
      </a>
    </div>

  </div>
</section>

<!-- Contact & Support Section -->
<section style="background-color: #f9fafb; padding: 5rem 2rem; font-family: 'Segoe UI', 'Helvetica Neue', sans-serif;">
  <div style="max-width: 640px; margin: 0 auto; padding: 3rem 2rem; background: #ffffff; border-radius: 1rem; box-shadow: 0 12px 28px rgba(0,0,0,0.07); text-align: center;">

    <!-- Hire / Say Hello -->
    <h3 style="font-size: 2rem; font-weight: 800; color: #1f2937; margin-bottom: 1.5rem;">
      Hire Me or Say Hello
    </h3>

    <p style="font-size: 1.1rem; color: #4b5563; margin-bottom: 1.75rem; line-height: 1.6;">
      <strong>Call:</strong> <a href="tel:+254111475368" style="color: #1d4ed8; text-decoration: none;">+254 111 475 368</a><br>
      <strong>Email:</strong> <a href="mailto:mwirigialex@351@gmail.com" style="color: #1d4ed8; text-decoration: none;">mwirigialex@351@gmail.com</a>
    </p>

    <a href="https://www.linkedin.com/in/alex-mwirigi-a15b2826b" target="_blank"
       style="display: inline-block; background-color: #0a66c2; color: white; padding: 0.85rem 2rem; border-radius: 0.75rem; font-weight: 600; text-decoration: none; box-shadow: 0 4px 14px rgba(0,0,0,0.1);">
       View LinkedIn Profile
    </a>

    <hr style="margin: 3rem 0; border: none; border-top: 1px solid #e0e0e0;">

    <!-- Support Section -->
    <h3 style="font-size: 1.75rem; font-weight: 700; color: #1f2937; margin-bottom: 1rem;">
      Support the Mission
    </h3>
    <p style="color: #4b5563; font-size: 1.05rem; margin-bottom: 2rem; line-height: 1.6;">
      If this vision inspires you, help us push further. <strong>Buy me a coffee</strong> and be part of the movement.
    </p>

    <a href="tel:+254111475368"
       style="background: #facc15; color: #1a1a1a; padding: 0.85rem 2rem; border-radius: 0.75rem; font-weight: 600; text-decoration: none; box-shadow: 0 4px 14px rgba(0,0,0,0.06);">
      ☕ Call: +254 111 475 368
    </a>

  </div>
</section>

<!-- Footer -->
<footer style="background:rgb(179, 196, 223); color:rgb(2, 7, 12); text-align: center; padding: 3rem 1rem; font-family: 'Segoe UI', sans-serif; margin-top: 5rem; font-size: 0.95rem;">
  
  <p style="margin-bottom: 0.75rem;">
    © 2025 <strong style="color:rgb(1, 6, 8);">Kenya School of Artificial Intelligence</strong>. All rights reserved.
  </p>
  
  <p style="margin-bottom: 0.75rem;">
    Built with vision, discipline, and purpose — in 🇰🇪 Kenya for Africa.
  </p>

  <p style="margin-top: 1.5rem; font-size: 0.85rem; color:rgb(1, 6, 10);">
    Crafted by <strong style="color:rgb(21, 102, 202);">Alex Mwirigi</strong> · Founder & AI Engineer
  </p>

</footer>


</body>
</html>