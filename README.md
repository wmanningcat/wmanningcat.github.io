
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Family Yoga Institute • Growing together</title>
  <meta name="description" content="Family Yoga Institute (FYI) offers prenatal, postnatal, and Mommy & Me yoga in Rancho Mission Viejo, CA. Growing together through mindful movement and community." />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&family=Cormorant+Garamond:wght@400;500;600;700&display=swap" rel="stylesheet">

  <style>
 /* ---------- Theme ---------- */
:root{
  --bg:#FAF9F6;
  --ink:#20302A;
  --muted:#4d6b63;
  --brand:#3E7C6D;     /* green-teal */
  --brand-2:#2C9F99;   /* teal */
  --accent:#7251A6;    /* purple */
  --accent-2:#C7B6E3;
  --ring: rgba(60,120,110,.2);
  --card:#ffffff;
  --shadow: 0 10px 30px rgba(28,53,46,.08);
  --radius: 18px;
}
*{box-sizing:border-box}
html,body{margin:0;background:var(--bg);color:var(--ink);font-family:Inter,system-ui,-apple-system,Segoe UI,Roboto,Arial,sans-serif;line-height:1.6}
a{color:var(--accent);text-decoration:none}
img{max-width:100%;display:block}
.container{width:min(1120px,92vw);margin-inline:auto}
.pill{display:inline-block;padding:.4rem .85rem;border-radius:999px;background:#e9f3f1;color:var(--brand);font-weight:600;font-size:.9rem;letter-spacing:.2px}
.btn{display:inline-flex;align-items:center;gap:.6rem;padding:.9rem 1.1rem;border-radius:14px;background:linear-gradient(135deg,var(--brand),var(--brand-2));color:#fff;font-weight:700;box-shadow:0 10px 18px rgba(46,124,109,.18);transition:.2s transform ease,.2s box-shadow ease}
.btn:hover{transform:translateY(-2px);box-shadow:0 16px 28px rgba(46,124,109,.28)}
.btn.alt{background:linear-gradient(135deg,var(--accent),#9a7ed1)}
.btn.ghost{background:transparent;border:2px solid var(--brand);color:var(--brand)}
.tag{padding:.35rem .7rem;border-radius:999px;background:#efeaf9;color:#5b3aa7;font-weight:600;font-size:.8rem}
h1,h2,h3{font-family:"Cormorant Garamond",serif;line-height:1.15;margin:0 0 .6rem}
h1{font-size:clamp(2.1rem,4.4vw,3.1rem)}
h2{font-size:clamp(1.6rem,3.2vw,2.2rem)}
h3{font-size:clamp(1.15rem,2.2vw,1.4rem)}
p{margin:.4rem 0 1rem}

/* ---------- Nav ---------- */
.nav{position:sticky;top:0;z-index:50;background:rgba(250,249,246,.72);backdrop-filter:saturate(180%) blur(8px);border-bottom:1px solid rgba(62,124,109,.08)}
.nav .inner{display:flex;align-items:center;justify-content:space-between;padding:.8rem 0}
.brand{display:flex;align-items:center;gap:.75rem}
.brand img{width:44px;height:44px;object-fit:contain;border-radius:10px}
.brand .name{font-family:"Cormorant Garamond",serif;font-weight:700;letter-spacing:.3px}
.nav ul{display:flex;gap:1rem;list-style:none;margin:0;padding:0;align-items:center}
.nav a{font-weight:600;color:var(--muted)}
.hamburger{display:none}

/* ---------- Hero (single column + bigger text) ---------- */
.hero{
  padding:4rem 0 2.2rem;
  background:
    radial-gradient(800px 300px at 80% -30%, #e9f3f1 10%, transparent 60%),
    radial-gradient(900px 320px at 0% -20%, #efeaf9 10%, transparent 60%);
}
.hero-grid{display:grid;grid-template-columns:1fr;gap:28px;align-items:center}
.sub{color:var(--muted)}
.hero .cta{display:flex;gap:.8rem;flex-wrap:wrap;margin-top:1rem}
/* Larger hero text */
.hero h1{
  font-size: clamp(2.8rem, 6vw, 4rem);
  line-height: 1.2;
}
.hero .sub{
  font-size: 1.25rem;
  line-height: 1.7;
}

/* ---------- Sections ---------- */
section{padding:64px 0}
.card{background:var(--card);border-radius:var(--radius);box-shadow:var(--shadow);border:1px solid rgba(0,0,0,.05)}
.grid-2{display:grid;grid-template-columns:1fr 1fr;gap:28px}
.grid-3{display:grid;grid-template-columns:repeat(3,1fr);gap:24px}
.eyebrow{font-weight:800;letter-spacing:.14em;text-transform:uppercase;color:var(--brand);font-size:.85rem;margin-bottom:.6rem}

/* ---------- Classes ---------- */
.class{padding:24px}
.class header{display:flex;align-items:center;gap:10px;margin-bottom:.2rem}
.class header h3{margin:0}
.checklist{margin:.6rem 0 0;padding:0 0 0 1.2rem}
.price{display:flex;gap:10px;align-items:center;margin:.8rem 0 0}
.price strong{font-size:1.1rem}

/* ---------- Bios ---------- */
.bio{padding:28px;display:grid;grid-template-columns:1.1fr 1.2fr;gap:28px;align-items:center}
.bio .photo{
  border-radius:16px;
  overflow:hidden;
  background:#f7f6fb;
  border:6px solid #efeaf9;
}
/* Let the image use its natural aspect ratio so faces aren't cropped */
.bio .photo img{
  width:100%;
  height:auto;
  border-radius:12px;
  object-fit:contain;
}
/* Stack instructor + FYI vertically on all screens */
#about .grid-2{
  grid-template-columns: 1fr !important;
}

/* ---------- FAQ ---------- */
.faq{max-width:980px;margin-inline:auto}
details{background:#fff;border-radius:14px;padding:1rem 1.1rem;border:1px solid rgba(0,0,0,.06);box-shadow:var(--shadow)}
details+details{margin-top:12px}
summary{cursor:pointer;font-weight:700;color:#283e37}
details[open]{outline:3px solid var(--ring)}

/* ---------- Schedule/Location ---------- */
.info-row{display:grid;grid-template-columns:1.1fr .9fr;gap:24px}
.kv{padding:22px}
.kv b{display:block;font-size:1.05rem}
.map{border:0;width:100%;height:320px;border-radius:14px}

/* ---------- Footer ---------- */
.foot{padding:34px 0;border-top:1px solid rgba(0,0,0,.06);color:var(--muted);font-size:.95rem}
.foot .row{display:flex;justify-content:space-between;gap:20px;flex-wrap:wrap}
.social a{margin-right:10px}

/* ---------- Mobile ---------- */
@media (max-width: 920px){
  .grid-2,.grid-3,.bio,.info-row{grid-template-columns:1fr}
  .brand .name{font-size:1.05rem}
  .nav ul{display:none}
  .hamburger{display:block}
  .mobile-menu{display:none;background:rgba(250,249,246,.97);padding:.8rem 0;border-bottom:1px solid rgba(0,0,0,.06)}
  .mobile-menu.open{display:block}
  .mobile-menu a{display:block;padding:.75rem 1rem;font-weight:700;color:var(--muted)}
}
  </style>
</head>
<body>

  <!-- NAV -->
  <nav class="nav">
    <div class="container inner">
      <div class="brand">
        <!-- Replace with your actual logo file -->
        <img src="assets/logo.png" alt="Family Yoga Institute logo" />
        <div class="name">Family Yoga Institute</div>
      </div>
      <ul>
        <li><a href="#classes">Classes</a></li>
        <li><a href="#schedule">Schedule & Location</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#faq">FAQ</a></li>
        <li><a class="btn" href="https://forms.gle/your-google-form-id" target="_blank" rel="noopener">Sign up</a></li>
      </ul>
      <button class="hamburger btn ghost" aria-label="Open menu" onclick="toggleMenu()">Menu</button>
    </div>
    <div id="mobileMenu" class="mobile-menu">
      <div class="container">
        <a href="#classes" onclick="toggleMenu()">Classes</a>
        <a href="#schedule" onclick="toggleMenu()">Schedule & Location</a>
        <a href="#about" onclick="toggleMenu()">About</a>
        <a href="#faq" onclick="toggleMenu()">FAQ</a>
        <a class="btn" style="margin:.6rem 0 0 .4rem" href="https://forms.gle/your-google-form-id" target="_blank" rel="noopener">Sign up</a>
      </div>
    </div>
  </nav>

  <!-- HERO -->
  <header class="hero" id="top">
    <div class="container hero-grid">
      <div>
        <span class="pill">Rancho Mission Viejo, CA</span>
        <h1 style="margin-top:.6rem">Growing together through <span style="color:var(--accent)">mindful movement</span> and community</h1>
        <p class="sub">
          Family Yoga Institute offers a nurturing space where moms and families can move, breathe, and grow together.
          Our classes support every stage of motherhood — from pregnancy to postnatal bonding and beyond.
        </p>
        <div class="cta">
          <a class="btn" href="https://forms.gle/your-google-form-id" target="_blank" rel="noopener">Reserve your spot</a>
          <a class="btn alt" href="#classes">Explore classes</a>
        </div>
      </div>
    </div>
  </header>

  <!-- CLASSES -->
  <section id="classes" class="container">
    <div style="text-align:center;margin-bottom:26px">
      <div class="eyebrow">Classes Offered</div>
      <h2>Mindful offerings for every stage of motherhood</h2>
      <p class="sub">Launching with prenatal and postnatal series. Future plans include on-site childcare so moms can practice without arranging a babysitter — and Mike will be teaching, too.</p>
    </div>

    <div class="grid-2">
      <!-- Prenatal -->
      <article class="card class">
        <header>
          <span class="tag">Prenatal • “Mindful Mommies To Be”</span>
        </header>
        <h3>7-Week Chakra Series – Prenatal Yoga</h3>
        <p><strong>Where:</strong> Rancho Mission Viejo (RMV) • peaceful, welcoming studio space</p>
        <ul class="checklist">
          <li>7 weekly 1-hour prenatal classes</li>
          <li>Chakra-focused sequences to balance energy &amp; support pregnancy</li>
          <li>Breathwork &amp; meditation for labor preparation</li>
          <li>Beautiful series handbook: chakra insights, affirmations, safe poses, at-home practices</li>
        </ul>
        <div class="price">
          <strong>Investment:</strong>
          <span>$200 full series (includes handbook) • or $35 drop-in</span>
        </div>
        <p style="margin-top:.6rem"><strong>Who:</strong> Expecting mothers (any trimester, with medical clearance)</p>
        <div class="cta">
          <a class="btn" href="https://forms.gle/your-google-form-id" target="_blank" rel="noopener">Sign up</a>
          <a class="btn ghost" href="#faq">Read FAQs</a>
        </div>
      </article>

      <!-- Mommy & Me -->
      <article class="card class">
        <header>
          <span class="tag">Postnatal • “Mindful Mommy &amp; Me”</span>
        </header>
        <h3>7-Week Chakra-Themed Series – Postnatal + Baby</h3>
        <p><strong>Where:</strong> Rancho Mission Viejo (RMV) • warm community setting</p>
        <ul class="checklist">
          <li>7 weekly 1-hour classes designed for moms &amp; babies (to crawling age)</li>
          <li>Chakra-based flows for postnatal healing &amp; emotional balance</li>
          <li>Bonding practices, songs, gentle movement &amp; sensory play</li>
          <li>Relaxation &amp; breathwork to calm your mind and soothe your baby</li>
        </ul>
        <div class="price">
          <strong>Investment:</strong>
          <span>$200 full series • or $35 drop-in</span>
        </div>
        <p style="margin-top:.6rem"><strong>Who:</strong> New moms cleared for exercise; babies welcome — feed/change/soothe anytime.</p>
        <div class="cta">
          <a class="btn" href="https://forms.gle/your-google-form-id" target="_blank" rel="noopener">Reserve spot</a>
          <a class="btn ghost" href="#faq">Read FAQs</a>
        </div>
      </article>
    </div>
  </section>

  <!-- SCHEDULE & LOCATION -->
  <section id="schedule">
    <div class="container">
      <div class="info-row">
        <article class="card kv">
          <div class="eyebrow">Schedule</div>
          <h2>7 consecutive weeks • 1 session per week</h2>
          <p class="sub">Exact days/times will be posted after the association meeting in September. Join the list via the signup form to get first pick of time slots.</p>
          <ul class="checklist">
            <li>Small groups for connection &amp; personal attention</li>
            <li>Planned on-site childcare coming soon</li>
            <li>Future: additional classes taught by Mike</li>
          </ul>
          <div class="cta">
            <a class="btn" href="https://forms.gle/your-google-form-id" target="_blank" rel="noopener">Get updates &amp; enroll</a>
          </div>
        </article>

        <article class="card kv">
          <div class="eyebrow">Location</div>
          <h2>Rancho Mission Viejo (RMV), SoCal</h2>
          <p>Classes are hosted within the RMV community. After program approval, the association will promote classes and provide space.</p>
          <iframe class="map" loading="lazy" referrerpolicy="no-referrer-when-downgrade"
            src="https://www.google.com/maps?q=Rancho%20Mission%20Viejo,%20CA&output=embed"
            title="Map of Rancho Mission Viejo, California"></iframe>
          <p class="sub" style="margin-top:.8rem">Questions? <a href="mailto:maryjaucian@gmail.com">maryjaucian@gmail.com</a> • <a href="tel:+19494688151">949-468-8151</a></p>
        </article>
      </div>
    </div>
  </section>

  <!-- ABOUT -->
  <section id="about" class="container">
    <div class="grid-2">
      <!-- Mary bio -->
      <article class="card bio">
        <div class="photo">
          <!-- Replace with a great photo of Mary + kids -->
          <img src="assets/mary-and-kids.jpg" alt="Mary Jaucian with her children">
        </div>
        <div>
          <div class="eyebrow">Meet your instructor</div>
          <h2>Mary Jaucian – Yoga Instructor | Certified Reiki Healer | Founder, Family Yoga Institute</h2>
          <p>Mary Jaucian began her yoga journey at just 14 years old, discovering early on the grounding, healing power of mindful movement. Now, with over 10 years of teaching experience and more than 300 certified training hours, she continues to guide others with compassion, clarity, and deep-rooted knowledge.</p>
          <p>As a mom of two and a proud resident of Rancho Mission Viejo (RMV), Mary understands firsthand the importance of balance, presence, and connection—both on and off the mat. She is the founder of the Family Yoga Institute, a heart-driven initiative focused on supporting families through yoga, mindfulness, and community-based education.</p>
          <p>Mary is also a certified Reiki healer, blending energetic awareness into her classes for a more holistic and healing experience.</p>
          <p>Mary specializes in teaching Mindful Mommies, a class series designed to help mothers reconnect with themselves, reduce stress, and cultivate joy through movement and breath. Her teaching style is intuitive, warm, and accessible—inviting students of all levels to move with intention and live with presence.</p>
        </div>
      </article>

      <!-- FYI bio -->
      <article class="card" style="padding:28px">
        <div class="eyebrow">About FYI</div>
        <h2>The Family Yoga Institute</h2>
        <p>The Family Yoga Institute was founded with a simple but powerful mission: to support families in growing together through the shared practice of yoga. Born from the realization that many mothers were putting their own wellness on hold to care for others, the Institute was created as a space where no one has to choose between self-care and family life.</p>
        <p>We believe that yoga should be accessible, sustainable, and normalized within the rhythms of everyday family living. Our classes are thoughtfully designed for both adults and children, offering opportunities for individual growth, parent-child connection, and community support.</p>
        <p>From Mindful Mommies to kids' yoga and inclusive family flows, the Family Yoga Institute provides a welcoming environment where breath, movement, and presence become tools for lifelong resilience. Whether you're a seasoned practitioner or just beginning your journey, we invite you to grow, move, and thrive—together.</p>
      </article>
    </div>
  </section>

  <!-- FAQ -->
  <section id="faq" class="faq">
    <div class="container">
      <div style="text-align:center;margin-bottom:18px">
        <div class="eyebrow">Prenatal &amp; Postnatal Yoga – FAQ</div>
        <h2>What moms ask most</h2>
      </div>

      <details>
        <summary>1) Do I need previous yoga experience?</summary>
        <p>No. Our classes are designed for all levels, including complete beginners. We focus on gentle, safe movements suitable for pregnancy or postpartum recovery.</p>
      </details>

      <details>
        <summary>2) When can I start prenatal yoga?</summary>
        <p>You can begin as soon as you feel comfortable and have medical clearance from your healthcare provider. Many women start in the second trimester, but some continue gentle practice throughout pregnancy.</p>
      </details>

      <details>
        <summary>3) When can I start postnatal yoga?</summary>
        <p>Most women can start 6–8 weeks after a vaginal birth or 8–12 weeks after a C-section — only after medical clearance. Everyone’s recovery is different, so listen to your body.</p>
      </details>

      <details>
        <summary>4) Are the poses safe for my stage of pregnancy or postpartum recovery?</summary>
        <p>Yes. Poses are modified according to your trimester or postpartum stage. We avoid deep twists, intense backbends, lying flat on your back after the first trimester, and any movements that cause strain or discomfort.</p>
      </details>

      <details>
        <summary>5) What should I bring to class?</summary>
        <ul>
          <li>Comfortable, stretchy clothing</li>
          <li>Water bottle</li>
          <li>Yoga mat</li>
          <li>Any props you like, such as a bolster or pillow for extra support</li>
        </ul>
      </details>

      <details>
        <summary>6) How is prenatal yoga different from regular yoga?</summary>
        <ul>
          <li>Creating space for your growing belly</li>
          <li>Supporting pelvic floor health</li>
          <li>Relieving pregnancy aches (back, hips, shoulders)</li>
          <li>Preparing your body and mind for labor through breathwork and relaxation</li>
        </ul>
      </details>

      <details>
        <summary>7) How is postnatal yoga different from regular yoga?</summary>
        <ul>
          <li>Restoring core and pelvic floor strength</li>
          <li>Improving posture and alignment after pregnancy</li>
          <li>Reducing tension from feeding, carrying, and caring for your baby</li>
          <li>Gentle reintroduction to movement without overstraining healing tissues</li>
        </ul>
      </details>

      <details>
        <summary>8) Can I participate if I have pregnancy-related conditions?</summary>
        <p>If you have conditions such as pelvic girdle pain, diastasis recti, or high blood pressure, let us know before class. We’ll adapt poses or recommend safe alternatives. Always get clearance from your healthcare provider first.</p>
      </details>

      <details>
        <summary>9) Will we do core work?</summary>
        <p>Yes, but in a safe, modified way. We focus on deep core activation and pelvic floor engagement, avoiding movements that put pressure on the abdominal wall or worsen separation.</p>
      </details>

      <details>
        <summary>10) Can I bring my baby to postnatal yoga?</summary>
        <p>Yes — babies are welcome in our postnatal classes. You can feed, change, or soothe your baby anytime during the session.</p>
      </details>
    </div>
  </section>

  <!-- CONTACT / CTA (simplified, no extra card) -->
  <section id="signup" class="container">
    <div class="card" style="padding:28px;">
      <div class="eyebrow">Join us</div>
      <h2>Ready to practice? Reserve your spot.</h2>
      <p class="sub">Spots are limited for a cozy, supportive vibe. Your registration helps us finalize days/times with the association.</p>
      <p><strong>Questions?</strong> Email <a href="mailto:maryjaucian@gmail.com">maryjaucian@gmail.com</a> or call/text <a href="tel:+19494688151">949-468-8151</a>.</p>
      <div class="cta">
        <a class="btn" href="https://forms.gle/your-google-form-id" target="_blank" rel="noopener">Open signup form</a>
        <a class="btn ghost" href="#top">Back to top</a>
      </div>
    </div>
  </section>

  <!-- FOOTER -->
  <footer class="foot">
    <div class="container row">
      <div>
        <strong>Family Yoga Institute (FYI)</strong> — Rancho Mission Viejo, CA<br/>
        © <span id="year"></span> Family Yoga Institute · All rights reserved
      </div>
      <div class="social">
        <a href="mailto:maryjaucian@gmail.com">Email</a> ·
        <a href="tel:+19494688151">Call/Text</a> ·
        <a href="#faq">FAQ</a>
      </div>
    </div>
  </footer>

  <script>
    // Mobile menu
    function toggleMenu(){
      const el = document.getElementById('mobileMenu');
      el.classList.toggle('open');
    }
    // Current year
    document.getElementById('year').textContent = new Date().getFullYear();

    // Smooth anchor scroll
    document.querySelectorAll('a[href^="#"]').forEach(a=>{
      a.addEventListener('click', e=>{
        const id=a.getAttribute('href').slice(1);
        const target=document.getElementById(id);
        if(target){
          e.preventDefault();
          // account for sticky nav height
          const offset = 72;
          const top = target.getBoundingClientRect().top + window.scrollY - offset;
          window.scrollTo({top, behavior:'smooth'});
        }
      });
    });
  </script>
</body>
</html>



