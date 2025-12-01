
-->

<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <meta name="description" content="UX product designer portfolio — case studies, process and contact." />
  <title>UX Portfolio — Your Name</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;800&display=swap" rel="stylesheet">
  <style>
    /* Modern minimal portfolio CSS — responsive and accessible */
    :root{
      --bg:#0f1724; --card:#0b1220; --muted:#94a3b8; --accent:#7c3aed; --glass:rgba(255,255,255,0.03);
      --radius:14px; font-family:Inter, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;
      color-scheme: dark;
    }
    *{box-sizing:border-box}
    html,body{height:100%;margin:0;background:linear-gradient(180deg,var(--bg),#061022);color:#e6eef8}
    a{color:inherit}
    .container{max-width:1100px;margin:36px auto;padding:24px}

    header{display:flex;gap:16px;align-items:center;justify-content:space-between}
    .brand{display:flex;gap:16px;align-items:center}
    .logo{width:54px;height:54px;border-radius:12px;background:linear-gradient(135deg,var(--accent),#3b82f6);display:grid;place-items:center;font-weight:800}
    h1{font-size:22px;margin:0}
    p.lead{margin:4px 0 0;color:var(--muted);font-size:14px}

    .grid{display:grid;grid-template-columns:1fr 340px;gap:24px;margin-top:28px}
    main{padding:20px;background:linear-gradient(180deg,rgba(255,255,255,0.02),transparent);border-radius:16px}
    aside{padding:20px;background:linear-gradient(180deg,rgba(255,255,255,0.01),transparent);border-radius:16px;height:fit-content}

    /* Projects list */
    .projects{display:grid;grid-template-columns:repeat(auto-fit,minmax(260px,1fr));gap:16px}
    .card{background:var(--card);padding:14px;border-radius:12px;box-shadow:0 6px 18px rgba(2,6,23,0.6);transition:transform .18s ease}
    .card:hover{transform:translateY(-6px)}
    .thumb{height:140px;border-radius:10px;overflow:hidden;display:block;margin-bottom:12px;background:linear-gradient(180deg,#021124, #06213a);display:grid;place-items:center}
    .card h3{margin:0 0 6px;font-size:16px}
    .card p{margin:0;color:var(--muted);font-size:13px}

    /* About */
    .about h2{margin-top:0}
    .skills{display:flex;flex-wrap:wrap;gap:8px;margin-top:8px}
    .chip{background:var(--glass);padding:8px 10px;border-radius:999px;font-size:13px;color:var(--muted)}

    /* Contact */
    .contact{margin-top:16px}
    .btn{display:inline-block;padding:10px 14px;border-radius:10px;background:linear-gradient(90deg,var(--accent),#3b82f6);text-decoration:none;color:white;font-weight:600}

    /* Modal */
    .modal{position:fixed;inset:0;display:none;align-items:center;justify-content:center;background:rgba(2,6,23,0.6);z-index:60}
    .modal.show{display:flex}
    .modal .sheet{width:min(920px,96%);max-height:86vh;overflow:auto;background:#071125;padding:20px;border-radius:12px}

    footer{margin-top:18px;text-align:center;color:var(--muted);font-size:13px}

    @media (max-width:880px){.grid{grid-template-columns:1fr}.brand h1{font-size:18px}.logo{width:44px;height:44px}}
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="brand">
        <div class="logo" aria-hidden>YN</div>
        <div>
          <h1 id="portfolio-title">Your Name — Product / UX Designer</h1>
          <p class="lead">I design simple, useful experiences — photography, research-driven design and product thinking.</p>
        </div>
      </div>
      <div>
        <a href="#contact" class="btn">Contact</a>
      </div>
    </header>

    <div class="grid">
      <main>
        <section aria-labelledby="projects-heading">
          <h2 id="projects-heading">Selected projects</h2>
          <p class="lead" style="margin-bottom:12px">Click a card to open a short case study and details.</p>

          <div class="projects" id="projects">

            <!-- PROJECT CARD TEMPLATE (duplicate for each project) -->
            <article class="card" tabindex="0" role="button" aria-pressed="false" data-title="Redesign: FinTrack" data-type="Case study" data-desc="A finance app redesign to improve onboarding and reduce drop-off by 32%." data-details='{"challenge":"High onboarding drop-off","role":"Lead UX","process":"Research → Wireframes → Prototyping → Testing","result":"32% reduction in drop-off"}'>
              <div class="thumb" aria-hidden>
                <!-- Placeholder SVG screenshot -->
                <svg width="100%" height="100%" viewBox="0 0 400 200" preserveAspectRatio="xMidYMid slice" xmlns="http://www.w3.org/2000/svg">
                  <rect width="100%" height="100%" fill="#071534"></rect>
                  <g fill="#0ea5a9" opacity="0.95"><rect x="18" y="28" width="120" height="16" rx="4"></rect><rect x="18" y="56" width="240" height="16" rx="4"></rect></g>
                </svg>
              </div>
              <h3>FinTrack — banking app</h3>
              <p>Onboarding redesign focused on clarity and trust. 6 week sprint.</p>
            </article>

            <article class="card" tabindex="0" role="button" aria-pressed="false" data-title="Research: EatRight" data-type="Research" data-desc="User research and prototype for a meal-planning product." data-details='{"challenge":"Low retention","role":"Researcher","process":"Interviews → Diary study → Prototype","result":"Actionable personas and flows"}'>
              <div class="thumb" aria-hidden>
                <svg width="100%" height="100%" viewBox="0 0 400 200" preserveAspectRatio="xMidYMid slice" xmlns="http://www.w3.org/2000/svg">
                  <rect width="100%" height="100%" fill="#071534"></rect>
                  <g fill="#f59e0b" opacity="0.95"><circle cx="80" cy="80" r="28"></circle><rect x="140" y="56" width="180" height="16" rx="6"></rect></g>
                </svg>
              </div>
              <h3>EatRight — meal-planner</h3>
              <p>Qualitative research that informed new personalization features.</p>
            </article>

            <article class="card" tabindex="0" role="button" aria-pressed="false" data-title="System: ShopFlow" data-type="Design system" data-desc="Design system and component library for an e-commerce platform." data-details='{"challenge":"Inconsistent UI","role":"Design system lead","process":"Inventory → Tokens → Components","result":"Faster development cycles"}'>
              <div class="thumb" aria-hidden>
                <svg width="100%" height="100%" viewBox="0 0 400 200" preserveAspectRatio="xMidYMid slice" xmlns="http://www.w3.org/2000/svg">
                  <rect width="100%" height="100%" fill="#071534"></rect>
                  <g fill="#60a5fa" opacity="0.95"><rect x="18" y="28" width="100" height="60" rx="6"></rect><rect x="140" y="40" width="220" height="12" rx="6"></rect></g>
                </svg>
              </div>
              <h3>ShopFlow — e‑commerce system</h3>
              <p>Design tokens, component library & documentation.</p>
            </article>

            <!-- Add more cards as needed -->

          </div>
        </section>

        <section class="about" aria-labelledby="about-heading" style="margin-top:22px">
          <h2 id="about-heading">About</h2>
          <p>I'm a product designer focused on research-led solutions, design systems and accessible interactions. I care about measurable outcomes and clear communication.</p>
          <div class="skills" aria-hidden>
            <span class="chip">User research</span>
            <span class="chip">Interaction design</span>
            <span class="chip">Prototyping</span>
            <span class="chip">Design systems</span>
            <span class="chip">Figma</span>
            <span class="chip">Accessibility</span>
          </div>
        </section>

      </main>

      <aside>
        <div style="display:flex;gap:12px;align-items:center;">
          <div style="width:68px;height:68px;border-radius:12px;background:linear-gradient(90deg,#15375b,#2a6f9e);display:grid;place-items:center;font-weight:800">YN</div>
          <div>
            <h3 style="margin:0">Your Name</h3>
            <p style="margin:4px 0 0;color:var(--muted);font-size:13px">Product Designer — based in Dublin</p>
          </div>
        </div>

        <div class="contact" id="contact">
          <h4 style="margin-top:16px">Contact</h4>
          <p style="margin:6px 0;color:var(--muted)">Email: <a href="mailto:you@domain.com">you@domain.com</a></p>
          <p style="margin:6px 0;color:var(--muted)">Resume: <a href="#" id="resume-link">Download (PDF)</a></p>
          <p style="margin:6px 0;color:var(--muted)">Or say hi on <a href="#">LinkedIn</a></p>
          <div style="margin-top:10px">
            <a class="btn" href="mailto:you@domain.com?subject=UX%20Portfolio%20enquiry">Say hello</a>
          </div>
        </div>

        <div style="margin-top:18px;color:var(--muted);font-size:13px">
          <strong>Availability</strong>
          <p style="margin:6px 0 0">Open to contract & full‑time roles.</p>
        </div>

      </aside>
    </div>

    <footer>
      Built with care — <span id="year"></span> • <a href="#" style="color:var(--muted);text-decoration:underline">Privacy</a>
    </footer>
  </div>

  <!-- Modal for case study -->
  <div class="modal" id="modal" role="dialog" aria-modal="true" aria-labelledby="modal-title">
    <div class="sheet" role="document">
      <button id="close-modal" aria-label="Close" style="float:right;background:none;border:none;color:var(--muted);font-size:18px">✕</button>
      <h2 id="modal-title">Project title</h2>
      <p id="modal-type" style="color:var(--muted)"></p>
      <p id="modal-desc"></p>
      <dl id="modal-details" style="color:var(--muted)"></dl>
    </div>
  </div>

  <script>
    // Small interactive bits
    document.getElementById('year').textContent = new Date().getFullYear();

    const cards = document.querySelectorAll('.card');
    const modal = document.getElementById('modal');
    const close = document.getElementById('close-modal');
    const mTitle = document.getElementById('modal-title');
    const mType = document.getElementById('modal-type');
    const mDesc = document.getElementById('modal-desc');
    const mDetails = document.getElementById('modal-details');

    function openCard(e){
      const el = e.currentTarget;
      const title = el.dataset.title || el.querySelector('h3').innerText;
      const type = el.dataset.type || '';
      const desc = el.dataset.desc || '';
      let details = {};
      try{ details = JSON.parse(el.dataset.details || '{}'); }catch(err){details={}};

      mTitle.textContent = title;
      mType.textContent = type;
      mDesc.textContent = desc;
      mDetails.innerHTML = '';
      for(const k in details){
        const dt = document.createElement('dt'); dt.textContent = k; dt.style.fontWeight='600';
        const dd = document.createElement('dd'); dd.textContent = details[k]; dd.style.margin='0 0 10px 0'; dd.style.color='var(--muted)';
        mDetails.appendChild(dt); mDetails.appendChild(dd);
      }
      modal.classList.add('show');
      modal.querySelector('.sheet').focus();
    }

    cards.forEach(card=>{
      card.addEventListener('click', openCard);
      card.addEventListener('keypress', (e)=>{ if(e.key==='Enter'||e.key===' ') openCard(e) });
    });

    close.addEventListener('click', ()=>modal.classList.remove('show'));
    modal.addEventListener('click', (e)=>{ if(e.target===modal) modal.classList.remove('show') });

    // Accessibility helpers
    // Ensure focus trap could be added; for brevity we keep modal simple but keyboard-operable
  </script>

  <!-- Local README (human-readable) -->
  <!--
  HOW TO DEPLOY (full commands - copy/paste into terminal)

  # in folder with index.html
  git init
  git add index.html
  git commit -m "Initial portfolio"
  git branch -M main
  git remote add origin https://github.com/<your-username>/ux-portfolio.git
  git push -u origin main

  # Then enable GitHub Pages in repo settings: choose Branch "main" and folder "/ (root)"
  # Or to use gh CLI:
  gh repo create <your-username>/ux-portfolio --public --source=. --remote=origin
  gh pages create --branch main --path /

  Customize: replace texts, add images, upload resume.pdf and change the link to ./assets/resume.pdf
  -->
</body>
</html>
