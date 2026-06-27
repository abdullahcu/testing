import { useEffect, useRef, useState } from "react";
import { motion, useInView, useScroll, useTransform, animate } from "motion/react";
import {
  ArrowRight, ArrowUpRight, Menu, X, Moon, Sun, Star, Mail, Phone,
  Linkedin, Facebook, MessageCircle, MapPin, ChevronUp,
  Target, TrendingUp, Search, Megaphone, MapPinned, Share2,
  MousePointerClick, LineChart, BarChart3, Sparkles,
} from "lucide-react";
import portrait from "@/assets/portrait.jpg";

const NAV = [
  { id: "home", label: "Home" },
  { id: "about", label: "About" },
  { id: "services", label: "Services" },
  { id: "portfolio", label: "Portfolio" },
  { id: "skills", label: "Skills" },
  { id: "blog", label: "Blog" },
  { id: "contact", label: "Contact" },
];

const SERVICES = [
  { icon: Facebook, title: "Facebook & Instagram Ads", desc: "Full-funnel Meta campaigns engineered for ROAS, from creative testing to scale." },
  { icon: Target, title: "Google Ads", desc: "Search, Performance Max and YouTube campaigns dialed in for high-intent conversions." },
  { icon: MousePointerClick, title: "Lead Generation", desc: "Predictable B2B and B2C lead pipelines with qualified, sales-ready prospects." },
  { icon: MapPinned, title: "Local Business Marketing", desc: "Google Business Profile, local SEO and geo-targeted ads that fill your calendar." },
  { icon: Search, title: "SEO", desc: "Technical SEO, content strategy and link building for compounding organic growth." },
  { icon: Share2, title: "Social Media Marketing", desc: "Brand-building content systems that turn followers into customers." },
  { icon: TrendingUp, title: "Conversion Rate Optimization", desc: "Landing pages and funnels A/B tested to lift conversion without raising spend." },
  { icon: Megaphone, title: "Marketing Strategy", desc: "Positioning, messaging and a 90-day roadmap built around your business goals." },
  { icon: BarChart3, title: "Analytics & Reporting", desc: "GA4, GTM and dashboards that turn data into clear, profitable decisions." },
];

const SKILLS = [
  { name: "Meta Ads", level: 95 },
  { name: "Google Ads", level: 93 },
  { name: "Google Analytics", level: 92 },
  { name: "Google Tag Manager", level: 88 },
  { name: "SEO", level: 90 },
  { name: "Email Marketing", level: 85 },
  { name: "Copywriting", level: 87 },
  { name: "Canva", level: 82 },
  { name: "WordPress", level: 84 },
  { name: "HubSpot", level: 88 },
  { name: "CRM", level: 86 },
  { name: "Marketing Automation", level: 89 },
];

const CASES = [
  {
    title: "Scaling a DTC Skincare Brand",
    industry: "E-commerce / Beauty",
    challenge: "Stagnant revenue with rising ad costs and inconsistent ROAS.",
    strategy: "Restructured Meta and Google accounts, launched UGC creative testing, rebuilt funnel.",
    before: { label: "Monthly Revenue", value: "$42K" },
    after: { label: "Monthly Revenue", value: "$187K" },
    metric: "+345% ROAS",
  },
  {
    title: "B2B SaaS Lead Engine",
    industry: "SaaS / B2B",
    challenge: "High CPL and unqualified demo requests draining the sales pipeline.",
    strategy: "LinkedIn + Google intent campaigns paired with lead scoring and nurture sequences.",
    before: { label: "Cost per Lead", value: "$184" },
    after: { label: "Cost per Lead", value: "$47" },
    metric: "-74% CPL",
  },
  {
    title: "Local Dental Practice Growth",
    industry: "Healthcare / Local",
    challenge: "Empty appointment book and weak local visibility against competitors.",
    strategy: "Local SEO overhaul, GBP optimization, and geo-targeted Meta lead ads.",
    before: { label: "New Patients / mo", value: "12" },
    after: { label: "New Patients / mo", value: "68" },
    metric: "+466% Bookings",
  },
];

const TESTIMONIALS = [
  { name: "Sarah Chen", role: "Founder", company: "Luma Skincare", rating: 5, quote: "Alex turned our ads from a money pit into our most reliable growth channel. We 4x'd revenue in six months." },
  { name: "Marcus Reid", role: "VP Marketing", company: "Northwind SaaS", rating: 5, quote: "The strategic clarity and execution speed are unmatched. Our pipeline has never been healthier." },
  { name: "Dr. Priya Shah", role: "Owner", company: "Bright Smile Dental", rating: 5, quote: "We finally have a predictable flow of new patients. Worth every dollar, ten times over." },
];

const STATS = [
  { label: "Campaigns Managed", value: 320, suffix: "+" },
  { label: "Leads Generated", value: 48000, suffix: "+" },
  { label: "Ad Spend Managed", value: 12, prefix: "$", suffix: "M+" },
  { label: "Average ROI", value: 410, suffix: "%" },
  { label: "Happy Clients", value: 140, suffix: "+" },
];

const POSTS = [
  { title: "The 2026 Performance Marketing Playbook", excerpt: "How AI-assisted creative testing is reshaping paid media efficiency.", tag: "Strategy", date: "May 28, 2026" },
  { title: "Why Your CPL Keeps Climbing (And How to Fix It)", excerpt: "A diagnostic framework for restoring lead-gen efficiency in saturated markets.", tag: "Lead Gen", date: "May 12, 2026" },
  { title: "GA4 + Server-Side Tracking: A Practical Guide", excerpt: "Reclaim attribution accuracy with a clean, privacy-first measurement stack.", tag: "Analytics", date: "April 30, 2026" },
];

function useDarkMode() {
  const [dark, setDark] = useState(false);
  useEffect(() => {
    const root = document.documentElement;
    dark ? root.classList.add("dark") : root.classList.remove("dark");
  }, [dark]);
  return [dark, setDark] as const;
}

function Counter({ value, prefix = "", suffix = "" }: { value: number; prefix?: string; suffix?: string }) {
  const ref = useRef<HTMLSpanElement>(null);
  const inView = useInView(ref, { once: true, margin: "-50px" });
  const [display, setDisplay] = useState(0);
  useEffect(() => {
    if (!inView) return;
    const controls = animate(0, value, {
      duration: 2,
      ease: "easeOut",
      onUpdate: (v) => setDisplay(Math.round(v)),
    });
    return () => controls.stop();
  }, [inView, value]);
  return (
    <span ref={ref}>
      {prefix}{display.toLocaleString()}{suffix}
    </span>
  );
}

function Section({ id, children, className = "" }: { id?: string; children: React.ReactNode; className?: string }) {
  return (
    <section id={id} className={`scroll-mt-24 px-6 py-24 sm:py-32 md:px-10 ${className}`}>
      <div className="mx-auto max-w-7xl">{children}</div>
    </section>
  );
}

function Eyebrow({ children }: { children: React.ReactNode }) {
  return (
    <div className="inline-flex items-center gap-2 rounded-full border border-border bg-surface/60 px-3 py-1 text-xs font-medium uppercase tracking-[0.18em] text-muted-foreground backdrop-blur">
      <span className="size-1.5 rounded-full bg-primary" />
      {children}
    </div>
  );
}

function FadeUp({ children, delay = 0 }: { children: React.ReactNode; delay?: number }) {
  return (
    <motion.div
      initial={{ opacity: 0, y: 24 }}
      whileInView={{ opacity: 1, y: 0 }}
      viewport={{ once: true, margin: "-80px" }}
      transition={{ duration: 0.6, ease: [0.22, 1, 0.36, 1], delay }}
    >
      {children}
    </motion.div>
  );
}

export default function Portfolio() {
  const [dark, setDark] = useDarkMode();
  const [open, setOpen] = useState(false);
  const [scrolled, setScrolled] = useState(false);
  const [showTop, setShowTop] = useState(false);
  const { scrollYProgress } = useScroll();
  const progressWidth = useTransform(scrollYProgress, [0, 1], ["0%", "100%"]);

  useEffect(() => {
    const onScroll = () => {
      setScrolled(window.scrollY > 24);
      setShowTop(window.scrollY > 600);
    };
    onScroll();
    window.addEventListener("scroll", onScroll, { passive: true });
    return () => window.removeEventListener("scroll", onScroll);
  }, []);

  const scrollTo = (id: string) => {
    document.getElementById(id)?.scrollIntoView({ behavior: "smooth", block: "start" });
    setOpen(false);
  };

  return (
    <div className="min-h-screen bg-background text-foreground">
      {/* Scroll progress */}
      <motion.div
        style={{ width: progressWidth }}
        className="fixed inset-x-0 top-0 z-[60] h-0.5 origin-left bg-primary"
      />

      {/* Nav */}
      <header
        className={`fixed inset-x-0 top-0 z-50 transition-all duration-300 ${
          scrolled ? "py-3" : "py-5"
        }`}
      >
        <div className="mx-auto max-w-7xl px-6 md:px-10">
          <nav
            className={`flex items-center justify-between rounded-2xl px-4 py-3 transition-all duration-300 ${
              scrolled ? "glass-card" : ""
            }`}
          >
            <button onClick={() => scrollTo("home")} className="flex items-center gap-2 font-display text-lg font-bold tracking-tight">
              <span className="grid size-8 place-items-center rounded-lg bg-[image:var(--gradient-primary)] text-primary-foreground shadow-[var(--shadow-glow)]">
                <Sparkles className="size-4" />
              </span>
              Alex Morgan
            </button>
            <div className="hidden items-center gap-1 lg:flex">
              {NAV.map((n) => (
                <button
                  key={n.id}
                  onClick={() => scrollTo(n.id)}
                  className="rounded-lg px-3 py-2 text-sm font-medium text-muted-foreground transition-colors hover:bg-accent hover:text-foreground"
                >
                  {n.label}
                </button>
              ))}
            </div>
            <div className="flex items-center gap-2">
              <button
                onClick={() => setDark(!dark)}
                aria-label="Toggle theme"
                className="grid size-9 place-items-center rounded-lg border border-border bg-surface/60 text-muted-foreground transition-colors hover:text-foreground"
              >
                {dark ? <Sun className="size-4" /> : <Moon className="size-4" />}
              </button>
              <button
                onClick={() => scrollTo("contact")}
                className="hidden rounded-lg bg-foreground px-4 py-2 text-sm font-medium text-background transition-transform hover:scale-[1.03] sm:inline-flex"
              >
                Let's talk
              </button>
              <button
                onClick={() => setOpen((o) => !o)}
                aria-label="Menu"
                className="grid size-9 place-items-center rounded-lg border border-border bg-surface/60 lg:hidden"
              >
                {open ? <X className="size-4" /> : <Menu className="size-4" />}
              </button>
            </div>
          </nav>
          {open && (
            <motion.div
              initial={{ opacity: 0, y: -8 }}
              animate={{ opacity: 1, y: 0 }}
              className="glass-card mt-2 grid gap-1 rounded-2xl p-3 lg:hidden"
            >
              {NAV.map((n) => (
                <button
                  key={n.id}
                  onClick={() => scrollTo(n.id)}
                  className="rounded-lg px-3 py-3 text-left text-sm font-medium text-foreground hover:bg-accent"
                >
                  {n.label}
                </button>
              ))}
            </motion.div>
          )}
        </div>
      </header>

      {/* Hero */}
      <Section id="home" className="relative pt-36 sm:pt-44">
        <div
          className="pointer-events-none absolute inset-0 -z-10"
          style={{ background: "var(--gradient-hero)" }}
        />
        <div className="grid items-center gap-12 lg:grid-cols-[1.15fr_0.85fr]">
          <div>
            <FadeUp>
              <Eyebrow>Digital Marketing Specialist</Eyebrow>
            </FadeUp>
            <FadeUp delay={0.05}>
              <h1 className="mt-6 font-display text-4xl font-bold leading-[1.05] tracking-tight sm:text-6xl lg:text-7xl">
                Helping businesses grow through{" "}
                <span className="gradient-text">data-driven</span> digital marketing.
              </h1>
            </FadeUp>
            <FadeUp delay={0.1}>
              <p className="mt-6 max-w-xl text-lg leading-relaxed text-muted-foreground">
                I build performance marketing systems that turn ad spend into predictable, profitable
                pipelines — across Meta, Google, SEO and lead generation.
              </p>
            </FadeUp>
            <FadeUp delay={0.15}>
              <div className="mt-8 flex flex-wrap items-center gap-3">
                <button
                  onClick={() => scrollTo("portfolio")}
                  className="group inline-flex items-center gap-2 rounded-xl bg-[image:var(--gradient-primary)] px-5 py-3 text-sm font-semibold text-primary-foreground shadow-[var(--shadow-glow)] transition-transform hover:scale-[1.03]"
                >
                  View my work
                  <ArrowRight className="size-4 transition-transform group-hover:translate-x-0.5" />
                </button>
                <button
                  onClick={() => scrollTo("contact")}
                  className="inline-flex items-center gap-2 rounded-xl border border-border bg-surface/60 px-5 py-3 text-sm font-semibold text-foreground backdrop-blur transition-colors hover:bg-accent"
                >
                  Get in touch
                </button>
              </div>
            </FadeUp>
            <FadeUp delay={0.25}>
              <div className="mt-12 flex flex-wrap items-center gap-x-8 gap-y-4 text-sm text-muted-foreground">
                <div><span className="font-display text-2xl font-bold text-foreground">8+</span> years experience</div>
                <div className="h-4 w-px bg-border" />
                <div><span className="font-display text-2xl font-bold text-foreground">140+</span> clients served</div>
                <div className="h-4 w-px bg-border" />
                <div><span className="font-display text-2xl font-bold text-foreground">$12M+</span> ad spend</div>
              </div>
            </FadeUp>
          </div>
          <FadeUp delay={0.1}>
            <div className="relative mx-auto w-full max-w-md">
              <div className="absolute -inset-4 rounded-[2rem] bg-[image:var(--gradient-primary)] opacity-20 blur-2xl" />
              <div className="glass-card relative overflow-hidden rounded-[2rem] p-2">
                <img
                  src={portrait}
                  alt="Alex Morgan portrait"
                  width={896}
                  height={1152}
                  className="aspect-[4/5] w-full rounded-[1.5rem] object-cover"
                />
              </div>
              <motion.div
                animate={{ y: [0, -8, 0] }}
                transition={{ duration: 4, repeat: Infinity, ease: "easeInOut" }}
                className="glass-card absolute -bottom-4 -left-4 hidden rounded-2xl p-4 sm:block"
              >
                <div className="flex items-center gap-3">
                  <div className="grid size-10 place-items-center rounded-xl bg-[image:var(--gradient-primary)] text-primary-foreground">
                    <TrendingUp className="size-5" />
                  </div>
                  <div>
                    <div className="font-display text-lg font-bold leading-none">+345%</div>
                    <div className="text-xs text-muted-foreground">avg ROAS lift</div>
                  </div>
                </div>
              </motion.div>
              <motion.div
                animate={{ y: [0, 8, 0] }}
                transition={{ duration: 4.5, repeat: Infinity, ease: "easeInOut" }}
                className="glass-card absolute -right-4 top-10 hidden rounded-2xl p-4 sm:block"
              >
                <div className="flex items-center gap-3">
                  <div className="grid size-10 place-items-center rounded-xl bg-accent text-accent-foreground">
                    <LineChart className="size-5" />
                  </div>
                  <div>
                    <div className="font-display text-lg font-bold leading-none">48K+</div>
                    <div className="text-xs text-muted-foreground">leads generated</div>
                  </div>
                </div>
              </motion.div>
            </div>
          </FadeUp>
        </div>
      </Section>

      {/* About */}
      <Section id="about" className="bg-surface/50">
        <div className="grid gap-12 lg:grid-cols-[0.9fr_1.1fr]">
          <FadeUp>
            <Eyebrow>About</Eyebrow>
            <h2 className="mt-4 font-display text-3xl font-bold tracking-tight sm:text-5xl">
              Strategy, execution and measurable growth — under one roof.
            </h2>
          </FadeUp>
          <div className="space-y-6 text-lg leading-relaxed text-muted-foreground">
            <FadeUp delay={0.05}>
              <p>
                I'm a senior digital marketing consultant with <span className="font-semibold text-foreground">8+ years</span> of
                experience scaling brands across e-commerce, SaaS, healthcare, real estate and local services.
              </p>
            </FadeUp>
            <FadeUp delay={0.1}>
              <p>
                My philosophy is simple: <span className="font-semibold text-foreground">marketing should make money</span>.
                Every campaign, landing page and email I build is tied to a clear business metric — revenue, qualified leads
                or customer lifetime value.
              </p>
            </FadeUp>
            <FadeUp delay={0.15}>
              <div className="grid grid-cols-2 gap-4 pt-4 sm:grid-cols-3">
                {["E-commerce", "SaaS", "Healthcare", "Real Estate", "Local Services", "B2B"].map((i) => (
                  <div key={i} className="rounded-xl border border-border bg-surface-elevated px-4 py-3 text-sm font-medium text-foreground">
                    {i}
                  </div>
                ))}
              </div>
            </FadeUp>
          </div>
        </div>
      </Section>

      {/* Services */}
      <Section id="services">
        <div className="mb-14 max-w-2xl">
          <FadeUp><Eyebrow>Services</Eyebrow></FadeUp>
          <FadeUp delay={0.05}>
            <h2 className="mt-4 font-display text-3xl font-bold tracking-tight sm:text-5xl">
              Full-stack marketing, built for outcomes.
            </h2>
          </FadeUp>
          <FadeUp delay={0.1}>
            <p className="mt-4 text-lg text-muted-foreground">
              Nine capabilities, one accountable partner. Engage me for a single channel or an end-to-end growth engine.
            </p>
          </FadeUp>
        </div>
        <div className="grid gap-5 sm:grid-cols-2 lg:grid-cols-3">
          {SERVICES.map((s, i) => (
            <FadeUp key={s.title} delay={i * 0.04}>
              <div className="group h-full rounded-2xl border border-border bg-surface-elevated p-6 shadow-[var(--shadow-soft)] transition-all duration-300 hover:-translate-y-1 hover:shadow-[var(--shadow-elevated)]">
                <div className="mb-5 inline-grid size-12 place-items-center rounded-xl bg-accent text-accent-foreground transition-colors group-hover:bg-[image:var(--gradient-primary)] group-hover:text-primary-foreground">
                  <s.icon className="size-5" />
                </div>
                <h3 className="font-display text-lg font-semibold tracking-tight">{s.title}</h3>
                <p className="mt-2 text-sm leading-relaxed text-muted-foreground">{s.desc}</p>
              </div>
            </FadeUp>
          ))}
        </div>
      </Section>

      {/* Stats */}
      <Section className="bg-surface/50">
        <div className="grid grid-cols-2 gap-y-10 sm:grid-cols-3 lg:grid-cols-5">
          {STATS.map((s, i) => (
            <FadeUp key={s.label} delay={i * 0.05}>
              <div className="text-center sm:text-left">
                <div className="font-display text-4xl font-bold tracking-tight sm:text-5xl">
                  <Counter value={s.value} prefix={s.prefix} suffix={s.suffix} />
                </div>
                <div className="mt-2 text-sm text-muted-foreground">{s.label}</div>
              </div>
            </FadeUp>
          ))}
        </div>
      </Section>

      {/* Portfolio */}
      <Section id="portfolio">
        <div className="mb-14 flex flex-wrap items-end justify-between gap-6">
          <div className="max-w-2xl">
            <FadeUp><Eyebrow>Case Studies</Eyebrow></FadeUp>
            <FadeUp delay={0.05}>
              <h2 className="mt-4 font-display text-3xl font-bold tracking-tight sm:text-5xl">
                Selected work that moved the needle.
              </h2>
            </FadeUp>
          </div>
        </div>
        <div className="grid gap-6 lg:grid-cols-3">
          {CASES.map((c, i) => (
            <FadeUp key={c.title} delay={i * 0.08}>
              <article className="group flex h-full flex-col overflow-hidden rounded-2xl border border-border bg-surface-elevated shadow-[var(--shadow-soft)] transition-all duration-300 hover:-translate-y-1 hover:shadow-[var(--shadow-elevated)]">
                <div className="relative aspect-[16/10] overflow-hidden bg-[image:var(--gradient-hero)]">
                  <div className="absolute inset-0 bg-[image:var(--gradient-primary)] opacity-10" />
                  <div className="absolute left-5 top-5">
                    <span className="rounded-full bg-background/80 px-3 py-1 text-xs font-medium text-foreground backdrop-blur">
                      {c.industry}
                    </span>
                  </div>
                  <div className="absolute bottom-5 right-5 rounded-xl bg-foreground px-4 py-2 font-display text-lg font-bold text-background">
                    {c.metric}
                  </div>
                </div>
                <div className="flex flex-1 flex-col p-6">
                  <h3 className="font-display text-xl font-semibold tracking-tight">{c.title}</h3>
                  <dl className="mt-4 space-y-3 text-sm">
                    <div>
                      <dt className="font-semibold text-foreground">Challenge</dt>
                      <dd className="mt-1 text-muted-foreground">{c.challenge}</dd>
                    </div>
                    <div>
                      <dt className="font-semibold text-foreground">Strategy</dt>
                      <dd className="mt-1 text-muted-foreground">{c.strategy}</dd>
                    </div>
                  </dl>
                  <div className="mt-5 grid grid-cols-2 gap-3 rounded-xl bg-surface p-4">
                    <div>
                      <div className="text-[10px] font-medium uppercase tracking-wider text-muted-foreground">Before</div>
                      <div className="mt-1 font-display text-lg font-bold text-muted-foreground line-through decoration-1">{c.before.value}</div>
                      <div className="text-xs text-muted-foreground">{c.before.label}</div>
                    </div>
                    <div>
                      <div className="text-[10px] font-medium uppercase tracking-wider text-primary">After</div>
                      <div className="mt-1 font-display text-lg font-bold text-foreground">{c.after.value}</div>
                      <div className="text-xs text-muted-foreground">{c.after.label}</div>
                    </div>
                  </div>
                  <button className="mt-6 inline-flex items-center gap-2 self-start text-sm font-semibold text-primary transition-transform group-hover:translate-x-1">
                    View details <ArrowUpRight className="size-4" />
                  </button>
                </div>
              </article>
            </FadeUp>
          ))}
        </div>
      </Section>

      {/* Skills */}
      <Section id="skills" className="bg-surface/50">
        <div className="mb-14 max-w-2xl">
          <FadeUp><Eyebrow>Skills & Tools</Eyebrow></FadeUp>
          <FadeUp delay={0.05}>
            <h2 className="mt-4 font-display text-3xl font-bold tracking-tight sm:text-5xl">
              The stack behind the results.
            </h2>
          </FadeUp>
        </div>
        <div className="grid gap-x-10 gap-y-6 sm:grid-cols-2 lg:grid-cols-3">
          {SKILLS.map((s, i) => (
            <FadeUp key={s.name} delay={i * 0.03}>
              <div>
                <div className="mb-2 flex items-baseline justify-between">
                  <span className="font-medium text-foreground">{s.name}</span>
                  <span className="font-display text-sm font-semibold text-muted-foreground">{s.level}%</span>
                </div>
                <div className="h-2 overflow-hidden rounded-full bg-accent">
                  <motion.div
                    initial={{ width: 0 }}
                    whileInView={{ width: `${s.level}%` }}
                    viewport={{ once: true, margin: "-50px" }}
                    transition={{ duration: 1.2, ease: [0.22, 1, 0.36, 1] }}
                    className="h-full rounded-full bg-[image:var(--gradient-primary)]"
                  />
                </div>
              </div>
            </FadeUp>
          ))}
        </div>
      </Section>

      {/* Testimonials */}
      <Section>
        <div className="mb-14 max-w-2xl">
          <FadeUp><Eyebrow>Testimonials</Eyebrow></FadeUp>
          <FadeUp delay={0.05}>
            <h2 className="mt-4 font-display text-3xl font-bold tracking-tight sm:text-5xl">
              Trusted by founders and marketing leaders.
            </h2>
          </FadeUp>
        </div>
        <div className="grid gap-6 md:grid-cols-3">
          {TESTIMONIALS.map((t, i) => (
            <FadeUp key={t.name} delay={i * 0.08}>
              <div className="flex h-full flex-col rounded-2xl border border-border bg-surface-elevated p-6 shadow-[var(--shadow-soft)]">
                <div className="flex gap-1 text-primary">
                  {Array.from({ length: t.rating }).map((_, k) => (
                    <Star key={k} className="size-4 fill-current" />
                  ))}
                </div>
                <p className="mt-4 flex-1 text-base leading-relaxed text-foreground">"{t.quote}"</p>
                <div className="mt-6 flex items-center gap-3 border-t border-border pt-5">
                  <div className="grid size-11 place-items-center rounded-full bg-[image:var(--gradient-primary)] font-display font-bold text-primary-foreground">
                    {t.name.split(" ").map((n) => n[0]).join("")}
                  </div>
                  <div>
                    <div className="font-semibold text-foreground">{t.name}</div>
                    <div className="text-xs text-muted-foreground">{t.role}, {t.company}</div>
                  </div>
                </div>
              </div>
            </FadeUp>
          ))}
        </div>
      </Section>

      {/* Blog */}
      <Section id="blog" className="bg-surface/50">
        <div className="mb-14 flex flex-wrap items-end justify-between gap-6">
          <div className="max-w-2xl">
            <FadeUp><Eyebrow>Blog</Eyebrow></FadeUp>
            <FadeUp delay={0.05}>
              <h2 className="mt-4 font-display text-3xl font-bold tracking-tight sm:text-5xl">
                Notes from the field.
              </h2>
            </FadeUp>
          </div>
          <FadeUp delay={0.1}>
            <button className="inline-flex items-center gap-2 text-sm font-semibold text-primary">
              All articles <ArrowRight className="size-4" />
            </button>
          </FadeUp>
        </div>
        <div className="grid gap-6 md:grid-cols-3">
          {POSTS.map((p, i) => (
            <FadeUp key={p.title} delay={i * 0.08}>
              <article className="group flex h-full flex-col overflow-hidden rounded-2xl border border-border bg-surface-elevated shadow-[var(--shadow-soft)] transition-all duration-300 hover:-translate-y-1 hover:shadow-[var(--shadow-elevated)]">
                <div className="aspect-[16/9] bg-[image:var(--gradient-hero)] relative">
                  <div className="absolute inset-0 bg-[image:var(--gradient-primary)] opacity-15" />
                  <span className="absolute left-5 top-5 rounded-full bg-background/80 px-3 py-1 text-xs font-medium backdrop-blur">{p.tag}</span>
                </div>
                <div className="flex flex-1 flex-col p-6">
                  <div className="text-xs text-muted-foreground">{p.date}</div>
                  <h3 className="mt-2 font-display text-lg font-semibold leading-snug tracking-tight">{p.title}</h3>
                  <p className="mt-2 flex-1 text-sm text-muted-foreground">{p.excerpt}</p>
                  <button className="mt-4 inline-flex items-center gap-2 self-start text-sm font-semibold text-primary transition-transform group-hover:translate-x-1">
                    Read more <ArrowRight className="size-4" />
                  </button>
                </div>
              </article>
            </FadeUp>
          ))}
        </div>
      </Section>

      {/* Contact */}
      <Section id="contact">
        <div className="grid gap-12 lg:grid-cols-[1fr_1.1fr]">
          <div>
            <FadeUp><Eyebrow>Contact</Eyebrow></FadeUp>
            <FadeUp delay={0.05}>
              <h2 className="mt-4 font-display text-3xl font-bold tracking-tight sm:text-5xl">
                Let's build your growth engine.
              </h2>
            </FadeUp>
            <FadeUp delay={0.1}>
              <p className="mt-4 text-lg text-muted-foreground">
                Tell me about your business and what you'd like to achieve. I'll respond within one business day.
              </p>
            </FadeUp>
            <FadeUp delay={0.15}>
              <ul className="mt-8 space-y-4 text-sm">
                {[
                  { icon: Mail, label: "hello@alexmorgan.co" },
                  { icon: Phone, label: "+1 (415) 555-0142" },
                  { icon: MapPin, label: "San Francisco, CA — Remote worldwide" },
                ].map((x) => (
                  <li key={x.label} className="flex items-center gap-3">
                    <span className="grid size-10 place-items-center rounded-xl bg-accent text-accent-foreground">
                      <x.icon className="size-4" />
                    </span>
                    <span className="font-medium text-foreground">{x.label}</span>
                  </li>
                ))}
              </ul>
            </FadeUp>
            <FadeUp delay={0.2}>
              <div className="mt-8 flex gap-3">
                {[Linkedin, Facebook, MessageCircle].map((Icon, i) => (
                  <a
                    key={i}
                    href="#"
                    aria-label="Social"
                    className="grid size-11 place-items-center rounded-xl border border-border bg-surface-elevated text-foreground transition-all hover:-translate-y-0.5 hover:bg-[image:var(--gradient-primary)] hover:text-primary-foreground"
                  >
                    <Icon className="size-4" />
                  </a>
                ))}
              </div>
            </FadeUp>
            <FadeUp delay={0.25}>
              <div className="mt-8 aspect-[16/9] overflow-hidden rounded-2xl border border-border bg-surface-elevated">
                <div className="relative h-full w-full bg-[image:var(--gradient-hero)]">
                  <div className="absolute inset-0 grid place-items-center">
                    <div className="flex items-center gap-2 rounded-full bg-background/80 px-4 py-2 text-sm font-medium backdrop-blur">
                      <MapPin className="size-4 text-primary" /> San Francisco, CA
                    </div>
                  </div>
                  <svg className="absolute inset-0 h-full w-full opacity-30" xmlns="http://www.w3.org/2000/svg">
                    <defs>
                      <pattern id="grid" width="32" height="32" patternUnits="userSpaceOnUse">
                        <path d="M 32 0 L 0 0 0 32" fill="none" stroke="currentColor" strokeWidth="0.5" />
                      </pattern>
                    </defs>
                    <rect width="100%" height="100%" fill="url(#grid)" />
                  </svg>
                </div>
              </div>
            </FadeUp>
          </div>

          <FadeUp delay={0.1}>
            <form
              onSubmit={(e) => { e.preventDefault(); alert("Thanks! I'll be in touch shortly."); }}
              className="glass-card rounded-3xl p-6 sm:p-8"
            >
              <div className="grid gap-4 sm:grid-cols-2">
                <Field label="Name" name="name" placeholder="Jane Doe" />
                <Field label="Email" name="email" type="email" placeholder="jane@company.com" />
              </div>
              <div className="mt-4 grid gap-4 sm:grid-cols-2">
                <Field label="Company" name="company" placeholder="Acme Inc" />
                <Field label="Budget" name="budget" placeholder="$5k – $25k / mo" />
              </div>
              <div className="mt-4">
                <label className="mb-2 block text-xs font-medium uppercase tracking-wider text-muted-foreground">
                  Project details
                </label>
                <textarea
                  rows={5}
                  placeholder="Tell me about your goals, channels and timeline..."
                  className="w-full resize-none rounded-xl border border-border bg-background px-4 py-3 text-sm text-foreground placeholder:text-muted-foreground focus:border-primary focus:outline-none focus:ring-2 focus:ring-primary/20"
                />
              </div>
              <button
                type="submit"
                className="mt-6 inline-flex w-full items-center justify-center gap-2 rounded-xl bg-[image:var(--gradient-primary)] px-5 py-3.5 text-sm font-semibold text-primary-foreground shadow-[var(--shadow-glow)] transition-transform hover:scale-[1.01]"
              >
                Send message <ArrowRight className="size-4" />
              </button>
            </form>
          </FadeUp>
        </div>
      </Section>

      {/* Footer */}
      <footer className="border-t border-border bg-surface/50 px-6 py-12 md:px-10">
        <div className="mx-auto grid max-w-7xl gap-10 md:grid-cols-[1.5fr_1fr_1fr]">
          <div>
            <div className="flex items-center gap-2 font-display text-lg font-bold">
              <span className="grid size-8 place-items-center rounded-lg bg-[image:var(--gradient-primary)] text-primary-foreground">
                <Sparkles className="size-4" />
              </span>
              Alex Morgan
            </div>
            <p className="mt-4 max-w-sm text-sm text-muted-foreground">
              Performance marketing for ambitious businesses. Strategy, execution and measurable growth.
            </p>
          </div>
          <div>
            <div className="mb-3 text-xs font-semibold uppercase tracking-wider text-foreground">Quick links</div>
            <ul className="space-y-2 text-sm text-muted-foreground">
              {NAV.map((n) => (
                <li key={n.id}>
                  <button onClick={() => scrollTo(n.id)} className="hover:text-foreground">{n.label}</button>
                </li>
              ))}
            </ul>
          </div>
          <div>
            <div className="mb-3 text-xs font-semibold uppercase tracking-wider text-foreground">Legal</div>
            <ul className="space-y-2 text-sm text-muted-foreground">
              <li><a href="#" className="hover:text-foreground">Privacy Policy</a></li>
              <li><a href="#" className="hover:text-foreground">Terms</a></li>
            </ul>
            <div className="mt-6 flex gap-3">
              {[Linkedin, Facebook, MessageCircle].map((Icon, i) => (
                <a key={i} href="#" aria-label="Social" className="grid size-9 place-items-center rounded-lg border border-border bg-surface-elevated text-muted-foreground hover:text-foreground">
                  <Icon className="size-4" />
                </a>
              ))}
            </div>
          </div>
        </div>
        <div className="mx-auto mt-10 flex max-w-7xl flex-col items-center justify-between gap-4 border-t border-border pt-6 text-xs text-muted-foreground sm:flex-row">
          <div>© {new Date().getFullYear()} Alex Morgan. All rights reserved.</div>
          <div>Crafted with care.</div>
        </div>
      </footer>

      {/* Back to top */}
      {showTop && (
        <motion.button
          initial={{ opacity: 0, scale: 0.8 }}
          animate={{ opacity: 1, scale: 1 }}
          onClick={() => window.scrollTo({ top: 0, behavior: "smooth" })}
          aria-label="Back to top"
          className="fixed bottom-6 right-6 z-50 grid size-12 place-items-center rounded-full bg-[image:var(--gradient-primary)] text-primary-foreground shadow-[var(--shadow-glow)] transition-transform hover:scale-110"
        >
          <ChevronUp className="size-5" />
        </motion.button>
      )}
    </div>
  );
}

function Field({ label, name, type = "text", placeholder }: { label: string; name: string; type?: string; placeholder?: string }) {
  return (
    <div>
      <label htmlFor={name} className="mb-2 block text-xs font-medium uppercase tracking-wider text-muted-foreground">
        {label}
      </label>
      <input
        id={name}
        name={name}
        type={type}
        placeholder={placeholder}
        className="w-full rounded-xl border border-border bg-background px-4 py-3 text-sm text-foreground placeholder:text-muted-foreground focus:border-primary focus:outline-none focus:ring-2 focus:ring-primary/20"
      />
    </div>
  );
}
