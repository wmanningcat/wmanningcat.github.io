import React from "react";

// Single-file React site for Family Yoga Institute (FYI)
// TailwindCSS is available by default. No external deps required.
// Replace GOOGLE_FORM_URL, LOCATION_TEXT, and SCHEDULE_ITEMS as needed.

const GOOGLE_FORM_URL = "https://forms.gle/your-form-id"; // TODO: paste real Google Form link
const EMAIL = "auntie.mary@example.com"; // TODO: replace with real email
const PHONE = "(555) 555-5555"; // TODO: replace with real phone
const LOCATION_TEXT = "Neighborhood Community Center, 123 Willow Lane, Your Town, ST"; // TODO

const SCHEDULE_ITEMS = [
  {
    title: "Mindful Mommy & Me",
    when: "Wednesdays • 10:00–10:45 AM",
    startDate: "Starting mid-September (pending HOA approval)",
    note: "Gentle stretches, bonding breathwork, and playful movement for caregivers and babies (6 weeks–18 months).",
  },
  {
    title: "Mindful Mommies To Be",
    when: "Saturdays • 9:00–9:55 AM",
    startDate: "Starting mid-September (pending HOA approval)",
    note: "Prenatal-friendly sequences to build strength, reduce stress, and prepare body & mind for birth.",
  },
];

export default function App() {
  return (
    <div className="min-h-screen bg-gradient-to-b from-teal-50 via-white to-purple-50 text-slate-800">
      {/* Brand palette */}
      <style>{`
        :root {
          --fyi-green: #3BAA7A; /* green */
          --fyi-teal: #00A3A3;  /* teal */
          --fyi-purple: #7C4DFF; /* purple */
        }
      `}</style>

      <Header />
      <Hero />
      <Highlights />
      <Classes />
      <Schedule />
      <About />
      <FAQ />
      <CTA />
      <Footer />
    </div>
  );
}

function Header() {
  return (
    <header className="sticky top-0 z-50 bg-white/80 backdrop-blur border-b border-teal-100">
      <div className="mx-auto max-w-6xl px-4 py-3 flex items-center justify-between">
        <div className="flex items-center gap-3">
          <Logo markOnly />
          <div className="leading-tight">
            <div className="font-semibold tracking-wide text-slate-900">Family Yoga Institute</div>
            <div className="text-xs text-slate-500 -mt-0.5">growing together</div>
          </div>
        </div>
        <nav className="hidden md:flex items-center gap-6 text-sm">
          <a href="#classes" className="hover:text-[var(--fyi-teal)]">Classes</a>
          <a href="#schedule" className="hover:text-[var(--fyi-teal)]">Schedule</a>
          <a href="#about" className="hover:text-[var(--fyi-teal)]">About</a>
          <a href="#faq" className="hover:text-[var(--fyi-teal)]">FAQ</a>
          <a href="#signup" className="px-4 py-2 rounded-xl border border-[var(--fyi-teal)] text-[var(--fyi-teal)] hover:bg-[var(--fyi-teal)] hover:text-white transition">Sign up</a>
        </nav>
      </div>
    </header>
  );
}

function Hero() {
  return (
    <section className="relative overflow-hidden">
      <div className="absolute inset-0 opacity-20 pointer-events-none" aria-hidden>
        <div className="absolute -top-24 -right-24 w-96 h-96 rounded-full bg-[var(--fyi-purple)] blur-3xl" />
        <div className="absolute -bottom-24 -left-24 w-96 h-96 rounded-full bg-[var(--fyi-teal)] blur-3xl" />
      </div>
      <div className="mx-auto max-w-6xl px-6 py-16 md:py-24 grid md:grid-cols-2 gap-10 items-center">
        <div>
          <h1 className="text-4xl md:text-5xl font-bold tracking-tight text-slate-900">
            Family Yoga Institute
          </h1>
          <p className="mt-4 text-lg text-slate-600">
            Community-centered yoga for moms, moms-to-be, and little ones —
            with a focus on mindfulness, connection, and accessible movement.
          </p>
          <p className="mt-3 text-sm text-slate-500">
            Pending final approval at the September association meeting, our neighborhood
            will promote classes and provide space. We’re excited to begin soon!
          </p>
          <div className="mt-6 flex flex-wrap gap-3">
            <a href="#classes" className="px-5 py-3 rounded-2xl bg-[var(--fyi-green)] text-white font-medium shadow hover:opacity-90">Explore classes</a>
            <a href="#signup" className="px-5 py-3 rounded-2xl border border-[var(--fyi-teal)] text-[var(--fyi-teal)] font-medium hover:bg-[var(--fyi-teal)] hover:text-white">Join the list</a>
          </div>
        </div>
        <div className="relative">
          <div className="aspect-[4/3] rounded-3xl bg-gradient-to-br from-teal-100 to-purple-100 border border-teal-200 shadow-inner flex items-center justify-center p-6">
            <Logo />
          </div>
          <p className="mt-3 text-center text-sm text-slate-500">Logo concept with tagline “growing together.” Colors: green, teal, purple.</p>
        </div>
      </div>
    </section>
  );
}

function Logo({ markOnly = false }) {
  return (
    <div className="flex items-center gap-3">
      <div className="relative w-12 h-12 md:w-16 md:h-16">
        <svg viewBox="0 0 100 100" className="w-full h-full">
          {/* Leaf circle */}
          <defs>
            <linearGradient id="leaf" x1="0" x2="1">
              <stop offset="0%" stopColor="#00A3A3" />
              <stop offset="100%" stopColor="#7C4DFF" />
            </linearGradient>
          </defs>
          <circle cx="50" cy="50" r="46" fill="url(#leaf)" opacity="0.15" />
          {/* Parent and child figure */}
          <path d="M35 60 C35 45 65 45 65 60 S35 75 35 60" fill="none" stroke="#3BAA7A" strokeWidth="6" strokeLinecap="round"/>
          <circle cx="40" cy="38" r="6" fill="#3BAA7A"/>
          <circle cx="60" cy="50" r="4" fill="#7C4DFF"/>
        </svg>
      </div>
      {!markOnly && (
        <div>
          <div className="text-xl font-semibold tracking-wide text-slate-900">Family Yoga Institute</div>
          <div className="text-xs text-slate-500 -mt-0.5">growing together</div>
        </div>
      )}
    </div>
  );
}

function Highlights() {
  return (
    <section className="mx-auto max-w-6xl px-6 py-12">
      <div className="grid md:grid-cols-3 gap-6">
        {[
          {
            title: "Community-supported",
            body: "Programming director is enthusiastic; HOA to promote and host upon approval in September.",
          },
          {
            title: "Pre & postnatal focus",
            body: "Mindful classes crafted for expecting moms and new caregivers with infants.",
          },
          {
            title: "Future-forward",
            body: "Plans include Mike joining as an instructor and on-site child care so moms can practice with peace of mind.",
          },
        ].map((c) => (
          <div key={c.title} className="rounded-3xl border border-teal-200 bg-white/60 p-6 shadow-sm">
            <h3 className="font-semibold text-slate-900">{c.title}</h3>
            <p className="mt-2 text-sm text-slate-600">{c.body}</p>
          </div>
        ))}
      </div>
    </section>
  );
}

function Classes() {
  return (
    <section id="classes" className="mx-auto max-w-6xl px-6 py-12">
      <div className="flex items-end justify-between">
        <h2 className="text-2xl md:text-3xl font-bold text-slate-900">Classes</h2>
        <a href="#signup" className="text-sm text-[var(--fyi-teal)] hover:underline">Reserve your spot →</a>
      </div>
      <div className="mt-6 grid md:grid-cols-2 gap-6">
        <ClassCard
          name="Mindful Mommy & Me"
          subtitle="Postnatal • 6 weeks–18 months"
          blurb="Gentle, playful movement that nurtures caregiver–baby connection. Expect cuddly poses, songs, and breath cues to soothe and center both of you. All levels welcome; feeding, diaper breaks, and tears are normal!"
          perks={["Bonding breathwork", "Pelvic-floor-friendly", "Community circle time"]}
        />
        <ClassCard
          name="Mindful Mommies To Be"
          subtitle="Prenatal • All trimesters"
          blurb="Supportive flows tailored to pregnancy: posture, mobility, and relaxation. Build confidence for birth with mindfulness, safe strength work, and restorative rest."
          perks={["Trimester-safe options", "Props & modifications", "Birth-prep breath"]}
        />
      </div>
    </section>
  );
}

function ClassCard({ name, subtitle, blurb, perks }) {
  return (
    <div className="rounded-3xl border border-purple-200 bg-white p-6 shadow-sm hover:shadow-md transition">
      <h3 className="text-xl font-semibold text-slate-900">{name}</h3>
      <p className="text-sm text-slate-500 mt-1">{subtitle}</p>
      <p className="mt-3 text-slate-700 text-sm leading-relaxed">{blurb}</p>
      <ul className="mt-4 flex flex-wrap gap-2">
        {perks.map((p) => (
          <li key={p} className="text-xs bg-teal-50 border border-teal-200 text-teal-700 px-3 py-1 rounded-full">{p}</li>
        ))}
      </ul>
    </div>
  );
}

function Schedule() {
  return (
    <section id="schedule" className="mx-auto max-w-6xl px-6 py-12">
      <h2 className="text-2xl md:text-3xl font-bold text-slate-900">Schedule & Location</h2>
      <div className="mt-6 grid md:grid-cols-3 gap-6">
        <div className="md:col-span-2 rounded-3xl border border-teal-200 bg-white p-6">
          <div className="grid sm:grid-cols-2 gap-4">
            {SCHEDULE_ITEMS.map((s) => (
              <div key={s.title} className="rounded-2xl border border-slate-200 p-4">
                <div className="font-semibold text-slate-900">{s.title}</div>
                <div className="text-sm text-slate-600 mt-1">{s.when}</div>
                <div className="text-xs text-slate-500 mt-1">{s.startDate}</div>
                <p className="text-sm text-slate-700 mt-2">{s.note}</p>
              </div>
            ))}
          </div>
          <div className="mt-4 text-xs text-slate-500">* Final dates may shift slightly based on venue scheduling.</div>
        </div>
        <div className="rounded-3xl border border-purple-200 bg-gradient-to-br from-purple-50 to-teal-50 p-6">
          <div className="font-semibold text-slate-900">Location</div>
          <p className="text-sm text-slate-700 mt-2">{LOCATION_TEXT}</p>
          <div className="mt-4 text-xs text-slate-500">The association plans to promote classes and provide space following September approval.</div>
        </div>
      </div>
    </section>
  );
}

function About() {
  return (
    <section id="about" className="mx-auto max-w-6xl px-6 py-12">
      <div className="grid md:grid-cols-2 gap-8 items-start">
        <div className="rounded-3xl border border-teal-200 bg-white p-6">
          <h3 className="text-xl font-semibold text-slate-900">About Auntie Mary</h3>
          <p className="mt-3 text-sm text-slate-700 leading-relaxed">
            Hi! I’m Mary, a community-minded yoga teacher passionate about supporting mothers at every stage —
            from pregnancy through postpartum and beyond. My teaching blends mindful movement, compassion,
            and practical tools for daily life. When I’m not on the mat, I’m dreaming up family-friendly
            wellness programs and ways to make yoga more accessible.
          </p>
        </div>
        <div className="rounded-3xl border border-purple-200 bg-white p-6">
          <h3 className="text-xl font-semibold text-slate-900">About the Family Yoga Institute (FYI)</h3>
          <p className="mt-3 text-sm text-slate-700 leading-relaxed">
            FYI is a neighborhood-based wellness hub focused on pre- and postnatal yoga and caregiver–child
            connection. Our mission is in our tagline: <span className="italic">growing together</span>.
            We aim to foster a supportive community, expand offerings over time, and eventually add on-site
            child care so moms can practice without the stress of arranging a sitter. In the future, Mike will
            also join the teaching team to broaden our class options.
          </p>
        </div>
      </div>
    </section>
  );
}

function FAQ() {
  return (
    <section id="faq" className="mx-auto max-w-6xl px-6 py-12">
      <h2 className="text-2xl md:text-3xl font-bold text-slate-900">FAQ</h2>
      <div className="mt-6 grid md:grid-cols-2 gap-6">
        {[
          {
            q: "Do I need yoga experience?",
            a: "Nope! Classes are beginner-friendly with lots of options and props."
          },
          {
            q: "What should I bring?",
            a: "A mat if you have one, water, and anything your little one needs. We’ll have a few extra mats."
          },
          {
            q: "When do classes start?",
            a: "We plan to begin after the September association meeting. Join the list to get notified first."
          },
          {
            q: "Will child care be available?",
            a: "That’s in the roadmap! We’re working toward offering on-site child care in future sessions."
          },
        ].map((f) => (
          <div key={f.q} className="rounded-2xl border border-slate-200 bg-white p-5">
            <div className="font-semibold text-slate-900">{f.q}</div>
            <div className="text-sm text-slate-700 mt-2">{f.a}</div>
          </div>
        ))}
      </div>
    </section>
  );
}

function CTA() {
  return (
    <section id="signup" className="mx-auto max-w-6xl px-6 py-12">
      <div className="rounded-3xl border border-teal-200 bg-white p-8 text-center shadow-sm">
        <Logo markOnly />
        <h2 className="mt-3 text-2xl md:text-3xl font-bold text-slate-900">Reserve your spot</h2>
        <p className="mt-2 text-sm text-slate-600">
          Add your name to be notified as soon as classes open. We’ll email details and early-bird options.
        </p>
        <div className="mt-5 flex flex-col sm:flex-row gap-3 justify-center">
          <a
            className="px-6 py-3 rounded-2xl bg-[var(--fyi-purple)] text-white font-medium hover:opacity-90"
            href={GOOGLE_FORM_URL}
            target="_blank"
            rel="noreferrer"
          >
            Fill out the Google Form
          </a>
          <a className="px-6 py-3 rounded-2xl border border-[var(--fyi-teal)] text-[var(--fyi-teal)] hover:bg-[var(--fyi-teal)] hover:text-white" href="#contact">Contact us</a>
        </div>
      </div>
    </section>
  );
}

function Footer() {
  return (
    <footer id="contact" className="mt-8 border-t border-teal-100 bg-white/70">
      <div className="mx-auto max-w-6xl px-6 py-10 grid md:grid-cols-4 gap-8">
        <div className="md:col-span-2">
          <Logo />
          <p className="mt-3 text-sm text-slate-600">
            Community-centered yoga for moms and families. Brand colors: green, teal, and purple.
          </p>
        </div>
        <div>
          <div className="font-semibold text-slate-900">Contact</div>
          <ul className="mt-2 text-sm text-slate-700">
            <li><a className="hover:underline" href={`mailto:${EMAIL}`}>{EMAIL}</a></li>
            <li className="mt-1"><a className="hover:underline" href={`tel:${PHONE}`}>{PHONE}</a></li>
          </ul>
        </div>
        <div>
          <div className="font-semibold text-slate-900">Location</div>
          <div className="mt-2 text-sm text-slate-700">{LOCATION_TEXT}</div>
        </div>
      </div>
      <div className="text-center text-xs text-slate-500 pb-8">© {new Date().getFullYear()} Family Yoga Institute. All rights reserved.</div>
    </footer>
  );
}
