<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Family Yoga Institute – Growing Together</title>
  <meta name="description" content="Family Yoga Institute (FYI): Community-centered yoga for moms, moms-to-be, and little ones." />
  <script src="https://cdn.tailwindcss.com"></script>
  <style>
    :root {
      --fyi-green: #3BAA7A;
      --fyi-teal: #00A3A3;
      --fyi-purple: #7C4DFF;
    }
    .btn { @apply px-5 py-3 rounded-2xl font-medium transition; }
    .btn-primary { background: var(--fyi-green); color: white; }
    .btn-outline { @apply border; border-color: var(--fyi-teal); color: var(--fyi-teal); }
    .btn-outline:hover { background: var(--fyi-teal); color: white; }
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
        <img src="logo.png" alt="Family Yoga Institute Logo" class="rounded-full shadow-lg max-h-72 max-w-full bg-white">
      </div>
    </div>
  </section>

  <!-- CLASSES SECTION -->
  <section id="classes" class="mx-auto max-w-6xl px-6 py-16">
    <h2 class="text-3xl font-bold mb-8">Our Classes</h2>
    <div class="grid md:grid-cols-2 gap-8">
      <div class="p-6 bg-white rounded-xl shadow">
        <h3 class="text-xl font-semibold text-fyi-green">Mindful Mommy and Me</h3>
        <p class="mt-2 text-slate-600">A gentle yoga flow for moms and their little ones, focusing on connection, breathwork, and movement you can do together.</p>
      </div>
      <div class="p-6 bg-white rounded-xl shadow">
        <h3 class="text-xl font-semibold text-fyi-purple">Mindful Mommies To Be</h3>
        <p class="mt-2 text-slate-600">A prenatal yoga class designed to nurture and support expectant moms, with a focus on breath, relaxation, and preparing the body for birth.</p>
      </div>
    </div>
  </section>

  <!-- ABOUT SECTION -->
  <section id="about" class="bg-white py-16">
    <div class="mx-auto max-w-4xl px-6">
      <h2 class="text-3xl font-bold mb-6">About Us</h2>
      <p class="text-slate-600">[About Me and About FYI text will go here – please provide content]</p>
    </div>
  </section>

  <!-- FAQ SECTION -->
  <section id="faq" class="mx-auto max-w-4xl px-6 py-16">
    <h2 class="text-3xl font-bold mb-6">FAQ</h2>
    <p class="text-slate-600">[FAQ answers will go here – please provide content]</p>
  </section>

  <!-- SIGN UP -->
  <section id="signup" class="bg-gradient-to-r from-fyi-green to-fyi-teal py-16">
    <div class="mx-auto max-w-4xl px-6 text-center text-white">
      <h2 class="text-3xl font-bold mb-4">Sign up for a class</h2>
      <a id="fyi-form" href="#" class="btn bg-white text-fyi-green font-bold">Sign Up Form</a>
    </div>
  </section>

  <!-- FOOTER -->
  <footer class="bg-slate-900 text-white py-8 mt-12">
    <div class="mx-auto max-w-6xl px-6 grid md:grid-cols-3 gap-6">
      <div>
        <h3 class="font-bold mb-2">Contact</h3>
        <p>Email: <a id="fyi-email" class="underline"></a></p>
        <p>Phone: <a id="fyi-phone" class="underline"></a></p>
      </div>
      <div>
        <h3 class="font-bold mb-2">Location</h3>
        <p id="fyi-location-footer"></p>
      </div>
      <div>
        <p>&copy; <span id="year"></span> Family Yoga Institute</p>
      </div>
    </div>
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
    document.getElementById('fyi-location-footer').textContent = SETTINGS.location;
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>

</body>
</html>

