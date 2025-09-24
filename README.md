<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Diiba's World - Inspiration & Creativity</title>
    <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@400;700&family=Inter:wght@300;400;500&display=swap" rel="stylesheet">
    <style>
        :root {
            --white: #FFFFFF;
            --beige: #F5F5DC;
            --cream: #FFFDD0;
            --light-peach: #FFDAB9;
            --pink: #FFC0CB;
            --text-dark: #4A4A4A;
            --text-light: #7A7A7A;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Inter', sans-serif;
            line-height: 1.6;
            color: var(--text-dark);
            background: radial-gradient(circle at 20% 30%, rgba(255, 218, 185, 0.3) 0%, transparent 20%),
                        radial-gradient(circle at 80% 70%, rgba(255, 192, 203, 0.3) 0%, transparent 20%),
                        radial-gradient(circle at 40% 80%, rgba(255, 245, 220, 0.3) 0%, transparent 20%),
                        var(--white);
            overflow-x: hidden;
            min-height: 100vh;
        }
        
        h1, h2, h3 {
            font-family: 'Dancing Script', cursive;
            color: var(--text-dark);
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Header Styles */
        header {
            background: var(--cream);
            padding: 1rem 0;
            position: sticky;
            top: 0;
            z-index: 100;
            box-shadow: 0 2px 10px rgba(0,0,0,0.05);
        }
        
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-family: 'Dancing Script', cursive;
            font-size: 2rem;
            color: var(--text-dark);
            text-decoration: none;
            font-weight: 700;
        }
        
        nav ul {
            display: flex;
            list-style: none;
            gap: 2rem;
        }
        
        nav a {
            text-decoration: none;
            color: var(--text-dark);
            font-weight: 500;
            transition: color 0.3s;
        }
        
        nav a:hover {
            color: var(--light-peach);
        }
        
        /* Hero Section */
        .hero {
            background: linear-gradient(to bottom, var(--beige), var(--cream));
            padding: 4rem 0;
            position: relative;
            overflow: hidden;
        }
        
        .hero-content {
            display: flex;
            flex-wrap: wrap;
            align-items: center;
            gap: 3rem;
            position: relative;
            z-index: 2;
        }
        
        .hero-image {
            flex: 1;
            min-width: 300px;
            text-align: center;
        }
        
        .hero-image img {
            width: 100%;
            max-width: 400px;
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
        }
        
        .hero-text {
            flex: 1;
            min-width: 300px;
        }
        
        .hero h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
        }
        
        .hero p {
            font-size: 1.2rem;
            margin-bottom: 1.5rem;
            color: var(--text-light);
        }
        
        .hero-quote {
            font-style: italic;
            background: var(--light-peach);
            padding: 1rem;
            border-radius: 10px;
            margin: 2rem 0;
            text-align: center;
        }
        
        /* Form Styles */
        form {
            display: flex;
            flex-direction: column;
            gap: 1rem;
            max-width: 500px;
            position: relative;
        }
        
        input, textarea {
            padding: 0.75rem;
            border: 1px solid var(--beige);
            border-radius: 10px;
            font-family: inherit;
            transition: all 0.3s ease;
        }
        
        input:focus, textarea:focus {
            outline: none;
            border-color: var(--pink);
            box-shadow: 0 0 0 3px rgba(255, 192, 203, 0.3);
        }
        
        button {
            padding: 0.75rem;
            background: var(--light-peach);
            color: var(--text-dark);
            font-weight: 500;
            cursor: pointer;
            transition: all 0.3s ease;
            border: none;
            border-radius: 10px;
            position: relative;
            overflow: hidden;
        }
        
        button:hover {
            background: var(--beige);
            transform: scale(1.05);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1), 0 0 15px rgba(255, 218, 185, 0.5);
        }
        
        button:active {
            transform: scale(0.98);
        }
        
        .confirmation {
            display: none;
            background: var(--light-peach);
            padding: 1rem;
            border-radius: 5px;
            text-align: center;
            margin-top: 1rem;
        }
        
        /* Section Styles */
        section {
            padding: 4rem 0;
            position: relative;
        }
        
        .section-title {
            font-size: 2.5rem;
            text-align: center;
            margin-bottom: 3rem;
            color: var(--light-peach);
        }
        
        /* Portfolio Section */
        .portfolio {
            background: var(--white);
        }
        
        .portfolio-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }
        
        .project {
            background: var(--cream);
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 4px 15px rgba(0,0,0,0.05);
            transition: transform 0.3s;
        }
        
        .project:hover {
            transform: translateY(-5px);
        }
        
        .project img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }
        
        .project-content {
            padding: 1.5rem;
        }
        
        /* Creative Section */
        .creative {
            background: var(--cream);
            position: relative;
            overflow: hidden;
        }
        
        .creative-banner {
            text-align: center;
            margin-bottom: 3rem;
            padding: 2rem;
            background: var(--light-peach);
            border-radius: 15px;
            position: relative;
            z-index: 2;
        }
        
        .creative-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(400px, 1fr));
            gap: 2rem;
            position: relative;
            z-index: 2;
        }
        
        .creative-item {
            background: var(--light-peach);
            padding: 2rem;
            border-radius: 15px;
            text-align: center;
            box-shadow: 0 4px 15px rgba(0,0,0,0.05);
            position: relative;
            overflow: hidden;
        }
        
        /* Motivational Section */
        .motivational {
            background: var(--beige);
            text-align: center;
        }
        
        .quote-box {
            background: var(--cream);
            padding: 2rem;
            border-radius: 15px;
            max-width: 600px;
            margin: 0 auto;
            box-shadow: 0 4px 15px rgba(0,0,0,0.05);
        }
        
        /* Contact Section */
        .contact {
            background: var(--white);
        }
        
        .social-links {
            display: flex;
            justify-content: center;
            gap: 1rem;
            margin-top: 2rem;
        }
        
        .social-links a {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 50px;
            height: 50px;
            background: var(--light-peach);
            border-radius: 50%;
            font-size: 1.5rem;
            text-decoration: none;
            transition: all 0.3s ease;
        }
        
        .social-links a:hover {
            transform: translateY(-3px);
            background: var(--pink);
        }
        
        /* Footer Styles */
        footer {
            background: var(--cream);
            padding: 3rem 0 1.5rem;
            border-top: 3px solid var(--light-peach);
        }
        
        .footer-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            margin-bottom: 2rem;
        }
        
        .footer-section h3 {
            font-size: 1.5rem;
            margin-bottom: 1rem;
            color: var(--text-dark);
        }
        
        .footer-links {
            list-style: none;
        }
        
        .footer-links li {
            margin-bottom: 0.5rem;
        }
        
        .footer-links a {
            text-decoration: none;
            color: var(--text-light);
            transition: color 0.3s;
        }
        
        .footer-links a:hover {
            color: var(--light-peach);
        }
        
        .footer-message {
            text-align: center;
            padding: 1rem;
            background: var(--light-peach);
            border-radius: 10px;
            margin: 1rem 0;
        }
        
        .copyright {
            text-align: center;
            margin-top: 2rem;
            padding-top: 1rem;
            border-top: 1px solid var(--beige);
            color: var(--text-light);
        }
        
        .back-to-top {
            position: fixed;
            bottom: 20px;
            right: 20px;
            background: var(--light-peach);
            width: 50px;
            height: 50px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            text-decoration: none;
            font-size: 1.5rem;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            transition: all 0.3s;
            z-index: 99;
        }
        
        .back-to-top:hover {
            background: var(--pink);
            transform: translateY(-3px);
        }
        
        /* Floating Elements */
        .floating-element {
            position: absolute;
            pointer-events: none;
            font-size: 1.2rem;
            animation: floatUp 6s linear infinite;
            opacity: 0.8;
            z-index: 1;
        }
        
        @keyframes floatUp {
            0% {
                transform: translateY(100vh) rotate(0deg);
                opacity: 0;
            }
            10% {
                opacity: 0.8;
            }
            90% {
                opacity: 0.6;
            }
            100% {
                transform: translateY(-100px) rotate(360deg);
                opacity: 0;
            }
        }
        
        /* Heart Burst Animation */
        .heart-burst {
            position: absolute;
            pointer-events: none;
            font-size: 1.5rem;
            animation: heartBurst 1s ease-out forwards;
            opacity: 0;
            z-index: 100;
        }
        
        @keyframes heartBurst {
            0% {
                transform: scale(0);
                opacity: 1;
            }
            50% {
                opacity: 1;
            }
            100% {
                transform: scale(3);
                opacity: 0;
            }
        }
        
        /* Responsive Styles */
        @media (max-width: 768px) {
            nav ul {
                gap: 1rem;
            }
            
            .hero-content {
                flex-direction: column;
            }
            
            .hero h1 {
                font-size: 2.5rem;
            }
            
            .creative-grid {
                grid-template-columns: 1fr;
            }
            
            .portfolio-grid {
                grid-template-columns: 1fr;
            }
            
            .footer-container {
                grid-template-columns: 1fr;
            }
            
            .floating-element {
                font-size: 1rem;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <nav class="container">
            <a href="#" class="logo">Diiba's World</a>
            <ul>
                <li><a href="#about">About</a></li>
                <li><a href="#portfolio">Portfolio</a></li>
                <li><a href="#creative">Creative</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero/About Section -->
    <section id="about" class="hero">
        <div class="container">
            <div class="hero-content">
                <div class="hero-image">
                    <img src="https://placeholder-image-service.onrender.com/image/400x500?prompt=Friendly%20person%20with%20warm%20smile%20in%20pastel%20setting&id=diiba-portrait" alt="Diiba smiling in a cozy pastel environment">
                </div>
                <div class="hero-text">
                    <h1>Hello, I'm Diiba 👋</h1>
                    <p>🎨 I'm a creator, dreamer, and lifelong learner.</p>
                    <p>🌸 I share personal growth, language adventures, wellness, and creative projects.</p>
                    <p>📍 Born in a sunny coastal town, currently exploring new adventures!</p>
                    
                    <div class="hero-quote">
                        "The best way to predict your future is to create it."
                    </div>
                    
                    <form id="newsletter" onsubmit="handleFormSubmit(event, 'newsletter')">
                        <input type="text" name="name" placeholder="Your Name" required>
                        <input type="email" name="email" placeholder="Your Email" required>
                        <button type="submit">Join My Newsletter</button>
                        <div id="newsletter-confirmation" class="confirmation">Thank you for signing up! Please check your email for a special welcome message 💌</div>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Portfolio Section -->
    <section id="portfolio" class="portfolio">
        <div class="container">
            <h2 class="section-title">My Creative Projects</h2>
            <div class="portfolio-grid">
                <div class="project">
                    <img src="https://placeholder-image-service.onrender.com/image/400x300?text=Creative+Writing+Project&id=project1" alt="Creative writing project with pastel aesthetics">
                    <div class="project-content">
                        <h3>Story Collection</h3>
                        <p>A series of short stories inspired by daily life and personal growth journeys.</p>
                    </div>
                </div>
                <div class="project">
                    <img src="https://placeholder-image-service.onrender.com/image/400x300?text=Digital+Art&id=project2" alt="Digital art with soft pastel colors">
                    <div class="project-content">
                        <h3>Digital Illustrations</h3>
                        <p>Hand-drawn digital art exploring emotions and personal reflections.</p>
                    </div>
                </div>
                <div class="project">
                    <img src="https://placeholder-image-service.onrender.com/image/400x300?text=Wellness+Journal&id=project3" alt="Wellness journal design with pastel theme">
                    <div class="project-content">
                        <h3>Wellness Journal</h3>
                        <p>A printable journal for tracking growth, goals, and daily reflections.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Creative Section -->
    <section id="creative" class="creative">
        <div class="container">
            <div class="creative-banner">
                <h2>🌟 Share Your Journey & Inspire Others 🌟</h2>
                <p>Add your wisdom to the Life Lessons Map or leave a note for your future self in the Time Capsule. Your story matters! 💌</p>
            </div>
            
            <div class="creative-grid">
                <div class="creative-item" id="life-lessons-container">
                    <h3>Life Lessons Map 🗺️</h3>
                    <p>Share a lesson you've learned or one you're seeking. Inspire others and help us map our journeys together!</p>
                    <form onsubmit="handleFormSubmit(event, 'life-lessons')">
                        <input type="text" name="name" placeholder="Your Name" required>
                        <textarea name="message" placeholder="Your life lesson..." required rows="3"></textarea>
                        <button type="submit">Add to Map</button>
                    </form>
                    <p style="margin-top: 1rem; font-style: italic;">✨ Share your wisdom and inspire others today!</p>
                </div>
                
                <div class="creative-item" id="time-capsule-container">
                    <h3>Time Capsule ⏳</h3>
                    <p>Write a note to your future self! Set a goal, a dream, or a reflection and watch it grow over time.</p>
                    <form onsubmit="handleFormSubmit(event, 'time-capsule')">
                        <input type="text" name="name" placeholder="Your Name" required>
                        <textarea name="message" placeholder="Your time capsule note..." required rows="3"></textarea>
                        <button type="submit">Submit to Capsule</button>
                    </form>
                    <p style="margin-top: 1rem; font-style: italic;">💌 Take a moment for yourself and leave a note for the future!</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Motivational Section -->
    <section class="motivational">
        <div class="container">
            <h2 class="section-title">Daily Inspiration</h2>
            <div class="quote-box">
                <p id="motivational-quote">"Your potential is endless; your journey is unique. Embrace both."</p>
                <button onclick="newQuote()" style="margin-top: 1rem;">New Motivation</button>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact">
        <div class="container">
            <h2 class="section-title">Let's Connect</h2>
            <form onsubmit="handleFormSubmit(event, 'contact')">
                <input type="text" name="name" placeholder="Your Name" required>
                <input type="email" name="email" placeholder="Your Email" required>
                <textarea name="message" placeholder="Your Message" rows="5" required></textarea>
                <button type="submit">Send Message</button>
            </form>
            
            <div class="social-links">
                <a href="https://instagram.com/yourhandle" aria-label="Instagram">📸</a>
                <a href="https://youtube.com/yourhandle" aria-label="YouTube">🎥</a>
                <a href="https://tiktok.com/yourhandle" aria-label="TikTok">🎵</a>
                <a href="https://linkedin.com/in/yourhandle" aria-label="LinkedIn">💼</a>
                <a href="mailto:your.email@example.com" aria-label="Email">✉️</a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-container">
                <div class="footer-section">
                    <h3>Stay Connected</h3>
                    <div class="social-links">
                        <a href="https://instagram.com/yourhandle" aria-label="Instagram">📸</a>
                        <a href="https://youtube.com/yourhandle" aria-label="YouTube">🎥</a>
                        <a href="https://tiktok.com/yourhandle" aria-label="TikTok">🎵</a>
                        <a href="https://linkedin.com/in/yourhandle" aria-label="LinkedIn">💼</a>
                        <a href="mailto:your.email@example.com" aria-label="Email">✉️</a>
                    </div>
                </div>
                
                <div class="footer-section">
                    <h3>Get Inspiration</h3>
                    <form class="newsletter-form">
                        <input type="email" placeholder="Your email for daily inspiration">
                        <button type="button">Subscribe</button>
                    </form>
                </div>
                
                <div class="footer-section">
                    <h3>Explore</h3>
                    <ul class="footer-links">
                        <li><a href="#about">About Me</a></li>
                        <li><a href="#portfolio">Portfolio</a></li>
                        <li><a href="#creative">Life Lessons Map</a></li>
                        <li><a href="#creative">Time Capsule</a></li>
                        <li><a href="#contact">Contact</a></li>
                    </ul>
                </div>
            </div>
            
            <div class="footer-message">
                <p>Keep dreaming, keep growing, and don't forget to sparkle today! 🌸</p>
            </div>
            
            <div class="copyright">
                <p>© 2025 Diiba's World. Made with love 💜</p>
                <p>Powered by cozy vibes and endless inspiration 🌈</p>
            </div>
        </div>
    </footer>

    <a href="#" class="back-to-top">↑</a>

    <script>
        // Smooth scrolling for navigation
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });

        // Motivational Quotes
        const quotes = [
            "Your potential is endless; your journey is unique. Embrace both.",
            "Growth begins at the end of your comfort zone.",
            "Be the reason someone smiles today.",
            "Your dreams are valid; your voice matters.",
            "Progress, not perfection, is the goal.",
            "Today is a new opportunity to grow and learn.",
            "You are capable of amazing things.",
            "Kindness is always in style.",
            "Your vibe attracts your tribe.",
            "Bloom where you are planted."
        ];
        
        function newQuote() {
            const randomQuote = quotes[Math.floor(Math.random() * quotes.length)];
            document.getElementById('motivational-quote').textContent = `"${randomQuote}"`;
        }

        // Create floating elements
        function createFloatingElements() {
            const elements = ['✨', '🌸', '💖', '💌'];
            const creativeSection = document.getElementById('creative');
            
            // Create 20 floating elements
            for (let i = 0; i < 20; i++) {
                const element = document.createElement('div');
                element.className = 'floating-element';
                element.textContent = elements[Math.floor(Math.random() * elements.length)];
                
                // Random position
                const posX = Math.random() * 100;
                const posY = Math.random() * 100;
                
                // Random size between 1rem and 2rem
                const size = 1 + Math.random();
                element.style.fontSize = `${size}rem`;
                
                // Random delay
                const delay = Math.random() * 5;
                element.style.animationDelay = `${delay}s`;
                
                // Random left position
                element.style.left = `${posX}%`;
                
                creativeSection.appendChild(element);
            }
        }
        
        // Heart burst animation
        function createHeartBurst(x, y) {
            const heart = document.createElement('div');
            heart.className = 'heart-burst';
            heart.textContent = '💖';
            heart.style.left = `${x}px`;
            heart.style.top = `${y}px`;
            document.body.appendChild(heart);
            
            // Remove after animation completes
            setTimeout(() => {
                heart.remove();
            }, 1000);
        }
        
        // Form submission handler
        function handleFormSubmit(event, formType) {
            event.preventDefault();
            
            // Show confirmation for newsletter
            if (formType === 'newsletter') {
                document.getElementById('newsletter-confirmation').style.display = 'block';
                
                // Generate welcome email content
                const welcomeEmail = `
                    Subject: 🌸 Welcome to diiba's World! 🌸

                    Hi ${event.target.name.value}!

                    Yay! You're officially part of my little world of inspiration and creativity. 🥰 I'm so happy you're here!

                    Get ready for cozy blog posts, motivational words, creative reflections, and a peek into my personal journey. Here, we'll share ideas, dreams, and lessons that help us grow together. ✨

                    Feel free to explore the Time Capsule and Life Lessons Map, where you can leave your own goals, thoughts, or reflections ; I can't wait to read them ! 💌and help you to bring them to life 🌸

                    Thank you for joining me – your presence makes this space brighter and more inspiring. Keep an eye on your inbox for updates, tips, and stories that I hope will make you smile and spark your creativity. 🌷

                    With love and excitement,
                    DIIBA 💖
                `;
                
                console.log("Welcome email content:\n", welcomeEmail);
            }
            
            // Create heart burst at button position
            const rect = event.target.querySelector('button').getBoundingClientRect();
            const x = rect.left + rect.width / 2;
            const y = rect.top + rect.height / 2;
            createHeartBurst(x, y);
            
            // Reset form
            event.target.reset();
        }
        
        // Back to top button
        window.addEventListener('scroll', function() {
            const backToTop = document.querySelector('.back-to-top');
            if (window.pageYOffset > 300) {
                backToTop.style.display = 'flex';
            } else {
                backToTop.style.display = 'none';
            }
        });
        
        // Initialize floating elements
        window.addEventListener('load', function() {
            createFloatingElements();
        });
    </script>
</body>
</html> 
