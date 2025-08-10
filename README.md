<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Family Yoga Institute – Growing Together</title>
  <meta name="description" content="Family Yoga Institute (FYI): Community-centered yoga for moms, moms-to-be, and little ones." />
  <script src="https://cdn.tailwindcss.com"></script>
  <style>
    :root{
      --fyi-green:#3BAA7A;
      --fyi-teal:#00A3A3;
      --fyi-purple:#7C4DFF;
    }
    .btn{ @apply px-5 py-3 rounded-2xl font-medium transition; }
    .btn-primary{ background:var(--fyi-green); color:white; }
    .btn-outline{ @apply border; border-color:var(--fyi-teal); color:var(--fyi-teal); }
    .btn-outline:hover{ background:var(--fyi-teal); color:white; }
  </style>
</head>
<body class="min-h-screen bg-gradient-to-b from-teal-50 via-white to-purple-50 text-slate-800">

  <!-- HERO -->
  <section class="relative overflow-hidden">
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
      <div class="relative flex items-center justify-center">
        <img src="logo.png" alt="Family Yoga Institute Logo" class="rounded-3xl shadow-lg max-h-72 max-w-full bg-white">
      </div>
    </div>
  </section>

  <!-- HIGHLIGHTS -->
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

  <!-- CLASSES -->
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
      </div>
      <div class="rounded-3xl border border-purple-200 bg-white p-6 shadow-sm hover:shadow-md transition">
        <h3 class="text-xl font-semibold text-slate-900">Mindful Mommies To Be</h3>
        <p class="text-sm text-slate-500 mt-1">Prenatal • All trimesters</p>
        <p class="mt-3 text-slate-700 text-sm leading-relaxed">Supportive flows tailored to pregnancy: posture, mobility, and relaxation. Build confidence for birth with mindfulness, safe strength work, and restorative rest.</p>
      </div>
    </div>
  </section>

  <!-- SCHEDULE & LOCATION -->
  <section id="schedule" class="mx-auto max-w-6xl px-6 py-12">
    <h2 class="text-2xl md:text-3xl font-bold text-slate-900">Schedule & Location</h2>
    <div class="mt-6 grid md:grid-cols-3 gap-6">
      <div class="md:col-span-2 rounded-3xl border border-teal-200 bg-white p-6">
        <div class="grid sm:grid-cols-2 gap-4">
          <div class="rounded-2xl border border-slate-200 p-4">
            <div class="font-semibold text-slate-900">Mindful Mommy & Me</div>
            <div class="text-sm text-slate-600 mt-1">Wednesdays • 10:00–10:45 AM</div>
            <div class="text-xs text-slate-500 mt-1">Starting mid-September (pending HOA approval)</div>
          </div>
          <div class="rounded-2xl border border-slate-200 p-4">
            <div class="font-semibold text-slate-900">Mindful Mommies To Be</div>
            <div class="text-sm text-slate-600 mt-1">Saturdays • 9:00–9:55 AM</div>
            <div class="text-xs text-slate-500 mt-1">Starting mid-September (pending HOA approval)</div>
          </div>
        </div>
      </div>
      <div class="rounded-3xl border border-purple-200 bg-gradient-to-br from-purple-50 to-teal-50 p-6">
        <div class="font-semibold text-slate-900">Location</div>
        <p class="text-sm text-slate-700 mt-2" id="fyi-location">Neighborhood Community Center, 123 Willow Lane, Your Town, ST</p>
      </div>
    </div>
  </section>

  <!-- ABOUT -->
  <section id="about" class="mx-auto max-w-6xl px-6 py-12">
    <div class="grid md:grid-cols-2 gap-8 items-start">
      <div class="rounded-3xl border border-teal-200 bg-white p-6">
        <h3 class="text-xl font-semibold text-slate-900">About Auntie Mary</h3>
        <p class="mt-3 text-sm text-slate-700 leading-relaxed">Hi! I’m Mary, a community-minded yoga teacher passionate about supporting mothers at every stage — from pregnancy through postpartum and beyond. My teaching blends mindful movement, compassion, and practical tools for daily life.</p>
      </div>
      <div class="rounded-3xl border border-purple-200 bg-white p-6">
        <h3 class="text-xl font-semibold text-slate-900">About the Family Yoga Institute (FYI)</h3>
        <p class="mt-3 text-sm text-slate-700 leading-relaxed">FYI is a neighborhood-based wellness hub focused on pre- and postnatal yoga and caregiver–child connection. Our mission is in our tagline: <em>growing together</em>. We aim to foster a supportive community and eventually add on-site child care so moms can practice without the stress of arranging a sitter.</p>
      </div>
    </div>
  </section>

  <!-- FAQ -->
  <section id="faq" class="mx-auto max-w-6xl px-6 py-12">
    <h2 class="text-2xl md:text-3xl font-bold text-slate-900">FAQ</h2>
    <div class="mt-6 grid md:grid-cols-2 gap-6">
      <div class="rounded-2xl border border-slate-200 bg-white p-5">
        <div class="font-semibold text-slate-900">Do I need yoga experience?</div>
        <div class="text-sm text-slate-700 mt-2">Nope! Classes are beginner-friendly with lots of options and props.</div>
      </div>
      <div class="rounded-2xl border border-slate-200 bg-white p-5">
        <div class="font-semibold text-slate-900">What should I bring?</div>
        <div class="text-sm text-slate-700 mt-2">A mat if you have one, water, and anything your little one needs.</div>
      </div>
    </div>
  </section>

  <!-- CTA -->
  <section id="signup" class="mx-auto max-w-6xl px-6 py-12">
    <div class="rounded-3xl border border-teal-200 bg-white p-8 text-center shadow-sm">
      <h2 class="mt-3 text-2xl md:text-3xl font-bold text-slate-900">Reserve your spot</h2>
      <p class="mt-2 text-sm text-slate-600">Add your name to be notified as soon as classes open.</p>
      <div class="mt-5 flex flex-col sm:flex-row gap-3 justify-center">
        <a class="btn btn-primary" id="fyi-form" href="#" target="_blank" rel="noreferrer">Fill out the Google Form</a>
        <a class="btn btn-outline" href="#contact">Contact us</a>
      </div>
    </div>
  </section>

  <!-- FOOTER -->
  <footer id="contact" class="mt-8 border-t border-teal-100 bg-white/70">
    <div class="mx-auto max-w-6xl px-6 py-10 grid md:grid-cols-4 gap-8">
      <div class="md:col-span-2">
        <img src="logo.png" alt="Family Yoga Institute Logo" class="h-12 w-auto rounded-2xl shadow-sm ring-1 ring-teal-200/50">
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

  <script>
    const SETTINGS = {
      googleForm: 'https://forms.gle/your-form-id',
      email: 'auntie.mary@example.com',
      phone: '(555) 555-5555',
      location: 'Neighborhood Community Center, 123 Willow Lane, Your Town, ST',
    };
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

