<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Muhammad Hamza Nawaz - AI Engineer</title>
    <style>
        :root {
            --primary: #2563eb;
            --secondary: #7e22ce;
            --accent: #f43f5e;
            --dark: #1e293b;
            --light: #f8fafc;
            --gray: #64748b;
            --gradient: linear-gradient(135deg, var(--primary), var(--secondary));
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: #0f172a;
            color: var(--light);
            line-height: 1.6;
            padding: 0;
            margin: 0;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        /* Header Section */
        .header {
            text-align: center;
            padding: 40px 20px;
            background: linear-gradient(to bottom, #0f172a, #1e293b);
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
            position: relative;
            overflow: hidden;
        }
        
        .header::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 1px;
            background: var(--gradient);
        }
        
        .profile-title {
            font-size: 2.5rem;
            margin-bottom: 10px;
            background: var(--gradient);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            font-weight: 700;
        }
        
        .profile-subtitle {
            font-size: 1.2rem;
            color: var(--gray);
            margin-bottom: 20px;
            max-width: 700px;
            margin-left: auto;
            margin-right: auto;
        }
        
        .typing-animation {
            font-size: 1.5rem;
            font-weight: 600;
            margin: 20px 0;
            min-height: 60px;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        /* Social Links */
        .social-links {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin: 20px 0;
            flex-wrap: wrap;
        }
        
        .social-btn {
            display: inline-flex;
            align-items: center;
            padding: 10px 20px;
            background: rgba(255, 255, 255, 0.05);
            border: 1px solid rgba(255, 255, 255, 0.1);
            border-radius: 50px;
            color: var(--light);
            text-decoration: none;
            transition: all 0.3s ease;
            backdrop-filter: blur(10px);
        }
        
        .social-btn:hover {
            background: rgba(255, 255, 255, 0.1);
            transform: translateY(-2px);
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
        }
        
        .social-btn i {
            margin-right: 8px;
        }
        
        /* Section Styling */
        .section {
            margin: 40px 0;
            padding: 30px;
            background: rgba(30, 41, 59, 0.5);
            border-radius: 16px;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.05);
            box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
        }
        
        .section-title {
            font-size: 1.8rem;
            margin-bottom: 25px;
            position: relative;
            padding-bottom: 10px;
            color: var(--light);
        }
        
        .section-title::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 60px;
            height: 3px;
            background: var(--gradient);
            border-radius: 3px;
        }
        
        /* Tech Stack */
        .tech-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 20px;
        }
        
        .tech-category {
            background: rgba(255, 255, 255, 0.03);
            padding: 20px;
            border-radius: 12px;
            border: 1px solid rgba(255, 255, 255, 0.05);
        }
        
        .tech-category h3 {
            font-size: 1.2rem;
            margin-bottom: 15px;
            color: var(--light);
            display: flex;
            align-items: center;
        }
        
        .tech-category h3 i {
            margin-right: 10px;
            color: var(--accent);
        }
        
        .tech-icons {
            display: flex;
            flex-wrap: wrap;
            gap: 15px;
        }
        
        .tech-item {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            width: 70px;
            height: 70px;
            background: rgba(255, 255, 255, 0.03);
            border-radius: 12px;
            transition: all 0.3s ease;
            border: 1px solid rgba(255, 255, 255, 0.05);
        }
        
        .tech-item:hover {
            transform: translateY(-5px);
            background: rgba(255, 255, 255, 0.08);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }
        
        .tech-item img {
            width: 30px;
            height: 30px;
            object-fit: contain;
        }
        
        .tech-item span {
            font-size: 0.7rem;
            margin-top: 5px;
            text-align: center;
            color: var(--gray);
        }
        
        /* Projects */
        .project-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 25px;
        }
        
        .project-card {
            background: rgba(255, 255, 255, 0.03);
            border-radius: 12px;
            padding: 20px;
            border: 1px solid rgba(255, 255, 255, 0.05);
            transition: all 0.3s ease;
            height: 100%;
            display: flex;
            flex-direction: column;
        }
        
        .project-card:hover {
            transform: translateY(-5px);
            background: rgba(255, 255, 255, 0.06);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.2);
        }
        
        .project-title {
            font-size: 1.2rem;
            margin-bottom: 10px;
            color: var(--light);
        }
        
        .project-desc {
            color: var(--gray);
            flex-grow: 1;
            margin-bottom: 15px;
        }
        
        .project-link {
            color: var(--primary);
            text-decoration: none;
            font-weight: 500;
            display: inline-flex;
            align-items: center;
        }
        
        .project-link:hover {
            text-decoration: underline;
        }
        
        /* Stats */
        .stats-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }
        
        .stat-card {
            background: rgba(255, 255, 255, 0.03);
            border-radius: 12px;
            padding: 20px;
            text-align: center;
            border: 1px solid rgba(255, 255, 255, 0.05);
        }
        
        .stat-number {
            font-size: 2rem;
            font-weight: 700;
            background: var(--gradient);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            margin-bottom: 10px;
        }
        
        .stat-label {
            color: var(--gray);
            font-size: 0.9rem;
        }
        
        /* Footer */
        .footer {
            text-align: center;
            padding: 40px 20px;
            margin-top: 60px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            color: var(--gray);
        }
        
        .connect-title {
            font-size: 1.5rem;
            margin-bottom: 20px;
            color: var(--light);
        }
        
        /* Responsive Design */
        @media (max-width: 768px) {
            .profile-title {
                font-size: 2rem;
            }
            
            .typing-animation {
                font-size: 1.2rem;
                min-height: 50px;
            }
            
            .tech-grid {
                grid-template-columns: 1fr;
            }
            
            .project-grid {
                grid-template-columns: 1fr;
            }
            
            .section {
                padding: 20px;
            }
        }
        
        /* Low GPU mode adjustments */
        .low-gpu-mode {
            /* Simplify animations and effects for low-power devices */
            backdrop-filter: none !important;
            box-shadow: none !important;
            transform: none !important;
        }
        
        /* Animation for typing effect */
        @keyframes typing {
            from { width: 0; }
            to { width: 100%; }
        }
        
        .typewriter {
            overflow: hidden;
            border-right: .15em solid var(--accent);
            white-space: nowrap;
            margin: 0 auto;
            letter-spacing: .05em;
            animation: typing 3.5s steps(40, end), blink-caret .75s step-end infinite;
        }
        
        @keyframes blink-caret {
            from, to { border-color: transparent; }
            50% { border-color: var(--accent); }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Header Section -->
        <header class="header">
            <h1 class="profile-title">Muhammad Hamza Nawaz</h1>
            <p class="profile-subtitle">AI Engineer | ML Specialist | Python Developer</p>
            
            <div class="typing-animation">
                <div class="typewriter">Always learning new things 🚀</div>
            </div>
            
            <div class="social-links">
                <a href="https://linkedin.com/in/muhammad-hamza-nawaz-a434501b3" class="social-btn">
                    <i>👔</i> LinkedIn
                </a>
                <a href="mailto:iamhamzanawaz14@gmail.com" class="social-btn">
                    <i>📧</i> Email
                </a>
                <a href="https://www.kaggle.com/muhammadhamzanawaz" class="social-btn">
                    <i>🏆</i> Kaggle
                </a>
                <a href="http://iamhamzanawaz.online" class="social-btn">
                    <i>🌐</i> Portfolio
                </a>
            </div>
        </header>

        <!-- Tech Stack Section -->
        <section class="section">
            <h2 class="section-title">🛠 Tech Toolbox</h2>
            
            <div class="tech-grid">
                <div class="tech-category">
                    <h3><i>💻</i> Languages</h3>
                    <div class="tech-icons">
                        <div class="tech-item">
                            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" alt="Python">
                            <span>Python</span>
                        </div>
                        <div class="tech-item">
                            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/cplusplus/cplusplus-original.svg" alt="C++">
                            <span>C++</span>
                        </div>
                        <div class="tech-item">
                            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mysql/mysql-original.svg" alt="SQL">
                            <span>SQL</span>
                        </div>
                    </div>
                </div>
                
                <div class="tech-category">
                    <h3><i>🤖</i> Machine Learning</h3>
                    <div class="tech-icons">
                        <div class="tech-item">
                            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/tensorflow/tensorflow-original.svg" alt="TensorFlow">
                            <span>TensorFlow</span>
                        </div>
                        <div class="tech-item">
                            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/pytorch/pytorch-original.svg" alt="PyTorch">
                            <span>PyTorch</span>
                        </div>
                        <div class="tech-item">
                            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/opencv/opencv-original.svg" alt="OpenCV">
                            <span>OpenCV</span>
                        </div>
                    </div>
                </div>
                
                <div class="tech-category">
                    <h3><i>📊</i> Data Processing</h3>
                    <div class="tech-icons">
                        <div class="tech-item">
                            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/pandas/pandas-original.svg" alt="Pandas">
                            <span>Pandas</span>
                        </div>
                        <div class="tech-item">
                            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/numpy/numpy-original.svg" alt="NumPy">
                            <span>NumPy</span>
                        </div>
                    </div>
                </div>
                
                <div class="tech-category">
                    <h3><i>⚡</i> Deployment & Tools</h3>
                    <div class="tech-icons">
                        <div class="tech-item">
                            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/flask/flask-original.svg" alt="Flask">
                            <span>Flask</span>
                        </div>
                        <div class="tech-item">
                            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/docker/docker-original.svg" alt="Docker">
                            <span>Docker</span>
                        </div>
                        <div class="tech-item">
                            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" alt="Git">
                            <span>Git</span>
                        </div>
                        <div class="tech-item">
                            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/amazonwebservices/amazonwebservices-original.svg" alt="AWS">
                            <span>AWS</span>
                        </div>
                        <div class="tech-item">
                            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/googlecloud/googlecloud-original.svg" alt="Google Cloud">
                            <span>GCP</span>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Projects Section -->
        <section class="section">
            <h2 class="section-title">🚀 What I'm Working On</h2>
            
            <div class="project-grid">
                <div class="project-card">
                    <h3 class="project-title">Advanced Object Detection System</h3>
                    <p class="project-desc">Real-time YOLOv7 + TensorRT implementation for high-performance object detection.</p>
                    <a href="https://github.com/yourusername/object-detection" class="project-link">View Project →</a>
                </div>
                
                <div class="project-card">
                    <h3 class="project-title">Automated ML Pipeline</h3>
                    <p class="project-desc">End-to-end ML workflow automation with hyperparameter tuning and model evaluation.</p>
                    <a href="https://github.com/yourusername/automl-pipeline" class="project-link">View Project →</a>
                </div>
                
                <div class="project-card">
                    <h3 class="project-title">AI-Powered Chatbot</h3>
                    <p class="project-desc">Transformer-based conversational assistant with custom knowledge integration.</p>
                    <a href="https://github.com/yourusername/ai-chatbot" class="project-link">View Project →</a>
                </div>
            </div>
        </section>

        <!-- Learning Section -->
        <section class="section">
            <h2 class="section-title">📚 Currently Learning</h2>
            
            <div class="stats-container">
                <div class="stat-card">
                    <div class="stat-number">Edge AI</div>
                    <div class="stat-label">Optimizing models for low-power devices</div>
                </div>
                
                <div class="stat-card">
                    <div class="stat-number">MLOps</div>
                    <div class="stat-label">Best practices for ML operations</div>
                </div>
                
                <div class="stat-card">
                    <div class="stat-number">Quantum ML</div>
                    <div class="stat-label">Exploring quantum computing for ML</div>
                </div>
            </div>
        </section>

        <!-- Stats Section -->
        <section class="section">
            <h2 class="section-title">📈 GitHub Stats</h2>
            
            <div class="stats-container">
                <div class="stat-card">
                    <div class="stat-number" id="repo-count">20+</div>
                    <div class="stat-label">Repositories</div>
                </div>
                
                <div class="stat-card">
                    <div class="stat-number" id="commit-count">500+</div>
                    <div class="stat-label">Commits</div>
                </div>
                
                <div class="stat-card">
                    <div class="stat-number" id="star-count">100+</div>
                    <div class="stat-label">Stars Earned</div>
                </div>
                
                <div class="stat-card">
                    <div class="stat-number" id="contributor-count">10+</div>
                    <div class="stat-label">Contributions</div>
                </div>
            </div>
            
            <div style="margin-top: 30px; text-align: center;">
                <img src="https://github-readme-stats.vercel.app/api?username=hamzanawazsangha&show_icons=true&theme=radical" alt="GitHub Stats" style="max-width: 100%; border-radius: 10px;">
                <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=hamzanawazsangha&layout=compact&theme=radical" alt="Top Languages" style="max-width: 100%; border-radius: 10px; margin-top: 20px;">
            </div>
        </section>

        <!-- Footer -->
        <footer class="footer">
            <h3 class="connect-title">📬 Let's Connect</h3>
            
            <div class="social-links">
                <a href="mailto:iamhamzanawaz14@gmail.com" class="social-btn">
                    <i>📧</i> iamhamzanawaz14@gmail.com
                </a>
                <a href="https://linkedin.com/in/muhammad-hamza-nawaz-a434501b3" class="social-btn">
                    <i>👔</i> LinkedIn
                </a>
                <a href="http://iamhamzanawaz.online" class="social-btn">
                    <i>🌐</i> Portfolio Website
                </a>
            </div>
            
            <p style="margin-top: 30px;">© 2023 Muhammad Hamza Nawaz. All rights reserved.</p>
        </footer>
    </div>

    <script>
        // Detect GPU capability and adjust UI accordingly
        function detectGPU() {
            try {
                const canvas = document.createElement('canvas');
                const gl = canvas.getContext('webgl') || canvas.getContext('experimental-webgl');
                
                if (!gl) {
                    return 'none';
                }
                
                const debugInfo = gl.getExtension('WEBGL_debug_renderer_info');
                const renderer = debugInfo ? gl.getParameter(debugInfo.UNMASKED_RENDERER_WEBGL) : 'unknown';
                
                // Check if it's a low-performance GPU
                const lowGpuKeywords = ['intel', 'hd graphics', 'iris', 'uhd graphics', 'mali', 'adreno', 'software', 'llvmpipe'];
                const isLowGpu = lowGpuKeywords.some(keyword => renderer.toLowerCase().includes(keyword));
                
                return isLowGpu ? 'low' : 'high';
            } catch (e) {
                return 'unknown';
            }
        }
        
        // Apply appropriate UI mode based on GPU capability
        function applyGPUMode() {
            const gpuCapability = detectGPU();
            
            if (gpuCapability === 'low') {
                document.body.classList.add('low-gpu-mode');
                console.log('Low GPU mode activated for better performance');
            }
        }
        
        // Initialize
        window.addEventListener('load', function() {
            applyGPUMode();
            
            // Simple animation for stats counting (GPU friendly)
            const stats = [
                { id: 'repo-count', target: 24, duration: 2000 },
                { id: 'commit-count', target: 587, duration: 2500 },
                { id: 'star-count', target: 134, duration: 2000 },
                { id: 'contributor-count', target: 16, duration: 1500 }
            ];
            
            stats.forEach(stat => {
                const element = document.getElementById(stat.id);
                if (!element) return;
                
                let start = 0;
                const increment = stat.target / (stat.duration / 16);
                
                const updateCount = () => {
                    start += increment;
                    if (start < stat.target) {
                        element.textContent = Math.round(start) + '+';
                        requestAnimationFrame(updateCount);
                    } else {
                        element.textContent = stat.target + '+';
                    }
                };
                
                requestAnimationFrame(updateCount);
            });
        });
    </script>
</body>
</html>
