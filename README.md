<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Mohamed Magdy – Senior BI & Data Governance</title>
<meta name="description" content="Mohamed Magdy is a Senior Business Intelligence Engineer and Data Governance Consultant specializing in Power BI, Informatica, and Data Management across banking and fintech.">
<meta name="keywords" content="Mohamed Magdy BI, Mohamed Magdy Data Engineer, Mohamed Magdy Power BI, Data Governance Egypt, BI Engineer Cairo">
<meta name="author" content="Mohamed Magdy">
<meta name="robots" content="index, follow">
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;600&family=DM+Sans:ital,wght@0,300;0,400;0,500;1,300&display=swap" rel="stylesheet"/>
<link rel="icon" type="image/png" href="icons/portfolio.png"/>
<style>
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
:root{
  --navy:#0B1F3A;--navy-mid:#16345C;--navy-light:#1E4A7A;
  --accent:#C6A857;--accent-light:#F0E4BE;--accent-dim:rgba(198,168,87,0.15);
  --light-bg:#F7F6F2;--white:#FFFFFF;
  --text-dark:#0B1F3A;--text-mid:#3D5470;--text-muted:#7A8FA8;
  --border:#DDE3EC;--radius:10px;
  --serif:'Playfair Display',Georgia,serif;--sans:'DM Sans',system-ui,sans-serif;
}
html{scroll-behavior:smooth}
body{font-family:var(--sans);color:var(--text-dark);background:var(--white);font-size:15px;line-height:1.7}

/* NAV */
nav{position:sticky;top:0;z-index:100;background:var(--navy);display:flex;align-items:center;justify-content:space-between;padding:0 3rem;height:60px}
.nav-logo{font-family:var(--serif);font-size:20px;color:var(--white);letter-spacing:.02em}
.nav-logo span{color:var(--accent)}
.nav-links{display:flex;gap:2rem;list-style:none}
.nav-links a{color:rgba(255,255,255,.75);text-decoration:none;font-size:12px;font-weight:500;letter-spacing:.07em;text-transform:uppercase;transition:color .2s}
.nav-links a:hover{color:var(--accent)}

/* HERO */
.hero{background:var(--navy);color:var(--white);padding:80px 3rem 70px;position:relative;overflow:hidden}
.hero::before{content:'';position:absolute;top:-80px;right:-100px;width:520px;height:520px;border-radius:50%;border:1px solid rgba(198,168,87,.12);pointer-events:none}
.hero::after{content:'';position:absolute;top:60px;right:50px;width:300px;height:300px;border-radius:50%;border:1px solid rgba(198,168,87,.07);pointer-events:none}
.hero-inner{max-width:960px;margin:0 auto;display:grid;grid-template-columns:1fr auto;gap:4rem;align-items:center;position:relative;z-index:1}
.hero-eyebrow{font-size:11px;font-weight:500;letter-spacing:.18em;text-transform:uppercase;color:var(--accent);margin-bottom:.9rem}
.hero h1{font-family:var(--serif);font-size:clamp(32px,4.5vw,50px);font-weight:600;line-height:1.15;margin-bottom:1rem}
.hero-subtitle{font-size:15px;color:rgba(255,255,255,.68);max-width:560px;margin-bottom:1.5rem;font-weight:300;line-height:1.75}
.hero-tags{display:flex;flex-wrap:wrap;gap:8px;margin-bottom:2rem}
.tag{background:var(--accent-dim);color:var(--accent);border:1px solid rgba(198,168,87,.3);border-radius:4px;padding:3px 11px;font-size:11px;font-weight:500;letter-spacing:.04em}
.hero-actions{display:flex;gap:12px;flex-wrap:wrap;margin-bottom:2.5rem}
.btn-primary{background:var(--accent);color:var(--navy);font-weight:500;padding:11px 26px;border-radius:6px;text-decoration:none;font-size:13px;transition:opacity .2s}
.btn-primary:hover{opacity:.88}
.btn-outline{border:1px solid rgba(255,255,255,.35);color:var(--white);font-weight:500;padding:11px 26px;border-radius:6px;text-decoration:none;font-size:13px;transition:border-color .2s}
.btn-outline:hover{border-color:rgba(255,255,255,.7)}
.hero-stats{display:flex;gap:2.5rem;padding-top:2rem;border-top:1px solid rgba(255,255,255,.1);flex-wrap:wrap}
.stat-num{font-family:var(--serif);font-size:28px;color:var(--accent);font-weight:600}
.stat-label{font-size:11px;color:rgba(255,255,255,.5);text-transform:uppercase;letter-spacing:.08em;margin-top:2px}
.hero-photo-wrap{flex-shrink:0}
.hero-photo{width:200px;height:200px;border-radius:50%;object-fit:cover;border:3px solid var(--accent);display:block}

/* COMPANIES SCROLL STRIP */
.strip-wrap{padding:36px 0;overflow:hidden;position:relative;background:var(--white);border-bottom:1px solid var(--border)}
.strip-wrap::before,.strip-wrap::after{content:'';position:absolute;top:0;bottom:0;width:80px;z-index:2;pointer-events:none}
.strip-wrap::before{left:0;background:linear-gradient(to right,var(--white),transparent)}
.strip-wrap::after{right:0;background:linear-gradient(to left,var(--white),transparent)}
.strip-label{text-align:center;font-size:10px;font-weight:500;letter-spacing:.14em;text-transform:uppercase;color:var(--text-muted);margin-bottom:20px}
#scroll-track{display:flex;gap:14px;width:max-content;animation:logoscroll 32s linear infinite}
#scroll-track:hover{animation-play-state:paused}
@keyframes logoscroll{from{transform:translateX(0)}to{transform:translateX(-50%)}}
.lcard{display:flex;flex-direction:column;align-items:center;justify-content:center;gap:6px;min-width:140px;height:88px;border-radius:10px;border:1px solid var(--border);background:var(--white);padding:10px 16px;transition:border-color .2s}
.lcard:hover{border-color:var(--accent)}
.limg{width:auto;height:36px;object-fit:contain;max-width:100px}
.lname{font-size:10px;font-weight:500;color:var(--text-muted);text-align:center;line-height:1.3;max-width:110px}
.lbadge{font-size:8px;letter-spacing:.07em;text-transform:uppercase;padding:2px 6px;border-radius:3px;font-weight:600}

/* SECTIONS */
section{padding:72px 3rem}
.section-inner{max-width:960px;margin:0 auto}
.section-label{font-size:11px;font-weight:500;letter-spacing:.18em;text-transform:uppercase;color:var(--accent);margin-bottom:.4rem}
.section-title{font-family:var(--serif);font-size:30px;font-weight:600;color:var(--navy);margin-bottom:2rem}
.divider-line{width:44px;height:2px;background:var(--accent);margin-bottom:2rem}

/* ABOUT */
.about-bg{background:var(--light-bg)}
.about-grid{display:grid;grid-template-columns:1fr 1fr;gap:3.5rem;align-items:start}
.about-text p{color:var(--text-mid);margin-bottom:.9rem;font-weight:300}
.about-text strong{color:var(--navy);font-weight:500}
.top-skills{display:flex;flex-wrap:wrap;gap:8px;margin-top:1.2rem}
.ts-pill{background:var(--white);border:1px solid var(--border);border-radius:20px;padding:5px 14px;font-size:12px;color:var(--text-mid);font-weight:400}
.cert-list{display:flex;flex-direction:column;gap:9px}
.cert-item{background:var(--white);border:1px solid var(--border);border-radius:var(--radius);padding:11px 15px;display:flex;align-items:center;gap:11px}
.cert-icon{width:30px;height:30px;background:var(--accent-light);border-radius:6px;display:flex;align-items:center;justify-content:center;flex-shrink:0}
.cert-icon svg{width:14px;height:14px;stroke:var(--accent);fill:none}
.cert-title{font-size:13px;font-weight:500;color:var(--navy)}
.cert-sub{font-size:12px;color:var(--text-muted)}

/* EXPERIENCE */
.exp-timeline{display:flex;flex-direction:column}
.exp-item{display:grid;grid-template-columns:190px 1fr;gap:2rem;padding:1.8rem 0;border-bottom:1px solid var(--border)}
.exp-item:last-child{border-bottom:none}
.exp-period{font-size:11px;font-weight:500;color:var(--accent);letter-spacing:.05em;text-transform:uppercase;margin-bottom:3px}
.exp-company{font-size:12px;color:var(--text-muted);line-height:1.5}
.exp-right h3{font-size:16px;font-weight:500;color:var(--navy);margin-bottom:3px}
.exp-loc{font-size:12px;color:var(--text-muted);margin-bottom:8px}
.exp-bullets{padding-left:.95rem;color:var(--text-mid);font-size:13px;font-weight:300}
.exp-bullets li{margin-bottom:4px}

/* SKILLS */
.skills-bg{background:var(--light-bg)}
.skills-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(210px,1fr));gap:18px}
.skill-card{background:var(--white);border:1px solid var(--border);border-radius:var(--radius);padding:18px}
.skill-card-title{font-size:11px;font-weight:500;color:var(--navy);margin-bottom:11px;padding-bottom:9px;border-bottom:1px solid var(--border);text-transform:uppercase;letter-spacing:.07em}
.skill-pills{display:flex;flex-wrap:wrap;gap:6px}
.pill{background:var(--light-bg);color:var(--text-mid);border-radius:4px;padding:3px 8px;font-size:11px}

/* PROJECTS */
.projects-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(280px,1fr));gap:20px}
.proj-card{border:1px solid var(--border);border-radius:var(--radius);overflow:hidden;background:var(--white);transition:border-color .2s,box-shadow .2s}
.proj-card:hover{border-color:var(--accent);box-shadow:0 4px 20px rgba(198,168,87,.1)}
.proj-org{font-size:10px;font-weight:500;letter-spacing:.1em;text-transform:uppercase;color:var(--accent);margin-bottom:5px}
.proj-period{font-size:11px;color:var(--text-muted);margin-bottom:6px}
.proj-card h3{font-size:14px;font-weight:500;color:var(--navy);margin-bottom:7px;line-height:1.4}
.proj-card p{font-size:12px;color:var(--text-mid);font-weight:300;line-height:1.6}
.proj-tags{display:flex;flex-wrap:wrap;gap:5px;margin-top:12px}
.proj-tag{background:var(--light-bg);color:var(--text-muted);border-radius:3px;padding:2px 7px;font-size:10px}
.proj-body{padding:20px}

/* SERVICES */
.services-bg{background:var(--light-bg)}
.serv-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(260px,1fr));gap:20px;margin-bottom:3rem}
.serv-card{background:var(--white);border:1px solid var(--border);border-radius:var(--radius);padding:22px;transition:border-color .2s,box-shadow .2s}
.serv-card:hover{border-color:var(--accent);box-shadow:0 4px 20px rgba(198,168,87,.1)}
.serv-icon{width:44px;height:44px;background:var(--accent-dim);border-radius:10px;display:flex;align-items:center;justify-content:center;margin-bottom:14px}
.serv-title{font-size:15px;font-weight:500;color:var(--navy);margin-bottom:8px}
.serv-desc{font-size:12px;color:var(--text-mid);font-weight:300;line-height:1.7;margin-bottom:14px}
.serv-pills{display:flex;flex-wrap:wrap;gap:5px}
.serv-pill{background:var(--accent-dim);color:var(--accent);border:1px solid rgba(198,168,87,.25);border-radius:3px;padding:2px 8px;font-size:10px;font-weight:500}
.serv-cta{background:var(--navy);border-radius:var(--radius);padding:36px 40px;display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;gap:1.5rem}
.serv-cta-label{font-size:11px;font-weight:500;letter-spacing:.14em;text-transform:uppercase;color:var(--accent);margin-bottom:6px}
.serv-cta-title{font-family:var(--serif);font-size:22px;font-weight:600;color:var(--white);margin-bottom:6px}
.serv-cta-sub{font-size:13px;color:rgba(255,255,255,.55);font-weight:300}

/* RECOMMENDATIONS */
.recs-bg{background:var(--light-bg)}
.recs-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(280px,1fr));gap:20px}
.rec-card{background:var(--white);border:1px solid var(--border);border-radius:var(--radius);padding:22px}
.rec-quote{font-size:28px;color:var(--accent);font-family:var(--serif);line-height:1;margin-bottom:10px}
.rec-text{font-size:13px;color:var(--text-mid);font-weight:300;line-height:1.7;font-style:italic;margin-bottom:16px}
.rec-author{display:flex;align-items:center;gap:10px}
.rec-avatar{width:36px;height:36px;border-radius:50%;background:var(--accent-light);display:flex;align-items:center;justify-content:center;font-size:13px;font-weight:500;color:var(--navy);flex-shrink:0}
.rec-name{font-size:13px;font-weight:500;color:var(--navy)}
.rec-role{font-size:11px;color:var(--text-muted)}

/* CONTACT */
.contact-bg{background:var(--navy);color:var(--white)}
.contact-bg .section-title{color:var(--white)}
.contact-grid{display:grid;grid-template-columns:1fr 1fr;gap:4rem;align-items:start}
.contact-desc{color:rgba(255,255,255,.65);font-weight:300;margin-bottom:1.5rem;font-size:14px}
.contact-links{display:flex;flex-direction:column;gap:12px}
.contact-link{display:flex;align-items:center;gap:11px;text-decoration:none;color:rgba(255,255,255,.8);font-size:13px;transition:color .2s}
.contact-link:hover{color:var(--accent)}
.contact-link-icon{width:34px;height:34px;border:1px solid rgba(255,255,255,.2);border-radius:7px;display:flex;align-items:center;justify-content:center;flex-shrink:0}
.contact-form{display:flex;flex-direction:column;gap:12px}
.contact-form input,.contact-form textarea{background:rgba(255,255,255,.07);border:1px solid rgba(255,255,255,.15);border-radius:6px;padding:11px 13px;color:var(--white);font-family:var(--sans);font-size:13px;resize:none;transition:border-color .2s}
.contact-form input::placeholder,.contact-form textarea::placeholder{color:rgba(255,255,255,.35)}
.contact-form input:focus,.contact-form textarea:focus{outline:none;border-color:var(--accent)}
.contact-form textarea{height:105px}
.btn-send{background:var(--accent);color:var(--navy);font-weight:500;padding:12px;border-radius:6px;border:none;cursor:pointer;font-size:13px;font-family:var(--sans);transition:opacity .2s}
.btn-send:hover{opacity:.88}

footer{background:#091829;padding:22px 3rem;display:flex;justify-content:space-between;align-items:center}
footer p{color:rgba(255,255,255,.35);font-size:12px}
.footer-logo{font-family:var(--serif);font-size:15px;color:rgba(255,255,255,.5)}
.footer-logo span{color:var(--accent)}

@media(max-width:700px){
  nav{padding:0 1.2rem}
  .nav-links{display:none}
  section{padding:56px 1.4rem}
  .hero{padding:52px 1.4rem}
  .hero-inner{grid-template-columns:1fr;gap:2rem}
  .hero-photo-wrap{display:flex;justify-content:center}
  .hero-stats{gap:1.5rem}
  .about-grid,.contact-grid{grid-template-columns:1fr;gap:2rem}
  .exp-item{grid-template-columns:1fr;gap:.4rem}
  .serv-cta{flex-direction:column;padding:24px}
  footer{flex-direction:column;gap:8px;text-align:center;padding:18px 1.4rem}
}
</style>

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Person",
  "name": "Mohamed Magdy",
  "jobTitle": "Senior BI Engineer & Data Governance Consultant",
  "url": "https://yourdomain.com",
  "sameAs": [
    "https://www.linkedin.com/in/mohamed-magdy-192413197",
    "https://github.com/mohamed-cs"
  ],
  "worksFor": {
    "@type": "Organization",
    "name": "Crédit Agricole Egypt"
  }
}
</script>
</head>
<body>

<!-- NAV -->
<nav>
  <div class="nav-logo">Mohamed <span>Magdy</span></div>
  <ul class="nav-links">
    <li><a href="#about">About</a></li>
    <li><a href="#experience">Experience</a></li>
    <li><a href="#skills">Skills</a></li>
    <li><a href="#projects">Projects</a></li>
    <li><a href="#services">Services</a></li>
    <li><a href="#recommendations">Reviews</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>
</nav>

<!-- HERO -->
<section class="hero" id="home">
  <div class="hero-inner">
    <div class="hero-left">
      <p class="hero-eyebrow">Senior BI Consultant &amp; Data Governance Consultant</p>
      <h1>Transforming Complex Data into Trusted, Insight-Driven Ecosystems</h1>
      <p class="hero-subtitle">4+ years bridging Business Intelligence, Data Management, and Governance across banking, energy, and fintech in Egypt and Saudi Arabia.</p>
      <div class="hero-tags">
        <span class="tag">Business Intelligence</span>
        <span class="tag">Data Governance</span>
        <span class="tag">Artificial Intelligence</span>
        <span class="tag">ETL / DWH</span>
        <span class="tag">NDMO &amp; PDPL Compliance</span>
        <span class="tag">Power BI · Tableau · MicroStrategy</span>
        <span class="tag">Informatica Suite (Power Center · Axon · EDC · IDQ)</span>
        <span class="tag">IDMC Suite (CDI · CDGC · CDQ)</span>
      </div>
      <div class="hero-actions">
        <a href="#projects" class="btn-primary">View My Work</a>
        <a href="#contact" class="btn-outline">Get In Touch</a>
      </div>
      <div class="hero-stats">
        <div><div class="stat-num">4+</div><div class="stat-label">Years Experience</div></div>
        <div><div class="stat-num">14+</div><div class="stat-label">Projects Delivered</div></div>
        <div><div class="stat-num">6+</div><div class="stat-label">Enterprise Clients</div></div>
        <div><div class="stat-num">9</div><div class="stat-label">LinkedIn Recommendations</div></div>
      </div>
    </div>
    <div class="hero-photo-wrap">
      <img class="hero-photo" src="images/Personal_img.jpg" alt="Mohamed Magdy"/>
    </div>
  </div>
</section>

<!-- COMPANIES SCROLL STRIP -->
<div class="strip-wrap">
  <p class="strip-label">Companies I've Worked With</p>
  <div id="scroll-track">
    <div class="lcard"><img class="limg" src="images/credit-agricole.png" alt="Crédit Agricole Egypt"/><span class="lname">Crédit Agricole Egypt</span><span class="lbadge" style="background:#E6F1FB;color:#185FA5">Banking</span></div>
    <div class="lcard"><img class="limg" src="images/ejada.png" alt="EJADA Consulting"/><span class="lname">EJADA Consulting</span><span class="lbadge" style="background:#EAF3DE;color:#3B6D11">Consulting</span></div>
    <div class="lcard"><img class="limg" src="images/ime.png" alt="IME"/><span class="lname">IME</span><span class="lbadge" style="background:#FAEEDA;color:#854F0B">Technology</span></div>
    <div class="lcard"><img class="limg" src="images/banque-du-caire.png" alt="Banque du Caire"/><span class="lname">Banque du Caire</span><span class="lbadge" style="background:#FBEAF0;color:#993556">Banking</span></div>
    <div class="lcard"><img class="limg" src="images/taqaa.png" alt="TAQA Arabia"/><span class="lname">TAQA Arabia</span><span class="lbadge" style="background:#E1F5EE;color:#0F6E56">Energy</span></div>
    <div class="lcard"><img class="limg" src="images/anb.png" alt="Arab National Bank"/><span class="lname">Arab National Bank</span><span class="lbadge" style="background:#EEEDFE;color:#534AB7">Banking</span></div>
    <div class="lcard"><img class="limg" src="images/saudi-post.png" alt="Saudi Post"/><span class="lname">Saudi Post (SPL)</span><span class="lbadge" style="background:#EAF3DE;color:#3B6D11">Government</span></div>
    <div class="lcard"><img class="limg" src="images/alrajhi-takaful.svg" alt="Al Rajhi Takaful"/><span class="lname">Al Rajhi Takaful</span><span class="lbadge" style="background:#FAECE7;color:#993C1D">Insurance</span></div>
    <div class="lcard"><img class="limg" src="images/neotek.png" alt="Neotek FinTech"/><span class="lname">Neotek FinTech</span><span class="lbadge" style="background:#E6F1FB;color:#185FA5">FinTech</span></div>
    <div class="lcard"><img class="limg" src="images/infatechs.png" alt="Infatechs"/><span class="lname">Infatechs</span><span class="lbadge" style="background:#FAEEDA;color:#854F0B">Technology</span></div>
    <!-- Duplicate for seamless loop -->
    <div class="lcard"><img class="limg" src="images/credit-agricole.png" alt="Crédit Agricole Egypt"/><span class="lname">Crédit Agricole Egypt</span><span class="lbadge" style="background:#E6F1FB;color:#185FA5">Banking</span></div>
    <div class="lcard"><img class="limg" src="images/ejada.png" alt="EJADA Consulting"/><span class="lname">EJADA Consulting</span><span class="lbadge" style="background:#EAF3DE;color:#3B6D11">Consulting</span></div>
    <div class="lcard"><img class="limg" src="images/ime.png" alt="IME"/><span class="lname">IME</span><span class="lbadge" style="background:#FAEEDA;color:#854F0B">Technology</span></div>
    <div class="lcard"><img class="limg" src="images/banque-du-caire.png" alt="Banque du Caire"/><span class="lname">Banque du Caire</span><span class="lbadge" style="background:#FBEAF0;color:#993556">Banking</span></div>
    <div class="lcard"><img class="limg" src="images/taqaa.png" alt="TAQA Arabia"/><span class="lname">TAQA Arabia</span><span class="lbadge" style="background:#E1F5EE;color:#0F6E56">Energy</span></div>
    <div class="lcard"><img class="limg" src="images/anb.png" alt="Arab National Bank"/><span class="lname">Arab National Bank</span><span class="lbadge" style="background:#EEEDFE;color:#534AB7">Banking</span></div>
    <div class="lcard"><img class="limg" src="images/saudi-post.png" alt="Saudi Post"/><span class="lname">Saudi Post (SPL)</span><span class="lbadge" style="background:#EAF3DE;color:#3B6D11">Government</span></div>
    <div class="lcard"><img class="limg" src="images/alrajhi-takaful.svg" alt="Al Rajhi Takaful"/><span class="lname">Al Rajhi Takaful</span><span class="lbadge" style="background:#FAECE7;color:#993C1D">Insurance</span></div>
    <div class="lcard"><img class="limg" src="images/neotek.png" alt="Neotek FinTech"/><span class="lname">Neotek FinTech</span><span class="lbadge" style="background:#E6F1FB;color:#185FA5">FinTech</span></div>
    <div class="lcard"><img class="limg" src="images/infatechs.png" alt="Infatechs"/><span class="lname">Infatechs</span><span class="lbadge" style="background:#FAEEDA;color:#854F0B">Technology</span></div>
  </div>
</div>

<!-- ABOUT -->
<section class="about-bg" id="about">
  <div class="section-inner">
    <p class="section-label">About Me</p>
    <h2 class="section-title">Data Engineer. Governance Consultant. Problem Solver.</h2>
    <div class="about-grid">
      <div class="about-text">
        <p>I'm a <strong>Senior BI &amp; Analytics Engineer</strong> and <strong>Data Governance Consultant</strong> with deep expertise in designing enterprise-scale data pipelines, warehouses, and governance frameworks.</p>
        <p>Currently at <strong>Crédit Agricole Bank</strong>, I focus on regulatory compliance reporting (ALM/CBE), ETL with Informatica PowerCenter, and Power BI dashboards. Previously, I led data governance implementations across Saudi Arabia aligned with <strong>NDMO, NDI, and PDPL</strong> standards for clients including Arab National Bank, Saudi Post, and Al Rajhi Takaful.</p>
        <p>My governance work spans establishing <strong>Data Ownership &amp; Stewardship models</strong>, defining <strong>Critical Data Elements (CDEs)</strong>, building <strong>Business Glossaries &amp; Governance Workflows</strong>, implementing <strong>metadata scanning, lineage analysis &amp; compliance monitoring</strong>, driving <strong>Data Classification</strong> frameworks, ensuring <strong>Data Quality</strong> standards, and managing end-to-end <strong>Metadata Management</strong> across enterprise environments.</p>
        <p>I am passionate about enabling organizations to build governed, high-quality, and scalable data environments that support strategic decision-making and regulatory compliance.</p>
        <div class="top-skills">
          <span class="ts-pill">Business Intelligence</span>
          <span class="ts-pill">Data Engineering</span>
          <span class="ts-pill">Data Analysis</span>
          <span class="ts-pill">Data Management</span>
          <span class="ts-pill">Data Modeling</span>
          <span class="ts-pill">8,751 LinkedIn Followers</span>
        </div>
      </div>
      <div>
        <p style="font-size:11px;font-weight:500;text-transform:uppercase;letter-spacing:.1em;color:var(--text-muted);margin-bottom:12px">Certifications &amp; Education</p>
        <div class="cert-list">
          <div class="cert-item">
            <div class="cert-icon"><svg viewBox="0 0 24 24" stroke-width="2"><path d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"/></svg></div>
            <div><div class="cert-title">Informatica IDMC, CDI &amp; CDGC</div><div class="cert-sub">Certified Professional</div></div>
          </div>
          <div class="cert-item">
            <div class="cert-icon"><svg viewBox="0 0 24 24" stroke-width="2"><path d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"/></svg></div>
            <div><div class="cert-title">PL-300: Microsoft Power BI Data Analyst</div><div class="cert-sub">Microsoft Certified</div></div>
          </div>
          <div class="cert-item">
            <div class="cert-icon"><svg viewBox="0 0 24 24" stroke-width="2"><path d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"/></svg></div>
            <div><div class="cert-title">DP-600: Microsoft Fabric Analytics Engineer</div><div class="cert-sub">Microsoft Certified</div></div>
          </div>
          <div class="cert-item">
            <div class="cert-icon"><svg viewBox="0 0 24 24" stroke-width="2"><path d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"/></svg></div>
            <div><div class="cert-title">DP-700: Microsoft Fabric Data Engineer</div><div class="cert-sub">Microsoft Certified</div></div>
          </div>
          <div class="cert-item">
            <div class="cert-icon"><svg viewBox="0 0 24 24" stroke-width="2"><path d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"/></svg></div>
            <div><div class="cert-title">Tableau Desktop Specialist</div><div class="cert-sub">Tableau Certified</div></div>
          </div>
          <div class="cert-item">
            <div class="cert-icon"><svg viewBox="0 0 24 24" stroke-width="2"><rect x="3" y="4" width="18" height="16" rx="2"/><path d="M8 9h8M8 13h5"/></svg></div>
            <div><div class="cert-title">Diploma in Applied Data Science</div><div class="cert-sub">WorldQuant University, 2020–2021</div></div>
          </div>
          <div class="cert-item">
            <div class="cert-icon"><svg viewBox="0 0 24 24" stroke-width="2"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01L12 2z"/></svg></div>
            <div><div class="cert-title">MSc Scientific Computing (ongoing)</div><div class="cert-sub">Ain Shams University · Neural Networks, CV, Optimization</div></div>
          </div>
          <div class="cert-item">
            <div class="cert-icon"><svg viewBox="0 0 24 24" stroke-width="2"><rect x="3" y="4" width="18" height="16" rx="2"/><path d="M8 9h8M8 13h5"/></svg></div>
            <div><div class="cert-title">BSc Computer &amp; Information Science</div><div class="cert-sub">Ain Shams University, 2019–2023</div></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- EXPERIENCE -->
<section id="experience">
  <div class="section-inner">
    <p class="section-label">Career</p>
    <h2 class="section-title">Professional Experience</h2>
    <div class="divider-line"></div>
    <div class="exp-timeline">
      <div class="exp-item">
        <div><div class="exp-period">Mar 2026 – Present</div><div class="exp-company">Crédit Agricole Bank<br>Cairo, Egypt · Banking</div></div>
        <div class="exp-right"><h3>Senior BI &amp; Analytics Engineer</h3><div class="exp-loc">Full-time</div>
        <ul class="exp-bullets">
          <li>Led automation of the CBE 1500 regulatory report (ALM), reverse-engineering legacy OBIEE logic.</li>
          <li>Reconciled data across core banking systems and DWH; resolved discrepancies in financial instruments, interest, maturity buckets, and liquidity gaps.</li>
          <li>Built ETL pipelines in Informatica PowerCenter, optimized complex SQL queries, and developed Power BI dashboards.</li>
          <li>Collaborated with Finance, Operations, and Data teams to validate business logic and regulatory requirements.</li>
        </ul></div>
      </div>
      <div class="exp-item">
        <div><div class="exp-period">Mar 2025 – Feb 2026</div><div class="exp-company">EJADA<br>Riyadh, Saudi Arabia · Consulting</div></div>
        <div class="exp-right"><h3>Data Management Specialist</h3><div class="exp-loc">Clients: ANB, Saudi Post, Neotek, Al Rajhi Takaful</div>
        <ul class="exp-bullets">
          <li>Administered Informatica Axon at Arab National Bank; designed ownership &amp; stewardship models and governance KPIs.</li>
          <li>Led NDMO/NDI data classification exercise across all Saudi Post departments; delivered training workshops.</li>
          <li>Configured Informatica EDC for metadata scanning, profiling, and end-to-end lineage at Neotek FinTech.</li>
          <li>Executed end-to-end CRM data migration from Eska, Penta &amp; Siebel to Microsoft Dynamics 365 for Al Rajhi Takaful.</li>
        </ul></div>
      </div>
      <div class="exp-item">
        <div><div class="exp-period">Jul 2023 – Feb 2025</div><div class="exp-company">IME<br>Cairo, Egypt · Technology</div></div>
        <div class="exp-right"><h3>Data Management Engineer</h3><div class="exp-loc">Full-time</div>
        <ul class="exp-bullets">
          <li>Designed scalable data pipelines and governance policies across multiple heterogeneous data sources.</li>
          <li>Implemented data quality monitoring, metadata management, and lifecycle management frameworks.</li>
          <li>Translated business requirements into dashboards and data models aligned with organizational goals.</li>
        </ul></div>
      </div>
      <div class="exp-item">
        <div><div class="exp-period">Feb 2024 – Jan 2025</div><div class="exp-company">Banque du Caire<br>Cairo, Egypt · Banking</div></div>
        <div class="exp-right"><h3>Senior BI &amp; Analytics Engineer</h3><div class="exp-loc">Full-time</div>
        <ul class="exp-bullets">
          <li>Migrated SAP Business Objects reports to MicroStrategy and a centralized data warehouse (FlexCube → T24/Temenos).</li>
          <li>Built dashboards for budgeting and retail MIS — customer segmentation, assets &amp; facilities portfolio.</li>
          <li>Performed source-to-target data reconciliation with DM sheet validation and flag verification.</li>
        </ul></div>
      </div>
      <div class="exp-item">
        <div><div class="exp-period">Jul 2022 – Jul 2023</div><div class="exp-company">TAQA Arabia<br>Cairo, Egypt · Energy</div></div>
        <div class="exp-right"><h3>Data Analytics &amp; Insights Analyst</h3><div class="exp-loc">Full-time</div>
        <ul class="exp-bullets">
          <li>Built ML models (regression + deep learning) for gas consumption prediction across Egypt — 92–95% accuracy.</li>
          <li>Automated HR payroll reporting for 4 companies: reduced 6-day process to under 5 minutes via Python EXE.</li>
          <li>Delivered Power BI dashboards and integrated multi-source data pipelines for operational decisions.</li>
        </ul></div>
      </div>
    </div>
  </div>
</section>

<!-- SKILLS -->
<section class="skills-bg" id="skills">
  <div class="section-inner">
    <p class="section-label">Expertise</p>
    <h2 class="section-title">Technical Skills</h2>
    <div class="skills-grid">
      <div class="skill-card"><div class="skill-card-title">Data Governance</div><div class="skill-pills"><span class="pill">Informatica Axon</span><span class="pill">IDMC</span><span class="pill">EDC</span><span class="pill">CDGC</span><span class="pill">CDQ</span><span class="pill">MCC</span></div></div>
      <div class="skill-card"><div class="skill-card-title">ETL / Integration</div><div class="skill-pills"><span class="pill">Informatica PowerCenter</span><span class="pill">CDI</span><span class="pill">IDQ</span><span class="pill">SSIS</span><span class="pill">DBT</span><span class="pill">Microsoft Fabric</span></div></div>
      <div class="skill-card"><div class="skill-card-title">BI &amp; Visualization</div><div class="skill-pills"><span class="pill">Power BI</span><span class="pill">MicroStrategy</span><span class="pill">Tableau</span><span class="pill">SAP BO</span><span class="pill">OBIEE</span></div></div>
      <div class="skill-card"><div class="skill-card-title">Databases &amp; Platforms</div><div class="skill-pills"><span class="pill">Oracle</span><span class="pill">SQL Server</span><span class="pill">Snowflake</span><span class="pill">Cloudera</span><span class="pill">Hadoop</span><span class="pill">Hive</span><span class="pill">Impala</span></div></div>
      <div class="skill-card"><div class="skill-card-title">Programming</div><div class="skill-pills"><span class="pill">SQL / PL-SQL</span><span class="pill">Python</span><span class="pill">Data Modeling</span><span class="pill">DWH Architecture</span><span class="pill">Java</span></div></div>
      <div class="skill-card"><div class="skill-card-title">Compliance</div><div class="skill-pills"><span class="pill">NDMO</span><span class="pill">NDI</span><span class="pill">PDPL</span><span class="pill">Data Classification</span><span class="pill">FlexCube</span></div></div>
    </div>
  </div>
</section>

<!-- PROJECTS -->
<section id="projects">
  <div class="section-inner">
    <p class="section-label">Selected Work</p>
    <h2 class="section-title">Key Projects</h2>
    <div class="projects-grid">

      <div class="proj-card">
        <div style="width:100%;height:160px;background:#0B2A4A;position:relative;overflow:hidden">
          <div style="position:absolute;inset:0;display:grid;grid-template-columns:repeat(5,1fr);align-items:flex-end;gap:3px;padding:12px 14px">
            <div style="background:rgba(198,168,87,.7);height:70px;border-radius:2px 2px 0 0"></div>
            <div style="background:rgba(198,168,87,.45);height:50px;border-radius:2px 2px 0 0"></div>
            <div style="background:rgba(198,168,87,.6);height:62px;border-radius:2px 2px 0 0"></div>
            <div style="background:rgba(198,168,87,.35);height:38px;border-radius:2px 2px 0 0"></div>
            <div style="background:rgba(198,168,87,.55);height:56px;border-radius:2px 2px 0 0"></div>
          </div>
          <div style="position:absolute;top:10px;left:14px;display:flex;gap:12px">
            <div style="text-align:center"><div style="font-size:14px;font-weight:600;color:#C6A857;font-family:'Playfair Display',serif">ALM</div><div style="font-size:9px;color:rgba(255,255,255,.4)">Regulatory</div></div>
            <div style="text-align:center"><div style="font-size:14px;font-weight:600;color:#C6A857;font-family:'Playfair Display',serif">CBE</div><div style="font-size:9px;color:rgba(255,255,255,.4)">1500 Report</div></div>
          </div>
        </div>
        <div class="proj-body"><div class="proj-org">Crédit Agricole Egypt</div><div class="proj-period">Feb 2026 – Apr 2026</div><h3>CBE 1500 Report Analysis &amp; Automation</h3><p>Led end-to-end analysis and automation of the CBE 1500 regulatory report. Reverse-engineered OBIEE logic, reconciled DWH data, and resolved ALM discrepancies in financial instruments, maturity buckets, and liquidity gaps.</p><div class="proj-tags"><span class="proj-tag">Informatica</span><span class="proj-tag">Power BI</span><span class="proj-tag">SQL</span><span class="proj-tag">ALM</span><span class="proj-tag">OBIEE</span></div></div>
      </div>

      <div class="proj-card">
        <div style="width:100%;height:160px;background:#16345C;position:relative;overflow:hidden">
          <div style="position:absolute;inset:0;display:flex;align-items:center;justify-content:center;gap:16px;padding:12px">
            <div style="display:flex;flex-direction:column;gap:6px">
              <div style="width:80px;height:7px;background:rgba(198,168,87,.6);border-radius:2px"></div>
              <div style="width:60px;height:7px;background:rgba(198,168,87,.4);border-radius:2px"></div>
              <div style="width:70px;height:7px;background:rgba(198,168,87,.5);border-radius:2px"></div>
              <div style="width:50px;height:7px;background:rgba(198,168,87,.35);border-radius:2px"></div>
            </div>
            <div style="width:56px;height:56px;border-radius:50%;border:2px solid rgba(198,168,87,.5);display:flex;align-items:center;justify-content:center">
              <div style="width:36px;height:36px;border-radius:50%;background:conic-gradient(rgba(198,168,87,.8) 70%,rgba(255,255,255,.1) 0)"></div>
            </div>
          </div>
        </div>
        <div class="proj-body"><div class="proj-org">Arab National Bank</div><div class="proj-period">Oct 2025 – Dec 2025</div><h3>Enterprise Data Governance &amp; Quality Implementation</h3><p>Implemented Informatica Axon org-wide. Designed ownership &amp; stewardship models, governed CDEs, built governance dashboards and KPIs. Managed Axon and IDQ migration from dev to production.</p><div class="proj-tags"><span class="proj-tag">Axon</span><span class="proj-tag">IDQ</span><span class="proj-tag">CDEs</span><span class="proj-tag">Data Governance</span></div></div>
      </div>

      <div class="proj-card">
        <div style="width:100%;height:160px;background:#0F3D2A;position:relative;overflow:hidden">
          <div style="position:absolute;inset:0;display:flex;align-items:center;justify-content:center;gap:16px;padding:12px">
            <div style="display:flex;flex-direction:column;gap:5px">
              <div style="font-size:10px;color:rgba(198,168,87,.9);letter-spacing:.06em">NDMO</div>
              <div style="font-size:10px;color:rgba(198,168,87,.8);letter-spacing:.06em">NDI</div>
              <div style="font-size:10px;color:rgba(198,168,87,.8);letter-spacing:.06em">CDEs</div>
              <div style="font-size:10px;color:rgba(198,168,87,.8);letter-spacing:.06em">MCC</div>
            </div>
            <div style="display:flex;flex-direction:column;gap:6px">
              <div style="width:70px;height:6px;background:rgba(198,168,87,.6);border-radius:2px"></div>
              <div style="width:55px;height:6px;background:rgba(198,168,87,.4);border-radius:2px"></div>
              <div style="width:65px;height:6px;background:rgba(198,168,87,.5);border-radius:2px"></div>
              <div style="width:45px;height:6px;background:rgba(198,168,87,.35);border-radius:2px"></div>
            </div>
          </div>
        </div>
        <div class="proj-body"><div class="proj-org">Saudi Post (SPL)</div><div class="proj-period">Jul 2025 – Sep 2025</div><h3>NDMO / NDI Data Classification Project</h3><p>Classified CDEs across all departments, conducted workshops, and supported IDMC/MCC for metadata scanning, lineage, and compliance monitoring.</p><div class="proj-tags"><span class="proj-tag">NDMO</span><span class="proj-tag">IDMC</span><span class="proj-tag">MCC</span><span class="proj-tag">NDI</span></div></div>
      </div>

      <div class="proj-card">
        <div style="width:100%;height:160px;background:#3D1A0A;position:relative;overflow:hidden">
          <div style="position:absolute;inset:0;display:flex;align-items:center;justify-content:center;gap:10px;padding:12px">
            <div style="display:flex;flex-direction:column;align-items:center;gap:4px"><div style="font-size:10px;color:rgba(198,168,87,.8)">Eska</div><div style="width:2px;height:18px;background:rgba(198,168,87,.4)"></div></div>
            <div style="display:flex;flex-direction:column;align-items:center;gap:4px"><div style="font-size:10px;color:rgba(198,168,87,.8)">Penta</div><div style="width:2px;height:18px;background:rgba(198,168,87,.4)"></div></div>
            <div style="display:flex;flex-direction:column;align-items:center;gap:4px"><div style="font-size:10px;color:rgba(198,168,87,.8)">Siebel</div><div style="width:2px;height:18px;background:rgba(198,168,87,.4)"></div></div>
            <div style="font-size:18px;color:rgba(198,168,87,.6)">→</div>
            <div style="background:rgba(198,168,87,.15);border:1px solid rgba(198,168,87,.5);border-radius:6px;padding:6px 12px;font-size:10px;color:rgba(198,168,87,.9)">Dynamics 365</div>
          </div>
        </div>
        <div class="proj-body"><div class="proj-org">Al Rajhi Takaful</div><div class="proj-period">Apr 2025 – May 2025</div><h3>CRM Migration: Legacy Systems → Dynamics 365</h3><p>End-to-end migration from Eska, Penta, and Siebel with cleansing, de-duplication, audit trail, automated scheduling, and Informatica server administration.</p><div class="proj-tags"><span class="proj-tag">Informatica</span><span class="proj-tag">Dynamics 365</span><span class="proj-tag">ETL</span><span class="proj-tag">Data Quality</span></div></div>
      </div>

      <div class="proj-card">
        <div style="width:100%;height:160px;background:#1A2A3D;position:relative;overflow:hidden">
          <div style="position:absolute;inset:0;display:flex;align-items:center;justify-content:center;padding:12px">
            <div style="display:flex;flex-direction:column;gap:8px">
              <div style="display:flex;align-items:center;gap:8px"><div style="width:10px;height:10px;border-radius:50%;background:rgba(198,168,87,.7)"></div><div style="font-size:10px;color:rgba(198,168,87,.8)">Metadata Scanning</div></div>
              <div style="display:flex;align-items:center;gap:8px"><div style="width:10px;height:10px;border-radius:50%;background:rgba(198,168,87,.55)"></div><div style="font-size:10px;color:rgba(198,168,87,.65)">Data Lineage</div></div>
              <div style="display:flex;align-items:center;gap:8px"><div style="width:10px;height:10px;border-radius:50%;background:rgba(198,168,87,.65)"></div><div style="font-size:10px;color:rgba(198,168,87,.75)">Business Glossary</div></div>
              <div style="display:flex;align-items:center;gap:8px"><div style="width:10px;height:10px;border-radius:50%;background:rgba(198,168,87,.45)"></div><div style="font-size:10px;color:rgba(198,168,87,.6)">Ownership Roles</div></div>
            </div>
          </div>
        </div>
        <div class="proj-body"><div class="proj-org">Neotek FinTech</div><div class="proj-period">Mar 2025 – Apr 2025</div><h3>Data Governance Enablement — EDC &amp; Axon</h3><p>Deployed Informatica EDC for automated metadata harvesting and lineage. Maintained glossaries, defined policies, and assigned ownership roles aligned with NDMO guidelines.</p><div class="proj-tags"><span class="proj-tag">EDC</span><span class="proj-tag">Axon</span><span class="proj-tag">Metadata</span><span class="proj-tag">NDMO</span></div></div>
      </div>

      <div class="proj-card">
        <div style="width:100%;height:160px;background:#1E1A3D;position:relative;overflow:hidden">
          <div style="position:absolute;inset:0;display:grid;grid-template-columns:repeat(4,1fr);align-items:flex-end;gap:4px;padding:12px 14px">
            <div style="background:rgba(198,168,87,.65);height:65px;border-radius:2px 2px 0 0"></div>
            <div style="background:rgba(198,168,87,.5);height:80px;border-radius:2px 2px 0 0"></div>
            <div style="background:rgba(198,168,87,.4);height:45px;border-radius:2px 2px 0 0"></div>
            <div style="background:rgba(198,168,87,.6);height:72px;border-radius:2px 2px 0 0"></div>
          </div>
          <div style="position:absolute;top:10px;left:14px;font-size:10px;color:rgba(198,168,87,.75)">Budgeting · Retail KPIs</div>
        </div>
        <div class="proj-body"><div class="proj-org">Banque du Caire</div><div class="proj-period">Jun 2024 – Jan 2025</div><h3>Dashboard Development for Budgeting &amp; Retail</h3><p>Designed interactive dashboards for customer segmentation, assets portfolio, and facilities portfolio. Enabled KPI monitoring for budgeting and retail operations teams.</p><div class="proj-tags"><span class="proj-tag">Power BI</span><span class="proj-tag">MicroStrategy</span><span class="proj-tag">Data Analysis</span><span class="proj-tag">KPI</span></div></div>
      </div>

      <div class="proj-card">
        <div style="width:100%;height:160px;background:#1A1E3D;position:relative;overflow:hidden">
          <div style="position:absolute;inset:0;display:flex;align-items:center;justify-content:center;gap:10px;padding:12px">
            <div style="background:rgba(198,168,87,.15);border:1px solid rgba(198,168,87,.5);border-radius:6px;padding:6px 12px;font-size:10px;color:rgba(198,168,87,.9)">SAP BO</div>
            <div style="font-size:18px;color:rgba(198,168,87,.6)">→</div>
            <div style="background:rgba(198,168,87,.15);border:1px solid rgba(198,168,87,.5);border-radius:6px;padding:6px 12px;font-size:10px;color:rgba(198,168,87,.9)">MicroStrategy</div>
            <div style="font-size:18px;color:rgba(198,168,87,.6)">→</div>
            <div style="background:rgba(198,168,87,.15);border:1px solid rgba(198,168,87,.5);border-radius:6px;padding:6px 12px;font-size:10px;color:rgba(198,168,87,.9)">DWH</div>
          </div>
        </div>
        <div class="proj-body"><div class="proj-org">Banque du Caire</div><div class="proj-period">Jun 2024 – Jan 2025</div><h3>BI Migration: SAP BO → MicroStrategy &amp; DWH</h3><p>Migrated core banking reports from SAP BO to MicroStrategy. Ensured accurate data mapping, optimized performance, and integrated with existing BI infrastructure.</p><div class="proj-tags"><span class="proj-tag">MicroStrategy</span><span class="proj-tag">SAP BO</span><span class="proj-tag">DWH</span><span class="proj-tag">Reconciliation</span></div></div>
      </div>

      <div class="proj-card">
        <div style="width:100%;height:160px;background:#1A2810;position:relative;overflow:hidden">
          <div style="position:absolute;inset:0;display:flex;align-items:center;justify-content:center;padding:12px">
            <div style="display:flex;flex-direction:column;gap:8px">
              <div style="display:flex;align-items:center;gap:8px"><div style="width:36px;height:6px;background:rgba(198,168,87,.7);border-radius:2px"></div><div style="font-size:10px;color:rgba(198,168,87,.8)">Source</div></div>
              <div style="display:flex;align-items:center;gap:8px"><div style="width:28px;height:6px;background:rgba(198,168,87,.5);border-radius:2px"></div><div style="font-size:10px;color:rgba(198,168,87,.65)">Validate</div></div>
              <div style="display:flex;align-items:center;gap:8px"><div style="width:32px;height:6px;background:rgba(198,168,87,.6);border-radius:2px"></div><div style="font-size:10px;color:rgba(198,168,87,.7)">Target</div></div>
              <div style="display:flex;align-items:center;gap:8px"><div style="width:22px;height:6px;background:rgba(198,168,87,.4);border-radius:2px"></div><div style="font-size:10px;color:rgba(198,168,87,.55)">DM Sheet</div></div>
            </div>
          </div>
        </div>
        <div class="proj-body"><div class="proj-org">Banque du Caire</div><div class="proj-period">Jan 2024 – Mar 2024</div><h3>Data Reconciliation on Banking Data Migration</h3><p>Validated source-to-target mappings against DM sheets, performed accuracy checks and flag verifications, and resolved discrepancies to ensure data integrity throughout migration.</p><div class="proj-tags"><span class="proj-tag">SQL</span><span class="proj-tag">Data Reconciliation</span><span class="proj-tag">DM Sheets</span><span class="proj-tag">Data Quality</span></div></div>
      </div>

      <div class="proj-card">
        <div style="width:100%;height:160px;background:#0B2A1A;position:relative;overflow:hidden">
          <div style="position:absolute;inset:0;display:grid;grid-template-columns:repeat(6,1fr);align-items:flex-end;gap:3px;padding:12px 14px">
            <div style="background:rgba(198,168,87,.5);height:55px;border-radius:2px 2px 0 0"></div>
            <div style="background:rgba(198,168,87,.65);height:78px;border-radius:2px 2px 0 0"></div>
            <div style="background:rgba(198,168,87,.45);height:60px;border-radius:2px 2px 0 0"></div>
            <div style="background:rgba(198,168,87,.7);height:85px;border-radius:2px 2px 0 0"></div>
            <div style="background:rgba(198,168,87,.4);height:45px;border-radius:2px 2px 0 0"></div>
            <div style="background:rgba(198,168,87,.6);height:68px;border-radius:2px 2px 0 0"></div>
          </div>
          <div style="position:absolute;top:10px;right:12px;font-size:13px;font-weight:600;color:#C6A857;font-family:'Playfair Display',serif">92–95%</div>
        </div>
        <div class="proj-body"><div class="proj-org">TAQA Arabia</div><div class="proj-period">Jan 2023 – Jun 2023</div><h3>Gas Consumption Prediction &amp; Optimization</h3><p>Built regression and deep learning models on 20 years of historical data — achieving 92–95% prediction accuracy to optimize gas distribution and reduce logistics costs across Egypt.</p><div class="proj-tags"><span class="proj-tag">Python</span><span class="proj-tag">Deep Learning</span><span class="proj-tag">Power BI</span><span class="proj-tag">ETL</span></div></div>
      </div>

      <div class="proj-card">
        <div style="width:100%;height:160px;background:#2A1A0A;position:relative;overflow:hidden">
          <div style="position:absolute;inset:0;display:flex;align-items:center;justify-content:center;gap:16px;padding:12px">
            <div style="text-align:center"><div style="font-size:26px;font-weight:600;color:#C6A857;font-family:'Playfair Display',serif">6 days</div><div style="font-size:10px;color:rgba(255,255,255,.4)">before</div></div>
            <div style="font-size:22px;color:rgba(198,168,87,.5)">→</div>
            <div style="text-align:center"><div style="font-size:26px;font-weight:600;color:#C6A857;font-family:'Playfair Display',serif">&lt;5 min</div><div style="font-size:10px;color:rgba(255,255,255,.4)">after</div></div>
          </div>
        </div>
        <div class="proj-body"><div class="proj-org">TAQA Arabia</div><div class="proj-period">Jan 2023 – Feb 2023</div><h3>Automated HR Payroll &amp; Performance System</h3><p>Transformed a 6-day, 3-person manual payroll process into a Python EXE completing in under 5 minutes — covering 4 companies with executive and individual performance dashboards.</p><div class="proj-tags"><span class="proj-tag">Python</span><span class="proj-tag">Excel</span><span class="proj-tag">Automation</span><span class="proj-tag">VBA</span></div></div>
      </div>

      <div class="proj-card">
        <div style="width:100%;height:160px;background:#2A1A3D;position:relative;overflow:hidden">
          <div style="position:absolute;inset:0;display:flex;align-items:center;justify-content:center;gap:16px;padding:12px">
            <div style="text-align:center"><div style="font-size:26px;font-weight:600;color:#C6A857;font-family:'Playfair Display',serif">95.7%</div><div style="font-size:10px;color:rgba(255,255,255,.4)">GCN accuracy</div></div>
            <div style="width:60px;height:60px;border-radius:50%;border:2px solid rgba(198,168,87,.4);display:flex;align-items:center;justify-content:center">
              <div style="width:40px;height:40px;border-radius:50%;background:conic-gradient(rgba(198,168,87,.8) 95.7%,rgba(255,255,255,.1) 0)"></div>
            </div>
          </div>
        </div>
        <div class="proj-body"><div class="proj-org">Ain Shams University</div><div class="proj-period">Dec 2022 – Jul 2023</div><h3>CNN-GNN Graph Breast-Fusion: Deep Learning for Cancer Classification</h3><p>Combined CNN and Graph Convolutional Networks for automated breast cancer classification in mammogram images. GCN achieved 95.7% accuracy using VGG16 embeddings and K-nearest neighbor graph construction.</p><div class="proj-tags"><span class="proj-tag">CNN</span><span class="proj-tag">GCN</span><span class="proj-tag">VGG16</span><span class="proj-tag">Python</span><span class="proj-tag">Healthcare AI</span></div></div>
      </div>

    </div>
  </div>
</section>

<!-- SERVICES -->
<section class="services-bg" id="services">
  <div class="section-inner">
    <p class="section-label">Freelance &amp; Consulting</p>
    <h2 class="section-title">How I Can Help You</h2>
    <div class="divider-line"></div>
    <div class="serv-grid">

      <div class="serv-card">
        <div class="serv-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="var(--accent)" stroke-width="1.6" width="24" height="24"><rect x="2" y="3" width="20" height="14" rx="2"/><path d="M8 21h8M12 17v4"/><path d="M7 10l3 3 3-3 4 4"/></svg>
        </div>
        <h3 class="serv-title">BI Dashboards &amp; Reports</h3>
        <p class="serv-desc">Interactive dashboards and reports tailored to your business KPIs — built in Power BI, Tableau, MicroStrategy, or Excel. From data connection to final delivery.</p>
        <div class="serv-pills">
          <span class="serv-pill">Power BI</span>
          <span class="serv-pill">Tableau</span>
          <span class="serv-pill">MicroStrategy</span>
          <span class="serv-pill">Excel</span>
        </div>
      </div>

      <div class="serv-card">
        <div class="serv-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="var(--accent)" stroke-width="1.6" width="24" height="24"><path d="M12 2v4M12 18v4M4.93 4.93l2.83 2.83M16.24 16.24l2.83 2.83M2 12h4M18 12h4M4.93 19.07l2.83-2.83M16.24 7.76l2.83-2.83"/></svg>
        </div>
        <h3 class="serv-title">Task &amp; Process Automation</h3>
        <p class="serv-desc">Turn repetitive manual workflows into fully automated solutions — Python scripts, Excel macros, scheduled jobs, and end-to-end pipeline automation that saves hours every week.</p>
        <div class="serv-pills">
          <span class="serv-pill">Python</span>
          <span class="serv-pill">VBA / Macros</span>
          <span class="serv-pill">ETL Pipelines</span>
          <span class="serv-pill">Scheduling</span>
        </div>
      </div>

      <div class="serv-card">
        <div class="serv-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="var(--accent)" stroke-width="1.6" width="24" height="24"><ellipse cx="12" cy="5" rx="9" ry="3"/><path d="M3 5v4c0 1.66 4.03 3 9 3s9-1.34 9-3V5"/><path d="M3 9v4c0 1.66 4.03 3 9 3s9-1.34 9-3V9"/><path d="M3 13v4c0 1.66 4.03 3 9 3s9-1.34 9-3v-4"/></svg>
        </div>
        <h3 class="serv-title">Data Engineering &amp; ETL</h3>
        <p class="serv-desc">Design and build robust data pipelines, warehouses, and integration workflows that consolidate your data from multiple sources into a single clean, reliable foundation.</p>
        <div class="serv-pills">
          <span class="serv-pill">SQL / PL-SQL</span>
          <span class="serv-pill">Informatica</span>
          <span class="serv-pill">SSIS</span>
          <span class="serv-pill">DWH Design</span>
        </div>
      </div>

      <div class="serv-card">
        <div class="serv-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="var(--accent)" stroke-width="1.6" width="24" height="24"><path d="M12 2a4 4 0 0 1 4 4 4 4 0 0 1-4 4 4 4 0 0 1-4-4 4 4 0 0 1 4-4"/><path d="M12 14a4 4 0 0 1 4 4 4 4 0 0 1-4 4 4 4 0 0 1-4-4 4 4 0 0 1 4-4"/><path d="M2 8a4 4 0 0 1 4 4 4 4 0 0 1-4-4"/><path d="M18 8a4 4 0 0 1 4 4 4 4 0 0 1-4-4"/></svg>
        </div>
        <h3 class="serv-title">Machine Learning &amp; AI</h3>
        <p class="serv-desc">Predictive models, forecasting engines, and AI-powered tools built for real business problems — from demand prediction and customer segmentation to deep learning applications.</p>
        <div class="serv-pills">
          <span class="serv-pill">Regression Models</span>
          <span class="serv-pill">Classification Models</span>
          <span class="serv-pill">Deep Learning</span>
          <span class="serv-pill">Forecasting</span>
        </div>
      </div>

      <div class="serv-card">
        <div class="serv-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="var(--accent)" stroke-width="1.6" width="24" height="24"><rect x="3" y="3" width="18" height="18" rx="2"/><path d="M3 9h18M9 21V9"/></svg>
        </div>
        <h3 class="serv-title">Advanced Excel Solutions</h3>
        <p class="serv-desc">Complex Excel models, dynamic dashboards, financial templates, automated reports, and custom formulas — turning plain spreadsheets into powerful business tools.</p>
        <div class="serv-pills">
          <span class="serv-pill">Power Query</span>
          <span class="serv-pill">Pivot Tables</span>
          <span class="serv-pill">Dynamic Dashboards</span>
          <span class="serv-pill">VBA</span>
        </div>
      </div>

      <div class="serv-card">
        <div class="serv-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="var(--accent)" stroke-width="1.6" width="24" height="24"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"/></svg>
        </div>
        <h3 class="serv-title">Data Governance Consulting</h3>
        <p class="serv-desc">End-to-end governance framework design — data ownership models, metadata management, data quality standards, business glossaries, and regulatory compliance aligned with NDMO and PDPL.</p>
        <div class="serv-pills">
          <span class="serv-pill">NDMO / PDPL</span>
          <span class="serv-pill">Data Quality</span>
          <span class="serv-pill">Metadata Mgmt</span>
          <span class="serv-pill">Informatica Axon</span>
        </div>
      </div>

     <div class="serv-card">
  <div class="serv-icon">
    <svg viewBox="0 0 24 24" fill="none" stroke="var(--accent)" stroke-width="1.6" width="24" height="24"><path d="M17 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2"/><circle cx="9" cy="7" r="4"/><path d="M23 21v-2a4 4 0 0 0-3-3.87"/><path d="M16 3.13a4 4 0 0 1 0 7.75"/></svg>
  </div>
  <h3 class="serv-title">Training &amp; Mentoring</h3>
  <p class="serv-desc">2+ years of hands-on instructor experience at GOMYCODE and AMIT Learning — delivering structured training in Power BI, Tableau, Excel, SQL, Python, machine learning, and data science fundamentals. Sessions tailored from beginner to advanced, one-on-one or group, online or on-site.</p>
  <div class="serv-pills">
    <span class="serv-pill">Power BI Training</span>
    <span class="serv-pill">Tableau</span>
    <span class="serv-pill">Excel &amp; Power Query</span>
    <span class="serv-pill">SQL Coaching</span>
    <span class="serv-pill">Python</span>
    <span class="serv-pill">Machine Learning</span>
    <span class="serv-pill">Career Guidance</span>
    <span class="serv-pill">1-on-1 Sessions</span>
  </div>
</div>

      <div class="serv-card">
        <div class="serv-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="var(--accent)" stroke-width="1.6" width="24" height="24"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"/></svg>
        </div>
        <h3 class="serv-title">Data Strategy Consultation</h3>
        <p class="serv-desc">Advisory sessions for startups and SMEs on building a solid data foundation — tool selection, architecture decisions, governance roadmaps, and actionable data strategies that scale.</p>
        <div class="serv-pills">
          <span class="serv-pill">Strategy Sessions</span>
          <span class="serv-pill">Tool Selection</span>
          <span class="serv-pill">Architecture Review</span>
          <span class="serv-pill">Roadmapping</span>
        </div>
      </div>

    </div>

    <div class="serv-cta">
      <div>
        <p class="serv-cta-label">Ready to work together?</p>
        <p class="serv-cta-title">Let's build something great with your data.</p>
        <p class="serv-cta-sub">Available for freelance projects, consulting engagements, and training sessions.</p>
      </div>
      <a href="#contact" class="btn-primary" style="white-space:nowrap;flex-shrink:0">Get a Free Consultation</a>
    </div>

  </div>
</section>

<!-- RECOMMENDATIONS -->
<section class="recs-bg" id="recommendations">
  <div class="section-inner">
    <p class="section-label">Social Proof</p>
    <h2 class="section-title">What Colleagues Say</h2>
    <div class="recs-grid">

      <div class="rec-card"><div class="rec-quote">"</div><p class="rec-text">I had the pleasure of working with Mohamed Magdy at Ejada. Mohamed consistently demonstrated exceptional skills in data management, efficiently driving projects and improving team productivity.</p><div class="rec-author"><div class="rec-avatar">ME</div><div><div class="rec-name">Moustafa El-Alfy</div><div class="rec-role">Data Governance Team Lead &amp; Technical Project Manager, Ejada · Managed Mohamed directly</div></div></div></div>

      <div class="rec-card"><div class="rec-quote">"</div><p class="rec-text">I had the pleasure of partnering with Mohamed Magdy on the MicroStrategy integration project, and he was easily one of the strongest contributors on the team. His technical depth across SQL, Python, and DAX modeling is genuinely impressive — he handled complex data logic with the kind of rigor that saves a project weeks of rework. What sets him apart is that he pairs that technical skill with real business sense: he listens to stakeholders, translates fuzzy requirements into clean deliverables, and pushes back thoughtfully when something doesn't make sense. Any data team would be lucky to have him.</p><div class="rec-author"><div class="rec-avatar">SG</div><div><div class="rec-name">Samer Girgis</div><div class="rec-role">Deputy General Manager (DGM) – Head of Data Management &amp; Analysis, Banque du Caire · Managed Mohamed directly</div></div></div></div>

      <div class="rec-card"><div class="rec-quote">"</div><p class="rec-text">Mohamed has consistently demonstrated great potential and a strong aptitude for excelling in this field. One of his standout qualities is his eagerness to learn and continuously enhance his knowledge of BI tools and technologies. He takes initiative in exploring new approaches and applies his learning effectively to deliver impactful results. He is a valuable asset to any team or company.</p><div class="rec-author"><div class="rec-avatar">MK</div><div><div class="rec-name">Moustafa Khafagy</div><div class="rec-role">Senior Sales Account Manager, IME · Managed Mohamed directly</div></div></div></div>

      <div class="rec-card"><div class="rec-quote">"</div><p class="rec-text">Magdy's prowess in data analytics has been instrumental in several of our most successful projects. He has an innate ability to sieve through enormous sets of data, extract meaningful insights, and translate these insights into actionable strategies. His exceptional skills in Python and SQL, combined with his adaptability to evolving technologies, place him at the forefront of the field. Beyond his technical skills, what truly sets Magdy apart is his interpersonal communication and his support to all those surrounding him — he naturally assumes mentoring roles, guiding junior staff with patience and expertise.</p><div class="rec-author"><div class="rec-avatar">RF</div><div><div class="rec-name">Rania Fawzy</div><div class="rec-role">Data Science Lead, QNB Egypt · Senior colleague</div></div></div></div>

      <div class="rec-card"><div class="rec-quote">"</div><p class="rec-text">I highly recommend Mohamed, who has been a key asset to our team as a BI Developer. He has demonstrated excellent skills in data preparation, analysis, reporting, and delivering high-quality solutions. He is a proactive problem solver who translates complex data into valuable business insights. His ability to collaborate effectively and meet tight deadlines while maintaining quality is exceptional. I'm confident he will continue to excel and add value in any future role.</p><div class="rec-author"><div class="rec-avatar">AS</div><div><div class="rec-name">Ahmed Salah</div><div class="rec-role">Head of Data Management &amp; Analytics, Banque du Caire · Managed Mohamed directly</div></div></div></div>

      <div class="rec-card"><div class="rec-quote">"</div><p class="rec-text">Mohamed Magdy is an excellent, dedicated candidate — very knowledgeable and supportive, honest and a problem solver. I recommend him to any organisation; he will add great value.</p><div class="rec-author"><div class="rec-avatar">WW</div><div><div class="rec-name">Walid Wafaie</div><div class="rec-role">Group HR Director, TAQA Gas · DBA, PHR · Managed Mohamed directly</div></div></div></div>

      <div class="rec-card"><div class="rec-quote">"</div><p class="rec-text">I worked closely with Mohamed on a business case during the hiring process and he showed exceptional performance. Being skillful, organized, attentive to details and having a very good business understanding, he delivered outstanding work.</p><div class="rec-author"><div class="rec-avatar">AM</div><div><div class="rec-name">Ahmed Mubarak</div><div class="rec-role">MBA | Strategy &amp; Analytics Manager, London Cab Egypt · Senior colleague</div></div></div></div>

      <div class="rec-card"><div class="rec-quote">"</div><p class="rec-text">Mohamed is such a genius person and really dedicated to his work — it was a pleasure working with him.</p><div class="rec-author"><div class="rec-avatar">AB</div><div><div class="rec-name">Ahmed Badr, MBA</div><div class="rec-role">Total Rewards &amp; Development Manager, TAQA Gas · Same team</div></div></div></div>

      <div class="rec-card"><div class="rec-quote">"</div><p class="rec-text">Mohamed is such a committed and dedicated programmer — helped me reach specific outcomes with a genius solution.</p><div class="rec-author"><div class="rec-avatar">AT</div><div><div class="rec-name">Ahmed El-Taher</div><div class="rec-role">Group HR Supervisor – Compensation &amp; Benefits, TAQA Gas · Same team</div></div></div></div>

    </div>
  </div>
</section>

<!-- CONTACT -->
<section class="contact-bg" id="contact">
  <div class="section-inner">
    <p class="section-label" style="color:var(--accent)">Let's Connect</p>
    <div class="contact-grid">
      <div>
        <h2 class="section-title">Open to Opportunities &amp; Consulting</h2>
        <p class="contact-desc">Whether you're hiring for a BI/data role, need a data governance consultant, or want to explore a project collaboration — I'd love to hear from you.</p>
        <div class="contact-links">
          <a class="contact-link" href="mailto:mohamedmagdy142000@gmail.com">
            <div class="contact-link-icon"><svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"/><polyline points="22,6 12,13 2,6"/></svg></div>
            mohamedmagdy142000@gmail.com
          </a>
          <a class="contact-link" href="tel:+966511946051">
            <div class="contact-link-icon"><svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><path d="M22 16.92v3a2 2 0 01-2.18 2 19.79 19.79 0 01-8.63-3.07A19.5 19.5 0 013.07 10.8 19.79 19.79 0 01.1 2.18a2 2 0 012-2.18h3a2 2 0 012 1.72c.127.96.361 1.903.7 2.81a2 2 0 01-.45 2.11L6.91 7.91a16 16 0 006.06 6.06l1.27-1.27a2 2 0 012.11-.45c.907.339 1.85.573 2.81.7a2 2 0 011.72 2.02z"/></svg></div>
            +966 511 946 051 (KSA) &nbsp;·&nbsp; +20 115 452 4570 (EG)
          </a>
          <a class="contact-link" href="https://www.linkedin.com/in/mohamed-magdy-192413197" target="_blank" rel="noopener">
            <div class="contact-link-icon"><svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><path d="M16 8a6 6 0 016 6v7h-4v-7a2 2 0 00-2-2 2 2 0 00-2 2v7h-4v-7a6 6 0 016-6z"/><rect x="2" y="9" width="4" height="12"/><circle cx="4" cy="4" r="2"/></svg></div>
            linkedin.com/in/mohamed-magdy-192413197
          </a>
          <a class="contact-link" href="https://github.com/mohamed-cs" target="_blank" rel="noopener">
            <div class="contact-link-icon"><svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 00-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0020 4.77 5.07 5.07 0 0019.91 1S18.73.65 16 2.48a13.38 13.38 0 00-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 005 4.77a5.44 5.44 0 00-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 009 18.13V22"/></svg></div>
            github.com/mohamed-cs
          </a>
        </div>
      </div>
      <div>
        <form class="contact-form" id="contact-form" action="https://formspree.io/f/xvzdanpk" method="POST">
          <input type="text" name="name" placeholder="Your name" required/>
          <input type="email" name="email" placeholder="Your email" required/>
          <input type="text" name="subject" placeholder="Subject — role, project, or consulting inquiry"/>
          <textarea name="message" placeholder="Tell me about the opportunity or project..."></textarea>
          <button class="btn-send" type="submit">Send Message</button>
          <p id="form-status" style="display:none;margin-top:12px"></p>
        </form>
      </div>
    </div>
  </div>
</section>

<footer>
  <div class="footer-logo">Mohamed <span>Magdy</span></div>
  <p>© 2026 · Senior BI &amp; Data Governance Professional · Cairo, Egypt</p>
</footer>

<script>
  const form = document.getElementById('contact-form');
  const status = document.getElementById('form-status');
  form.addEventListener('submit', async (e) => {
    e.preventDefault();
    const data = new FormData(form);
    try {
      const res = await fetch(form.action, {method:'POST',body:data,headers:{'Accept':'application/json'}});
      if (res.ok) {
        status.textContent = "✅ Message sent! I'll get back to you soon.";
        status.style.color = 'green';
        form.reset();
      } else {
        status.textContent = "❌ Something went wrong. Please try again.";
        status.style.color = 'red';
      }
    } catch {
      status.textContent = "❌ Network error. Please try again.";
      status.style.color = 'red';
    }
    status.style.display = 'block';
  });
</script>
</body>
</html>
