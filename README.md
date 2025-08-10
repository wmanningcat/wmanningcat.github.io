
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
      <div class="relative flex items-center justify-center">
        <img src="logo.png" alt="Family Yoga Institute Logo" class="rounded-full shadow-lg max-h-72 max-w-full">
      </div>
    </div>
  </section>

  <!-- HIGHLIGHTS -->
  <!-- rest of code stays the same -->

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

