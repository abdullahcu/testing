<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Elite Residence — Premium Real Estate in Dhaka</title>
<meta name="description" content="Discover premium flats, plots and houses in Dhaka's most elite neighborhoods — Gulshan, Banani, Bashundhara and more."/>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@500;600;700&family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
<style>
  :root{
    --bg:#fbfaf7;
    --surface:#ffffff;
    --ink:#0f1c2e;
    --ink-soft:#3a475a;
    --muted:#7a8699;
    --line:#e7e3dc;
    --accent:#0b3d91;       /* Elite Royal Blue */
    --accent-2:#0a6b4a;     /* Emerald */
    --gold:#b6924a;
    --radius:14px;
    --shadow:0 10px 30px rgba(15,28,46,.08);
    --shadow-lg:0 30px 60px rgba(15,28,46,.18);
    --serif:'Cormorant Garamond', serif;
    --sans:'Inter', system-ui, sans-serif;
  }
  *{box-sizing:border-box;margin:0;padding:0}
  html{scroll-behavior:smooth}
  body{font-family:var(--sans);background:var(--bg);color:var(--ink);line-height:1.55;-webkit-font-smoothing:antialiased}
  img{display:block;max-width:100%}
  a{color:inherit;text-decoration:none}
  .container{max-width:1240px;margin:0 auto;padding:0 24px}

  /* HEADER */
  header.site{
    position:sticky;top:0;z-index:50;
    background:rgba(255,255,255,.85);
    backdrop-filter:saturate(180%) blur(14px);
    border-bottom:1px solid var(--line);
  }
  .nav{display:flex;align-items:center;justify-content:space-between;height:78px;gap:24px}
  .brand{display:flex;align-items:center;gap:12px}
  .brand .mark{width:42px;height:42px}
  .brand-text{display:flex;flex-direction:column;line-height:1}
  .brand-text .name{font-family:var(--serif);font-weight:700;font-size:22px;letter-spacing:.5px}
  .brand-text .tag{font-size:10px;letter-spacing:3px;text-transform:uppercase;color:var(--muted);margin-top:4px}
  nav.primary{display:flex;gap:32px}
  nav.primary a{font-size:14px;font-weight:500;color:var(--ink-soft);position:relative;padding:6px 0;transition:color .2s}
  nav.primary a:hover{color:var(--accent)}
  nav.primary a::after{content:"";position:absolute;left:0;right:0;bottom:0;height:2px;background:var(--accent);transform:scaleX(0);transform-origin:left;transition:transform .25s}
  nav.primary a:hover::after{transform:scaleX(1)}
  .cta-call{display:inline-flex;align-items:center;gap:10px;padding:10px 18px;border:1px solid var(--ink);border-radius:999px;font-size:13px;font-weight:600;transition:all .2s}
  .cta-call:hover{background:var(--ink);color:#fff}

  /* CATEGORY TABS */
  .cat-tabs{display:flex;justify-content:center;gap:8px;padding:18px 0;border-bottom:1px solid var(--line);background:#fff}
  .cat-tabs button{
    background:transparent;border:1px solid var(--line);padding:9px 22px;border-radius:999px;
    font-family:var(--sans);font-size:13px;font-weight:500;color:var(--ink-soft);cursor:pointer;transition:all .2s;letter-spacing:.5px
  }
  .cat-tabs button:hover{border-color:var(--accent);color:var(--accent)}
  .cat-tabs button.active{background:var(--ink);color:#fff;border-color:var(--ink)}

  /* HERO */
  .hero{
    position:relative;min-height:640px;display:flex;align-items:center;
    background:
      linear-gradient(135deg, rgba(11,28,46,.72), rgba(11,28,46,.45)),
      url('https://images.unsplash.com/photo-1600585154340-be6161a56a0c?auto=format&fit=crop&w=2000&q=80') center/cover no-repeat;
    color:#fff;
  }
  .hero-inner{padding:120px 0 160px;max-width:860px}
  .eyebrow{display:inline-block;font-size:11px;letter-spacing:4px;text-transform:uppercase;color:#e9d9b3;border:1px solid rgba(233,217,179,.4);padding:6px 14px;border-radius:999px;margin-bottom:24px}
  h1.hero-title{font-family:var(--serif);font-weight:600;font-size:clamp(38px,5.5vw,68px);line-height:1.08;letter-spacing:-.5px;margin-bottom:18px}
  h1.hero-title em{font-style:italic;color:#e9d9b3;font-weight:500}
  .hero p.sub{font-size:17px;color:#dde3ec;max-width:620px;font-weight:300}

  /* SEARCH BAR */
  .search-wrap{position:relative;margin-top:-70px;z-index:10}
  .search{
    background:#fff;border-radius:var(--radius);box-shadow:var(--shadow-lg);
    padding:22px;display:grid;grid-template-columns:1.2fr 1fr 1fr auto;gap:14px;align-items:end;
  }
  .field label{display:block;font-size:11px;letter-spacing:1.5px;text-transform:uppercase;color:var(--muted);margin-bottom:8px;font-weight:600}
  .field select,.field input{
    width:100%;padding:12px 14px;border:1px solid var(--line);border-radius:8px;
    font-family:var(--sans);font-size:14px;color:var(--ink);background:#fff;
    transition:border-color .2s
  }
  .field select:focus,.field input:focus{outline:none;border-color:var(--accent)}
  .search button.search-btn{
    background:var(--accent);color:#fff;border:none;padding:14px 30px;border-radius:8px;
    font-weight:600;font-size:14px;letter-spacing:.5px;cursor:pointer;height:46px;
    display:flex;align-items:center;gap:8px;transition:background .2s
  }
  .search button.search-btn:hover{background:#082e6b}

  /* SECTION */
  section.section{padding:90px 0}
  .section-head{text-align:center;max-width:680px;margin:0 auto 50px}
  .section-head .eyebrow-d{display:inline-block;font-size:11px;letter-spacing:4px;text-transform:uppercase;color:var(--accent);font-weight:600;margin-bottom:14px}
  .section-head h2{font-family:var(--serif);font-size:clamp(32px,3.6vw,46px);font-weight:600;line-height:1.15;margin-bottom:14px}
  .section-head p{color:var(--muted);font-size:16px}

  /* LOCATION FILTER PILLS */
  .loc-pills{display:flex;justify-content:center;flex-wrap:wrap;gap:10px;margin-bottom:48px}
  .loc-pills button{
    padding:10px 22px;border-radius:999px;background:#fff;border:1px solid var(--line);
    font-family:var(--sans);font-size:13px;font-weight:500;color:var(--ink-soft);cursor:pointer;
    transition:all .2s;letter-spacing:.3px
  }
  .loc-pills button:hover{border-color:var(--accent);color:var(--accent);transform:translateY(-1px)}
  .loc-pills button.active{background:var(--accent);color:#fff;border-color:var(--accent)}

  /* PROPERTY GRID */
  .grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(330px,1fr));gap:30px}
  .card{
    background:#fff;border-radius:var(--radius);overflow:hidden;box-shadow:var(--shadow);
    transition:transform .35s, box-shadow .35s;cursor:pointer;display:flex;flex-direction:column;
    border:1px solid var(--line)
  }
  .card:hover{transform:translateY(-6px);box-shadow:var(--shadow-lg)}
  .card .img{position:relative;aspect-ratio:4/3;overflow:hidden}
  .card .img img{width:100%;height:100%;object-fit:cover;transition:transform .6s}
  .card:hover .img img{transform:scale(1.06)}
  .card .tag{
    position:absolute;top:14px;left:14px;background:rgba(255,255,255,.95);
    color:var(--accent);padding:5px 12px;border-radius:4px;font-size:11px;font-weight:600;
    letter-spacing:1px;text-transform:uppercase
  }
  .card .fav{
    position:absolute;top:14px;right:14px;width:36px;height:36px;border-radius:50%;
    background:rgba(255,255,255,.95);display:flex;align-items:center;justify-content:center;color:var(--ink-soft)
  }
  .card .body{padding:22px;display:flex;flex-direction:column;gap:12px;flex:1}
  .card h3{font-family:var(--serif);font-size:22px;font-weight:600;line-height:1.25}
  .card .loc{font-size:13px;color:var(--muted);display:flex;align-items:center;gap:6px}
  .card .specs{display:flex;gap:14px;font-size:13px;color:var(--ink-soft);padding:12px 0;border-top:1px solid var(--line);border-bottom:1px solid var(--line);margin-top:auto}
  .card .specs span{display:flex;align-items:center;gap:5px}
  .card .foot{display:flex;justify-content:space-between;align-items:center;gap:10px}
  .price{font-family:var(--serif);font-size:22px;font-weight:700;color:var(--accent)}
  .btn-visit{
    background:var(--ink);color:#fff;border:none;padding:9px 16px;border-radius:6px;
    font-size:12px;font-weight:600;cursor:pointer;letter-spacing:.5px;transition:background .2s
  }
  .btn-visit:hover{background:var(--accent)}

  .empty{grid-column:1/-1;text-align:center;padding:60px 20px;color:var(--muted)}

  /* DETAIL PAGE */
  .detail{display:none;padding:40px 0 90px;background:var(--bg);min-height:100vh}
  .detail.active{display:block;animation:fadeIn .4s ease}
  @keyframes fadeIn{from{opacity:0;transform:translateY(8px)}to{opacity:1;transform:translateY(0)}}
  .back-btn{
    display:inline-flex;align-items:center;gap:8px;background:#fff;border:1px solid var(--line);
    padding:10px 18px;border-radius:999px;font-size:13px;font-weight:500;cursor:pointer;margin-bottom:30px;
    transition:all .2s
  }
  .back-btn:hover{background:var(--ink);color:#fff;border-color:var(--ink)}
  .detail-hero{display:grid;grid-template-columns:2fr 1fr;gap:14px;height:520px;margin-bottom:40px;border-radius:var(--radius);overflow:hidden}
  .detail-hero img{width:100%;height:100%;object-fit:cover}
  .detail-hero .side{display:grid;grid-template-rows:1fr 1fr;gap:14px}
  .detail-grid{display:grid;grid-template-columns:1.7fr 1fr;gap:50px}
  .detail-main h1{font-family:var(--serif);font-size:42px;font-weight:600;line-height:1.15;margin-bottom:8px}
  .detail-main .loc-line{color:var(--muted);font-size:15px;margin-bottom:24px}
  .detail-main .specs-row{display:flex;gap:30px;padding:22px;background:#fff;border-radius:var(--radius);border:1px solid var(--line);margin-bottom:36px}
  .detail-main .specs-row > div{display:flex;flex-direction:column}
  .detail-main .specs-row .k{font-size:11px;letter-spacing:1.5px;text-transform:uppercase;color:var(--muted);margin-bottom:6px}
  .detail-main .specs-row .v{font-family:var(--serif);font-size:22px;font-weight:600;color:var(--ink)}
  .detail-main h3.dh{font-family:var(--serif);font-size:26px;font-weight:600;margin:30px 0 14px}
  .detail-main p.desc{color:var(--ink-soft);font-size:15px;line-height:1.8}
  .features{display:grid;grid-template-columns:repeat(2,1fr);gap:12px 20px;margin-top:14px}
  .features li{list-style:none;display:flex;align-items:center;gap:10px;font-size:14px;color:var(--ink-soft)}
  .features li::before{content:"";width:18px;height:18px;border-radius:50%;background:var(--accent-2);display:inline-flex;flex-shrink:0;
    background-image:url("data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24' fill='none' stroke='white' stroke-width='3' stroke-linecap='round' stroke-linejoin='round'><polyline points='20 6 9 17 4 12'/></svg>");
    background-size:12px;background-position:center;background-repeat:no-repeat}
  .booking{
    background:#fff;border:1px solid var(--line);border-radius:var(--radius);padding:30px;
    position:sticky;top:100px;box-shadow:var(--shadow)
  }
  .booking .price-big{font-family:var(--serif);font-size:34px;font-weight:700;color:var(--accent);margin-bottom:4px}
  .booking .price-sub{font-size:12px;color:var(--muted);margin-bottom:24px}
  .booking input,.booking textarea{
    width:100%;padding:12px 14px;border:1px solid var(--line);border-radius:8px;font-family:var(--sans);
    font-size:14px;margin-bottom:12px;color:var(--ink)
  }
  .booking input:focus,.booking textarea:focus{outline:none;border-color:var(--accent)}
  .booking textarea{resize:vertical;min-height:90px}
  .booking .btn-primary{
    width:100%;background:var(--accent);color:#fff;border:none;padding:14px;border-radius:8px;
    font-weight:600;font-size:14px;cursor:pointer;letter-spacing:.5px;margin-bottom:10px;transition:background .2s
  }
  .booking .btn-primary:hover{background:#082e6b}
  .booking .btn-outline{
    width:100%;background:transparent;color:var(--ink);border:1px solid var(--ink);padding:14px;border-radius:8px;
    font-weight:600;font-size:14px;cursor:pointer;letter-spacing:.5px;transition:all .2s
  }
  .booking .btn-outline:hover{background:var(--ink);color:#fff}

  /* FOOTER */
  footer.site{background:#0a1322;color:#c4ccd8;padding:80px 0 30px;margin-top:80px}
  .foot-grid{display:grid;grid-template-columns:1.4fr 1fr 1fr 1fr;gap:50px;margin-bottom:50px}
  .foot-grid h4{font-family:var(--serif);font-size:18px;color:#fff;margin-bottom:18px;font-weight:600}
  .foot-grid ul{list-style:none}
  .foot-grid li{margin-bottom:10px;font-size:14px}
  .foot-grid a:hover{color:#fff}
  .foot-brand p{font-size:14px;line-height:1.7;margin:14px 0 20px;color:#8b95a7;max-width:300px}
  .socials{display:flex;gap:10px}
  .socials a{
    width:40px;height:40px;border-radius:50%;background:rgba(255,255,255,.06);
    display:flex;align-items:center;justify-content:center;color:#c4ccd8;transition:all .2s;cursor:pointer
  }
  .socials a:hover{background:var(--accent);color:#fff;transform:translateY(-2px)}
  .foot-bottom{border-top:1px solid rgba(255,255,255,.08);padding-top:24px;display:flex;justify-content:space-between;flex-wrap:wrap;gap:12px;font-size:13px;color:#8b95a7}
  .foot-bottom a{margin-left:20px}

  @media (max-width:900px){
    nav.primary{display:none}
    .search{grid-template-columns:1fr 1fr;gap:12px;padding:18px}
    .search button.search-btn{grid-column:1/-1;width:100%}
    .detail-hero{grid-template-columns:1fr;height:auto}
    .detail-hero .side{grid-template-rows:auto auto;grid-template-columns:1fr 1fr}
    .detail-hero img{height:240px}
    .detail-grid{grid-template-columns:1fr;gap:30px}
    .booking{position:static}
    .foot-grid{grid-template-columns:1fr 1fr;gap:30px}
    .detail-main .specs-row{flex-wrap:wrap;gap:18px}
  }
</style>
</head>
<body>

<!-- HOME PAGE -->
<div id="home-page">

  <header class="site">
    <div class="container nav">
      <a href="#" class="brand" aria-label="Elite Residence">
        <!-- Creative SVG Logo -->
        <svg class="mark" viewBox="0 0 64 64" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
          <defs>
            <linearGradient id="lg" x1="0" y1="0" x2="1" y2="1">
              <stop offset="0%" stop-color="#0b3d91"/>
              <stop offset="100%" stop-color="#0a6b4a"/>
            </linearGradient>
          </defs>
          <rect x="2" y="2" width="60" height="60" rx="12" fill="url(#lg)"/>
          <path d="M16 36 L32 20 L48 36 L48 48 L36 48 L36 40 L28 40 L28 48 L16 48 Z"
                fill="none" stroke="#fff" stroke-width="2.2" stroke-linejoin="round"/>
          <circle cx="32" cy="14" r="2.2" fill="#e9d9b3"/>
        </svg>
        <div class="brand-text">
          <span class="name">Elite Residence</span>
          <span class="tag">Premium Properties</span>
        </div>
      </a>

      <nav class="primary">
        <a href="#listings">Properties</a>
        <a href="#about">About</a>
        <a href="#services">Services</a>
        <a href="#agents">Agents</a>
        <a href="#contact">Contact</a>
      </nav>

      <a href="tel:+8801518962973" class="cta-call">
        <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z"/></svg>
        +880 1518-962973
      </a>
    </div>

    <div class="cat-tabs container" id="catTabs">
      <button class="active" data-cat="all">All Properties</button>
      <button data-cat="Flat">Flat</button>
      <button data-cat="Plot">Plot</button>
      <button data-cat="House">House</button>
    </div>
  </header>

  <!-- HERO -->
  <section class="hero">
    <div class="container hero-inner">
      <span class="eyebrow">Trusted by 2,500+ Investors</span>
      <h1 class="hero-title">Find Your Premium <em>Dream Property</em> in Dhaka</h1>
      <p class="sub">Curated luxury flats, exclusive plots and signature houses in the city's most prestigious neighborhoods — backed by transparent dealings and an elite real estate network.</p>
    </div>
  </section>

  <!-- SEARCH -->
  <div class="container search-wrap">
    <div class="search">
      <div class="field">
        <label>Keyword</label>
        <input type="text" id="fKeyword" placeholder="e.g. Penthouse, Skyline Tower"/>
      </div>
      <div class="field">
        <label>Property Type</label>
        <select id="fType">
          <option value="all">All Types</option>
          <option value="Flat">Flat</option>
          <option value="Plot">Plot</option>
          <option value="House">House</option>
        </select>
      </div>
      <div class="field">
        <label>Location</label>
        <select id="fLocation">
          <option value="all">All Locations</option>
          <option>Uttara</option>
          <option>Gulshan</option>
          <option>Bashundhara</option>
          <option>Badda</option>
          <option>Banani</option>
          <option>Mirpur</option>
        </select>
      </div>
      <button class="search-btn" id="searchBtn">
        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2"><circle cx="11" cy="11" r="8"/><path d="m21 21-4.3-4.3"/></svg>
        Search
      </button>
    </div>
  </div>

  <!-- LISTINGS -->
  <section class="section" id="listings">
    <div class="container">
      <div class="section-head">
        <span class="eyebrow-d">Featured Listings</span>
        <h2>Handpicked Premium Properties</h2>
        <p>Filter by Dhaka's most sought-after neighborhoods to explore residences that match your lifestyle.</p>
      </div>

      <div class="loc-pills" id="locPills">
        <button class="active" data-loc="all">All Locations</button>
        <button data-loc="Uttara">Uttara</button>
        <button data-loc="Gulshan">Gulshan</button>
        <button data-loc="Bashundhara">Bashundhara</button>
        <button data-loc="Badda">Badda</button>
        <button data-loc="Banani">Banani</button>
        <button data-loc="Mirpur">Mirpur</button>
      </div>

      <div class="grid" id="propertyGrid"></div>
    </div>
  </section>

  <!-- FOOTER -->
  <footer class="site" id="contact">
    <div class="container">
      <div class="foot-grid">
        <div class="foot-brand">
          <div class="brand">
            <svg class="mark" viewBox="0 0 64 64" xmlns="http://www.w3.org/2000/svg">
              <rect x="2" y="2" width="60" height="60" rx="12" fill="url(#lg)"/>
              <path d="M16 36 L32 20 L48 36 L48 48 L36 48 L36 40 L28 40 L28 48 L16 48 Z" fill="none" stroke="#fff" stroke-width="2.2" stroke-linejoin="round"/>
              <circle cx="32" cy="14" r="2.2" fill="#e9d9b3"/>
            </svg>
            <div class="brand-text"><span class="name" style="color:#fff">Elite Residence</span><span class="tag">Premium Properties</span></div>
          </div>
          <p>Dhaka's trusted name for premium real estate — connecting discerning buyers with extraordinary properties across the city.</p>
          <div class="socials" id="socials">
            <a data-url="https://facebook.com" aria-label="Facebook"><svg width="16" height="16" viewBox="0 0 24 24" fill="currentColor"><path d="M22 12a10 10 0 1 0-11.6 9.9v-7H7.9V12h2.5V9.8c0-2.5 1.5-3.9 3.8-3.9 1.1 0 2.2.2 2.2.2v2.5h-1.3c-1.2 0-1.6.8-1.6 1.6V12h2.8l-.5 2.9h-2.3v7A10 10 0 0 0 22 12z"/></svg></a>
            <a data-url="https://instagram.com" aria-label="Instagram"><svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="2" y="2" width="20" height="20" rx="5"/><path d="M16 11.4A4 4 0 1 1 12.6 8 4 4 0 0 1 16 11.4z"/><line x1="17.5" y1="6.5" x2="17.5" y2="6.5"/></svg></a>
            <a data-url="https://linkedin.com" aria-label="LinkedIn"><svg width="16" height="16" viewBox="0 0 24 24" fill="currentColor"><path d="M20.5 2h-17A1.5 1.5 0 0 0 2 3.5v17A1.5 1.5 0 0 0 3.5 22h17a1.5 1.5 0 0 0 1.5-1.5v-17A1.5 1.5 0 0 0 20.5 2zM8 19H5v-9h3zM6.5 8.3A1.8 1.8 0 1 1 8.3 6.5 1.8 1.8 0 0 1 6.5 8.3zM19 19h-3v-4.7c0-1.1 0-2.6-1.6-2.6s-1.8 1.2-1.8 2.5V19h-3v-9h2.9v1.3a3.2 3.2 0 0 1 2.8-1.6c3 0 3.6 2 3.6 4.5z"/></svg></a>
            <a data-url="https://youtube.com" aria-label="YouTube"><svg width="16" height="16" viewBox="0 0 24 24" fill="currentColor"><path d="M23 7.2s-.2-1.5-.9-2.2c-.8-.9-1.8-.9-2.2-1C16.7 3.7 12 3.7 12 3.7s-4.7 0-7.9.2c-.4.1-1.4.1-2.2 1C1.2 5.7 1 7.2 1 7.2S.8 8.9.8 10.7v1.6c0 1.7.2 3.5.2 3.5s.2 1.5.9 2.2c.8.9 1.9.8 2.4.9 1.7.2 7.7.2 7.7.2s4.7 0 7.9-.2c.4-.1 1.4-.1 2.2-1 .7-.7.9-2.2.9-2.2s.2-1.7.2-3.5v-1.6c0-1.7-.2-3.5-.2-3.5zM9.7 14.3V8.4l6.1 3z"/></svg></a>
          </div>
        </div>
        <div>
          <h4>Properties</h4>
          <ul>
            <li><a href="#listings">Flats</a></li>
            <li><a href="#listings">Plots</a></li>
            <li><a href="#listings">Houses</a></li>
            <li><a href="#listings">Penthouses</a></li>
          </ul>
        </div>
        <div>
          <h4>Locations</h4>
          <ul>
            <li><a href="#">Gulshan</a></li>
            <li><a href="#">Banani</a></li>
            <li><a href="#">Bashundhara</a></li>
            <li><a href="#">Uttara</a></li>
          </ul>
        </div>
        <div>
          <h4>Contact</h4>
          <ul>
            <li>Gulshan Avenue, Dhaka 1212</li>
            <li>+880 1518-962973</li>
            <li>hello@eliteresidence.com</li>
          </ul>
        </div>
      </div>
      <div class="foot-bottom">
        <span>© <span id="year"></span> Elite Residence. All rights reserved.</span>
        <div>
          <a href="#">Privacy</a><a href="#">Terms</a><a href="#">Sitemap</a>
        </div>
      </div>
    </div>
  </footer>

</div>

<!-- DETAIL PAGE -->
<div id="detail-page" class="detail">
  <div class="container">
    <button class="back-btn" id="backBtn">
      <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="15 18 9 12 15 6"/></svg>
      Back to Home
    </button>
    <div id="detailContent"></div>
  </div>
</div>

<script>
/* ============================================================
   ELITE RESIDENCE — Property Database
   ------------------------------------------------------------
   This array holds the property listings. It is built to scale
   to 100+ properties. To add more:

     properties.push({
       id: 9,
       type: 'Flat',                  // Flat | Plot | House
       title: 'Skyline Penthouse',
       location: 'Gulshan',
       address: 'Road 41, Gulshan 2, Dhaka',
       beds: 4, baths: 5, sqft: 3800,
       price: 'BDT 6.5 Crore',
       image: 'https://images.unsplash.com/...?w=1200',
       gallery: ['url1','url2','url3'],
       features: ['Private elevator','Smart home','Rooftop pool'],
       description: 'Long description text...'
     });

   You can also generate them programmatically:
     for (let i = 9; i <= 100; i++) { properties.push({...}); }
   The grid renders ALL items in `properties` automatically,
   so any added items appear instantly after filter logic.
   ============================================================ */

const properties = [
  {
    id:1, type:'Flat', title:'Skyline Penthouse Residence',
    location:'Gulshan', address:'Road 41, Gulshan 2, Dhaka',
    beds:4, baths:5, sqft:3800, price:'BDT 6.5 Crore',
    image:'https://images.unsplash.com/photo-1545324418-cc1a3fa10c00?auto=format&fit=crop&w=1200&q=80',
    gallery:[
      'https://images.unsplash.com/photo-1545324418-cc1a3fa10c00?auto=format&fit=crop&w=1600&q=80',
      'https://images.unsplash.com/photo-1600585154340-be6161a56a0c?auto=format&fit=crop&w=900&q=80',
      'https://images.unsplash.com/photo-1600566753190-17f0baa2a6c3?auto=format&fit=crop&w=900&q=80'
    ],
    features:['Private elevator access','Floor-to-ceiling windows','Smart home automation','Rooftop infinity pool','24/7 concierge','Italian marble flooring'],
    description:'Set high above Gulshan, this signature penthouse offers panoramic skyline views, a private elevator entrance and meticulously crafted interiors. Designed for those who appreciate quiet luxury, every detail — from the imported stone to the bespoke joinery — has been considered.'
  },
  {
    id:2, type:'House', title:'The Banani Garden Villa',
    location:'Banani', address:'Road 11, Banani, Dhaka',
    beds:5, baths:6, sqft:5600, price:'BDT 12.8 Crore',
    image:'https://images.unsplash.com/photo-1600596542815-ffad4c1539a9?auto=format&fit=crop&w=1200&q=80',
    gallery:[
      'https://images.unsplash.com/photo-1600596542815-ffad4c1539a9?auto=format&fit=crop&w=1600&q=80',
      'https://images.unsplash.com/photo-1613490493576-7fde63acd811?auto=format&fit=crop&w=900&q=80',
      'https://images.unsplash.com/photo-1600566753086-00f18fe6ba62?auto=format&fit=crop&w=900&q=80'
    ],
    features:['Private landscaped garden','Double-height living room','Home theatre','Servant quarters','Covered parking for 4 cars','Generator backup'],
    description:'A standalone luxury villa in the heart of Banani, blending contemporary architecture with timeless craftsmanship. Expansive entertaining spaces flow into a private garden — a rare offering in central Dhaka.'
  },
  {
    id:3, type:'Flat', title:'Bashundhara Sky Apartments',
    location:'Bashundhara', address:'Block J, Bashundhara R/A, Dhaka',
    beds:3, baths:4, sqft:2400, price:'BDT 2.5 Crore',
    image:'https://images.unsplash.com/photo-1502672260266-1c1ef2d93688?auto=format&fit=crop&w=1200&q=80',
    gallery:[
      'https://images.unsplash.com/photo-1502672260266-1c1ef2d93688?auto=format&fit=crop&w=1600&q=80',
      'https://images.unsplash.com/photo-1560448204-e02f11c3d0e2?auto=format&fit=crop&w=900&q=80',
      'https://images.unsplash.com/photo-1556909114-f6e7ad7d3136?auto=format&fit=crop&w=900&q=80'
    ],
    features:['Modular kitchen','Master suite with walk-in closet','Community gym','Children play area','Reserved parking','High-speed elevators'],
    description:'A modern family residence in Bashundhara with a thoughtful layout, abundant natural light and a community designed around quiet, secure living.'
  },
  {
    id:4, type:'Plot', title:'Premium Corner Plot — Uttara',
    location:'Uttara', address:'Sector 18, Uttara, Dhaka',
    beds:0, baths:0, sqft:4200, price:'BDT 4.2 Crore',
    image:'https://images.unsplash.com/photo-1500382017468-9049fed747ef?auto=format&fit=crop&w=1200&q=80',
    gallery:[
      'https://images.unsplash.com/photo-1500382017468-9049fed747ef?auto=format&fit=crop&w=1600&q=80',
      'https://images.unsplash.com/photo-1464822759023-fed622ff2c3b?auto=format&fit=crop&w=900&q=80',
      'https://images.unsplash.com/photo-1466692476868-aef1dfb1e735?auto=format&fit=crop&w=900&q=80'
    ],
    features:['Corner-facing','Wide approach road','Ready for construction','Clean title','Premium neighborhood','Utility connections nearby'],
    description:'A rare corner plot in one of Uttara\'s most sought-after sectors. Ideal for building a custom residence or boutique low-rise development.'
  },
  {
    id:5, type:'Flat', title:'Mirpur Heights Family Flat',
    location:'Mirpur', address:'Mirpur DOHS, Dhaka',
    beds:3, baths:3, sqft:1850, price:'BDT 1.45 Crore',
    image:'https://images.unsplash.com/photo-1493809842364-78817add7ffb?auto=format&fit=crop&w=1200&q=80',
    gallery:[
      'https://images.unsplash.com/photo-1493809842364-78817add7ffb?auto=format&fit=crop&w=1600&q=80',
      'https://images.unsplash.com/photo-1560448204-603b3fc33ddc?auto=format&fit=crop&w=900&q=80',
      'https://images.unsplash.com/photo-1583847268964-b28dc8f51f92?auto=format&fit=crop&w=900&q=80'
    ],
    features:['Spacious balcony','South facing','Secure community','Backup power','Lift access','Children park'],
    description:'A bright, well-ventilated family home in the disciplined Mirpur DOHS community — offering comfort, security and excellent connectivity.'
  },
  {
    id:6, type:'House', title:'Badda Modern Townhouse',
    location:'Badda', address:'Pragati Sarani, Badda, Dhaka',
    beds:4, baths:4, sqft:3200, price:'BDT 5.2 Crore',
    image:'https://images.unsplash.com/photo-1605276374104-dee2a0ed3cd6?auto=format&fit=crop&w=1200&q=80',
    gallery:[
      'https://images.unsplash.com/photo-1605276374104-dee2a0ed3cd6?auto=format&fit=crop&w=1600&q=80',
      'https://images.unsplash.com/photo-1600210492486-724fe5c67fb0?auto=format&fit=crop&w=900&q=80',
      'https://images.unsplash.com/photo-1600607687939-ce8a6c25118c?auto=format&fit=crop&w=900&q=80'
    ],
    features:['Three-story design','Rooftop terrace','Modular kitchen','Home office','Two-car garage','CCTV throughout'],
    description:'Contemporary townhouse with clean lines, generous interiors and a rooftop terrace — ideal for modern families seeking privacy with connectivity.'
  },
  {
    id:7, type:'Flat', title:'Gulshan Lakeview Residence',
    location:'Gulshan', address:'Road 79, Gulshan 2, Dhaka',
    beds:3, baths:4, sqft:2950, price:'BDT 4.85 Crore',
    image:'https://images.unsplash.com/photo-1512917774080-9991f1c4c750?auto=format&fit=crop&w=1200&q=80',
    gallery:[
      'https://images.unsplash.com/photo-1512917774080-9991f1c4c750?auto=format&fit=crop&w=1600&q=80',
      'https://images.unsplash.com/photo-1600585154526-990dced4db0d?auto=format&fit=crop&w=900&q=80',
      'https://images.unsplash.com/photo-1600585152915-d208bec867a1?auto=format&fit=crop&w=900&q=80'
    ],
    features:['Lakefront views','Private balcony','Imported fittings','Gymnasium','Swimming pool','Concierge service'],
    description:'A boutique lakefront residence in Gulshan, offering uninterrupted lake views, refined interiors and access to premium building amenities.'
  },
  {
    id:8, type:'Plot', title:'Bashundhara Investment Plot',
    location:'Bashundhara', address:'Block L, Bashundhara R/A, Dhaka',
    beds:0, baths:0, sqft:3000, price:'BDT 2.9 Crore',
    image:'https://images.unsplash.com/photo-1486325212027-8081e485255e?auto=format&fit=crop&w=1200&q=80',
    gallery:[
      'https://images.unsplash.com/photo-1486325212027-8081e485255e?auto=format&fit=crop&w=1600&q=80',
      'https://images.unsplash.com/photo-1448630360428-65456885c650?auto=format&fit=crop&w=900&q=80',
      'https://images.unsplash.com/photo-1500382017468-9049fed747ef?auto=format&fit=crop&w=900&q=80'
    ],
    features:['Ready plot','Clear documents','Wide road frontage','Premium block','Excellent ROI','Near international school'],
    description:'A blue-chip investment plot in a rapidly appreciating block of Bashundhara, with strong long-term value and ready-to-build status.'
  }
  // ---- Add more properties here, up to 100, using the same shape ----
];

const WHATSAPP_NUMBER = '8801518962973';

let currentCat = 'all';
let currentLoc = 'all';
let currentType = 'all';
let currentKeyword = '';

const grid = document.getElementById('propertyGrid');

function buildCard(p){
  const specs = p.type === 'Plot'
    ? `<span>📐 ${p.sqft} sqft</span><span>📍 Plot</span><span>✓ Ready</span>`
    : `<span>🛏 ${p.beds} Beds</span><span>🛁 ${p.baths} Baths</span><span>📐 ${p.sqft} sqft</span>`;
  return `
    <article class="card" data-id="${p.id}">
      <div class="img">
        <img src="${p.image}" alt="${p.title}" loading="lazy"/>
        <span class="tag">${p.type}</span>
        <span class="fav"><svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M20.84 4.61a5.5 5.5 0 0 0-7.78 0L12 5.67l-1.06-1.06a5.5 5.5 0 0 0-7.78 7.78l1.06 1.06L12 21.23l7.78-7.78 1.06-1.06a5.5 5.5 0 0 0 0-7.78z"/></svg></span>
      </div>
      <div class="body">
        <h3>${p.title}</h3>
        <div class="loc">📍 ${p.address}</div>
        <div class="specs">${specs}</div>
        <div class="foot">
          <span class="price">${p.price}</span>
          <button class="btn-visit" data-action="visit" data-id="${p.id}">Schedule a Visit</button>
        </div>
      </div>
    </article>`;
}

function renderGrid(){
  const list = properties.filter(p=>{
    if(currentCat !== 'all' && p.type !== currentCat) return false;
    if(currentType !== 'all' && p.type !== currentType) return false;
    if(currentLoc !== 'all' && p.location !== currentLoc) return false;
    if(currentKeyword){
      const k = currentKeyword.toLowerCase();
      if(!(p.title.toLowerCase().includes(k) || p.address.toLowerCase().includes(k) || p.location.toLowerCase().includes(k))) return false;
    }
    return true;
  });
  if(!list.length){
    grid.innerHTML = `<div class="empty"><h3 style="font-family:var(--serif);font-size:22px;margin-bottom:6px">No properties match your filters</h3><p>Try adjusting the location or property type.</p></div>`;
    return;
  }
  grid.innerHTML = list.map(buildCard).join('');
}

/* Category tabs */
document.getElementById('catTabs').addEventListener('click', e=>{
  const b = e.target.closest('button'); if(!b) return;
  document.querySelectorAll('#catTabs button').forEach(x=>x.classList.remove('active'));
  b.classList.add('active');
  currentCat = b.dataset.cat;
  renderGrid();
});

/* Location pills */
document.getElementById('locPills').addEventListener('click', e=>{
  const b = e.target.closest('button'); if(!b) return;
  document.querySelectorAll('#locPills button').forEach(x=>x.classList.remove('active'));
  b.classList.add('active');
  currentLoc = b.dataset.loc;
  document.getElementById('fLocation').value = currentLoc === 'all' ? 'all' : currentLoc;
  renderGrid();
});

/* Search button */
document.getElementById('searchBtn').addEventListener('click', ()=>{
  currentKeyword = document.getElementById('fKeyword').value.trim();
  currentType = document.getElementById('fType').value;
  currentLoc = document.getElementById('fLocation').value;
  // sync location pills
  document.querySelectorAll('#locPills button').forEach(x=>{
    x.classList.toggle('active', x.dataset.loc === currentLoc);
  });
  document.getElementById('listings').scrollIntoView({behavior:'smooth'});
  renderGrid();
});

/* WhatsApp action */
function whatsappLink(p){
  const msg = `Hello Elite Residence,\n\nI am interested in scheduling a visit for the following property:\n\n• Property: ${p.title}\n• Type: ${p.type}\n• Location: ${p.address}\n• Price: ${p.price}\n\nPlease share availability. Thank you.`;
  return `https://wa.me/${WHATSAPP_NUMBER}?text=${encodeURIComponent(msg)}`;
}

/* Card clicks (open detail OR visit button) */
grid.addEventListener('click', e=>{
  const visitBtn = e.target.closest('[data-action="visit"]');
  if(visitBtn){
    e.stopPropagation();
    const p = properties.find(x=>x.id == visitBtn.dataset.id);
    window.open(whatsappLink(p), '_blank', 'noopener');
    return;
  }
  const card = e.target.closest('.card');
  if(card){ openDetail(card.dataset.id); }
});

/* DETAIL PAGE */
const detailPage = document.getElementById('detail-page');
const homePage = document.getElementById('home-page');
const detailContent = document.getElementById('detailContent');

function openDetail(id){
  const p = properties.find(x=>x.id == id);
  if(!p) return;
  const specsHTML = p.type === 'Plot'
    ? `<div><div class="k">Plot Area</div><div class="v">${p.sqft} sqft</div></div>
       <div><div class="k">Type</div><div class="v">${p.type}</div></div>
       <div><div class="k">Status</div><div class="v">Ready</div></div>`
    : `<div><div class="k">Bedrooms</div><div class="v">${p.beds}</div></div>
       <div><div class="k">Bathrooms</div><div class="v">${p.baths}</div></div>
       <div><div class="k">Area</div><div class="v">${p.sqft} sqft</div></div>
       <div><div class="k">Type</div><div class="v">${p.type}</div></div>`;

  detailContent.innerHTML = `
    <div class="detail-hero">
      <img src="${p.gallery[0]}" alt="${p.title}"/>
      <div class="side">
        <img src="${p.gallery[1]||p.gallery[0]}" alt=""/>
        <img src="${p.gallery[2]||p.gallery[0]}" alt=""/>
      </div>
    </div>
    <div class="detail-grid">
      <div class="detail-main">
        <span class="eyebrow-d" style="font-size:11px;letter-spacing:4px;text-transform:uppercase;color:var(--accent);font-weight:600">${p.type} · For Sale</span>
        <h1 style="margin-top:10px">${p.title}</h1>
        <div class="loc-line">📍 ${p.address}</div>
        <div class="specs-row">${specsHTML}</div>

        <h3 class="dh">About this property</h3>
        <p class="desc">${p.description}</p>

        <h3 class="dh">Property features</h3>
        <ul class="features">
          ${p.features.map(f=>`<li>${f}</li>`).join('')}
        </ul>
      </div>

      <aside class="booking">
        <div class="price-big">${p.price}</div>
        <div class="price-sub">Inclusive of registration assistance</div>
        <input type="text" placeholder="Full name"/>
        <input type="tel" placeholder="Phone number"/>
        <input type="email" placeholder="Email address"/>
        <textarea placeholder="I'd like to schedule a visit..."></textarea>
        <button class="btn-primary" id="bookBtn">Schedule a Visit</button>
        <button class="btn-outline" id="contactAgent">Contact Agent</button>
      </aside>
    </div>
  `;
  homePage.style.display = 'none';
  detailPage.classList.add('active');
  window.scrollTo({top:0,behavior:'instant'});

  document.getElementById('bookBtn').onclick = ()=> window.open(whatsappLink(p),'_blank','noopener');
  document.getElementById('contactAgent').onclick = ()=> window.open(whatsappLink(p),'_blank','noopener');
}

document.getElementById('backBtn').addEventListener('click', ()=>{
  detailPage.classList.remove('active');
  homePage.style.display = '';
  window.scrollTo({top:0,behavior:'smooth'});
});

/* Social icons */
document.getElementById('socials').addEventListener('click', e=>{
  const a = e.target.closest('a'); if(!a) return;
  e.preventDefault();
  window.open(a.dataset.url,'_blank','noopener');
});

document.getElementById('year').textContent = new Date().getFullYear();

renderGrid();
</script>
</body>
</html>
