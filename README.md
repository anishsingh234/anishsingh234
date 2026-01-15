<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Anish Kumar Singh - Full Stack Developer</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #2c3e50;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            padding: 20px;
        }

        .container {
            max-width: 900px;
            margin: 0 auto;
            background: white;
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
            border-radius: 12px;
            overflow: hidden;
        }

        .header {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 60px 40px;
            text-align: center;
        }

        .header h1 {
            font-size: 2.8em;
            margin-bottom: 8px;
            font-weight: 700;
            letter-spacing: -0.5px;
        }

        .header .title {
            font-size: 1.2em;
            font-weight: 300;
            opacity: 0.95;
            margin-bottom: 15px;
        }

        .header .contact {
            display: flex;
            justify-content: center;
            gap: 25px;
            flex-wrap: wrap;
            font-size: 0.95em;
        }

        .contact-item {
            display: flex;
            align-items: center;
            gap: 6px;
        }

        .contact-item a {
            color: white;
            text-decoration: none;
            transition: opacity 0.3s;
        }

        .contact-item a:hover {
            opacity: 0.8;
        }

        .content {
            padding: 50px 40px;
        }

        .section {
            margin-bottom: 40px;
        }

        .section-title {
            font-size: 1.4em;
            font-weight: 700;
            color: #667eea;
            margin-bottom: 20px;
            padding-bottom: 10px;
            border-bottom: 3px solid #667eea;
            display: inline-block;
        }

        .education-item {
            margin-bottom: 25px;
        }

        .degree {
            font-size: 1.1em;
            font-weight: 700;
            color: #2c3e50;
            margin-bottom: 5px;
        }

        .university {
            color: #667eea;
            font-weight: 600;
            margin-bottom: 8px;
        }

        .timeline {
            color: #7f8c8d;
            font-size: 0.95em;
            margin-bottom: 10px;
        }

        .coursework {
            color: #555;
            font-size: 0.95em;
            line-height: 1.7;
        }

        .experience-item {
            margin-bottom: 30px;
            background: #f8f9fa;
            padding: 20px;
            border-radius: 8px;
            border-left: 4px solid #667eea;
        }

        .job-title {
            font-size: 1.15em;
            font-weight: 700;
            color: #2c3e50;
            margin-bottom: 5px;
        }

        .company {
            color: #667eea;
            font-weight: 600;
            margin-bottom: 8px;
        }

        .job-description {
            list-style: none;
            margin-top: 12px;
        }

        .job-description li {
            padding: 6px 0;
            padding-left: 20px;
            position: relative;
            color: #555;
            font-size: 0.95em;
        }

        .job-description li:before {
            content: "▸";
            position: absolute;
            left: 0;
            color: #667eea;
            font-weight: bold;
        }

        .project-item {
            margin-bottom: 28px;
            padding: 20px;
            background: #f8f9fa;
            border-radius: 8px;
            border-left: 4px solid #764ba2;
        }

        .project-title {
            font-size: 1.1em;
            font-weight: 700;
            color: #2c3e50;
            margin-bottom: 8px;
        }

        .project-tech {
            color: #764ba2;
            font-weight: 600;
            font-size: 0.9em;
            margin-bottom: 10px;
        }

        .project-description {
            color: #555;
            font-size: 0.95em;
            line-height: 1.7;
            list-style: none;
        }

        .project-description li {
            padding: 5px 0;
            padding-left: 20px;
            position: relative;
        }

        .project-description li:before {
            content: "→";
            position: absolute;
            left: 0;
            color: #764ba2;
            font-weight: bold;
        }

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }

        .skill-category {
            background: #f8f9fa;
            padding: 18px;
            border-radius: 8px;
            border-top: 3px solid #667eea;
        }

        .skill-category h4 {
            color: #667eea;
            margin-bottom: 12px;
            font-size: 0.95em;
            font-weight: 700;
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }

        .skill-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
        }

        .skill-tag {
            background: white;
            color: #667eea;
            padding: 6px 12px;
            border-radius: 20px;
            font-size: 0.85em;
            border: 1px solid #667eea;
            font-weight: 500;
            transition: all 0.3s;
        }

        .skill-tag:hover {
            background: #667eea;
            color: white;
        }

        .cert-item {
            padding: 12px 0;
            color: #555;
            font-size: 0.95em;
            padding-left: 20px;
            position: relative;
        }

        .cert-item:before {
            content: "✓";
            position: absolute;
            left: 0;
            color: #667eea;
            font-weight: bold;
        }

        @media (max-width: 768px) {
            .header {
                padding: 40px 25px;
            }

            .header h1 {
                font-size: 2em;
            }

            .content {
                padding: 30px 25px;
            }

            .skills-grid {
                grid-template-columns: 1fr;
            }

            .header .contact {
                gap: 15px;
            }
        }

        @media print {
            body {
                background: white;
                padding: 0;
            }

            .container {
                box-shadow: none;
                border-radius: 0;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Header -->
        <div class="header">
            <h1>Anish Kumar Singh</h1>
            <p class="title">Full Stack Developer | AI/ML Enthusiast | Problem Solver</p>
            <div class="contact">
                <div class="contact-item">
                    <span>📧</span>
                    <a href="mailto:anishsingh210204@gmail.com">anishsingh210204@gmail.com</a>
                </div>
                <div class="contact-item">
                    <span>📱</span>
                    <span>7061186007</span>
                </div>
                <div class="contact-item">
                    <span>🔗</span>
                    <a href="https://linkedin.com/in/anish-ai/">LinkedIn</a>
                </div>
                <div class="contact-item">
                    <span>💻</span>
                    <a href="https://github.com/anishsingh234">GitHub</a>
                </div>
            </div>
        </div>

        <!-- Content -->
        <div class="content">
            <!-- Education -->
            <section class="section">
                <h2 class="section-title">🎓 Education</h2>
                <div class="education-item">
                    <div class="degree">B.Tech. in Computer Science</div>
                    <div class="university">Uttarakhand Technical University, Dehradun</div>
                    <div class="timeline">AI and Machine Learning Specialization | Aug 2022 – Jun 2026</div>
                    <div class="coursework">
                        <strong>Relevant Coursework:</strong> Data Structures & Algorithms, Object-Oriented Programming, Machine Learning, Database Management Systems, Artificial Intelligence, Deep Learning, Natural Language Processing
                    </div>
                </div>
            </section>

            <!-- Experience -->
            <section class="section">
                <h2 class="section-title">💼 Professional Experience</h2>
                <div class="experience-item">
                    <div class="job-title">Full Stack Developer Intern</div>
                    <div class="company">Exponent Solutions | Nov 2025 – Present</div>
                    <ul class="job-description">
                        <li>Developing full-stack web and mobile applications using Next.js and React Native with modern development practices</li>
                        <li>Building responsive frontend interfaces and robust backend services with efficient database architecture</li>
                        <li>Writing comprehensive unit and integration tests ensuring code quality and reliability</li>
                        <li>Designing optimized database schemas and implementing efficient data querying across multiple databases</li>
                        <li>Collaborating with team members to deliver scalable and maintainable solutions</li>
                    </ul>
                </div>
            </section>

            <!-- Projects -->
            <section class="section">
                <h2 class="section-title">🚀 Featured Projects</h2>
                
                <div class="project-item">
                    <div class="project-title">NutriMate – AI Diet Planner</div>
                    <div class="project-tech">React Native | Expo | TypeScript | Gemini AI | React Context</div>
                    <ul class="project-description">
                        <li>Developed cross-platform AI-powered diet planning mobile app for personalized meal recommendations</li>
                        <li>Implemented real-time nutritional tracking system for calories, protein, and carbohydrates</li>
                        <li>Integrated Google Gemini AI API with fallback logic ensuring uninterrupted user experience</li>
                        <li>Ensured secure data handling using Expo Secure Store and optimized UI with React Native Reanimated</li>
                    </ul>
                </div>

                <div class="project-item">
                    <div class="project-title">Trip Bandhu – AI Trip Planner</div>
                    <div class="project-tech">Next.js | ConvexDB | Clerk | shadcn/ui | Gemini AI</div>
                    <ul class="project-description">
                        <li>Built AI-powered platform to create personalized trip timelines and manage travel itineraries</li>
                        <li>Integrated ConvexDB for real-time data storage and Clerk authentication for secure access</li>
                        <li>Implemented AI itinerary generation using Gemini AI 2.0 for day-by-day trip recommendations</li>
                        <li>Designed responsive interface using React, shadcn/ui, and Acernity UI components</li>
                    </ul>
                </div>

                <div class="project-item">
                    <div class="project-title">HealSync – Doctor Appointment Platform</div>
                    <div class="project-tech">Next.js | Prisma ORM | MongoDB | Clerk | Tailwind CSS</div>
                    <ul class="project-description">
                        <li>Developed full-featured platform with booking, cancellation, and consultation management</li>
                        <li>Built comprehensive doctor dashboard with appointment handling and video call integration</li>
                        <li>Implemented admin panel for doctor verification and role-based access control</li>
                        <li>Deployed production-ready application on Vercel with optimized performance</li>
                    </ul>
                </div>

                <div class="project-item">
                    <div class="project-title">DarkStore IMS – Inventory Management System</div>
                    <div class="project-tech">React | Next.js | Prisma | MongoDB | GraphQL | Recharts</div>
                    <ul class="project-description">
                        <li>Built full-stack inventory system with role-based access and real-time dashboards</li>
                        <li>Implemented secure APIs and comprehensive data visualization</li>
                    </ul>
                </div>
            </section>

            <!-- Technical Skills -->
            <section class="section">
                <h2 class="section-title">🛠 Technical Skills</h2>
                <div class="skills-grid">
                    <div class="skill-category">
                        <h4>Languages</h4>
                        <div class="skill-tags">
                            <span class="skill-tag">Python</span>
                            <span class="skill-tag">JavaScript</span>
                            <span class="skill-tag">TypeScript</span>
                            <span class="skill-tag">C++</span>
                            <span class="skill-tag">SQL</span>
                        </div>
                    </div>
                    <div class="skill-category">
                        <h4>Frontend</h4>
                        <div class="skill-tags">
                            <span class="skill-tag">React</span>
                            <span class="skill-tag">Next.js</span>
                            <span class="skill-tag">React Native</span>
                            <span class="skill-tag">Tailwind CSS</span>
                            <span class="skill-tag">shadcn/ui</span>
                        </div>
                    </div>
                    <div class="skill-category">
                        <h4>Backend</h4>
                        <div class="skill-tags">
                            <span class="skill-tag">Node.js</span>
                            <span class="skill-tag">Express.js</span>
                            <span class="skill-tag">GraphQL</span>
                            <span class="skill-tag">Prisma ORM</span>
                        </div>
                    </div>
                    <div class="skill-category">
                        <h4>Databases</h4>
                        <div class="skill-tags">
                            <span class="skill-tag">MongoDB</span>
                            <span class="skill-tag">MySQL</span>
                            <span class="skill-tag">ConvexDB</span>
                        </div>
                    </div>
                    <div class="skill-category">
                        <h4>Tools & Platforms</h4>
                        <div class="skill-tags">
                            <span class="skill-tag">Git</span>
                            <span class="skill-tag">VS Code</span>
                            <span class="skill-tag">Clerk</span>
                            <span class="skill-tag">Vercel</span>
                        </div>
                    </div>
                    <div class="skill-category">
                        <h4>Specializations</h4>
                        <div class="skill-tags">
                            <span class="skill-tag">Machine Learning</span>
                            <span class="skill-tag">AI</span>
                            <span class="skill-tag">NLP</span>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Certifications -->
            <section class="section">
                <h2 class="section-title">📜 Certifications</h2>
                <div class="cert-item">Career Essentials in Generative AI — Microsoft & LinkedIn Learning</div>
                <div class="cert-item">SQL (Basic) — HackerRank</div>
                <div class="cert-item">Java Certificate — HackerRank</div>
            </section>
        </div>
    </div>
</body>
</html>
