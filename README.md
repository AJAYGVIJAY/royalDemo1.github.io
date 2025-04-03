<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ajay Gowripura Vijayakumar | Data Analyst & AI Specialist</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.1/font/bootstrap-icons.css">
    <style>
        :root {
            --primary: #2c3e50;
            --secondary: #3498db;
            --accent: #e74c3c;
            --dark: #2c3e50;
            --light: #f8f9fa;
            --gradient: linear-gradient(135deg, #3498db 0%, #2c3e50 100%);
        }

        body {
            font-family: 'Inter', system-ui, sans-serif;
            line-height: 1.6;
            color: var(--dark);
            background: var(--light);
            scroll-behavior: smooth;
        }

        /* Modern Navigation */
        .navbar {
            background: rgba(44, 62, 80, 0.95) !important;
            backdrop-filter: blur(10px);
            box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
            transition: all 0.3s ease;
        }

        .nav-link {
            position: relative;
            padding: 0.5rem 1.5rem !important;
            transition: all 0.3s ease;
        }

        .nav-link::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            width: 0;
            height: 2px;
            background: var(--secondary);
            transition: all 0.3s ease;
        }

        .nav-link:hover::after {
            width: 60%;
            left: 20%;
        }

        /* Hero Section */
        .hero {
            position: relative;
            padding: 8rem 0;
            background: var(--gradient),
                        url('img/hero-bg.jpg') center/cover;
            color: white;
            overflow: hidden;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.4);
        }

        .profile-img {
            width: 180px;
            height: 180px;
            border: 4px solid white;
            animation: float 6s ease-in-out infinite;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-20px); }
        }

        /* About Section */
        .about-section {
            padding: 5rem 0;
            background: var(--light);
        }

        .skill-badge {
            background: var(--secondary);
            color: white;
            padding: 0.6rem 1.2rem;
            border-radius: 25px;
            transition: all 0.3s ease;
            display: inline-flex;
            align-items: center;
            margin: 0.5rem;
        }

        .skill-badge:hover {
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(52, 152, 219, 0.3);
        }

        /* Experience Section */
        .experience-section {
            padding: 5rem 0;
            background: rgba(249, 249, 249, 0.95);
        }

        .timeline {
            position: relative;
            padding-left: 30px;
        }

        .timeline::before {
            content: '';
            position: absolute;
            left: 10px;
            top: 0;
            height: 100%;
            width: 2px;
            background: linear-gradient(to bottom, var(--secondary), rgba(52, 152, 219, 0.3));
        }

        .timeline-item {
            position: relative;
            margin-bottom: 2rem;
            padding-left: 30px;
            background: white;
            border-radius: 10px;
            padding: 1.5rem;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
        }

        .timeline-item::before {
            content: '';
            position: absolute;
            left: -8px;
            top: 1.5rem;
            width: 16px;
            height: 16px;
            background: var(--light);
            border: 3px solid var(--secondary);
            border-radius: 50%;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
        }

        /* Projects Section */
        .projects-section {
            padding: 5rem 0;
        }

        .project-card {
            border: none;
            border-radius: 15px;
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            overflow: hidden;
            background: white;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.05);
        }

        .project-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 25px rgba(0, 0, 0, 0.1);
        }

        .project-image {
            height: 220px;
            object-fit: cover;
            transition: transform 0.3s ease;
        }

        .project-card:hover .project-image {
            transform: scale(1.05);
        }

        /* Contact Section */
        .contact-section {
            padding: 5rem 0;
            background: var(--gradient);
            color: white;
        }

        .contact-card {
            background: rgba(255, 255, 255, 0.9);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            box-shadow: 0 8px 32px rgba(31, 38, 135, 0.15);
            border: 1px solid rgba(255, 255, 255, 0.18);
            color: var(--dark);
        }

        .btn-cta {
            padding: 0.8rem 1.8rem;
            border-radius: 50px;
            font-weight: 500;
            transition: all 0.3s ease;
            display: inline-flex;
            align-items: center;
        }

        @media (max-width: 768px) {
            .hero {
                padding: 5rem 0;
            }
            .profile-img {
                width: 140px;
                height: 140px;
            }
        }
    </style>
</head>
<body>
    <!-- Navigation -->
    <nav class="navbar navbar-expand-lg navbar-dark fixed-top">
        <div class="container">
            <a class="navbar-brand fw-bold" href="#">AJAY GOWRIPURA VIJAYAKUMAR</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item"><a class="nav-link" href="#about">About</a></li>
                    <li class="nav-item"><a class="nav-link" href="#experience">Experience</a></li>
                    <li class="nav-item"><a class="nav-link" href="#projects">Projects</a></li>
                    <li class="nav-item"><a class="nav-link" href="#contact">Contact</a></li>
                </ul>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <header class="hero">
        <div class="container text-center position-relative">
            <img src="ajayimage.jpeg" alt="Ajay GV" class="profile-img rounded-circle mb-4">
            <h1 class="display-4 fw-bold mb-3">HELLO WORLD! I AM AJAY,</H1>
            <H3>Data Analyst & ML Specialist </H3>
            <div class="d-flex justify-content-center gap-3">
                <a href="#contact" class="btn btn-light btn-lg px-4 py-2">
                    <i class="bi bi-chat-dots me-2"></i>Get in Touch
                </a>
            </div>
        </div>
    </header>

    <!-- About Section -->
    <section id="about" class="about-section">
        <div class="container">
            <div class="row align-items-center">
                <div class="col-lg-6">
                    <h2 class="display-5 fw-bold mb-4">About Me</h2>
                    <p class="lead mb-4">
                        Customer-focused Data Analyst and AI graduate student with expertise in fraud detection, 
                        ETL optimization, and machine learning. Passionate about solving complex problems through 
                        data-driven solutions.
                    </p>
                    <div class="mb-5">
                        <h3 class="h4 fw-bold mb-4">Technical Skills</h3>
                        <div class="d-flex flex-wrap">
                            <span class="skill-badge">SQL</span>
                            <span class="skill-badge">Python</span>
                            <span class="skill-badge">Machine Learning</span>
                            <span class="skill-badge">Data Mining</span>
                            <span class="skill-badge">Power BI/Tableau</span>
                            <span class="skill-badge">Data Visualization</span> 
                            <span class="skill-badge">Maths and Statistics</span>
                            <span class="skill-badge">Customer Service and Communication</span>
                        </div>
                    </div>
                </div>
                <div class="col-lg-6">
                    <div class="timeline">
                        <h2 class="h5 fw-bold">Education</h2>
                        <div class="timeline-item">
                            
                            <div class="timeline-content">
                                <h4 class="h6 text-primary">MSc Data Science & AI</h4>
                                <p class="mb-1">University of Liverpool</p>
                                
                                <small class="text-muted">2023 - 2025</small>
                                <p>Key Modules: Machine Learning and Bioinspired Optimisation, Data Mining, Data Visualisation, Database and
                                    information system, Maths and Statistics, and Python programming.</p>
                            </div>
                        </div>
                        <div class="timeline-item">
                            <div class="timeline-content">
                                <h4 class="h6 text-primary">Bachelors in Engineering</h4>
                                <p class="mb-1">University BDT College of Engineering</p>
                                <small class="text-muted">2018 - 2022</small>
                                <p>Key Modules: Engineering Mathematics, Statistics, Computer Programming, Analytics, Reasoning, Documenting.</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Experience Section -->
    <section id="experience" class="experience-section">
        <div class="container">
            <h2 class="display-5 fw-bold text-center mb-5">Professional Experience</h2>
            
            <div class="row">
                <div class="col-lg-8 mx-auto">
                    <div class="timeline">
                        <!-- Infosys Experience -->
                        <div class="timeline-item">
                            <div class="timeline-header">
                                <h3 class="h5 fw-bold">Data & Systems Analyst</h3>
                                <p class="text-muted mb-2">Infosys Limited | Aug 2022 - Sep 2023</p>
                            </div>
                            <ul class="list-unstyled">
                                <li class="mb-2">
                                    <i class="bi bi-check-circle-fill text-primary me-2"></i>
                                    Reduced system incidents by 65% through SQL-driven root cause analysis
                                </li>
                                <li class="mb-2">
                                    <i class="bi bi-check-circle-fill text-primary me-2"></i>
                                    Boosted data retrieval speed by 28% via automated workflows
                                </li>
                                <li class="mb-2">
                                    <i class="bi bi-check-circle-fill text-primary me-2"></i>
                                    Developed ETL processes ensuring 99.8% data accuracy
                                </li>
                            </ul>
                        </div>

                        <!-- Sainsbury's Experience -->
                        <div class="timeline-item">
                            <div class="timeline-header">
                                <h3 class="h5 fw-bold">Online Retail Assistant</h3>
                                <p class="text-muted mb-2">Sainsbury’s Argos | Oct 2023 - Present</p>
                            </div>
                            <ul class="list-unstyled">
                                <li class="mb-2">
                                    <i class="bi bi-check-circle-fill text-primary me-2"></i>
                                    Optimized inventory tracking reducing stockouts by 40%
                                </li>
                                <li class="mb-2">
                                    <i class="bi bi-check-circle-fill text-primary me-2"></i>
                                    Processed 100+ daily transactions with 99.9% accuracy
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
<!-- Projects Section -->
<!-- Projects Section -->
<section id="projects" class="projects-section">
    <div class="container">
        <h2 class="display-5 fw-bold text-center mb-5">Featured Projects</h2>
        <div class="row g-4">
            <!-- Credit Card Fraud Detection -->
            <div class="col-md-4">
                <div class="project-card h-100">
                    <img src="creditcardimage.png" class="card-img-top project-image" alt="Fraud Detection System">
                    <div class="card-body">
                        <h3 class="h5 fw-bold mb-3">Credit Card Fraud Detection System</h3>
                        <div class="d-flex flex-wrap gap-2 mb-4">
                            <span class="badge bg-primary">Machine Learning</span>
                            <span class="badge bg-primary">Anomaly Detection</span>
                            <span class="badge bg-primary">Imbalanced Data</span>
                        </div>
                        
                        <div class="achievements mb-4">
                            <div class="d-flex gap-3 mb-3">
                                <div class="text-center">
                                    <div class="h4 text-primary">99.96%</div>
                                    <small class="text-muted">Accuracy</small>
                                </div>
                                <div class="text-center">
                                    <div class="h4 text-primary">94.12%</div>
                                    <small class="text-muted">Precision</small>
                                </div>
                                <div class="text-center">
                                    <div class="h4 text-primary">81.63%</div>
                                    <small class="text-muted">Recall</small>
                                </div>
                            </div>
                            
                            <ul class="list-unstyled">
                                <li class="mb-2">
                                    <i class="bi bi-check-circle text-primary me-2"></i>
                                    Hybrid ensemble model combining Isolation Forest and XGBoost
                                </li>
                                <li class="mb-2">
                                    <i class="bi bi-check-circle text-primary me-2"></i>
                                    SMOTE oversampling for class imbalance
                                </li>
                                <li class="mb-2">
                                    <i class="bi bi-check-circle text-primary me-2"></i>
                                    ROC-AUC score of 0.9081 achieved
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Material Science Prediction -->
            <div class="col-md-4">
                <div class="project-card h-100">
                    <img src="materialscienceimage.png" class="card-img-top project-image" alt="Material Science Analysis">
                    <div class="card-body">
                        <h3 class="h5 fw-bold mb-3">Material Property Prediction</h3>
                        <div class="d-flex flex-wrap gap-2 mb-4">
                            <span class="badge bg-primary">Deep Learning</span>
                            <span class="badge bg-primary">Materials Science</span>
                            <span class="badge bg-primary">MAE Optimization</span>
                        </div>
                        
                        <div class="achievements mb-4">
                            <div class="d-flex gap-3 mb-3">
                                <div class="text-center">
                                    <div class="h4 text-primary">R² 0.999</div>
                                    <small class="text-muted">Model Fit</small>
                                </div>
                                <div class="text-center">
                                    <div class="h4 text-primary">MAE 6.35e-5</div>
                                    <small class="text-muted">Prediction Error</small>
                                </div>
                                <div class="text-center">
                                    <div class="h4 text-primary">58%</div>
                                    <small class="text-muted">Performance Gain</small>
                                </div>
                            </div>
                            
                            <ul class="list-unstyled">
                                <li class="mb-2">
                                    <i class="bi bi-check-circle text-primary me-2"></i>
                                    Geometric deep learning models for crystals
                                </li>
                                <li class="mb-2">
                                    <i class="bi bi-check-circle text-primary me-2"></i>
                                    Novel XRD feature engineering pipeline
                                </li>
                                <li class="mb-2">
                                    <i class="bi bi-check-circle text-primary me-2"></i>
                                    58% better than classical methods
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Car Price Prediction -->
            <div class="col-md-4">
                <div class="project-card h-100">
                    <img src="carpriceimage.png" class="card-img-top project-image" alt="Car Price Prediction">
                    <div class="card-body">
                        <h3 class="h5 fw-bold mb-3">Car Price Prediction System</h3>
                        <div class="d-flex flex-wrap gap-2 mb-4">
                            <span class="badge bg-primary">Machine Learning</span>
                            <span class="badge bg-primary">Regression Analysis</span>
                            <span class="badge bg-primary">Feature Engineering</span>
                        </div>
                        
                        <div class="achievements mb-4">
                            <div class="d-flex gap-3 mb-3">
                                <div class="text-center">
                                    <div class="h4 text-primary">96%</div>
                                    <small class="text-muted">R² Score</small>
                                </div>
                                <div class="text-center">
                                    <div class="h4 text-primary">$2,914</div>
                                    <small class="text-muted">MAE</small>
                                </div>
                                <div class="text-center">
                                    <div class="h4 text-primary">4.8/5</div>
                                    <small class="text-muted">Generalization</small>
                                </div>
                            </div>
                            
                            <ul class="list-unstyled">
                                <li class="mb-2">
                                    <i class="bi bi-check-circle text-primary me-2"></i>
                                    Hybrid ensemble model using XGBoost
                                </li>
                                <li class="mb-2">
                                    <i class="bi bi-check-circle text-primary me-2"></i>
                                    Advanced feature engineering pipeline
                                </li>
                                <li class="mb-2">
                                    <i class="bi bi-check-circle text-primary me-2"></i>
                                    Outlier detection and imbalance handling
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</section>

    <!-- Contact Section -->
    <section id="contact" class="contact-section">
        <div class="container">
            <div class="row justify-content-center">
                <div class="col-lg-8">
                    <div class="contact-card p-4">
                        <div class="text-center mb-5">
                            <h2 class="display-5 fw-bold mb-3">Let's Connect</h2>
                            <p class="lead">Open to collaborations and new opportunities</p>
                        </div>
                        
                        <div class="d-flex flex-wrap justify-content-center gap-3">
                            <!-- Email -->
                            <a href="mailto:ajaygowripuravijayakumar@gmail.com" 
                               class="btn btn-primary btn-cta"
                               target="_blank"
                               rel="noopener">
                               <i class="bi bi-envelope-at me-2"></i>Email Me
                            </a>

                            <!-- LinkedIn -->
                            <a href="https://linkedin.com/in/ajaygv" 
                               class="btn btn-primary btn-cta"
                               target="_blank"
                               rel="noopener noreferrer">
                               <i class="bi bi-linkedin me-2"></i>LinkedIn
                            </a>

                            <!-- Resume -->
                            <a href="https://drive.google.com/uc?export=download&id=YOUR_FILE_ID" 
                               class="btn btn-success btn-cta"
                               download>
                               <i class="bi bi-file-earmark-pdf me-2"></i>Download CV
                            </a>
                        </div>

                        <!-- Contact Info -->
                        <div class="text-center mt-5">
                            <div class="d-flex flex-column gap-2">
                                <div class="h5">
                                    <i class="bi bi-geo-alt me-2"></i>Liverpool, UK
                                </div>
                                <div class="h5">
                                    <i class="bi bi-phone me-2"></i>+44 7549 078291
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
    <script>
        // Smooth scroll functionality
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });

        // Intersection Observer for animations
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                }
            });
        }, { threshold: 0.1 });

        document.querySelectorAll('.timeline-item, .project-card').forEach((el) => {
            observer.observe(el);
        });
    </script>
</body>
</html>
