<html><head><base href="." />
<meta charset="utf-8" />
<title>fwog.dev - Gorilla Tag Mod Menu</title>
<style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Inter', sans-serif;
  }

  body {
    background: #0f0f0f;
    color: #ffffff;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  .hero {
    margin-top: 50px;
    padding: 4rem 2rem;
    text-align: center;
    max-width: 1200px;
  }

  h1 {
    font-size: 4rem;
    margin-bottom: 1rem;
    background: linear-gradient(45deg, #00ff88, #00ffee);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }

  .description {
    font-size: 1.2rem;
    color: #888;
    margin-bottom: 2rem;
    line-height: 1.6;
  }

  .buy-button {
    background: linear-gradient(45deg, #00ff88, #00ffee);
    color: #000;
    padding: 1rem 2rem;
    border-radius: 8px;
    text-decoration: none;
    font-weight: 600;
    font-size: 1.1rem;
    transition: all 0.3s ease;
  }

  .buy-button:hover {
    transform: translateY(-2px);
    box-shadow: 0 5px 15px rgba(0, 255, 136, 0.4);
  }

  .features {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 2rem;
    padding: 4rem 2rem;
    max-width: 1200px;
  }

  .feature-card {
    background: rgba(30, 30, 30, 0.5);
    padding: 2rem;
    border-radius: 12px;
    border: 1px solid rgba(0, 255, 136, 0.1);
    transition: all 0.3s ease;
  }

  .feature-card:hover {
    transform: translateY(-10px);
    background: rgba(40, 40, 40, 0.6);
    border-color: rgba(0, 255, 136, 0.3);
    box-shadow: 0 10px 20px rgba(0, 255, 136, 0.2);
  }

  .feature-title {
    color: #00ff88;
    margin-bottom: 1rem;
    font-size: 1.3rem;
  }

  @keyframes float {
    0% { transform: translateY(0px); }
    50% { transform: translateY(-20px); }
    100% { transform: translateY(0px); }
  }

  .floating-gorilla {
    animation: float 6s ease-in-out infinite;
    margin: 2rem 0;
  }
</style>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
</head>
<body>
  <div class="hero">
    <svg class="floating-gorilla" width="120" height="120" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
      <path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm0 18c-4.41 0-8-3.59-8-8s3.59-8 8-8 8 3.59 8 8-3.59 8-8 8z" fill="#00ff88"/>
      <circle cx="12" cy="12" r="3" fill="#00ff88"/>
    </svg>
    <h1>fwog.dev</h1>
    <p class="description">Experience Gorilla Tag like never before with our premium mod menu. Featuring advanced customization, enhanced gameplay features, and a sleek user interface.</p>
    <a href="https://discord.gg/8bHG693Haa" target="_blank" class="buy-button">Purchase Now</a>
  </div>

  <div class="features">
    <div class="feature-card">
      <h3 class="feature-title">Advanced Features</h3>
      <p>Unlock powerful modifications and customization options to enhance your gameplay experience.</p>
    </div>
    <div class="feature-card">
      <h3 class="feature-title">User-Friendly Interface</h3>
      <p>Intuitive design makes it easy to access and customize all features on the fly.</p>
    </div>
    <div class="feature-card">
      <h3 class="feature-title">Regular Updates</h3>
      <p>Stay ahead with frequent updates and new features added regularly.</p>
    </div>
  </div>

  <script>
    document.querySelectorAll('a').forEach(link => {
      link.addEventListener('click', e => {
        if (link.classList.contains('buy-button')) {
          // Add a subtle pop effect when clicking the buy button
          e.target.style.transform = 'scale(0.95)';
          setTimeout(() => {
            e.target.style.transform = 'translateY(-2px)';
          }, 100);
        }
      });
    });
  </script>
</body></html>
