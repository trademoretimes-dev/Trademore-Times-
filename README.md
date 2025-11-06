

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Trademore Times - Your Neighbourhood, Your News</title>
    <style>
        /* Color Scheme - Vibrant and Community-like */
        :root {
            --primary: #2E86AB;      /* Trustworthy blue */
            --secondary: #A23B72;    /* Vibrant magenta */
            --accent: #F18F01;       /* Energetic orange */
            --light: #F7F9FC;        /* Clean white */
            --dark: #2D3047;         /* Deep navy */
            --success: #4CAF50;      /* Green for highlights */
        }

        /* Base Styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            background-color: var(--light);
        }

        /* Header & Navigation */
        header {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
            padding: 1rem 0;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }

        .header-content {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 0 2rem;
        }

        .logo {
            font-size: 2rem;
            font-weight: bold;
        }

        .tagline {
            font-style: italic;
            opacity: 0.9;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 2rem;
        }

        nav a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s ease;
        }

        nav a:hover {
            color: var(--accent);
        }

        /* Main Content */
        main {
            max-width: 1200px;
            margin: 2rem auto;
            padding: 0 2rem;
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(46, 134, 171, 0.8), rgba(162, 59, 114, 0.8)), url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 600"><rect fill="%232E86AB" width="1200" height="600"/></svg>');
            color: white;
            padding: 4rem 2rem;
            text-align: center;
            border-radius: 15px;
            margin-bottom: 3rem;
        }

        .hero h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
        }

        .hero p {
            font-size: 1.2rem;
            max-width: 600px;
            margin: 0 auto;
        }

        /* Article Grid */
        .articles-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin: 2rem 0;
        }

        .article-card {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .article-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0,0,0,0.15);
        }

        .article-image {
            height: 200px;
            background: var(--primary);
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-weight: bold;
        }

        .article-content {
            padding: 1.5rem;
        }

        .article-category {
            background: var(--accent);
            color: white;
            padding: 0.3rem 0.8rem;
            border-radius: 20px;
            font-size: 0.8rem;
            font-weight: bold;
            display: inline-block;
            margin-bottom: 1rem;
        }

        .article-title {
            font-size: 1.3rem;
            margin-bottom: 0.5rem;
            color: var(--dark);
        }

        .article-excerpt {
            color: #666;
            margin-bottom: 1rem;
        }

        .read-more {
            color: var(--primary);
            text-decoration: none;
            font-weight: bold;
            display: inline-block;
        }

        /* Section Styles */
        .section-title {
            color: var(--primary);
            border-bottom: 3px solid var(--accent);
            padding-bottom: 0.5rem;
            margin: 2rem 0 1rem 0;
        }

        /* Interactive Elements */
        .poll-container, .trivia-container {
            background: white;
            padding: 2rem;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            margin: 2rem 0;
        }

        .poll-options {
            margin: 1rem 0;
        }

        .poll-option {
            margin: 0.5rem 0;
            padding: 0.5rem;
            background: var(--light);
            border-radius: 5px;
            cursor: pointer;
            transition: background 0.3s ease;
        }

        .poll-option:hover {
            background: #e8eef2;
        }

        .vote-btn {
            background: var(--primary);
            color: white;
            border: none;
            padding: 0.7rem 1.5rem;
            border-radius: 5px;
            cursor: pointer;
            font-weight: bold;
        }

        .vote-btn:hover {
            background: #257194;
        }

        /* Footer */
        footer {
            background: var(--dark);
            color: white;
            text-align: center;
            padding: 2rem;
            margin-top: 4rem;
        }

        .footer-content {
            max-width: 1200px;
            margin: 0 auto;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                text-align: center;
                gap: 1rem;
            }

            nav ul {
                flex-wrap: wrap;
                justify-content: center;
                gap: 1rem;
            }

            .hero h1 {
                font-size: 2rem;
            }

            .articles-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="header-content">
            <div class="logo">Trademore Times</div>
            <div class="tagline">"Your Neighbourhood, Your News"</div>
            <nav>
                <ul>
                    <li><a href="#home">Home</a></li>
                    <li><a href="#about">About</a></li>
                    <li><a href="#community">Community News</a></li>
                    <li><a href="#practical">Practical Living</a></li>
                    <li><a href="#human-interest">Human Interest</a></li>
                    <li><a href="#lifestyle">Lifestyle</a></li>
                    <li><a href="#interactive">Interactive</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Main Content -->
    <main>
        <!-- Home Page -->
        <section id="home">
            <div class="hero">
                <h1>Welcome to Trademore Times</h1>
                <p>Bringing you the latest stories, news, and events from our vibrant community</p>
            </div>

            <h2 class="section-title">Latest Stories</h2>
            <div class="articles-grid">
                <!-- Article 1 -->
                <div class="article-card">
                    <div class="article-image" style="background: var(--success);">NEW PARK OPENING</div>
                    <div class="article-content">
                        <span class="article-category">Community News</span>
                        <h3 class="article-title">New Community Park Opens This Weekend</h3>
                        <p class="article-excerpt">After months of anticipation, the new Riverside Park officially opens with a community celebration...</p>
                        <a href="#" class="read-more">Read More →</a>
                    </div>
                </div>

                <!-- Article 2 -->
                <div class="article-card">
                    <div class="article-image" style="background: var(--secondary);">LOCAL HERO</div>
                    <div class="article-content">
                        <span class="article-category">Human Interest</span>
                        <h3 class="article-title">Local Teacher Wins National Award</h3>
                        <p class="article-excerpt">Sarah Johnson recognized for her innovative approach to community-based learning...</p>
                        <a href="#" class="read-more">Read More →</a>
                    </div>
                </div>

                <!-- Article 3 -->
                <div class="article-card">
                    <div class="article-image" style="background: var(--accent);">FAMILY GUIDE</div>
                    <div class="article-content">
                        <span class="article-category">Lifestyle & Family</span>
                        <h3 class="article-title">Summer Activities for Kids in Trademore</h3>
                        <p class="article-excerpt">Discover fun and educational activities to keep your children engaged this summer...</p>
                        <a href="#" class="read-more">Read More →</a>
                    </div>
                </div>
            </div>
        </section>

        <!-- About Page -->
        <section id="about" style="display: none;">
            <div class="hero">
                <h1>About Trademore Times</h1>
                <p>Dedicated to serving our community with trusted local journalism</p>
            </div>

            <div class="article-card">
                <div class="article-content">
                    <h2>Our Mission</h2>
                    <p>Trademore Times was founded in 2010 with a simple goal: to keep our neighbors informed, connected, and engaged with what matters most in our community.</p>
                    
                    <h3>What We Believe</h3>
                    <p>Strong communities are built on shared knowledge and open communication. We're committed to:</p>
                    <ul>
                        <li>Reporting local news with accuracy and integrity</li>
                        <li>Celebrating the achievements of our residents</li>
                        <li>Providing practical information for daily living</li>
                        <li>Creating spaces for community conversation</li>
                    </ul>

                    <h3>Our Team</h3>
                    <p>We're your neighbors - local journalists, photographers, and community contributors who live and work in Trademore.</p>
                </div>
            </div>
        </section>

        <!-- Community News Page -->
        <section id="community" style="display: none;">
            <h1 class="section-title">Community News</h1>
            <div class="articles-grid">
                <div class="article-card">
                    <div class="article-content">
                        <span class="article-category">Update</span>
                        <h3 class="article-title">Road Construction Schedule Released</h3>
                        <p class="article-excerpt">Main Street improvements to begin next month with minimal disruption to local businesses...</p>
                        <a href="#" class="read-more">Read More →</a>
                    </div>
                </div>
                <div class="article-card">
                    <div class="article-content">
                        <span class="article-category">Event</span>
                        <h3 class="article-title">Annual Food Drive This Saturday</h3>
                        <p class="article-excerpt">Local organizations team up to support families in need. Drop-off locations throughout Trademore...</p>
                        <a href="#" class="read-more">Read More →</a>
                    </div>
                </div>
            </div>
        </section>

        <!-- Interactive Page -->
        <section id="interactive" style="display: none;">
            <h1 class="section-title">Interactive & Fun</h1>
            
            <div class="poll-container">
                <h3>Community Poll: What's Your Favorite Local Spot?</h3>
                <div class="poll-options">
                    <div class="poll-option" onclick="selectOption(this)">Riverside Park</div>
                    <div class="poll-option" onclick="selectOption(this)">Downtown Cafe</div>
                    <div class="poll-option" onclick="selectOption(this)">Community Library</div>
                    <div class="poll-option" onclick="selectOption(this)">Local Farmers Market</div>
                </div>
                <button class="vote-btn" onclick="submitVote()">Submit Vote</button>
                <div id="poll-results" style="margin-top: 1rem;"></div>
            </div>

            <div class="trivia-container">
                <h3>Trademore Trivia</h3>
                <p>What year was Trademore's community center built?</p>
                <div class="poll-options">
                    <div class="poll-option" onclick="checkAnswer(this, 1995)">1995</div>
                    <div class="poll-option" onclick="checkAnswer(this, 2002)">2002</div>
                    <div class="poll-option" onclick="checkAnswer(this, 1988)">1988</div>
                    <div class="poll-option" onclick="checkAnswer(this, 2010)">2010</div>
                </div>
            </div>
        </section>

        <!-- Other sections would follow similar structure -->
    </main>

    <!-- Footer -->
    <footer>
        <div class="footer-content">
            <p>&copy; 2024 Trademore Times. All rights reserved.</p>
            <p>"Your Neighbourhood, Your News"</p>
            <p>Contact: editor@trademoretimes.com | (555) 123-NEWS</p>
        </div>
    </footer>

    <script>
        // Navigation functionality
        function showSection(sectionId) {
            // Hide all sections
            document.querySelectorAll('main > section').forEach(section => {
                section.style.display = 'none';
            });
            
            // Show selected section
            document.getElementById(sectionId).style.display = 'block';
        }

        // Set up navigation clicks
        document.querySelectorAll('nav a').forEach(link => {
            link.addEventListener('click', function(e) {
                e.preventDefault();
                const sectionId = this.getAttribute('href').substring(1);
                showSection(sectionId);
                
                // Scroll to top
                window.scrollTo(0, 0);
            });
        });

        // Show home section by default
        showSection('home');

        // Interactive poll functionality
        let selectedOption = null;

        function selectOption(element) {
            // Remove selected class from all options
            document.querySelectorAll('.poll-option').forEach(opt => {
                opt.style.background = '';
            });
            
            // Add selected class to clicked option
            element.style.background = '#e8eef2';
            selectedOption = element.textContent;
        }

        function submitVote() {
            if (selectedOption) {
                document.getElementById('poll-results').innerHTML = 
                    `<p>Thanks for voting! You selected: <strong>${selectedOption}</strong></p>`;
            } else {
                alert('Please select an option first!');
            }
        }

        // Trivia functionality
        function checkAnswer(element, correctAnswer) {
            const userAnswer = parseInt(element.textContent);
            if (userAnswer === correctAnswer) {
                element.style.background = 'var(--success)';
                element.style.color = 'white';
                setTimeout(() => {
                    alert('Correct! The community center was built in 1995.');
                }, 100);
            } else {
                element.style.background = '#ff4444';
                element.style.color = 'white';
                setTimeout(() => {
                    alert('Not quite! Try again.');
                    element.style.background = '';
                    element.style.color = '';
                }, 1000);
            }
        }

        // Add some dynamic content loading simulation
        window.addEventListener('load', function() {
            console.log('Trademore Times - Community News Portal Loaded');
            
            // Simulate loading latest articles
            setTimeout(() => {
                const loadingElements = document.querySelectorAll('.article-excerpt');
                loadingElements.forEach((el, index) => {
                    el.style.opacity = '1';
                    el.style.transition = 'opacity 0.5s ease';
                });
            }, 500);
        });
    </script>
</body>
</html>
```
