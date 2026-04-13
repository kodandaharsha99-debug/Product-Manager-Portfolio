<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Harsha Iragavarapu — Product Manager Portfolio</title>
<link href="https://fonts.googleapis.com/css2?family=DM+Serif+Display:ital@0;1&family=DM+Sans:ital,opsz,wght@0,9..40,300;0,9..40,400;0,9..40,500;0,9..40,600;1,9..40,300&display=swap" rel="stylesheet"/>
<style>
  :root {
    --ink: #111111;
    --ink-muted: #5a5a5a;
    --ink-faint: #9a9a9a;
    --bg: #f8f7f4;
    --bg-card: #ffffff;
    --accent: #1a4ed8;
    --accent-light: #e8eeff;
    --green: #14532d;
    --green-light: #dcfce7;
    --border: #e5e5e0;
    --rule: #d4d4cc;
    --max: 860px;
    --serif: 'DM Serif Display', Georgia, serif;
    --sans: 'DM Sans', system-ui, sans-serif;
  }

  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

  html { font-size: 16px; scroll-behavior: smooth; }

  body {
    background: var(--bg);
    color: var(--ink);
    font-family: var(--sans);
    font-weight: 400;
    line-height: 1.7;
    -webkit-font-smoothing: antialiased;
  }

  /* ── Layout ── */
  .page {
    max-width: var(--max);
    margin: 0 auto;
    padding: 0 24px;
  }

  /* ── Header ── */
  header {
    border-bottom: 1px solid var(--rule);
    padding: 18px 0;
    position: sticky;
    top: 0;
    background: rgba(248, 247, 244, 0.96);
    backdrop-filter: blur(6px);
    z-index: 100;
  }
  header .page {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 16px;
    flex-wrap: wrap;
  }
  .header-name {
    font-family: var(--serif);
    font-size: 1.1rem;
    letter-spacing: -0.01em;
    color: var(--ink);
  }
  .header-links {
    display: flex;
    gap: 6px;
    align-items: center;
    flex-wrap: wrap;
  }
  .header-links a {
    display: inline-block;
    padding: 5px 14px;
    border: 1px solid var(--border);
    border-radius: 999px;
    font-size: 0.78rem;
    font-weight: 500;
    color: var(--ink-muted);
    text-decoration: none;
    transition: border-color .2s, color .2s, background .2s;
    letter-spacing: 0.02em;
  }
  .header-links a:hover {
    border-color: var(--accent);
    color: var(--accent);
    background: var(--accent-light);
  }

  /* ── Hero ── */
  .hero {
    padding: 80px 0 64px;
    border-bottom: 1px solid var(--rule);
  }
  .hero-eyebrow {
    font-size: 0.75rem;
    font-weight: 600;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    color: var(--accent);
    margin-bottom: 20px;
  }
  .hero h1 {
    font-family: var(--serif);
    font-size: clamp(2.4rem, 5vw, 3.4rem);
    line-height: 1.12;
    letter-spacing: -0.025em;
    color: var(--ink);
    max-width: 640px;
    margin-bottom: 28px;
  }
  .hero h1 em {
    font-style: italic;
    color: var(--accent);
  }
  .hero-bio {
    font-size: 1.05rem;
    color: var(--ink-muted);
    max-width: 560px;
    line-height: 1.75;
    font-weight: 300;
  }
  .hero-tags {
    display: flex;
    gap: 8px;
    flex-wrap: wrap;
    margin-top: 32px;
  }
  .tag {
    font-size: 0.74rem;
    font-weight: 500;
    letter-spacing: 0.04em;
    padding: 4px 12px;
    background: var(--bg-card);
    border: 1px solid var(--border);
    border-radius: 4px;
    color: var(--ink-muted);
  }

  /* ── Section Structure ── */
  .section {
    padding: 72px 0;
    border-bottom: 1px solid var(--rule);
  }
  .section-label {
    font-size: 0.7rem;
    font-weight: 600;
    letter-spacing: 0.14em;
    text-transform: uppercase;
    color: var(--ink-faint);
    margin-bottom: 10px;
  }
  .section-num {
    display: inline-block;
    width: 24px;
    height: 24px;
    border-radius: 50%;
    background: var(--ink);
    color: white;
    font-size: 0.7rem;
    font-weight: 600;
    text-align: center;
    line-height: 24px;
    margin-right: 8px;
    vertical-align: middle;
    position: relative;
    top: -1px;
  }
  .section h2 {
    font-family: var(--serif);
    font-size: clamp(1.6rem, 3vw, 2.1rem);
    line-height: 1.18;
    letter-spacing: -0.02em;
    color: var(--ink);
    margin-bottom: 8px;
  }
  .section-sub {
    font-size: 0.9rem;
    color: var(--ink-faint);
    margin-bottom: 40px;
    font-weight: 300;
  }

  /* ── Case Study Cards ── */
  .ps-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 1px;
    background: var(--border);
    border: 1px solid var(--border);
    border-radius: 10px;
    overflow: hidden;
    margin-bottom: 32px;
  }
  .ps-block {
    background: var(--bg-card);
    padding: 28px 30px;
  }
  .ps-block h4 {
    font-size: 0.68rem;
    font-weight: 700;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    color: var(--ink-faint);
    margin-bottom: 10px;
  }
  .ps-block p {
    font-size: 0.92rem;
    color: var(--ink-muted);
    line-height: 1.65;
  }
  .ps-block.solution { background: #fafafa; }

  /* ── Metrics Bar ── */
  .metrics {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 1px;
    background: var(--border);
    border: 1px solid var(--border);
    border-radius: 10px;
    overflow: hidden;
    margin-bottom: 32px;
  }
  .metric-cell {
    background: var(--bg-card);
    padding: 24px 26px;
    text-align: left;
  }
  .metric-num {
    font-family: var(--serif);
    font-size: 2rem;
    letter-spacing: -0.03em;
    color: var(--green);
    line-height: 1;
    margin-bottom: 4px;
  }
  .metric-label {
    font-size: 0.8rem;
    color: var(--ink-muted);
    line-height: 1.4;
  }

  /* ── Security Section ── */
  .security-summary {
    background: var(--bg-card);
    border: 1px solid var(--border);
    border-radius: 10px;
    padding: 30px 32px;
    margin-bottom: 24px;
    font-size: 0.95rem;
    color: var(--ink-muted);
    line-height: 1.75;
  }
  .intervention-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 16px;
    margin-bottom: 24px;
  }
  .intervention-card {
    background: var(--bg-card);
    border: 1px solid var(--border);
    border-radius: 10px;
    padding: 24px 26px;
  }
  .intervention-card h4 {
    font-size: 0.75rem;
    font-weight: 700;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    color: var(--accent);
    margin-bottom: 8px;
  }
  .intervention-card p {
    font-size: 0.88rem;
    color: var(--ink-muted);
    line-height: 1.6;
  }
  .result-banner {
    background: var(--green-light);
    border: 1px solid #bbf7d0;
    border-radius: 10px;
    padding: 18px 26px;
    font-size: 0.88rem;
    color: var(--green);
    font-weight: 500;
    display: flex;
    align-items: center;
    gap: 10px;
  }
  .result-banner::before {
    content: "✓";
    width: 22px; height: 22px;
    background: var(--green);
    color: white;
    border-radius: 50%;
    display: inline-flex; align-items: center; justify-content: center;
    font-size: 0.75rem;
    font-weight: 700;
    flex-shrink: 0;
  }
  /* ── Philosophy ── */
  .philosophy-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 16px;
  }
  .phil-card {
    background: var(--bg-card);
    border: 1px solid var(--border);
    border-radius: 10px;
    padding: 28px 26px;
    position: relative;
    overflow: hidden;
  }
  .phil-card::before {
    content: '';
    position: absolute;
    top: 0; left: 0;
    width: 3px; height: 100%;
    background: var(--accent);
  }
  .phil-card h3 {
    font-family: var(--serif);
    font-size: 1.05rem;
    color: var(--ink);
    margin-bottom: 10px;
    line-height: 1.3;
  }
  .phil-card p {
    font-size: 0.85rem;
    color: var(--ink-muted);
    line-height: 1.65;
  }

  /* ── Sprint ── */
  .sprint-grid {
    display: grid;
    grid-template-columns: 2fr 1fr;
    gap: 16px;
  }
  .sprint-items {
    display: flex;
    flex-direction: column;
    gap: 16px;
  }
  .sprint-item {
    background: var(--bg-card);
    border: 1px solid var(--border);
    border-radius: 10px;
    padding: 22px 26px;
    display: flex;
    gap: 16px;
    align-items: flex-start;
  }
  .sprint-icon {
    font-size: 1.3rem;
    line-height: 1;
    margin-top: 2px;
    flex-shrink: 0;
  }
  .sprint-item h4 {
    font-size: 0.88rem;
    font-weight: 600;
    color: var(--ink);
    margin-bottom: 4px;
  }
  .sprint-item p {
    font-size: 0.82rem;
    color: var(--ink-muted);
    line-height: 1.55;
  }
  .arsenal-card {
    background: var(--ink);
    border-radius: 10px;
    padding: 26px;
    color: white;
  }
  .arsenal-card h4 {
    font-size: 0.68rem;
    font-weight: 700;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    color: rgba(255,255,255,0.5);
    margin-bottom: 16px;
  }
  .arsenal-list {
    list-style: none;
    display: flex;
    flex-direction: column;
    gap: 10px;
  }
  .arsenal-list li {
    font-size: 0.85rem;
    color: rgba(255,255,255,0.85);
    display: flex;
    align-items: center;
    gap: 8px;
  }
  .arsenal-list li::before {
    content: '';
    width: 5px; height: 5px;
    background: var(--accent);
    border-radius: 50%;
    flex-shrink: 0;
  }

  /* ── Footer ── */
  footer {
    padding: 40px 0;
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 12px;
    flex-wrap: wrap;
  }
  footer p {
    font-size: 0.8rem;
    color: var(--ink-faint);
  }
  footer .footer-links {
    display: flex;
    gap: 16px;
  }
  footer .footer-links a {
    font-size: 0.8rem;
    color: var(--ink-faint);
    text-decoration: none;
    transition: color .2s;
  }
  footer .footer-links a:hover { color: var(--accent); }

  /* ── Animations ── */
  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(16px); }
    to   { opacity: 1; transform: translateY(0); }
  }
  .hero-eyebrow { animation: fadeUp .5s ease both; }
  .hero h1      { animation: fadeUp .55s .07s ease both; }
  .hero-bio     { animation: fadeUp .55s .14s ease both; }
  .hero-tags    { animation: fadeUp .55s .2s ease both; }

  /* ── Flow Diagram ── */
  .flow-wrap {
    margin-top: 28px;
    display: grid;
    grid-template-columns: 1fr 40px 1fr;
    align-items: start;
  }
  .flow-col {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 28px 20px;
    border-radius: 12px;
  }
  .flow-col--before { background: #fff5f5; border: 1px solid #fecaca; }
  .flow-col--after  { background: #f0fdf4; border: 1px solid #bbf7d0; }
  .flow-col-label {
    font-size: 0.68rem;
    font-weight: 700;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    margin-bottom: 20px;
    padding: 4px 12px;
    border-radius: 999px;
  }
  .flow-col-label--bad  { background: #fee2e2; color: #991b1b; }
  .flow-col-label--good { background: #dcfce7; color: #14532d; }
  .flow-node {
    background: white;
    border: 1px solid var(--border);
    border-radius: 8px;
    padding: 10px 16px;
    font-size: 0.82rem;
    font-weight: 500;
    color: var(--ink);
    text-align: center;
    width: 100%;
    line-height: 1.4;
  }
  .flow-node span {
    display: block;
    font-size: 0.72rem;
    font-weight: 400;
    color: var(--ink-faint);
    margin-top: 2px;
  }
  .flow-node--start   { background: var(--ink); color: white; border-color: var(--ink); font-weight: 600; }
  .flow-node--danger  { background: #fef2f2; border-color: #fca5a5; color: #991b1b; font-weight: 600; }
  .flow-node--bad-end { background: #fee2e2; border-color: #f87171; color: #7f1d1d; font-weight: 600; }
  .flow-node--gate    { background: #eff6ff; border-color: #93c5fd; color: #1e40af; font-weight: 600; }
  .flow-node--log     { background: #fefce8; border-color: #fde68a; color: #78350f; }
  .flow-node--deny    { background: #fef2f2; border-color: #fca5a5; color: #7f1d1d; font-size: 0.78rem; }
  .flow-node--good-end{ background: #dcfce7; border-color: #4ade80; color: #14532d; font-weight: 600; }
  .flow-arrow {
    font-size: 1rem;
    color: var(--ink-faint);
    margin: 6px 0;
    line-height: 1;
  }
  .flow-arrow--branch {
    font-size: 0.75rem;
    color: var(--ink-faint);
    font-style: italic;
  }
  .flow-diamond {
    width: 80px; height: 80px;
    background: white;
    border: 1.5px solid #86efac;
    transform: rotate(45deg);
    display: flex; flex-direction: row; align-items: center; justify-content: center;
    margin: 8px 0;
    flex-shrink: 0;
  }
  .flow-diamond span {
    transform: rotate(-45deg);
    font-size: 0.68rem;
    font-weight: 600;
    color: var(--green);
    text-align: center;
    line-height: 1.3;
  }
  .flow-branch-row {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 10px;
    width: 100%;
    margin-top: 6px;
  }
  .flow-branch-no, .flow-branch-yes {
    display: flex; flex-direction: column; align-items: center; gap: 6px;
  }
  .flow-branch-label {
    font-size: 0.68rem;
    font-weight: 700;
    letter-spacing: 0.08em;
    text-transform: uppercase;
    color: var(--ink-faint);
  }
  .flow-divider {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    padding-top: 60px;
    gap: 6px;
  }
  .flow-divider-line {
    width: 1px; height: 60px;
    background: var(--rule);
  }
  .flow-divider-badge {
    width: 28px; height: 28px;
    border-radius: 50%;
    background: var(--bg);
    border: 1px solid var(--rule);
    font-size: 0.7rem;
    font-weight: 700;
    color: var(--ink-faint);
    display: flex; align-items: center; justify-content: center;
  }

  /* ── Responsive ── */
  @media (max-width: 620px) {
    .ps-grid, .metrics, .intervention-grid,
    .philosophy-grid, .sprint-grid {
      grid-template-columns: 1fr;
    }
    .flow-wrap {
      grid-template-columns: 1fr;
    }
    .flow-divider { flex-direction: row; padding-top: 0; padding: 12px 0; }
    .flow-divider-line { width: 60px; height: 1px; }
    .hero { padding: 52px 0 48px; }
    .section { padding: 52px 0; }
  }
</style>
</head>
<body>

<!-- ═══════════════════════════════════════════ HEADER ═══ -->
<header>
  <div class="page">
    <span class="header-name">Harsha Iragavarapu</span>
    <nav class="header-links">
      <a href="https://www.linkedin.com/in/harsha-iragavarapu-a46795205/">LinkedIn</a>
      <a href="https://drive.google.com/file/d/1yQipn42GxBGQPeFOb3wxpg5jmasm0VDp/view?usp=drive_link">Resume PDF</a>
      <a href="/cdn-cgi/l/email-protection#3c554e5d5b5d4a5d4e5d4c4912545d4e4f545d05057c455d545353125f5351">Email</a>
    </nav>
  </div>
</header>

<!-- ═══════════════════════════════════════════ HERO ══════ -->
<section class="hero">
  <div class="page">
    <p class="hero-eyebrow">Harsha Iragavarapu · Product Manager · 3.7+ Years</p>
    <h1>Building <em>High-Integrity</em> Systems<br/>for Complex Operations</h1>
    <p class="hero-bio">
      I don't just ship features — I engineer systems where data accuracy and security are non-negotiable. From manufacturing payroll infrastructure to high-security government vaults, my work is defined by one principle: the system must be right, every single time.
    </p>
    <div class="hero-tags">
      <span class="tag">System & Security First</span>
      <span class="tag">Full Lifecycle PM</span>
      <span class="tag">GovTech</span>
      <span class="tag">HRMS / SaaS</span>
      <span class="tag">AI Integration</span>
      <span class="tag">JIRA Workflow Architect</span>
      <span class="tag">SQL</span>
      <span class="tag">Flutter</span>
    </div>
  </div>
</section>

<!-- ════════════════════════════════════════ CASE STUDY 1 ═ -->
<section class="section">
  <div class="page">
    <p class="section-label"><span class="section-num">I</span>Case Study — HRMS</p>
    <h2>Asakta HRMS — Re-engineering Payroll<br/>Integrity from the Ground Up</h2>
    <p class="section-sub">System architecture · Data integrity · Manufacturing · AI augmentation</p>

    <div class="ps-grid">
      <div class="ps-block">
        <h4>The Business Problem</h4>
        <p>Manufacturing environments were plagued by payroll discrepancies and attendance fraud. Clock-in data was unreliable, manual entry introduced errors at every step, and finance teams spent days each month reconciling numbers that should have been exact. The root cause wasn't process — it was a system that had no integrity guarantees built in.</p>
      </div>
      <div class="ps-block solution">
        <h4>The System Intervention</h4>
        <p>Re-engineered the attendance logic and underlying system architecture end-to-end — ensuring 100% data integrity from clock-in to payroll calculation. Every data point is validated at source; no manual overrides without audit trails. As a strategic addition, deployed an <strong>AI FAQ Chatbot</strong> to absorb routine employee queries, freeing HR from administrative load and allowing them to focus on exceptions that actually require human judgment.</p>
      </div>
    </div>

    <div class="metrics">
      <div class="metric-cell">
        <div class="metric-num">100%</div>
        <div class="metric-label">Attendance accuracy<br/>Integrity enforced at source</div>
      </div>
      <div class="metric-cell">
        <div class="metric-num">0</div>
        <div class="metric-label">Payroll discrepancies<br/>Across every pay cycle</div>
      </div>
      <div class="metric-cell">
        <div class="metric-num">6–8 hrs</div>
        <div class="metric-label">HR admin time saved daily<br/>via AI chatbot deployment</div>
      </div>
    </div>
  </div>
</section>

<!-- ════════════════════════════════════════ CASE STUDY 2 ═ -->
<section class="section">
  <div class="page">
    <p class="section-label"><span class="section-num">II</span>Case Study — GovTech</p>
    <h2>The Strong Room — Designing for<br/>the Unverified Actor</h2>
    <p class="section-sub">Security architecture · Edge-case design · Access control · Compliance</p>

    <div class="security-summary">
      A government vault management system had a structural security gap: the authentication flow had no defined protocol for unverified individuals. An unknown actor could reach the point of physical access with no mandatory secondary check triggered. This wasn't a bug — it was a missing requirement that the original system design had never considered. Catastrophic breaches don't always come from attacks. Sometimes they come from gaps nobody thought to close.
    </div>

    <div class="intervention-grid">
      <div class="intervention-card">
        <h4>The System Design</h4>
        <p>Designed a <strong>Conditional Authentication Gate</strong> — a branch in the access flow that activates specifically when primary identification fails. Rather than allowing the process to fall through or hard-stop with no record, the gate routes the event to a structured secondary path. The system now has an explicit answer for every identity scenario, including the ones that were previously invisible.</p>
      </div>
      <div class="intervention-card">
        <h4>The "Other" Protocol</h4>
        <p>Introduced a Treasurer-level <strong>"Other" Identification Protocol</strong>: any unverified actor triggers a mandatory manual logging step — name, stated purpose, and timestamp — that must be completed and approved <em>before</em> access is considered. The design principle: no entry path exists without an audit trail. Denial is also recorded. Every outcome is attributable.</p>
      </div>
    </div>

    <div class="result-banner">
      Result: 100% auditable, secure path for all non-standard entries. The critical loophole is structurally closed — not patched, not monitored. Closed.
    </div>

    <!-- ── Side-by-side flow: Before vs After ── -->
    <div class="flow-wrap">
      <div class="flow-col flow-col--before">
        <div class="flow-col-label flow-col-label--bad">Before — The Loophole</div>

        <div class="flow-node flow-node--start">Actor Requests Access</div>
        <div class="flow-arrow">↓</div>
        <div class="flow-node">Primary ID Check</div>
        <div class="flow-arrow flow-arrow--branch">↓ &nbsp; Unverified?</div>
        <div class="flow-node flow-node--danger">⚠ No Protocol Defined</div>
        <div class="flow-arrow">↓</div>
        <div class="flow-node flow-node--bad-end">Access Granted<br/><span>No record. No audit trail.</span></div>
      </div>

      <div class="flow-divider">
        <div class="flow-divider-line"></div>
        <div class="flow-divider-badge">vs</div>
        <div class="flow-divider-line"></div>
      </div>

      <div class="flow-col flow-col--after">
        <div class="flow-col-label flow-col-label--good">After — The Fix</div>

        <div class="flow-node flow-node--start">Actor Requests Access</div>
        <div class="flow-arrow">↓</div>
        <div class="flow-node">Primary ID Check</div>
        <div class="flow-arrow flow-arrow--branch">↓ &nbsp; Unverified?</div>
        <div class="flow-node flow-node--gate">🔒 Conditional Auth Gate<br/><span>Treasurer notified</span></div>
        <div class="flow-arrow">↓</div>
        <div class="flow-node flow-node--log">"Other" Protocol Triggered<br/><span>Name · Purpose · Timestamp logged</span></div>
        <div class="flow-arrow">↓</div>
        <div class="flow-diamond">
          <span>Treasurer<br/>Approves?</span>
        </div>
        <div class="flow-branch-row">
          <div class="flow-branch-no">
            <div class="flow-branch-label">No</div>
            <div class="flow-node flow-node--deny">Access Denied<br/><span>Attempt recorded</span></div>
          </div>
          <div class="flow-branch-yes">
            <div class="flow-branch-label">Yes</div>
            <div class="flow-node flow-node--good-end">Access Granted<br/><span>Fully auditable</span></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ══════════════════════════════════════════ PHILOSOPHY ═ -->
<section class="section">
  <div class="page">
    <p class="section-label"><span class="section-num">III</span>Product Philosophy</p>
    <h2>How I Think About Products</h2>
    <p class="section-sub">Three principles that define every system I build</p>

    <div class="philosophy-grid">
      <div class="phil-card">
        <h3>Trust Through Accuracy</h3>
        <p>A product is only as good as its data integrity. In payroll, security, and compliance systems, a single incorrect record doesn't just cause an error — it erodes the trust the entire system is built on. I design for correctness first, features second.</p>
      </div>
      <div class="phil-card">
        <h3>Security for the Real World</h3>
        <p>The happy path is easy. Real systems fail at the edges — the unverified actor, the missing record, the scenario nobody mapped in the original spec. I treat edge cases and unverified actors as first-class design requirements, not post-launch patches.</p>
      </div>
      <div class="phil-card">
        <h3>The Augmented PM</h3>
        <p>Building in Flutter (WalkWise), deep-diving AI Architecture, and querying data with SQL isn't a side project — it's how I stay technically credible with engineering, and make better product decisions faster. I build to understand, not just to ship.</p>
      </div>
    </div>
  </div>
</section>

<!-- ══════════════════════════════════════════ SPRINT ═════ -->
<section class="section">
  <div class="page">
    <p class="section-label"><span class="section-num">IV</span>Technical Arsenal & Current Sprint</p>
    <h2>What I'm Building & How I Work</h2>
    <p class="section-sub">Applied learning — tools in active use, not on a résumé</p>

    <div class="sprint-grid">
      <div class="sprint-items">
        <div class="sprint-item">
          <span class="sprint-icon">🚀</span>
          <div>
            <h4>WalkWise — Flutter / Agentic Development</h4>
            <p>Building a full consumer product from scratch in Flutter using agentic development patterns. Acting as both PM and developer — defining requirements, writing code, and making real architecture calls. This is how I stay technically honest.</p>
          </div>
        </div>
        <div class="sprint-item">
          <span class="sprint-icon">🧠</span>
          <div>
            <h4>AI Architecture — SME-Level System Design</h4>
            <p>Going beyond prompting to understand how AI components fit into production systems — where they degrade, how they scale, and when not to use them. The goal is the depth needed to make real build-vs-integrate decisions, not just use AI as a feature label.</p>
          </div>
        </div>
      </div>

      <div class="arsenal-card">
        <h4>Technical Arsenal</h4>
        <ul class="arsenal-list">
          <li>JIRA — Expert &amp; Workflow Architect</li>
          <li>SQL — Product data analysis</li>
          <li>Flutter — Active development (WalkWise)</li>
          <li>AI Strategy — System integration</li>
          <li>Edge-case &amp; security-first design</li>
        </ul>
      </div>
    </div>
  </div>
</section>

<!-- ═══════════════════════════════════════════ FOOTER ════ -->
<footer class="page">
  <p>Building high-integrity systems for complex operations. Open to senior PM and product strategy roles.</p>
  <div class="footer-links">
    <a href="https://www.linkedin.com/in/harsha-iragavarapu-a46795205/">LinkedIn</a>
    <a href="https://drive.google.com/file/d/1yQipn42GxBGQPeFOb3wxpg5jmasm0VDp/view?usp=drive_link">Resume</a>
    <!-- <a href="/cdn-cgi/l/email-protection#deb -->
