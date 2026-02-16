<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Neha | Digital Growth & Performance Marketing Specialist</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --primary: #6366f1;
            --secondary: #8b5cf6;
            --dark: #1e293b;
            --light: #f8fafc;
            --accent: #ec4899;
            --gray: #64748b;
            --success: #10b981;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: var(--dark);
            overflow-x: hidden;
        }

        .hero {
            background: linear-gradient(135deg, var(--primary) 0%, var(--secondary) 100%);
            color: white;
            padding: 100px 20px 80px;
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 600"><circle cx="100" cy="100" r="100" fill="rgba(255,255,255,0.05)"/><circle cx="900" cy="400" r="150" fill="rgba(255,255,255,0.05)"/><circle cx="600" cy="200" r="80" fill="rgba(255,255,255,0.05)"/></svg>');
            animation: float 20s ease-in-out infinite;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-20px); }
        }

        .hero-content {
            position: relative;
            z-index: 1;
            max-width: 900px;
            margin: 0 auto;
        }

        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 20px;
            font-weight: 700;
            animation: fadeInUp 0.8s ease;
        }

        .hero .subtitle {
            font-size: 1.5rem;
            margin-bottom: 20px;
            opacity: 0.95;
            animation: fadeInUp 0.8s ease 0.2s backwards;
        }

        .hero .value-statement {
            font-size: 1.1rem;
            margin-bottom: 30px;
            opacity: 0.9;
            max-width: 800px;
            margin-left: auto;
            margin-right: auto;
            animation: fadeInUp 0.8s ease 0.3s backwards;
        }

        .hero-stats {
            display: flex;
            justify-content: center;
            gap: 50px;
            margin-top: 40px;
            flex-wrap: wrap;
            animation: fadeInUp 0.8s ease 0.4s backwards;
        }

        .stat {
            text-align: center;
        }

        .stat-number {
            font-size: 2.5rem;
            font-weight: 700;
            display: block;
        }

        .stat-label {
            font-size: 0.9rem;
            opacity: 0.9;
        }

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 80px 20px;
        }

        .section-title {
            font-size: 2.5rem;
            margin-bottom: 20px;
            text-align: center;
            color: var(--dark);
            position: relative;
            padding-bottom: 20px;
        }

        .section-subtitle {
            text-align: center;
            color: var(--gray);
            font-size: 1.1rem;
            margin-bottom: 50px;
            max-width: 700px;
            margin-left: auto;
            margin-right: auto;
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background: linear-gradient(90deg, var(--primary), var(--secondary));
            border-radius: 2px;
        }

        .kpi-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin-bottom: 60px;
        }

        .kpi-card {
            background: white;
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.08);
            text-align: center;
            transition: all 0.3s ease;
            border-top: 4px solid var(--success);
        }

        .kpi-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(0,0,0,0.15);
        }

        .kpi-number {
            font-size: 3rem;
            font-weight: 700;
            color: var(--success);
            margin-bottom: 10px;
        }

        .kpi-label {
            font-size: 1.1rem;
            color: var(--dark);
            font-weight: 600;
            margin-bottom: 10px;
        }

        .kpi-description {
            font-size: 0.9rem;
            color: var(--gray);
        }

        .about-section {
            background: var(--light);
        }

        .responsibilities-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 25px;
            margin-bottom: 40px;
        }

        .responsibility-card {
            background: white;
            padding: 25px;
            border-radius: 12px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.08);
            border-left: 4px solid var(--primary);
        }

        .responsibility-card h4 {
            color: var(--primary);
            font-size: 1.1rem;
            margin-bottom: 10px;
        }

        .responsibility-card ul {
            list-style: none;
            margin-top: 10px;
        }

        .responsibility-card li {
            padding-left: 20px;
            margin-bottom: 8px;
            position: relative;
            color: var(--gray);
            font-size: 0.95rem;
            line-height: 1.6;
        }

        .responsibility-card li::before {
            content: '•';
            position: absolute;
            left: 0;
            color: var(--primary);
            font-weight: 700;
        }

        .case-study-grid {
            display: grid;
            gap: 40px;
        }

        .case-study {
            background: white;
            border-radius: 20px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            transition: all 0.3s ease;
        }

        .case-study:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 50px rgba(0,0,0,0.15);
        }

        .case-study-header {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
            padding: 30px;
        }

        .case-study-tag {
            display: inline-block;
            background: rgba(255,255,255,0.2);
            padding: 5px 15px;
            border-radius: 20px;
            font-size: 0.85rem;
            margin-bottom: 10px;
        }

        .case-study h3 {
            font-size: 1.8rem;
            margin-bottom: 10px;
        }

        .case-study-client {
            opacity: 0.9;
            font-size: 1.1rem;
        }

        .case-study-body {
            padding: 35px;
        }

        .challenge-section, .solution-section, .results-section {
            margin-bottom: 25px;
        }

        .challenge-section h4, .solution-section h4, .results-section h4 {
            color: var(--primary);
            font-size: 1.2rem;
            margin-bottom: 10px;
            font-weight: 700;
        }

        .challenge-section p, .solution-section p {
            color: var(--gray);
            line-height: 1.7;
            margin-bottom: 10px;
        }

        .solution-list {
            list-style: none;
            margin-top: 10px;
        }

        .solution-list li {
            padding-left: 25px;
            margin-bottom: 8px;
            position: relative;
            color: var(--gray);
            line-height: 1.6;
        }

        .solution-list li::before {
            content: '✓';
            position: absolute;
            left: 0;
            color: var(--success);
            font-weight: 700;
        }

        .results-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 20px;
            margin-top: 15px;
        }

        .result-item {
            background: #f0fdf4;
            padding: 20px;
            border-radius: 10px;
            text-align: center;
            border: 2px solid #86efac;
        }

        .result-number {
            font-size: 2rem;
            font-weight: 700;
            color: var(--success);
            display: block;
            margin-bottom: 5px;
        }

        .result-label {
            font-size: 0.85rem;
            color: var(--dark);
            font-weight: 600;
        }

        .tools-used {
            margin-top: 20px;
            padding-top: 20px;
            border-top: 1px solid #e5e7eb;
        }

        .tools-used h5 {
            font-size: 0.9rem;
            color: var(--gray);
            margin-bottom: 10px;
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }

        .tool-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }

        .tool-tag {
            background: #e0e7ff;
            color: var(--primary);
            padding: 6px 14px;
            border-radius: 20px;
            font-size: 0.85rem;
            font-weight: 500;
        }

        .cta-section {
            background: linear-gradient(135deg, var(--dark) 0%, #334155 100%);
            color: white;
            text-align: center;
            padding: 80px 20px;
        }

        .cta-section h2 {
            font-size: 2.5rem;
            margin-bottom: 20px;
        }

        .cta-section p {
            font-size: 1.2rem;
            margin-bottom: 40px;
            opacity: 0.9;
            max-width: 800px;
            margin-left: auto;
            margin-right: auto;
        }

        .cta-buttons {
            display: flex;
            gap: 20px;
            justify-content: center;
            flex-wrap: wrap;
        }

        .btn {
            padding: 15px 40px;
            border-radius: 50px;
            font-size: 1.1rem;
            font-weight: 600;
            text-decoration: none;
            transition: all 0.3s ease;
            display: inline-block;
            border: 2px solid transparent;
        }

        .btn-primary {
            background: var(--accent);
            color: white;
        }

        .btn-primary:hover {
            background: #db2777;
            transform: translateY(-3px);
            box-shadow: 0 10px 30px rgba(236, 72, 153, 0.4);
        }

        .btn-secondary {
            background: transparent;
            color: white;
            border-color: white;
        }

        .btn-secondary:hover {
            background: white;
            color: var(--dark);
        }

        .footer {
            background: var(--dark);
            color: white;
            text-align: center;
            padding: 40px 20px;
        }

        .footer p {
            opacity: 0.8;
        }

        .social-links {
            display: flex;
            gap: 20px;
            justify-content: center;
            margin-bottom: 20px;
        }

        .social-links a {
            color: white;
            font-size: 1.5rem;
            transition: all 0.3s ease;
        }

        .social-links a:hover {
            color: var(--accent);
            transform: translateY(-3px);
        }

        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2.5rem;
            }

            .hero .subtitle {
                font-size: 1.2rem;
            }

            .hero-stats {
                gap: 30px;
            }

            .section-title {
                font-size: 2rem;
            }

            .results-grid {
                grid-template-columns: 1fr 1fr;
            }
        }
    </style>
</head>
<body>
    <!-- Hero Section -->
    <section class="hero">
        <div class="hero-content">
            <h1>NEHA</h1>
            <p class="subtitle">Digital Growth & Performance Marketing Specialist</p>
            <p class="value-statement">
                Driving measurable business growth through performance campaigns, marketing analytics, and AI-powered workflows. Proven track record optimizing 10+ client accounts with focus on ROI and data-driven decision making.
            </p>
            
            <div class="hero-stats">
                <div class="stat">
                    <span class="stat-number">2.5+</span>
                    <span class="stat-label">Years Experience</span>
                </div>
                <div class="stat">
                    <span class="stat-number">10+</span>
                    <span class="stat-label">Clients Managed</span>
                </div>
                <div class="stat">
                    <span class="stat-number">20%</span>
                    <span class="stat-label">Avg CPC Reduction</span>
                </div>
                <div class="stat">
                    <span class="stat-number">35%</span>
                    <span class="stat-label">Engagement Growth</span>
                </div>
            </div>
        </div>
    </section>

    <!-- Key Metrics & ROI Overview -->
    <section class="container">
        <h2 class="section-title">Track Record & Key Metrics</h2>
        <p class="section-subtitle">Measurable business outcomes across campaigns and clients</p>
        <div class="kpi-grid">
            <div class="kpi-card">
                <div class="kpi-number">30%</div>
                <div class="kpi-label">Cost Reduction</div>
                <p class="kpi-description">Operational efficiency through AI-assisted workflows and automation</p>
            </div>
            <div class="kpi-card">
                <div class="kpi-number">20%</div>
                <div class="kpi-label">CPC Optimization</div>
                <p class="kpi-description">Average paid campaign cost reduction through A/B testing and targeting refinement</p>
            </div>
            <div class="kpi-card">
                <div class="kpi-number">35%</div>
                <div class="kpi-label">Engagement Lift</div>
                <p class="kpi-description">Organic engagement growth through SEO and content optimization strategies</p>
            </div>
            <div class="kpi-card">
                <div class="kpi-number">10+</div>
                <div class="kpi-label">Concurrent Clients</div>
                <p class="kpi-description">Multi-industry portfolio management across B2B, e-commerce, and hospitality</p>
            </div>
        </div>
    </section>

    <!-- Core Responsibilities -->
    <section class="about-section">
        <div class="container">
            <h2 class="section-title">Core Responsibilities & Expertise</h2>
            <p class="section-subtitle">Strategic capabilities that drive performance outcomes</p>
            <div class="responsibilities-grid">
                <div class="responsibility-card">
                    <h4>Performance Campaign Management</h4>
                    <ul>
                        <li>Google Ads & Meta campaign structuring and optimization</li>
                        <li>A/B testing frameworks for creative and targeting</li>
                        <li>Conversion rate optimization and funnel analysis</li>
                        <li>Budget allocation and bid strategy management</li>
                    </ul>
                </div>
                <div class="responsibility-card">
                    <h4>Marketing Analytics & Reporting</h4>
                    <ul>
                        <li>Power BI dashboard development for executive reporting</li>
                        <li>GA4 implementation and conversion tracking</li>
                        <li>ROI analysis and attribution modeling</li>
                        <li>Performance insights and strategic recommendations</li>
                    </ul>
                </div>
                <div class="responsibility-card">
                    <h4>SEO & Organic Growth</h4>
                    <ul>
                        <li>Technical SEO audits and implementation</li>
                        <li>Keyword strategy and content optimization</li>
                        <li>Search Console analysis and performance monitoring</li>
                        <li>Organic traffic growth and engagement metrics</li>
                    </ul>
                </div>
                <div class="responsibility-card">
                    <h4>AI-Enhanced Workflows</h4>
                    <ul>
                        <li>Microsoft Copilot integration for campaign planning</li>
                        <li>AI-assisted competitive research and analysis</li>
                        <li>Content structuring and ideation automation</li>
                        <li>Workflow efficiency improvements and time savings</li>
                    </ul>
                </div>
                <div class="responsibility-card">
                    <h4>Client Portfolio & Stakeholder Management</h4>
                    <ul>
                        <li>Strategic coordination across diverse client accounts and industries</li>
                        <li>Cross-functional team collaboration and workflow optimization</li>
                        <li>Executive-level reporting and stakeholder communication</li>
                        <li>Campaign roadmaps and strategic planning frameworks</li>
                    </ul>
                </div>
                <div class="responsibility-card">
                    <h4>Lead Generation & Conversion</h4>
                    <ul>
                        <li>B2B and hospitality lead funnel development</li>
                        <li>Landing page optimization and testing</li>
                        <li>Lead quality improvement and scoring</li>
                        <li>Conversion tracking and pipeline analysis</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Case Studies -->
    <section class="container">
        <h2 class="section-title">Client Success Stories & Case Studies</h2>
        <p class="section-subtitle">Real results from strategic campaigns and optimizations</p>
        
        <div class="case-study-grid">
            <!-- Case Study 1: Multi-Client E-commerce Portfolio -->
            <div class="case-study">
                <div class="case-study-header">
                    <span class="case-study-tag">E-commerce & Luxury Retail</span>
                    <h3>Multi-Client E-commerce Optimization</h3>
                    <p class="case-study-client">Dhaanvi Jewellers, Shri Banaras Swarna Kala Kendra & Heritage Jewelry Brands</p>
                </div>
                <div class="case-study-body">
                    <div class="challenge-section">
                        <h4>Challenge</h4>
                        <p>Managing digital presence for multiple traditional jewelry retailers with limited online visibility, high CPCs in competitive luxury market, and need to reach high-net-worth customers while maintaining brand premium positioning.</p>
                    </div>
                    <div class="solution-section">
                        <h4>Strategy & Implementation</h4>
                        <ul class="solution-list">
                            <li>Developed targeted Meta and Google Ads campaigns focused on high-intent luxury purchase keywords</li>
                            <li>Implemented local SEO strategies with Google My Business optimization for foot traffic</li>
                            <li>Created cohesive social media content strategy balancing heritage storytelling with product showcases</li>
                            <li>Set up conversion tracking and attribution models to measure online-to-offline journey</li>
                            <li>A/B tested ad creatives, targeting parameters, and landing page designs</li>
                        </ul>
                    </div>
                    <div class="results-section">
                        <h4>Results Achieved</h4>
                        <div class="results-grid">
                            <div class="result-item">
                                <span class="result-number">20%</span>
                                <span class="result-label">CPC Reduction</span>
                            </div>
                            <div class="result-item">
                                <span class="result-number">35%</span>
                                <span class="result-label">Engagement Growth</span>
                            </div>
                            <div class="result-item">
                                <span class="result-number">3x</span>
                                <span class="result-label">Lead Quality</span>
                            </div>
                        </div>
                    </div>
                    <div class="tools-used">
                        <h5>Tools & Platforms Used</h5>
                        <div class="tool-tags">
                            <span class="tool-tag">Meta Business Suite</span>
                            <span class="tool-tag">Google Ads</span>
                            <span class="tool-tag">Google My Business</span>
                            <span class="tool-tag">GA4</span>
                            <span class="tool-tag">SEMrush</span>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Case Study 2: Hospitality Lead Generation -->
            <div class="case-study">
                <div class="case-study-header">
                    <span class="case-study-tag">Hospitality & Travel</span>
                    <h3>Luxury Villa Booking Campaign</h3>
                    <p class="case-study-client">GoaPlans, Villa in Goa & Dinner Cruise Party</p>
                </div>
                <div class="case-study-body">
                    <div class="challenge-section">
                        <h4>Challenge</h4>
                        <p>Highly competitive Goa hospitality market with seasonal demand fluctuations. Needed to drive qualified bookings during peak season while building brand awareness year-round. High customer acquisition costs threatening profitability.</p>
                    </div>
                    <div class="solution-section">
                        <h4>Strategy & Implementation</h4>
                        <ul class="solution-list">
                            <li>Built seasonal campaign strategy with dynamic budgets aligned to booking patterns</li>
                            <li>Implemented retargeting campaigns for website visitors who didn't complete bookings</li>
                            <li>Developed SEO content targeting long-tail luxury villa and event booking keywords</li>
                            <li>Created Instagram and Facebook campaigns showcasing property features and experiences</li>
                            <li>Set up conversion tracking from inquiry to booking completion</li>
                        </ul>
                    </div>
                    <div class="results-section">
                        <h4>Results Achieved</h4>
                        <div class="results-grid">
                            <div class="result-item">
                                <span class="result-number">45%</span>
                                <span class="result-label">Booking Increase</span>
                            </div>
                            <div class="result-item">
                                <span class="result-number">25%</span>
                                <span class="result-label">Lower CAC</span>
                            </div>
                            <div class="result-item">
                                <span class="result-number">60%</span>
                                <span class="result-label">Organic Traffic</span>
                            </div>
                        </div>
                    </div>
                    <div class="tools-used">
                        <h5>Tools & Platforms Used</h5>
                        <div class="tool-tags">
                            <span class="tool-tag">Meta Ads</span>
                            <span class="tool-tag">Google Search Ads</span>
                            <span class="tool-tag">Google Analytics 4</span>
                            <span class="tool-tag">SEMrush</span>
                            <span class="tool-tag">Canva</span>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Case Study 3: B2B Industrial Marketing -->
            <div class="case-study">
                <div class="case-study-header">
                    <span class="case-study-tag">B2B Industrial</span>
                    <h3>Industrial Sector Lead Generation</h3>
                    <p class="case-study-client">Daiki Axis India</p>
                </div>
                <div class="case-study-body">
                    <div class="challenge-section">
                        <h4>Challenge</h4>
                        <p>Complex B2B industrial sales cycle requiring high-quality leads, not just volume. Long decision-making process needed nurture strategies. Executive team needed real-time visibility into campaign ROI and lead pipeline.</p>
                    </div>
                    <div class="solution-section">
                        <h4>Strategy & Implementation</h4>
                        <ul class="solution-list">
                            <li>Developed LinkedIn and Google Search campaigns targeting decision-makers in industrial sectors</li>
                            <li>Built Power BI dashboards integrating GA4, Google Ads, and CRM data for executive reporting</li>
                            <li>Implemented lead scoring system to identify high-intent prospects</li>
                            <li>Created content marketing funnel with technical resources and case studies</li>
                            <li>Used Microsoft Copilot for competitive intelligence and industry research automation</li>
                        </ul>
                    </div>
                    <div class="results-section">
                        <h4>Results Achieved</h4>
                        <div class="results-grid">
                            <div class="result-item">
                                <span class="result-number">2.5x</span>
                                <span class="result-label">Lead Quality</span>
                            </div>
                            <div class="result-item">
                                <span class="result-number">30%</span>
                                <span class="result-label">Time Savings</span>
                            </div>
                            <div class="result-item">
                                <span class="result-number">Real-time</span>
                                <span class="result-label">ROI Tracking</span>
                            </div>
                        </div>
                    </div>
                    <div class="tools-used">
                        <h5>Tools & Platforms Used</h5>
                        <div class="tool-tags">
                            <span class="tool-tag">Power BI</span>
                            <span class="tool-tag">LinkedIn Campaign Manager</span>
                            <span class="tool-tag">Google Ads</span>
                            <span class="tool-tag">GA4</span>
                            <span class="tool-tag">Microsoft Copilot</span>
                            <span class="tool-tag">Search Console</span>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Case Study 4: Multi-Client Agency Management -->
            <div class="case-study">
                <div class="case-study-header">
                    <span class="case-study-tag">Digital Agency Operations</span>
                    <h3>Multi-Client Portfolio Optimization</h3>
                    <p class="case-study-client">ColorTouch - 10+ Client Portfolio Management</p>
                </div>
                <div class="case-study-body">
                    <div class="challenge-section">
                        <h4>Challenge</h4>
                        <p>Managing diverse client portfolio spanning jewelry, hospitality, travel, and technology sectors. Each client had different KPIs, budgets, and reporting requirements. Need for standardized processes while maintaining customized strategies.</p>
                    </div>
                    <div class="solution-section">
                        <h4>Strategy & Implementation</h4>
                        <ul class="solution-list">
                            <li>Developed scalable campaign frameworks adaptable across industries</li>
                            <li>Created standardized monthly reporting templates with client-specific KPIs</li>
                            <li>Implemented cross-client learnings to improve campaign performance</li>
                            <li>Built automation workflows for routine tasks using AI tools</li>
                            <li>Coordinated with design teams for consistent content quality across accounts</li>
                        </ul>
                    </div>
                    <div class="results-section">
                        <h4>Results Achieved</h4>
                        <div class="results-grid">
                            <div class="result-item">
                                <span class="result-number">10+</span>
                                <span class="result-label">Clients Managed</span>
                            </div>
                            <div class="result-item">
                                <span class="result-number">35%</span>
                                <span class="result-label">Avg Growth</span>
                            </div>
                            <div class="result-item">
                                <span class="result-number">100%</span>
                                <span class="result-label">Client Retention</span>
                            </div>
                        </div>
                    </div>
                    <div class="tools-used">
                        <h5>Tools & Platforms Used</h5>
                        <div class="tool-tags">
                            <span class="tool-tag">Power BI</span>
                            <span class="tool-tag">Meta Business Suite</span>
                            <span class="tool-tag">Google Ads Manager</span>
                            <span class="tool-tag">GA4</span>
                            <span class="tool-tag">SEMrush</span>
                            <span class="tool-tag">ChatGPT</span>
                            <span class="tool-tag">Google Search Console</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="footer">
        <div class="social-links">
            <a href="mailto:nehajalindra638@gmail.com" title="Email">📧</a>
            <a href="https://linkedin.com/in/neha-jalendra-740121287" target="_blank" title="LinkedIn">💼</a>
            <a href="tel:+917011688097" title="Phone">📱</a>
        </div>
        <p>© 2026 Neha | Digital Growth & Performance Marketing Specialist</p>
        <p style="margin-top: 10px; font-size: 0.9rem;">Faridabad, Haryana | Open to Remote, Hybrid, and Onsite Opportunities</p>
    </footer>

    <!-- CTA Section -->
    <section class="cta-section">
        <h2>Let's Drive Growth Through Data & Strategy</h2>
        <p>
            I bring a rare combination: strategic thinking backed by hands-on execution, analytical rigor balanced with creative problem-solving, and the ability to transform marketing data into business intelligence that drives decisions. Whether it's optimizing multi-million dollar campaigns, building analytics infrastructure from scratch, or integrating AI into marketing workflows—I deliver measurable impact.
        </p>
        <p style="margin-top: 20px; font-size: 1.1rem;">
            <strong>Open to:</strong> Performance Marketing | Growth Marketing | Marketing Analytics | Digital Strategy roles at consulting firms, technology companies, and data-driven organizations where marketing is treated as a growth engine, not a cost center.
        </p>
        <p style="margin-top: 15px; font-size: 1rem; opacity: 0.85;">
            Particularly interested in environments that value analytical thinking, continuous optimization, cross-functional collaboration, and the intersection of marketing strategy with emerging AI capabilities.
        </p>
        <div class="cta-buttons">
            <a href="mailto:nehajalindra638@gmail.com" class="btn btn-primary">Start a Conversation</a>
            <a href="https://linkedin.com/in/neha-jalendra-740121287" target="_blank" class="btn btn-secondary">Connect on LinkedIn</a>
        </div>
    </section>
</body>
</html><img width="1907" height="961" alt="image" src="https://github.com/user-attachments/assets/a93f985e-b725-48e3-835d-ba3cac37b311" />
