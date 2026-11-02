
html = r'''<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta name="description" content="Chetan Samra | DevOps & Azure Cloud Engineer portfolio" />
  <title>Chetan Samra | DevOps & Azure Cloud Engineer</title>
  <style>
    :root {
      --navy: #07152f;
      --cyan: #08c9ee;
      --blue: #4388ff;
      --purple: #8b5cf6;
      --green: #079b83;
      --orange: #e77b08;
      --ink: #18243a;
      --muted: #64748b;
      --line: #dbe4ef;
      --surface: #f6f9ff;
    }
    * { box-sizing: border-box; }
    html { scroll-behavior: smooth; }
    body {
      margin: 0;
      font-family: Inter, "Segoe UI", Arial, sans-serif;
      color: var(--ink);
      background: #fff;
    }
    .hero {
      position: relative;
      overflow: hidden;
      min-height: 290px;
      padding: 66px 20px 90px;
      text-align: center;
      color: white;
      background: linear-gradient(115deg, #35d0ed 0%, #4388ff 100%);
    }
    .hero::before, .hero::after {
      content: "";
      position: absolute;
      left: -5%;
      width: 110%;
      height: 80px;
      bottom: -43px;
      border-radius: 50% 50% 0 0;
      background: rgba(255,255,255,.35);
      transform: rotate(-2deg);
    }
    .hero::after {
      bottom: -57px;
      background: white;
      transform: rotate(1.5deg);
    }
    .hero-inner { position: relative; z-index: 1; }
    .hero h1 {
      margin: 0;
      font-size: clamp(2.6rem, 7vw, 4.5rem);
      letter-spacing: -2px;
      font-weight: 800;
    }
    .hero .role {
      margin: 16px 0 0;
      font-size: clamp(1rem, 2.8vw, 1.55rem);
      font-weight: 650;
    }
    .hero .experience {
      margin-top: 13px;
      font-size: .98rem;
      color: rgba(255,255,255,.92);
      letter-spacing: .3px;
    }
    main { max-width: 1120px; margin: auto; padding: 38px 22px 60px; }
    .intro { text-align: center; }
    .intro h2 {
      color: #00bfe9;
      font-size: clamp(1.5rem, 4vw, 2.25rem);
      margin: 0 0 16px;
      font-weight: 750;
    }
    .tagline {
      color: #9672f4;
      font-family: ui-monospace, SFMono-Regular, Menlo, monospace;
      font-size: clamp(.9rem, 2vw, 1.15rem);
      font-weight: 700;
      letter-spacing: .5px;
      margin: 0 0 30px;
    }
    .metrics {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 9px;
      margin: 0 auto 34px;
    }
    .metric {
      display: inline-flex;
      align-items: center;
      min-height: 43px;
      background: var(--navy);
      color: white;
      text-transform: uppercase;
      letter-spacing: 1.1px;
      font-size: .78rem;
      font-weight: 700;
    }
    .metric span { padding: 12px 16px; }
    .metric strong { padding: 12px 17px; background: #0788ca; }
    .metric:nth-child(2) strong { background: var(--green); }
    .metric:nth-child(3) strong { background: var(--orange); }
    .metric:nth-child(4) strong { background: #7938ed; }
    .nav-pills {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      border: 1px solid var(--line);
      margin: 0 -22px 34px;
      padding: 10px;
      gap: 9px;
      background: #fff;
    }
    .nav-pills a {
      text-decoration: none;
      color: white;
      padding: 9px 13px;
      font-size: .78rem;
      font-weight: 700;
      background: #087dbb;
      transition: transform .2s, opacity .2s;
    }
    .nav-pills a:hover { transform: translateY(-3px); opacity: .88; }
    .nav-pills a:nth-child(2) { background: #334155; }
    .nav-pills a:nth-child(3) { background: #0d9488; }
    .nav-pills a:nth-child(4) { background: #7c3aed; }
    .nav-pills a:nth-child(5) { background: #e66b16; }
    .nav-pills a:nth-child(6) { background: #2563eb; }
    section { padding: 26px 0; scroll-margin-top: 20px; }
    .section-title {
      font-size: 1.55rem;
      margin: 0 0 18px;
      color: #087fbd;
    }
    .section-title::after {
      content: "";
      display: block;
      width: 58px;
      height: 4px;
      border-radius: 4px;
      margin-top: 9px;
      background: linear-gradient(90deg, var(--cyan), var(--purple));
    }
    .about {
      color: #475569;
      line-height: 1.8;
      max-width: 900px;
    }
    .cards {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 15px;
    }
    .card {
      padding: 20px;
      border: 1px solid var(--line);
      border-radius: 13px;
      background: linear-gradient(145deg, #fff, var(--surface));
      box-shadow: 0 7px 22px rgba(15, 45, 85, .06);
    }
    .card h3 { margin: 0 0 9px; font-size: 1.05rem; color: #172554; }
    .card p { margin: 0; color: var(--muted); line-height: 1.65; font-size: .93rem; }
    .chips { display: flex; flex-wrap: wrap; gap: 10px; }
    .chip {
      padding: 9px 13px;
      border-radius: 7px;
      color: #075985;
      background: #e0f5ff;
      border: 1px solid #b8e8fb;
      font-size: .88rem;
      font-weight: 650;
    }
    .contact {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 10px;
      padding-top: 18px;
    }
    .contact a {
      color: white;
      background: #172033;
      text-decoration: none;
      padding: 11px 15px;
      border-radius: 5px;
      font-size: .9rem;
      font-weight: 650;
    }
    .contact a:hover { background: #087fbd; }
    footer {
      text-align: center;
      padding: 25px 15px;
      color: #64748b;
      background: #f1f6fc;
      font-size: .88rem;
    }
    @media (max-width: 600px) {
      .hero { min-height: 255px; padding-top: 55px; }
      .metric { width: 100%; justify-content: space-between; }
      .metric span, .metric strong { padding: 11px 12px; }
      .nav-pills { margin-left: -22px; margin-right: -22px; }
      .nav-pills a { flex: 1 1 42%; text-align: center; }
    }
  </style>
</head>
<body>
  <header class="hero">
    <div class="hero-inner">
      <h1>Chetan Samra</h1>
      <p class="role">DevOps &amp; Azure Cloud Engineer • Infrastructure Automation</p>
      <p class="experience">13 Years IT Experience&nbsp; | &nbsp;5+ Years DevOps &amp; Cloud</p>
    </div>
  </header>

  <main>
    <div class="intro">
      <h2>Azure Cloud • DevOps • DevSecOps • IaC</h2>
      <p class="tagline">▶ Building Secure, Scalable &amp; Automated Cloud Infrastructure</p>

      <div class="metrics">
        <div class="metric"><span>☁️ Azure Cloud</span><strong>Enterprise Ready</strong></div>
        <div class="metric"><span>⚙️ Terraform IaC</span><strong>Automation</strong></div>
        <div class="metric"><span>🚀 CI/CD</span><strong>Delivery Pipelines</strong></div>
        <div class="metric"><span>🛡️ DevSecOps</span><strong>Security First</strong></div>
      </div>
    </div>

    <nav class="nav-pills" aria-label="Page navigation">
      <a href="#about">⭐ About Me</a>
      <a href="#architecture">🏛️ Architecture</a>
      <a href="#azure">☁️ Azure</a>
      <a href="#iac">⚙️ IaC &amp; CI/CD</a>
      <a href="#security">🛡️ Security</a>
      <a href="#projects">🚀 Projects</a>
    </nav>

    <section id="about">
      <h2 class="section-title">About Me</h2>
      <p class="about">
        I am a DevOps and Azure Cloud Engineer with 13 years of overall IT experience,
        including 5+ years of hands-on experience in DevOps and cloud engineering.
        I focus on Azure infrastructure, Terraform-based automation, CI/CD pipelines,
        cloud governance, secure deployments and operational reliability. I enjoy
        designing repeatable solutions that make infrastructure delivery safer and faster.
      </p>
    </section>

    <section id="architecture">
      <h2 class="section-title">Cloud Architecture &amp; Governance</h2>
      <div class="cards">
        <article class="card"><h3>Azure Landing Zones</h3><p>Management groups, subscriptions, policy, RBAC and enterprise governance foundations.</p></article>
        <article class="card"><h3>Hub-Spoke Networking</h3><p>VNet design, peering, routing, NSGs, Azure Firewall and hybrid connectivity concepts.</p></article>
        <article class="card"><h3>Resilience &amp; Operations</h3><p>Monitoring, Log Analytics, backup, disaster recovery and operational reliability.</p></article>
      </div>
    </section>

    <section id="azure">
      <h2 class="section-title">Azure Technologies</h2>
      <div class="chips">
        <span class="chip">Azure Virtual Network</span><span class="chip">Virtual Machines</span>
        <span class="chip">Storage Accounts</span><span class="chip">Azure Bastion</span>
        <span class="chip">Load Balancer</span><span class="chip">Application Gateway</span>
        <span class="chip">Azure Firewall</span><span class="chip">Key Vault</span>
        <span class="chip">Private Endpoint</span><span class="chip">Entra ID / RBAC</span>
        <span class="chip">Azure Policy</span><span class="chip">Azure Monitor</span>
        <span class="chip">Log Analytics</span><span class="chip">Backup &amp; ASR</span>
        <span class="chip">AKS</span><span class="chip">Container Apps</span>
      </div>
    </section>

    <section id="iac">
      <h2 class="section-title">Infrastructure as Code &amp; CI/CD</h2>
      <div class="cards">
        <article class="card"><h3>Terraform</h3><p>Reusable modules, remote state, variables, workspaces, plan/apply, imports and drift management.</p></article>
        <article class="card"><h3>Azure DevOps</h3><p>YAML pipelines, repositories, variable groups, service connections and self-hosted agents.</p></article>
        <article class="card"><h3>Delivery Toolchain</h3><p>GitHub Actions, Jenkins, Git, Docker, Kubernetes, Bash and PowerShell.</p></article>
      </div>
    </section>

    <section id="security">
      <h2 class="section-title">DevSecOps &amp; Quality</h2>
      <div class="chips">
        <span class="chip">Checkov</span><span class="chip">tfsec</span>
        <span class="chip">TFLint</span><span class="chip">SonarQube</span>
        <span class="chip">TruffleHog</span><span class="chip">Gitleaks</span>
        <span class="chip">Secret Management</span><span class="chip">Least Privilege</span>
      </div>
    </section>

    <section id="projects">
      <h2 class="section-title">Featured Projects</h2>
      <div class="cards">
        <article class="card"><h3>Azure Infrastructure Automation</h3><p>Terraform modules and CI/CD workflows for repeatable Azure resource provisioning.</p></article>
        <article class="card"><h3>Enterprise Landing Zone Patterns</h3><p>Cloud governance, subscription structure, network segmentation and security controls.</p></article>
        <article class="card"><h3>DevSecOps Pipeline</h3><p>Infrastructure validation, security scanning, review gates and controlled deployments.</p></article>
      </div>
    </section>

    <div class="contact">
      <!-- Replace the example links below with your real profile URLs and email. -->
      <a href="mailto:YOUR_EMAIL@example.com">✉ Email</a>
      <a href="https://www.linkedin.com/in/YOUR-LINKEDIN/" target="_blank" rel="noopener noreferrer">in LinkedIn</a>
      <a href="https://github.com/SamraChetan" target="_blank" rel="noopener noreferrer">⌘ GitHub</a>
    </div>
  </main>

  <footer>Designed with ☁️ by Chetan Samra · Azure | DevOps | Terraform | DevSecOps</footer>
</body>
</html>
'''

path = Path("/mnt/data/index.html")
path.write_text(html, encoding="utf-8")
print(f"Created: {path}")
