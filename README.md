
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Family Yoga Institute – Growing Together</title>
  <meta name="description" content="Family Yoga Institute (FYI): Community-centered yoga for moms, moms-to-be, and little ones." />
  <!-- Tailwind via CDN (copy-paste friendly) -->
  <script src="https://cdn.tailwindcss.com"></script>
  <style>
    :root{
      --fyi-green:#3BAA7A; /* green */
      --fyi-teal:#00A3A3;  /* teal */
      --fyi-purple:#7C4DFF; /* purple */
    }
    .btn{ @apply px-5 py-3 rounded-2xl font-medium transition; }
    .btn-primary{ background:var(--fyi-green); color:white; }
    .btn-outline{ @apply border; border-color:var(--fyi-teal); color:var(--fyi-teal); }
    .btn-outline:hover{ background:var(--fyi-teal); color:white; }
  </style>
</head>
<body class="min-h-screen bg-gradient-to-b from-teal-50 via-white to-purple-50 text-slate-800">
  <!-- ====== HEADER ====== -->
  <header class="sticky top-0 z-50 bg-white/80 backdrop-blur border-b border-teal-100">
    <div class="mx-auto max-w-6xl px-4 py-3 flex items-center justify-between">
      <div class="flex items-center gap-3">
        <div class="relative w-12 h-12">
          <!-- Simple inline logo mark -->
          <svg viewBox="0 0 100 100" class="w-full h-full">
            <defs>
              <linearGradient id="leaf" x1="0" x2="1">
                <stop offset="0%" stop-color="#00A3A3" />
                <stop offset="100%" stop-color="#7C4DFF" />
              </linearGradient>
            </defs>
            <circle cx="50" cy="50" r="46" fill="url(#leaf)" opacity="0.15" />
            <path d="M35 60 C35 45 65 45 65 60 S35 75 35 60" fill="none" stroke="#3BAA7A" stroke-width="6" stroke-linecap="round"/>
            <circle cx="40" cy="38" r="6" fill="#3BAA7A"/>
            <circle cx="60" cy="50" r="4" fill="#7C4DFF"/>
          </svg>
        </div>
        <div class="leading-tight">
          <div class="font-semibold tracking-wide text-slate-900">Family Yoga Institute</div>
          <div class="text-xs text-slate-500 -mt-0.5">growing together</div>
        </div>
      </div>
      <nav class="hidden md:flex items-center gap-6 text-sm">
        <a href="#classes" class="hover:text-[color:var(--fyi-teal)]">Classes</a>
        <a href="#schedule" class="hover:text-[color:var(--fyi-teal)]">Schedule</a>
        <a href="#about" class="hover:text-[color:var(--fyi-teal)]">About</a>
        <a href="#faq" class="hover:text-[color:var(--fyi-teal)]">FAQ</a>
        <a href="#signup" class="px-4 py-2 rounded-xl border" style="border-color:var(--fyi-teal); color:var(--fyi-teal);">Sign up</a>
      </nav>
    </div>
  </header>

  <!-- ====== HERO ====== -->
  <section class="relative overflow-hidden">
    <div class="absolute inset-0 opacity-20 pointer-events-none" aria-hidden>
      <div class="absolute -top-24 -right-24 w-96 h-96 rounded-full" style="background:var(--fyi-purple); filter:blur(36px);"></div>
      <div class="absolute -bottom-24 -left-24 w-96 h-96 rounded-full" style="background:var(--fyi-teal); filter:blur(36px);"></div>
    </div>
    <div class="mx-auto max-w-6xl px-6 py-16 md:py-24 grid md:grid-cols-2 gap-10 items-center">
      <div>
        <h1 class="text-4xl md:text-5xl font-bold tracking-tight text-slate-900">Family Yoga Institute</h1>
        <p class="mt-4 text-lg text-slate-600">Community-centered yoga for moms, moms-to-be, and little ones — with a focus on mindfulness, connection, and accessible movement.</p>
        <p class="mt-3 text-sm text-slate-500">Pending final approval at the September association meeting, our neighborhood will promote classes and provide space. We’re excited to begin soon!</p>
        <div class="mt-6 flex flex-wrap gap-3">
          <a href="#classes" class="btn btn-primary">Explore classes</a>
          <a href="#signup" class="btn btn-outline">Join the list</a>
        </div>
      </div>
      <div class="relative">
        <div class="aspect-[4/3] rounded-3xl bg-gradient-to-br from-teal-100 to-purple-100 border border-teal-200 shadow-inner flex items-center justify-center p-6">
          <!-- Big logo -->
          <svg viewBox="0 0 100 100" class="w-40 h-40">
            <defs>
              <linearGradient id="leaf2" x1="0" x2="1">
                <stop offset="0%" stop-color="#00A3A3" />
                <stop offset="100%" stop-color="#7C4DFF" />
              </linearGradient>
            </defs>
            <circle cx="50" cy="50" r="46" fill="url(#leaf2)" opacity="0.15" />
            <path d="M35 60 C35 45 65 45 65 60 S35 75 35 60" fill="none" stroke="#3BAA7A" stroke-width="6" stroke-linecap="round"/>
            <circle cx="40" cy="38" r="6" fill="#3BAA7A"/>
            <circle cx="60" cy="50" r="4" fill="#7C4DFF"/>
          </svg>
        </div>
        <p class="mt-3 text-center text-sm text-slate-500">Logo concept with tagline “growing together.” Colors: green, teal, purple.</p>
      </div>
    </div>
  </section>

  <!-- ====== HIGHLIGHTS ====== -->
  <section class="mx-auto max-w-6xl px-6 py-12">
    <div class="grid md:grid-cols-3 gap-6">
      <div class="rounded-3xl border border-teal-200 bg-white/60 p-6 shadow-sm">
        <h3 class="font-semibold text-slate-900">Community-supported</h3>
        <p class="mt-2 text-sm text-slate-600">Programming director is enthusiastic; HOA to promote and host upon approval in September.</p>
      </div>
      <div class="rounded-3xl border border-teal-200 bg-white/60 p-6 shadow-sm">
        <h3 class="font-semibold text-slate-900">Pre & postnatal focus</h3>
        <p class="mt-2 text-sm text-slate-600">Mindful classes crafted for expecting moms and new caregivers with infants.</p>
      </div>
      <div class="rounded-3xl border border-teal-200 bg-white/60 p-6 shadow-sm">
        <h3 class="font-semibold text-slate-900">Future-forward</h3>
        <p class="mt-2 text-sm text-slate-600">Plans include Mike joining as an instructor and on-site child care so moms can practice with peace of mind.</p>
      </div>
    </div>
  </section>

  <!-- ====== CLASSES ====== -->
  <section id="classes" class="mx-auto max-w-6xl px-6 py-12">
    <div class="flex items-end justify-between">
      <h2 class="text-2xl md:text-3xl font-bold text-slate-900">Classes</h2>
      <a href="#signup" class="text-sm" style="color:var(--fyi-teal)">Reserve your spot →</a>
    </div>
    <div class="mt-6 grid md:grid-cols-2 gap-6">
      <div class="rounded-3xl border border-purple-200 bg-white p-6 shadow-sm hover:shadow-md transition">
        <h3 class="text-xl font-semibold text-slate-900">Mindful Mommy & Me</h3>
        <p class="text-sm text-slate-500 mt-1">Postnatal • 6 weeks–18 months</p>
        <p class="mt-3 text-slate-700 text-sm leading-relaxed">Gentle, playful movement that nurtures caregiver–baby connection. Expect cuddly poses, songs, and breath cues to soothe and center both of you. All levels welcome; feeding, diaper breaks, and tears are normal!</p>
        <ul class="mt-4 flex flex-wrap gap-2">
          <li class="text-xs bg-teal-50 border border-teal-200 text-teal-700 px-3 py-1 rounded-full">Bonding breathwork</li>
          <li class="text-xs bg-teal-50 border border-teal-200 text-teal-700 px-3 py-1 rounded-full">Pelvic-floor-friendly</li>
          <li class="text-xs bg-teal-50 border border-teal-200 text-teal-700 px-3 py-1 rounded-full">Community circle time</li>
        </ul>
      </div>
      <div class="rounded-3xl border border-purple-200 bg-white p-6 shadow-sm hover:shadow-md transition">
        <h3 class="text-xl font-semibold text-slate-900">Mindful Mommies To Be</h3>
        <p class="text-sm text-slate-500 mt-1">Prenatal • All trimesters</p>
        <p class="mt-3 text-slate-700 text-sm leading-relaxed">Supportive flows tailored to pregnancy: posture, mobility, and relaxation. Build confidence for birth with mindfulness, safe strength work, and restorative rest.</p>
        <ul class="mt-4 flex flex-wrap gap-2">
          <li class="text-xs bg-teal-50 border border-teal-200 text-teal-700 px-3 py-1 rounded-full">Trimester-safe options</li>
          <li class="text-xs bg-teal-50 border border-teal-200 text-teal-700 px-3 py-1 rounded-full">Props & modifications</li>
          <li class="text-xs bg-teal-50 border border-teal-200 text-teal-700 px-3 py-1 rounded-full">Birth-prep breath</li>
        </ul>
      </div>
    </div>
  </section>

  <!-- ====== SCHEDULE & LOCATION ====== -->
  <section id="schedule" class="mx-auto max-w-6xl px-6 py-12">
    <h2 class="text-2xl md:text-3xl font-bold text-slate-900">Schedule & Location</h2>
    <div class="mt-6 grid md:grid-cols-3 gap-6">
      <div class="md:col-span-2 rounded-3xl border border-teal-200 bg-white p-6">
        <div class="grid sm:grid-cols-2 gap-4">
          <div class="rounded-2xl border border-slate-200 p-4">
            <div class="font-semibold text-slate-900">Mindful Mommy & Me</div>
            <div class="text-sm text-slate-600 mt-1">Wednesdays • 10:00–10:45 AM</div>
            <div class="text-xs text-slate-500 mt-1">Starting mid-September (pending HOA approval)</div>
            <p class="text-sm text-slate-700 mt-2">Gentle stretches, bonding breathwork, and playful movement for caregivers and babies (6 weeks–18 months).</p>
          </div>
          <div class="rounded-2xl border border-slate-200 p-4">
            <div class="font-semibold text-slate-900">Mindful Mommies To Be</div>
            <div class="text-sm text-slate-600 mt-1">Saturdays • 9:00–9:55 AM</div>
            <div class="text-xs text-slate-500 mt-1">Starting mid-September (pending HOA approval)</div>
            <p class="text-sm text-slate-700 mt-2">Prenatal-friendly sequences to build strength, reduce stress, and prepare body & mind for birth.</p>
          </div>
        </div>
        <div class="mt-4 text-xs text-slate-500">* Final dates may shift slightly based on venue scheduling.</div>
      </div>
      <div class="rounded-3xl border border-purple-200 bg-gradient-to-br from-purple-50 to-teal-50 p-6">
        <div class="font-semibold text-slate-900">Location</div>
        <p class="text-sm text-slate-700 mt-2" id="fyi-location">Neighborhood Community Center, 123 Willow Lane, Your Town, ST</p>
        <div class="mt-4 text-xs text-slate-500">The association plans to promote classes and provide space following September approval.</div>
      </div>
    </div>
  </section>

  <!-- ====== ABOUT ====== -->
  <section id="about" class="mx-auto max-w-6xl px-6 py-12">
    <div class="grid md:grid-cols-2 gap-8 items-start">
      <div class="rounded-3xl border border-teal-200 bg-white p-6">
        <h3 class="text-xl font-semibold text-slate-900">About Auntie Mary</h3>
        <p class="mt-3 text-sm text-slate-700 leading-relaxed">Hi! I’m Mary, a community-minded yoga teacher passionate about supporting mothers at every stage — from pregnancy through postpartum and beyond. My teaching blends mindful movement, compassion, and practical tools for daily life. When I’m not on the mat, I’m dreaming up family-friendly wellness programs and ways to make yoga more accessible.</p>
      </div>
      <div class="rounded-3xl border border-purple-200 bg-white p-6">
        <h3 class="text-xl font-semibold text-slate-900">About the Family Yoga Institute (FYI)</h3>
        <p class="mt-3 text-sm text-slate-700 leading-relaxed">FYI is a neighborhood-based wellness hub focused on pre- and postnatal yoga and caregiver–child connection. Our mission is in our tagline: <em>growing together</em>. We aim to foster a supportive community, expand offerings over time, and eventually add on-site child care so moms can practice without the stress of arranging a sitter. In the future, Mike will also join the teaching team to broaden our class options.</p>
      </div>
    </div>
  </section>

  <!-- ====== FAQ ====== -->
  <section id="faq" class="mx-auto max-w-6xl px-6 py-12">
    <h2 class="text-2xl md:text-3xl font-bold text-slate-900">FAQ</h2>
    <div class="mt-6 grid md:grid-cols-2 gap-6">
      <div class="rounded-2xl border border-slate-200 bg-white p-5">
        <div class="font-semibold text-slate-900">Do I need yoga experience?</div>
        <div class="text-sm text-slate-700 mt-2">Nope! Classes are beginner-friendly with lots of options and props.</div>
      </div>
      <div class="rounded-2xl border border-slate-200 bg-white p-5">
        <div class="font-semibold text-slate-900">What should I bring?</div>
        <div class="text-sm text-slate-700 mt-2">A mat if you have one, water, and anything your little one needs. We’ll have a few extra mats.</div>
      </div>
      <div class="rounded-2xl border border-slate-200 bg-white p-5">
        <div class="font-semibold text-slate-900">When do classes start?</div>
        <div class="text-sm text-slate-700 mt-2">We plan to begin after the September association meeting. Join the list to get notified first.</div>
      </div>
      <div class="rounded-2xl border border-slate-200 bg-white p-5">
        <div class="font-semibold text-slate-900">Will child care be available?</div>
        <div class="text-sm text-slate-700 mt-2">That’s in the roadmap! We’re working toward offering on-site child care in future sessions.</div>
      </div>
    </div>
  </section>

  <!-- ====== CTA / SIGNUP ====== -->
  <section id="signup" class="mx-auto max-w-6xl px-6 py-12">
    <div class="rounded-3xl border border-teal-200 bg-white p-8 text-center shadow-sm">
      <div class="flex items-center justify-center gap-3">
        <div class="relative w-12 h-12">
          <svg viewBox="0 0 100 100" class="w-full h-full">
            <defs>
              <linearGradient id="leaf3" x1="0" x2="1">
                <stop offset="0%" stop-color="#00A3A3" />
                <stop offset="100%" stop-color="#7C4DFF" />
              </linearGradient>
            </defs>
            <circle cx="50" cy="50" r="46" fill="url(#leaf3)" opacity="0.15" />
            <path d="M35 60 C35 45 65 45 65 60 S35 75 35 60" fill="none" stroke="#3BAA7A" stroke-width="6" stroke-linecap="round"/>
            <circle cx="40" cy="38" r="6" fill="#3BAA7A"/>
            <circle cx="60" cy="50" r="4" fill="#7C4DFF"/>
          </svg>
        </div>
        <div class="text-left">
          <h2 class="text-2xl md:text-3xl font-bold text-slate-900">Reserve your spot</h2>
          <p class="mt-1 text-sm text-slate-600">Add your name to be notified as soon as classes open. We’ll email details and early-bird options.</p>
        </div>
      </div>
      <div class="mt-5 flex flex-col sm:flex-row gap-3 justify-center">
        <a class="btn btn-primary" id="fyi-form" href="#" target="_blank" rel="noreferrer">Fill out the Google Form</a>
        <a class="btn btn-outline" href="#contact">Contact us</a>
      </div>
    </div>
  </section>

  <!-- ====== FOOTER ====== -->
  <footer id="contact" class="mt-8 border-t border-teal-100 bg-white/70">
    <div class="mx-auto max-w-6xl px-6 py-10 grid md:grid-cols-4 gap-8">
      <div class="md:col-span-2">
        <div class="flex items-center gap-3">
          <div class="relative w-12 h-12">
            <svg viewBox="0 0 100 100" class="w-full h-full">
              <defs>
                <linearGradient id="leaf4" x1="0" x2="1">
                  <stop offset="0%" stop-color="#00A3A3" />
                  <stop offset="100%" stop-color="#7C4DFF" />
                </linearGradient>
              </defs>
              <circle cx="50" cy="50" r="46" fill="url(#leaf4)" opacity="0.15" />
              <path d="M35 60 C35 45 65 45 65 60 S35 75 35 60" fill="none" stroke="#3BAA7A" stroke-width="6" stroke-linecap="round"/>
              <circle cx="40" cy="38" r="6" fill="#3BAA7A"/>
              <circle cx="60" cy="50" r="4" fill="#7C4DFF"/>
            </svg>
          </div>
          <div>
            <div class="text-xl font-semibold tracking-wide text-slate-900">Family Yoga Institute</div>
            <div class="text-xs text-slate-500 -mt-0.5">growing together</div>
          </div>
        </div>
        <p class="mt-3 text-sm text-slate-600">Community-centered yoga for moms and families. Brand colors: green, teal, and purple.</p>
      </div>
      <div>
        <div class="font-semibold text-slate-900">Contact</div>
        <ul class="mt-2 text-sm text-slate-700">
          <li><a class="hover:underline" id="fyi-email" href="mailto:auntie.mary@example.com">auntie.mary@example.com</a></li>
          <li class="mt-1"><a class="hover:underline" id="fyi-phone" href="tel:(555) 555-5555">(555) 555-5555</a></li>
        </ul>
      </div>
      <div>
        <div class="font-semibold text-slate-900">Location</div>
        <div class="mt-2 text-sm text-slate-700" id="fyi-location-footer">Neighborhood Community Center, 123 Willow Lane, Your Town, ST</div>
      </div>
    </div>
    <div class="text-center text-xs text-slate-500 pb-8">© <span id="year"></span> Family Yoga Institute. All rights reserved.</div>
  </footer>

  <!-- ====== SIMPLE EDITABLE SETTINGS ====== -->
  <script>
    // EDIT THESE 4 LINES ONLY (or directly edit the HTML above)
    const SETTINGS = {
      googleForm: 'https://forms.gle/your-form-id',
      email: 'auntie.mary@example.com',
      phone: '(555) 555-5555',
      location: 'Neighborhood Community Center, 123 Willow Lane, Your Town, ST',
    };

    // Apply settings
    document.getElementById('fyi-form').href = SETTINGS.googleForm;
    document.getElementById('fyi-email').href = 'mailto:' + SETTINGS.email;
    document.getElementById('fyi-email').textContent = SETTINGS.email;
    document.getElementById('fyi-phone').href = 'tel:' + SETTINGS.phone;
    document.getElementById('fyi-phone').textContent = SETTINGS.phone;
    document.getElementById('fyi-location').textContent = SETTINGS.location;
    document.getElementById('fyi-location-footer').textContent = SETTINGS.location;
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>
</body>
</html>

