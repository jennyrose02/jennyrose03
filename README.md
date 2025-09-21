<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Jennyrose Jarabe — UX Designer</title>
  <style>
    :root{
      --bg:#f6f7fb;
      --card:#ffffff;
      --accent:#0b6cff;
      --muted:#6b7280;
      --text:#0f1724;
      --paper-padding:28px;
      --maxw:900px;
      font-family: Inter, ui-sans-serif, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
    }
    html,body{height:100%}
    body{
      margin:0;
      background:linear-gradient(180deg,var(--bg),#eef2ff 60%);
      color:var(--text);
      display:flex;
      align-items:center;
      justify-content:center;
      padding:28px;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
    }

    .container{
      width:100%;
      max-width:var(--maxw);
      background:var(--card);
      box-shadow:0 8px 30px rgba(16,24,40,0.08);
      border-radius:12px;
      overflow:hidden;
      display:grid;
      grid-template-columns: 320px 1fr;
      gap:0;
    }

    /* LEFT column */
    .left{
      background:linear-gradient(180deg,#fafbff,#f6f8ff);
      padding:var(--paper-padding);
      border-right:1px solid rgba(15,23,36,0.04);
      min-height:420px;
    }
    .photo {
      width:96px;height:96px;border-radius:12px;
      background:linear-gradient(135deg,var(--accent),#7c5cff);
      display:flex;align-items:center;justify-content:center;
      color:white;font-weight:700;font-size:28px;margin-bottom:14px;
      box-shadow:0 6px 18px rgba(11,108,255,0.12);
    }
    .name{
      font-size:20px;font-weight:700;letter-spacing:1px;margin-bottom:4px;
    }
    .title{color:var(--muted);font-weight:600;margin-bottom:18px;}

    .contact, .section{
      margin-top:12px;
      font-size:14px;
    }
    .contact-item{display:flex;gap:8px;align-items:center;color:var(--muted);margin-bottom:8px;}
    .contact-item strong{color:var(--text);font-weight:600;min-width:78px;display:inline-block;}

    .skills-list{
      display:flex;flex-direction:column;gap:8px;margin-top:8px;
    }
    .skill{
      font-weight:600;
    }
    .skill-sub{color:var(--muted);font-weight:500;font-size:13px;margin-top:4px}

    /* RIGHT column */
    .right{
      padding:var(--paper-padding);
    }
    .summary{
      margin-bottom:18px;font-size:15px;color:#0f1724;line-height:1.45;
    }

    .heading{
      display:flex;align-items:center;justify-content:space-between;margin-bottom:10px;
    }
    .heading h3{margin:0;font-size:16px;letter-spacing:0.4px}
    .job{
      padding:12px;border-radius:10px;margin-bottom:12px;border:1px solid rgba(15,23,36,0.04);
    }
    .job h4{margin:0;font-size:15px;}
    .job .meta{color:var(--muted);font-size:13px;margin-bottom:8px;}
    .job ul{margin:6px 0 0 18px;color:var(--muted);line-height:1.45}

    .education-item{margin-bottom:12px;}
    .education-item strong{display:block}

    /* print-friendly */
    @media print{
      body{background:white}
      .container{box-shadow:none;border-radius:0}
      .left{background:white}
    }

    /* responsive */
    @media (max-width:820px){
      .container{grid-template-columns:1fr;max-width:720px}
      .left{border-right:none;border-bottom:1px solid rgba(15,23,36,0.04)}
    }
  </style>
</head>
<body>
  <div class="container" role="document" aria-label="Resume — Jennyrose Jarabe">
    <aside class="left" aria-label="Personal details and skills">
      <div style="display:flex;gap:14px;align-items:center;">
        <div class="photo" aria-hidden="true">JJ</div>
        <div>
          <div class="name">Jennyrose Jarabe</div>
          <div class="title">UX Designer</div>
        </div>
      </div>

      <div class="contact">
        <div class="contact-item"><strong>Phone</strong> <span>09630543999</span></div>
        <div class="contact-item"><strong>Email</strong> <span>jennyrosejarabe1@gmail.com</span></div>
      </div>

      <div class="section" aria-labelledby="education-heading">
        <div id="education-heading" style="font-weight:700;margin-top:10px">Education</div>
        <div class="education-item">
          <strong>STI West Negros University</strong>
          <div class="meta" style="color:var(--muted);font-size:13px">2023 — 2027</div>
        </div>
        <div class="education-item">
          <strong>I-TECH College Bago City, INC</strong>
          <div class="meta" style="color:var(--muted);font-size:13px">2022 — 2023</div>
        </div>
      </div>

      <div class="section" aria-labelledby="skills-heading">
        <div id="skills-heading" style="font-weight:700;margin-top:6px">Skills</div>
        <div class="skills-list" style="margin-top:8px">
          <div class="skill">Information Architecture<div class="skill-sub">Site maps, content strategy</div></div>
          <div class="skill">Wireframing<div class="skill-sub">Lo-fi & hi-fi wireframes</div></div>
          <div class="skill">Prototyping<div class="skill-sub">Clickable prototypes & testing</div></div>
        </div>
      </div>
    </aside>

    <main class="right" aria-label="Experience and summary">
      <section class="summary" aria-labelledby="summary-heading">
        <div id="summary-heading" style="font-weight:700;margin-bottom:8px">Summary</div>
        <div>
          A passionate UX Designer with over 3 years' experience in website design, development and UX.
          Known for playing hard and working even harder. Focused on information architecture, wireframing,
          prototyping and visual communication.
        </div>
      </section>

      <section aria-labelledby="experience-heading" style="margin-top:6px">
        <div class="heading"><h3 id="experience-heading">Work Experience</h3></div>

        <article class="job" aria-labelledby="job-ux">
          <h4 id="job-ux">UX Designer — Really Great Company</h4>
          <div class="meta">2019 — 2021</div>
          <ul>
            <li>Information architecture for websites, apps and software.</li>
            <li>Wireframing and prototyping to test functionality.</li>
            <li>Visual communication in layout, colour and typography.</li>
          </ul>
        </article>

        <article class="job" aria-labelledby="job-webdev">
          <h4 id="job-webdev">Web Developer — Really Great Company</h4>
          <div class="meta">2017 — 2019</div>
          <ul>
            <li>Database administration and IT management.</li>
            <li>Website backups and server migration.</li>
            <li>Front end and back end development.</li>
          </ul>
        </article>

        <article class="job" aria-labelledby="job-webdesigner">
          <h4 id="job-webdesigner">Web Designer — Really Great Company</h4>
          <div class="meta">Role details</div>
          <ul>
            <li>Website design and development from concept to delivery.</li>
            <li>Delivered 10+ websites from concept to completion.</li>
            <li>Developed visual style guides and design systems.</li>
          </ul>
        </article>
      </section>

      <section aria-labelledby="more-heading" style="margin-top:12px">
        <div class="heading"><h3 id="more-heading">Additional</h3></div>
        <div style="color:var(--muted);font-size:14px;line-height:1.5">
          Available for freelance and full-time roles. Portfolio and references available upon request.
        </div>
      </section>
    </main>
  </div>
</body>
</html>
