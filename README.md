<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>SM INFRATECH — Premium Civil Construction</title>
  <meta name="description" content="SM INFRATECH — Premium building & civil works: RCC, bungalows, renovation, waterproofing & road works. Proprietor: Suyash Salgaonkar. Kudal, Sindhudurg." />
  <meta name="theme-color" content="#071326" />
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700;800&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg:#f6f8fb;
      --dark:#071326;
      --card:#0f1724;
      --accent:#f59e0b;
      --muted:#6b7280;
      --radius-lg:18px;
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      font-family:Inter,system-ui,-apple-system,"Segoe UI",Roboto,Arial;
      background:linear-gradient(180deg,#f6f8fb 0%, #ffffff 60%);
      color:var(--dark);
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      line-height:1.45;
    }
    a{color:inherit}
    .wrap{max-width:1200px;margin:0 auto;padding:22px}

    /* Header */
    header{
      position:sticky; top:14px; z-index:60;
      display:flex;align-items:center;justify-content:space-between;gap:10px;
      background:linear-gradient(90deg, rgba(255,255,255,0.7), rgba(255,255,255,0.35));
      backdrop-filter: blur(6px) saturate(120%);
      padding:10px; border-radius:14px;
      box-shadow: 0 10px 30px rgba(7,19,38,0.06);
    }
    .brand{display:flex;gap:12px;align-items:center}
    .logo-box{
      width:64px;height:64px;border-radius:12px;background:linear-gradient(180deg,var(--card),#071326);display:flex;align-items:center;justify-content:center;
      box-shadow:inset 0 -8px 18px rgba(0,0,0,0.35);
    }
    .brand-title h1{margin:0;font-size:18px;color:#fff;letter-spacing:0.3px}
    .brand-title p{margin:0;font-size:12px;color:rgba(255,255,255,0.85)}

    .nav-links{display:flex;gap:10px;align-items:center}
    .nav-links a{font-weight:600;padding:8px 12px;border-radius:10px;text-decoration:none}
    .nav-links a:hover{background:rgba(7,19,38,0.04)}
    .btn-primary{background:var(--accent);color:var(--card);font-weight:700;padding:10px 14px;border-radius:12px;border:none;cursor:pointer}

    /* Hero */
    .hero{
      display:flex;gap:18px;align-items:stretch;margin-top:18px;
      background:linear-gradient(90deg,#071326,#0f2a42);
      border-radius:var(--radius-lg);
      color:white;overflow:hidden;box-shadow:0 18px 60px rgba(7,19,38,0.18)
    }
    .hero-left{flex:1;padding:36px}
    .kicker{display:inline-block;background:rgba(245,158,11,0.12);color:var(--accent);padding:6px 10px;border-radius:999px;font-weight:700;font-size:13px}
    .hero h2{margin:18px 0 8px;font-size:34px;line-height:1.03;letter-spacing:-0.5px}
    .hero p{color:rgba(255,255,255,0.85);max-width:58ch}
    .hero-actions{margin-top:18px;display:flex;gap:12px;flex-wrap:wrap}
    .hero-right{flex-basis:420px;background:linear-gradient(180deg, rgba(255,255,255,0.03), rgba(255,255,255,0.02));display:flex;align-items:center;justify-content:center;padding:10px}
    .hero-media{width:100%;height:100%;max-height:420px;object-fit:cover;border-left:1px solid rgba(255,255,255,0.04)}

    /* Stats */
    .stats{display:grid;grid-template-columns:repeat(3,1fr);gap:12px;margin-top:-26px}
    .stat{background:white;border-radius:12px;padding:18px;box-shadow:0 12px 30px rgba(7,19,38,0.06);text-align:center}
    .stat h3{margin:0;font-size:22px;color:var(--dark)}
    .stat p{margin:6px 0 0;color:var(--muted);font-size:13px}

    /* Services */
    section{margin-top:24px}
    .section-head{display:flex;align-items:center;justify-content:space-between;gap:10px;margin-bottom:12px}
    .section-head h2{margin:0;font-size:20px}
    .section-head p{margin:0;color:var(--muted)}
    .services-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:14px}
    .service-card{background:white;border-radius:12px;padding:16px;border:1px solid rgba(7,19,38,0.03);box-shadow:0 10px 26px rgba(7,19,38,0.04);text-align:center}
    .service-card svg{width:56px;height:56px;margin-bottom:10px}
    .service-card h4{margin:6px 0 0;font-size:16px}
    .service-card p{margin:8px 0 0;color:var(--muted);font-size:14px}

    /* Carousel */
    .carousel{position:relative;overflow:hidden;border-radius:12px}
    .slides{display:flex;gap:12px;transition:transform .5s cubic-bezier(.22,.9,.3,1);padding:16px}
    .slide{min-width:260px;background:white;border-radius:12px;overflow:hidden;box-shadow:0 10px 30px rgba(7,19,38,0.06)}
    .slide img{width:100%;height:180px;object-fit:cover}
    .control{position:absolute;top:50%;transform:translateY(-50%);pointer-events:auto;border-radius:999px;background:rgba(7,19,38,0.6);color:white;border:none;padding:8px;cursor:pointer}
    .control.left{left:8px} .control.right{right:8px}

    /* Modal */
    .modal{position:fixed;inset:0;display:none;align-items:center;justify-content:center;background:rgba(2,6,23,0.75);z-index:120}
    .modal.show{display:flex}
    .modal img{max-width:95%;max-height:90%;border-radius:10px;box-shadow:0 30px 60px rgba(0,0,0,0.6)}

    /* Contact */
    .grid-2{display:grid;grid-template-columns:1fr 380px;gap:16px}
    .card{background:white;border-radius:12px;padding:16px;border:1px solid rgba(7,19,38,0.03);box-shadow:0 12px 30px rgba(7,19,38,0.04)}
    .field{display:flex;flex-direction:column;margin-bottom:10px}
    .field label{font-size:13px;margin-bottom:6px;color:var(--dark)}
    .field input, .field textarea{padding:10px;border-radius:8px;border:1px solid rgba(7,19,38,0.06);font-size:15px}
    .submit{background:var(--accent);border:none;padding:12px;border-radius:10px;font-weight:800;cursor:pointer;width:100%}
    .small-muted{font-size:13px;color:var(--muted)}

    .float-wa{position:fixed;right:18px;bottom:18px;background:#25D366;color:white;padding:12px 14px;border-radius:999px;display:flex;gap:10px;align-items:center;z-index:120;box-shadow:0 14px 40px rgba(37,211,102,0.12)}

    footer{margin-top:30px;text-align:center;color:var(--muted);font-size:14px;padding:18px}

    @media(min-width:1000px){ /* show desktop nav if wide */ }
    @media(max-width:980px){
      .wrap{padding:16px}
      .grid-2{grid-template-columns:1fr}
      .hero{flex-direction:column}
      .hero-right{display:none}
      .stats{grid-template-columns:repeat(1,1fr)}
    }

    /* premium header text improvement */
    .brand-title h1 { color: gold; font-weight:800; text-shadow: 0 4px 18px rgba(0,0,0,0.45); }
  </style>
</head>
<body>
  <div class="wrap" role="document">
    <!-- HEADER -->
    <header role="banner" aria-label="SM INFRATECH header">
      <div class="brand" aria-hidden="false">
        <div class="logo-box" role="img" aria-label="SM INFRATECH logo">
          <!-- Inline premium building SVG -->
          <svg width="48" height="48" viewBox="0 0 64 64" fill="none" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
            <rect width="64" height="64" rx="12" fill="#071326"/>
            <path d="M14 48h36v6H14z" fill="#f59e0b"/>
            <g stroke="#fff" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
              <path d="M20 46V26h8v20"/>
              <path d="M32 46V18h8v28"/>
              <path d="M44 46V30h4v16"/>
              <path d="M12 32h40"/>
            </g>
          </svg>
        </div>
        <div class="brand-title">
          <h1>SM INFRATECH</h1>
          <p style="margin-top:4px;color:#cbd5e1;font-size:12px">Proprietor: Suyash Salgaonkar</p>
        </div>
      </div>

      <nav class="desktop" aria-label="Primary">
        <div class="nav-links" role="navigation">
          <a href="#services">Services</a>
          <a href="#projects">Projects</a>
          <a href="#contact">Contact</a>
          <button class="btn-primary" onclick="document.querySelector('#contact')?.scrollIntoView({behavior:'smooth'})">Get Quote</button>
        </div>
      </nav>
    </header>

    <!-- HERO -->
    <section class="hero" role="region" aria-label="Hero section">
      <div class="hero-left">
        <span class="kicker">Trusted Contractor • Sindhudurg</span>
        <h2><span id="typeTarget">We build strong & lasting structures</span></h2>
        <p>SM INFRATECH delivers premium civil contracting: RCC frames, bungalows, renovation, waterproofing and road works — with clear BOQ, experienced supervision and on-time delivery.</p>

        <div class="hero-actions">
          <a class="btn-primary" href="#contact">Request Quote</a>
          <a class="btn-primary" style="background:transparent;color:white;border:1px solid rgba(255,255,255,0.12)" href="#projects">See Projects</a>
        </div>

        <div class="stats" aria-hidden="false">
          <div class="stat"><h3 id="c1">0+</h3><p>Projects Completed</p></div>
          <div class="stat"><h3 id="c2">0</h3><p>Expert Team</p></div>
          <div class="stat"><h3 id="c3">0</h3><p>Years Combined</p></div>
        </div>
      </div>

      <div class="hero-right" aria-hidden="true">
        <img class="hero-media" src="https://images.unsplash.com/photo-1454165804606-c3d57bc86b40?q=80&w=1400&auto=format&fit=crop" alt="Construction site with crane and building">
      </div>
    </section>

    <!-- SERVICES -->
    <section id="services" aria-labelledby="services-head">
      <div class="section-head">
        <div>
          <h2 id="services-head">Our Services</h2>
          <p class="small-muted">End-to-end contracting: design, BOQ, execution, finishing & maintenance.</p>
        </div>
        <div class="small-muted">Contact for custom packages</div>
      </div>

      <div class="services-grid" role="list">
        <article class="service-card" role="listitem">
          <svg viewBox="0 0 24 24" fill="none" aria-hidden="true"><rect width="24" height="24" rx="4" fill="#fff"/><path d="M6 15V9h12v6" stroke="#0b1220" stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round"/></svg>
          <h4>Building Construction</h4>
          <p>Turnkey RCC frames, masonry & complete finishes.</p>
        </article>

        <article class="service-card" role="listitem">
          <svg viewBox="0 0 24 24" fill="none" aria-hidden="true"><rect width="24" height="24" rx="4" fill="#fff"/><path d="M4 20h16" stroke="#0b1220" stroke-width="1.6" stroke-linecap="round"/></svg>
          <h4>Bungalows & Villas</h4>
          <p>Vastu-aligned planning, premium finishes & site supervision.</p>
        </article>

        <article class="service-card" role="listitem">
          <svg viewBox="0 0 24 24" fill="none" aria-hidden="true"><rect width="24" height="24" rx="4" fill="#fff"/><path d="M6 12h12" stroke="#0b1220" stroke-width="1.6" stroke-linecap="round"/></svg>
          <h4>RCC Works</h4>
          <p>Beams, slabs, columns, shuttering & steel schedules.</p>
        </article>

        <article class="service-card" role="listitem">
          <svg viewBox="0 0 24 24" fill="none" aria-hidden="true"><rect width="24" height="24" rx="4" fill="#fff"/><path d="M12 4v16" stroke="#0b1220" stroke-width="1.6" stroke-linecap="round"/></svg>
          <h4>Renovation</h4>
          <p>Structural repairs, plastering, tiling & interior upgrades.</p>
        </article>

        <article class="service-card" role="listitem">
          <svg viewBox="0 0 24 24" fill="none" aria-hidden="true"><rect width="24" height="24" rx="4" fill="#fff"/><path d="M6 15h12" stroke="#0b1220" stroke-width="1.6" stroke-linecap="round"/></svg>
          <h4>Waterproofing</h4>
          <p>Terrace membranes, bathroom & basement solutions.</p>
        </article>

        <article class="service-card" role="listitem">
          <svg viewBox="0 0 24 24" fill="none" aria-hidden="true"><rect width="24" height="24" rx="4" fill="#fff"/><path d="M3 12h18" stroke="#0b1220" stroke-width="1.6" stroke-linecap="round"/></svg>
          <h4>Road Works</h4>
          <p>WBM, BT surfacing and small drainage works.</p>
        </article>
      </div>
    </section>

    <!-- PROJECTS -->
    <section id="projects" aria-labelledby="projects-head">
      <div class="section-head">
        <div>
          <h2 id="projects-head">Recent Projects</h2>
          <p class="small-muted">Real site images — replace these placeholders with your photos for the final site.</p>
        </div>
        <div>
          <button class="btn-primary" onclick="openGallery(0)">Open Gallery</button>
        </div>
      </div>

      <div class="carousel" aria-roledescription="carousel" tabindex="0">
        <div style="position:absolute;inset:0;pointer-events:none">
          <button class="control left" aria-label="Previous" onclick="slideLeft()">❮</button>
          <button class="control right" aria-label="Next" onclick="slideRight()">❯</button>
        </div>
        <div class="slides" id="slides">
          <article class="slide"><img src="https://images.unsplash.com/photo-1503387762-592deb58ef4e?q=80&w=1200&auto=format&fit=crop" alt="RCC site"><div class="meta" style="padding:12px"><strong>Residential RCC Frame</strong><p class="small-muted">Sindhudurg</p></div></article>
          <article class="slide"><img src="https://images.unsplash.com/photo-1494526585095-c41746248156?q=80&w=1200&auto=format&fit=crop" alt="Villa"><div class="meta" style="padding:12px"><strong>Luxury Villa Exterior</strong><p class="small-muted">Vastu-aligned finishing</p></div></article>
          <article class="slide"><img src="https://images.unsplash.com/photo-1454165804606-c3d57bc86b40?q=80&w=1200&auto=format&fit=crop" alt="Interior"><div class="meta" style="padding:12px"><strong>Interior Renovation</strong><p class="small-muted">Kitchen & tile upgrades</p></div></article>
          <article class="slide"><img src="https://images.unsplash.com/photo-1581091215367-59ab6b66d85f?q=80&w=1200&auto=format&fit=crop" alt="Road"><div class="meta" style="padding:12px"><strong>Road & Drainage</strong><p class="small-muted">WBM + BT surfacing</p></div></article>
        </div>
      </div>
    </section>

    <!-- GALLERY MODAL -->
    <div class="modal" id="modal" role="dialog" aria-modal="true" aria-label="Project photo">
      <button id="closeModal" aria-label="Close gallery" style="position:absolute;top:28px;right:28px;border:none;background:transparent;color:white;font-size:20px;cursor:pointer">✕</button>
      <img id="modalImg" src="" alt="Project large photo">
    </div>

    <!-- CONTACT -->
    <section id="contact" aria-labelledby="contact-head">
      <div class="section-head">
        <div>
          <h2 id="contact-head">Contact & Quick Quote</h2>
          <p class="small-muted">Call or WhatsApp for quick replies — or fill the form and we'll respond within 24 hours.</p>
        </div>
        <div class="small-muted">Phone: +91 74208 97311</div>
      </div>

      <div class="grid-2">
        <div>
          <div class="card">
            <h3>SM INFRATECH</h3>
            <p class="small-muted">Proprietor: <strong>Suyash Salgaonkar</strong></p>
            <p style="margin-top:8px"><strong>Phone:</strong> <a href="tel:+917420897311">+91 74208 97311</a></p>
            <p style="margin-top:6px"><strong>Email:</strong> <a href="mailto:allianceacuity@gmail.com">allianceacuity@gmail.com</a></p>
            <p style="margin-top:6px"><strong>Address:</strong> At Post Kudal, Sindhudurg, Maharashtra — 416520</p>
            <div style="margin-top:12px;display:flex;gap:10px">
              <a class="btn-primary" href="https://wa.me/917420897311?text=Hi%20SM%20INFRATECH%2C%20I%20need%20a%20quote" target="_blank" rel="noopener">WhatsApp</a>
              <a class="btn-primary" style="background:transparent;color:var(--dark);border:1px solid rgba(7,19,38,0.06)" href="#projects">View Projects</a>
            </div>
          </div>

          <div style="margin-top:12px" class="card">
            <h4>Why choose SM INFRATECH?</h4>
            <ul style="margin:8px 0 0;padding-left:18px;color:var(--muted)">
              <li>Clear BOQ & accurate estimates</li>
              <li>Experienced site supervision</li>
              <li>Quality materials & timely completion</li>
            </ul>
          </div>
        </div>

        <form id="quote" class="card" name="quote" onsubmit="return handleForm(event)" method="POST" data-netlify="true" netlify-honeypot="bot-field">
          <input type="hidden" name="form-name" value="quote">
          <p style="display:none"><label>Don’t fill if human: <input name="bot-field"></label></p>

          <h3>Request a Quote</h3>
          <div class="field"><label for="qname">Your Name</label><input id="qname" name="name" required placeholder="e.g., Rahul Patil"></div>
          <div class="field"><label for="qphone">Phone</label><input id="qphone" name="phone" required placeholder="+91 98xxxx"></div>
          <div class="field"><label for="qdetails">Project Details</label><textarea id="qdetails" name="details" placeholder="Location, area (sqft), work type, desired timeline"></textarea></div>

          <div style="display:flex;gap:8px">
            <button class="submit" type="submit">Send via WhatsApp</button>
            <button class="btn-primary" type="button" onclick="copyExample()" style="background:transparent;color:var(--dark);border:1px solid rgba(7,19,38,0.06)">Copy Example</button>
          </div>

          <p id="formMsg" class="small-muted" style="margin-top:10px;display:none"></p>
        </form>
      </div>
    </section>

    <footer role="contentinfo">© <span id="year"></span> SM INFRATECH • Built with care in Kudal • All rights reserved</footer>
  </div>

  <!-- Floating WhatsApp -->
  <a class="float-wa" href="https://wa.me/917420897311?text=Hi%20SM%20INFRATECH%2C%20I%20need%20a%20quote" target="_blank" rel="noopener" aria-label="Chat on WhatsApp">
    <svg width="20" height="20" viewBox="0 0 24 24" fill="none" aria-hidden="true" xmlns="http://www.w3.org/2000/svg">
      <path d="M20.52 3.478A11.915 11.915 0 0012 0C5.373 0 .02 5.354 0 11.98-.04 15.05.98 17.98 3.18 20.29L0 24l3.76-1.02A11.96 11.96 0 0012 24c6.627 0 12-5.373 12-12 0-3.2-1.23-6.2-3.48-8.522z" fill="#25D366"/>
      <path d="M17.47 14.04c-.31-.16-1.82-.9-2.1-1-.28-.11-.48-.16-.68.16-.19.31-.74 1-.9 1.21-.16.21-.32.25-.62.09-.31-.16-1.31-.48-2.49-1.53-.92-.82-1.54-1.83-1.72-2.14-.18-.31 0-.48.13-.64.13-.16.31-.42.47-.63.16-.21.21-.36.31-.6.1-.24.05-.44-.03-.63-.08-.19-.68-1.64-.93-2.22-.24-.58-.49-.5-.67-.51-.17 0-.36-.01-.55-.01-.19 0-.5.07-.76.36-.26.28-1 1-1 2.44 0 1.44.93 2.86 1.06 3.07.13.21 1.86 2.86 4.5 3.9 2.64 1.05 2.64.7 3.12.66.48-.05 1.56-.64 1.78-1.26.22-.62.22-1.15.16-1.27-.06-.12-.3-.2-.61-.36z" fill="#fff"/>
    </svg>
    WhatsApp
  </a>

  <script>
    document.getElementById('year').textContent = new Date().getFullYear();

    // Counters
    const counters = [{id:'c1',to:24},{id:'c2',to:8},{id:'c3',to:14}];
    function animateCounters(){
      counters.forEach(c=>{
        const el=document.getElementById(c.id);
        if(!el) return;
        let start=0, end=c.to, step=Math.ceil(end/30);
        const t=setInterval(()=>{
          start+=step;
          if(start>=end){ el.textContent = end + (c.id==='c1'?'+':''); clearInterval(t); }
          else el.textContent = start + (c.id==='c1'?'+':'');
        },40);
      });
    }
    const statEl=document.querySelector('.stats');
    if(statEl){
      const io=new IntersectionObserver((entries,ob)=>{
        entries.forEach(e=>{ if(e.isIntersecting){ animateCounters(); ob.disconnect(); }});
      },{threshold:.3});
      io.observe(statEl);
    }

    // Typewriter
    (function(){
      const el=document.getElementById('typeTarget');
      if(!el) return;
      const phrases=['We build strong & lasting structures','Precision. Transparency. Timely delivery','RCC, Bungalows, Renovation & Roadworks'];
      let i=0,j=0,forward=true;
      function step(){
        const full=phrases[i];
        el.textContent=full.slice(0,j);
        if(forward){ j++; if(j>full.length){ forward=false; setTimeout(step,1000); return; } }
        else { j--; if(j===0){ forward=true; i=(i+1)%phrases.length; } }
        setTimeout(step, forward?40:20);
      }
      step();
    })();

    // Carousel
    const slides=document.getElementById('slides'); let idx=0;
    function updateSlides(){ const width=slides.children[0].offsetWidth + 12; slides.style.transform=`translateX(-${idx*width}px)`;}
    function slideRight(){ idx = Math.min(idx + 1, slides.children.length - 1); updateSlides(); }
    function slideLeft(){ idx = Math.max(idx - 1, 0); updateSlides(); }
    window.addEventListener('resize', updateSlides);

    // Touch swipe
    (function(){
      let startX=0, startTime=0;
      slides.addEventListener('touchstart', e=>{ startX=e.touches[0].clientX; startTime=Date.now();});
      slides.addEventListener('touchend', e=>{
        const dx = e.changedTouches[0].clientX - startX; const dt = Date.now() - startTime;
        if(Math.abs(dx)>40 && dt<600){ if(dx<0) slideRight(); else slideLeft(); }
      });
    })();

    // Modal gallery
    const modal=document.getElementById('modal'), modalImg=document.getElementById('modalImg');
    function openGallery(startIndex=0){
      const imgs = Array.from(document.querySelectorAll('.slide img')).map(i=>i.src);
      modalImg.src = imgs[startIndex] || imgs[0];
      modal.classList.add('show');
    }
    document.getElementById('closeModal')?.addEventListener('click', ()=> modal.classList.remove('show'));
    modal.addEventListener('click', e=>{ if(e.target===modal) modal.classList.remove('show'); });

    // Form handler: open WhatsApp then fallback to mailto
    function handleForm(ev){
      ev.preventDefault();
      const name=encodeURIComponent(document.getElementById('qname').value.trim());
      const phone=encodeURIComponent(document.getElementById('qphone').value.trim());
      const details=encodeURIComponent(document.getElementById('qdetails').value.trim());
      if(!name||!phone){ alert('Please enter name and phone.'); return false; }
      const text=`Website%20Enquiry%0AName:%20${name}%0APhone:%20${phone}%0ADetails:%20${details}`;
      window.open(`https://wa.me/917420897311?text=${text}`,'_blank');
      document.getElementById('formMsg').style.display='block';
      document.getElementById('formMsg').textContent='Opening WhatsApp... if it did not open, an email will be prepared.';
      setTimeout(()=>{ location.href = `mailto:allianceacuity@gmail.com?subject=Quote%20Request&body=${text}`; }, 1100);
      return false;
    }

    // copy example helper
    function copyExample(){ const sample = `Name: Suyash Salgaonkar\nPhone: +91 7420897311\nDetails: 3BHK bungalow, area 1200 sqft, location Kudal.`; navigator.clipboard?.writeText(sample).then(()=> alert('Sample copied.')); }

    // initial adjust
    updateSlides();
  </script>
</body>
</html>
