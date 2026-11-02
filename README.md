
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chetan Samra | Azure DevOps Engineer</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: 'Segoe UI', Arial, sans-serif;
            background: #ffffff;
            color: #172033;
        }

        /* HERO SECTION */

        .hero {
            background: linear-gradient(120deg, #36d1ed, #4388ff);
            color: white;
            text-align: center;
            padding: 65px 20px 90px;
            position: relative;
            overflow: hidden;
        }

        .hero h1 {
            font-size: clamp(42px, 7vw, 68px);
            font-weight: 800;
            letter-spacing: -2px;
        }

        .hero h2 {
            font-size: clamp(17px, 3vw, 27px);
            margin-top: 15px;
        }

        .hero p {
            margin-top: 15px;
            font-size: 17px;
        }

        /* MAIN CONTENT */

        .container {
            max-width: 1150px;
            margin: auto;
            padding: 45px 20px;
        }

        .intro {
            text-align: center;
        }

        .intro h2 {
            color: #00bfe9;
            font-size: clamp(25px, 4vw, 36px);
            margin-bottom: 25px;
        }

        .tagline {
            color: #9672f4;
            font-size: 20px;
            font-weight: bold;
            margin-bottom: 35px;
        }

        /* METRICS */

        .metrics {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 10px;
            margin-bottom: 35px;
        }

        .metric {
            display: flex;
            background: #07152f;
            color: white;
            font-weight: bold;
            letter-spacing: 1px;
            font-size: 13px;
        }

        .metric span {
            padding: 13px 17px;
        }

        .metric strong {
            padding: 13px 17px;
            background: #0788ca;
        }

        .metric:nth-child(2) strong {
            background: #079b83;
        }

        .metric:nth-child(3) strong {
            background: #e77b08;
        }

        .metric:nth-child(4) strong {
            background: #7938ed;
        }

        /* NAVIGATION */

        .navigation {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 10px;
            padding: 15px;
            border: 1px solid #dbe4ef;
        }

        .navigation a {
            color: white;
            text-decoration: none;
            padding: 11px 16px;
            font-size: 13px;
            font-weight: bold;
            background: #087dbb;
            transition: 0.3s;
        }

        .navigation a:hover {
            transform: translateY(-4px);
            opacity: 0.85;
        }

        .navigation a:nth-child(2) {
            background: #334155;
        }

        .navigation a:nth-child(3) {
            background: #0d9488;
        }

        .navigation a:nth-child(4) {
            background: #7c3aed;
        }

        .navigation a:nth-child(5) {
            background: #e66b16;
        }

        .navigation a:nth-child(6) {
            background: #2563eb;
        }

        /* SECTION */

        section {
            padding: 35px 0;
            scroll-margin-top: 20px;
        }

        .section-title {
            color: #087fbd;
            font-size: 27px;
            margin-bottom: 22px;
        }

        .section-title::after {
            content: "";
            display: block;
            width: 65px;
            height: 4px;
            margin-top: 10px;
            background: linear-gradient(90deg, #08c9ee, #8b5cf6);
        }

        .about {
            color: #64748b;
            line-height: 1.9;
            font-size: 16px;
        }

        /* CARDS */

        .cards {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(230px, 1fr));
            gap: 20px;
        }

        .card {
            padding: 23px;
            border: 1px solid #dbe4ef;
            border-radius: 12px;
            background: linear-gradient(145deg, #ffffff, #f2f7ff);
            box-shadow: 0 7px 22px rgba(15,45,85,0.06);
            transition: 0.3s;
        }

        .card:hover {
            transform: translateY(-7px);
            box-shadow: 0 12px 28px rgba(15,45,85,0.13);
        }

        .card h3 {
            color: #172554;
            margin-bottom: 12px;
            font-size: 19px;
        }

        .card p {
            color: #64748b;
            line-height: 1.7;
            font-size: 14px;
        }

        /* SKILLS */

        .skills {
            display: flex;
            flex-wrap: wrap;
            gap: 12px;
        }

        .skill {
            background: #e0f5ff;
            border: 1px solid #b8e8fb;
            color: #075985;
            padding: 11px 17px;
            border-radius: 7px;
            font-size: 14px;
            font-weight: bold;
            transition: 0.3s;
        }

        .skill:hover {
            background: #087dbb;
            color: white;
            transform: scale(1.05);
        }

        /* CONTACT */

        .contact {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 12px;
            padding: 30px 0;
        }

        .contact a {
            text-decoration: none;
            color: white;
            background: #172033;
            padding: 13px 20px;
            border-radius: 5px;
            font-weight: bold;
            transition: 0.3s;
        }

        .contact a:hover {
            background: #087fbd;
            transform: translateY(-3px);
        }

        /* FOOTER */

        footer {
            background: #f1f6fc;
            text-align: center;
            padding: 25px;
            color: #64748b;
            font-size: 14px;
        }

        @media(max-width: 600px) {
            .hero {
                padding: 50px 15px 70px;
            }

            .metric {
                width: 100%;
                justify-content: space-between;
            }

            .metric span,
            .metric strong {
                padding: 12px;
            }

            .navigation a {
                flex: 1 1 40%;
                text-align: center;
            }
        }
    </style>
</head>

<body>

    <!-- HERO SECTION -->

    <header class="hero">

        <h1>Chetan Samra</h1>

        <h2>
            Senior DevOps & Azure Cloud Engineer
        </h2>

        <p>
            13 Years IT Experience | 5+ Years DevOps & Cloud
        </p>

    </header>


    <div class="container">

        <!-- INTRO -->

        <div class="intro">

            <h2>
                Enterprise Azure Cloud & DevOps Specialist
            </h2>

            <p class="tagline">
                ▶ Automating Infrastructure with Terraform & CI/CD
            </p>


            <!-- METRICS -->

            <div class="metrics">

                <div class="metric">
                    <span>☁️ AZURE CLOUD</span>
                    <strong>ENTERPRISE READY</strong>
                </div>

                <div class="metric">
                    <span>⚙️ TERRAFORM</span>
                    <strong>IaC AUTOMATION</strong>
                </div>

                <div class="metric">
                    <span>🚀 CI/CD</span>
                    <strong>DELIVERY PIPELINES</strong>
                </div>

                <div class="metric">
                    <span>🛡️ DEVSECOPS</span>
                    <strong>SECURITY FIRST</strong>
                </div>

            </div>

        </div>


        <!-- NAVIGATION -->

        <nav class="navigation">

            <a href="#about">⭐ About Me</a>

            <a href="#architecture">🏛️ Architecture</a>

            <a href="#azure">☁️ Azure</a>

            <a href="#iac">⚙️ IaC & CI/CD</a>

            <a href="#security">🛡️ Security</a>

            <a href="#projects">🚀 Projects</a>

        </nav>


        <!-- ABOUT -->

        <section id="about">

            <h2 class="section-title">
                About Me
            </h2>

            <p class="about">

                I am a DevOps and Azure Cloud Engineer with
                13 years of overall IT experience, including
                5+ years of hands-on experience in DevOps
                and Cloud Engineering.

                I specialize in Azure Cloud Infrastructure,
                Terraform Infrastructure as Code,
                CI/CD automation, Azure Landing Zones,
                cloud governance, security and enterprise
                infrastructure management.

                My focus is on building scalable, secure,
                automated and reliable cloud environments.

            </p>

        </section>


        <!-- ARCHITECTURE -->

        <section id="architecture">

            <h2 class="section-title">
                Enterprise Cloud Architecture
            </h2>

            <div class="cards">

                <div class="card">

                    <h3>🏛️ Azure Landing Zones</h3>

                    <p>
                        Management Groups, Subscriptions,
                        Azure Policy, RBAC and enterprise
                        cloud governance.
                    </p>

                </div>


                <div class="card">

                    <h3>🌐 Hub-Spoke Architecture</h3>

                    <p>
                        VNet Peering, Azure Firewall,
                        Network Security Groups,
                        Routing and Hybrid Connectivity.
                    </p>

                </div>


                <div class="card">

                    <h3>🔄 High Availability & DR</h3>

                    <p>
                        Azure Backup, Site Recovery,
                        Monitoring, Disaster Recovery
                        and infrastructure reliability.
                    </p>

                </div>

            </div>

        </section>


        <!-- AZURE SKILLS -->

        <section id="azure">

            <h2 class="section-title">
                Azure Cloud Technologies
            </h2>

            <div class="skills">

                <span class="skill">Azure Virtual Machines</span>

                <span class="skill">Azure Networking</span>

                <span class="skill">Virtual Networks</span>

                <span class="skill">VNet Peering</span>

                <span class="skill">Azure Bastion</span>

                <span class="skill">Load Balancer</span>

                <span class="skill">Application Gateway</span>

                <span class="skill">Azure Firewall</span>

                <span class="skill">Storage Accounts</span>

                <span class="skill">Azure Key Vault</span>

                <span class="skill">Private Endpoints</span>

                <span class="skill">Azure Entra ID</span>

                <span class="skill">RBAC & PIM</span>

                <span class="skill">Azure Policy</span>

                <span class="skill">Management Groups</span>

                <span class="skill">Azure Monitor</span>

                <span class="skill">Log Analytics</span>

                <span class="skill">Azure Backup</span>

                <span class="skill">Azure Site Recovery</span>

                <span class="skill">AKS</span>

                <span class="skill">Container Apps</span>

            </div>

        </section>


        <!-- TERRAFORM AND CICD -->

        <section id="iac">

            <h2 class="section-title">
                Infrastructure as Code & CI/CD
            </h2>

            <div class="cards">

                <div class="card">

                    <h3>⚙️ Terraform</h3>

                    <p>
                        Terraform Modules, Remote State,
                        Backend Configuration, Variables,
                        Outputs, Import, for_each,
                        Infrastructure Provisioning
                        and Drift Management.
                    </p>

                </div>


                <div class="card">

                    <h3>🚀 Azure DevOps</h3>

                    <p>
                        YAML Pipelines, Azure Repos,
                        Variable Groups, Service Connections,
                        Self Hosted Agents and
                        Multi-Stage CI/CD Pipelines.
                    </p>

                </div>


                <div class="card">

                    <h3>🐙 GitHub & Jenkins</h3>

                    <p>
                        GitHub Actions, Jenkins,
                        Git Workflow, Pull Requests,
                        Branching Strategy and
                        Automated Deployments.
                    </p>

                </div>


                <div class="card">

                    <h3>🐳 Containers</h3>

                    <p>
                        Docker, Kubernetes, AKS,
                        Container Images, Helm,
                        Deployments and Container Security.
                    </p>

                </div>

            </div>

        </section>


        <!-- DEVSECOPS -->

        <section id="security">

            <h2 class="section-title">
                DevSecOps & Security Tools
            </h2>

            <div class="skills">

                <span class="skill">Checkov</span>

                <span class="skill">tfsec</span>

                <span class="skill">TFLint</span>

                <span class="skill">SonarQube</span>

                <span class="skill">TruffleHog</span>

                <span class="skill">Gitleaks</span>

                <span class="skill">Super-Linter</span>

                <span class="skill">Secret Management</span>

                <span class="skill">RBAC</span>

                <span class="skill">Managed Identity</span>

                <span class="skill">Service Principal</span>

            </div>

        </section>


        <!-- OTHER SKILLS -->

        <section id="tools">

            <h2 class="section-title">
                Additional Technical Skills
            </h2>

            <div class="skills">

                <span class="skill">Linux Administration</span>

                <span class="skill">Bash Scripting</span>

                <span class="skill">PowerShell</span>

                <span class="skill">Python Basics</span>

                <span class="skill">Git</span>

                <span class="skill">Jira</span>

                <span class="skill">ServiceNow</span>

                <span class="skill">ITIL / ITSM</span>

                <span class="skill">Agile / Scrum</span>

            </div>

        </section>


        <!-- PROJECTS -->

        <section id="projects">

            <h2 class="section-title">
                Featured Projects
            </h2>

            <div class="cards">

                <div class="card">

                    <h3>☁️ Azure Infrastructure Automation</h3>

                    <p>
                        Automated Azure resource provisioning
                        using Terraform modules and Azure
                        DevOps CI/CD pipelines.
                    </p>

                </div>


                <div class="card">

                    <h3>🏛️ Enterprise Landing Zone</h3>

                    <p>
                        Enterprise cloud governance,
                        subscription architecture,
                        networking and security controls.
                    </p>

                </div>


                <div class="card">

                    <h3>🛡️ DevSecOps Pipeline</h3>

                    <p>
                        Integrated infrastructure validation,
                        security scanning, code quality checks
                        and controlled deployments.
                    </p>

                </div>


                <div class="card">

                    <h3>🚀 Multi-Environment CI/CD</h3>

                    <p>
                        Automated Dev, Test, UAT and
                        Production deployments with
                        approval gates and Terraform.
                    </p>

                </div>

            </div>

        </section>


        <!-- CONTACT -->

        <div class="contact">

            <!-- Update these links with your real details -->

            <a href="mailto:YOUR_EMAIL@example.com">
                ✉ Email Me
            </a>

            <a href="https://www.linkedin.com/in/YOUR-LINKEDIN/"
               target="_blank">
                in LinkedIn
            </a>

            <a href="https://github.com/SamraChetan"
               target="_blank">
                🐙 GitHub
            </a>

        </div>

    </div>


    <!-- FOOTER -->

    <footer>

        <p>
            Designed with ❤️ by Chetan Samra
        </p>

        <p>
            Azure Cloud | DevOps | Terraform | DevSecOps
        </p>

        <p>
            © 2026 Chetan Samra. All Rights Reserved.
        </p>

    </footer>

</body>
</html>
