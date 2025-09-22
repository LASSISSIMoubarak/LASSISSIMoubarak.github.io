<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Moubarak LASSISSI - Data Scientist</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary-color: #2c3e50;
            --secondary-color: #3498db;
            --accent-color: #e74c3c;
            --light-color: #ecf0f1;
            --dark-color: #2c3e50;
            --text-color: #333;
            --transition: all 0.3s ease;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: var(--text-color);
            background-color: #f9f9f9;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        header {
            background: linear-gradient(135deg, var(--primary-color) 0%, var(--dark-color) 100%);
            color: white;
            padding: 2rem 0;
            position: relative;
        }
        
        .header-content {
            display: flex;
            align-items: center;
            justify-content: space-between;
            flex-wrap: wrap;
        }
        
        .profile-img {
            width: 180px;
            height: 180px;
            border-radius: 50%;
            object-fit: cover;
            border: 5px solid rgba(255, 255, 255, 0.3);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }
        
        .profile-text {
            flex: 1;
            padding: 0 2rem;
            min-width: 300px;
        }
        
        h1 {
            font-size: 2.5rem;
            margin-bottom: 0.5rem;
        }
        
        .tagline {
            font-size: 1.2rem;
            font-weight: 300;
            margin-bottom: 1rem;
            color: var(--light-color);
        }
        
        .social-links {
            display: flex;
            gap: 1rem;
            margin-top: 1rem;
        }
        
        .social-links a {
            color: white;
            font-size: 1.5rem;
            transition: var(--transition);
        }
        
        .social-links a:hover {
            color: var(--secondary-color);
            transform: translateY(-3px);
        }
        
        section {
            padding: 3rem 0;
        }
        
        section:nth-child(even) {
            background-color: white;
        }
        
        h2 {
            font-size: 2rem;
            margin-bottom: 2rem;
            color: var(--primary-color);
            position: relative;
            padding-bottom: 0.5rem;
        }
        
        h2::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 60px;
            height: 3px;
            background-color: var(--secondary-color);
        }
        
        .card {
            background: white;
            border-radius: 8px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            padding: 1.5rem;
            margin-bottom: 1.5rem;
            transition: var(--transition);
            border-left: 4px solid var(--secondary-color);
        }
        
        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.15);
        }
        
        .card h3 {
            color: var(--primary-color);
            margin-bottom: 0.5rem;
            font-size: 1.3rem;
        }
        
        .card .date {
            color: var(--secondary-color);
            font-weight: 500;
            margin-bottom: 0.5rem;
        }
        
        .skills-container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 1.5rem;
        }
        
        .skill-category {
            background: white;
            padding: 1.5rem;
            border-radius: 8px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
        .skill-category h3 {
            color: var(--primary-color);
            margin-bottom: 1rem;
            font-size: 1.3rem;
        }
        
        .skill-list {
            display: flex;
            flex-wrap: wrap;
            gap: 0.8rem;
        }
        
        .skill-item {
            background: var(--light-color);
            padding: 0.5rem 1rem;
            border-radius: 20px;
            font-size: 0.9rem;
            transition: var(--transition);
        }
        
        .skill-item:hover {
            background: var(--secondary-color);
            color: white;
            transform: translateY(-3px);
        }
        
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(350px, 1fr));
            gap: 2rem;
        }
        
        .project-card {
            background: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: var(--transition);
        }
        
        .project-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.15);
        }
        
        .project-content {
            padding: 1.5rem;
        }
        
        .project-card h3 {
            color: var(--primary-color);
            margin-bottom: 0.5rem;
        }
        
        .project-meta {
            color: var(--secondary-color);
            font-size: 0.9rem;
            margin-bottom: 1rem;
        }
        
        .project-meta a {
            color: var(--secondary-color);
            text-decoration: none;
        }

        .project-meta a:hover {
            text-decoration: underline;
        }

        .languages-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 1.5rem;
        }
        
        .language-item {
            display: flex;
            align-items: center;
            background: white;
            padding: 1rem;
            border-radius: 8px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
        .language-icon {
            font-size: 1.8rem;
            margin-right: 1rem;
            color: var(--secondary-color);
        }
        
        .contact-info {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 1.5rem;
        }
        
        .contact-item {
            display: flex;
            align-items: center;
            background: white;
            padding: 1.5rem;
            border-radius: 8px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: var(--transition);
        }
        
        .contact-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.15);
        }
        
        .contact-icon {
            font-size: 2rem;
            margin-right: 1rem;
            color: var(--secondary-color);
        }

        .contact-item a {
            color: var(--primary-color);
            text-decoration: none;
        }

        .contact-item a:hover {
            text-decoration: underline;
            color: var(--secondary-color);
        }
        
        footer {
            background: var(--dark-color);
            color: white;
            text-align: center;
            padding: 2rem 0;
            margin-top: 2rem;
        }
        
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                text-align: center;
            }
            
            .profile-text {
                padding: 1rem 0;
            }
            
            .social-links {
                justify-content: center;
            }
            
            h1 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <div class="header-content">
                <img src="Moubarak.png" alt="Moubarak LASSISSI" class="profile-img">
                <div class="profile-text">
                    <h1>Moubarak LASSISSI</h1>
                    <p class="tagline">Data Scientist specialized in statistical engineering, machine learning and deep learning</p>
                    <p>Expert in processing complex datasets (oceanographic, biological, transportation) and skilled in advanced modeling (ML/DL), Big Data, and data quality assurance.</p>
                    <div class="social-links">
                        <a href="https://www.linkedin.com/in/moubarak-lassissi-610b87202" target="_blank"><i class="fab fa-linkedin"></i></a>
                        <a href="https://github.com/LASSISSIMoubarak/LASSISSIMoubarak" target="_blank"><i class="fab fa-github"></i></a>
                        <a href="mailto:lassissimoubarak20@gmail.com"><i class="fas fa-envelope"></i></a>
                    </div>
                </div>
            </div>
        </div>
    </header>

    <section id="projects">
        <div class="container">
            <h2>Projects</h2>
            <div class="projects-grid">
                <div class="project-card">
                    <div class="project-content">
                        <h3>Traffic Prediction using Functional Data</h3>
                        <p class="project-meta"><i class="fas fa-file-code"></i> 
                           <a href="https://github.com/LASSISSIMoubarak/LASSISSIMoubarak/blob/main/datachalenge.py" target="_blank">datachallenge.py</a>
                        </p>
                        <p>Prediction of transport card validations (passenger flow) using functional data analysis.</p>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-content">
                        <h3>Kernel Approximation for Faster Machine Learning</h3>
                        <p class="project-meta"><i class="fas fa-file-code"></i> 
                           <a href="https://github.com/LASSISSIMoubarak/LASSISSIMoubarak/blob/main/Kernel_approximation.ipynb" target="_blank">kernel_approximation.ipynb</a>
                        </p>
                        <p>Implementation of Random Fourier Features to speed up kernel-based methods.</p>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-content">
                        <h3>CNN for Image Classification</h3>
                        <p class="project-meta"><i class="fas fa-file-code"></i> 
                           <a href="https://github.com/LASSISSIMoubarak/LASSISSIMoubarak/blob/main/TP_CNN.ipynb" target="_blank">TP_CNN.ipynb</a>
                        </p>
                        <p>Simple CNN architecture for multiclass image classification.</p>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-content">
                        <h3>Functional Data Clustering</h3>
                        <p class="project-meta"><i class="fas fa-university"></i> University of Nantes</p>
                        <p>Implementation and evaluation of clustering methods applied to functional data.</p>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-content">
                        <h3>Multivariate ANOVA and Multi-block Analysis</h3>
                        <p class="project-meta"><i class="fas fa-file-code"></i> 
                           <a href="https://github.com/LASSISSIMoubarak/LASSISSIMoubarak/blob/main/ANOVA%20MULT%20SENSO%20ET%20VOLA.R" target="_blank">ANOVA_MULT_SENSO_ET_VOLA.R</a>
                        </p>
                        <p>Application of advanced statistical methods to multivariate biological data.</p>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-content">
                      <h3>Bayesian Model (Mediation)</h3>
                      <p class="project-meta">
                        <i class="fas fa-file-code"></i> 
                        <a href="https://github.com/LASSISSIMoubarak/LASSISSIMoubarak/blob/main/Projet%20_stat_bayes_stan.R" target="_blank">
                            Stan_Bayesian_model.R
                        </a>
                        </p>
                        <p>
                        Bayesian mediation analysis to assess how the perceived risk of contracting Covid influences the population’s beliefs. 
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="contact">
        <div class="container">
            <h2>Contact</h2>
            <div class="contact-info">
                <div class="contact-item">
                    <i class="fas fa-envelope contact-icon"></i>
                    <div>
                        <h3>Email</h3>
                        <p><a href="mailto:lassissimoubarak20@gmail.com">lassissimoubarak20@gmail.com</a></p>
                    </div>
                </div>

                <div class="contact-item">
                    <i class="fab fa-linkedin contact-icon"></i>
                    <div>
                        <h3>LinkedIn</h3>
                        <p><a href="https://www.linkedin.com/in/moubarak-lassissi-610b87202" target="_blank">linkedin.com/in/moubarak-lassissi-610b87202</a></p>
                    </div>
                </div>

                <div class="contact-item">
                    <i class="fab fa-github contact-icon"></i>
                    <div>
                        <h3>GitHub</h3>
                        <p><a href="https://github.com/LASSISSIMoubarak/LASSISSIMoubarak" target="_blank">github.com/LASSISSIMoubarak</a></p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <footer>
        <div class="container">
            <p>&copy; 2025 Moubarak LASSISSI - Data Scientist</p>
        </div>
    </footer>
</body>
</html>
