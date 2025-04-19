# Frogcoin-website
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>FROG Token</title>
  <link href="https://fonts.googleapis.com/css2?family=Fredoka+One&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Fredoka One', sans-serif;
      background-color: #e0f7e9;
      color: #333;
      margin: 0;
      padding: 0;
      scroll-behavior: smooth;
    }
    header {
      background: linear-gradient(135deg, #98e9b1, #6dd47e);
      padding: 30px;
      text-align: center;
      color: white;
    }
    h1, .subtitle {
      margin: 0;
      padding: 10px 0;
    }
    .contract {
      margin-top: 20px;
      font-size: 18px;
      color: #ffffff;
      background-color: #2a9d6f;
      padding: 10px 20px;
      display: inline-block;
      border-radius: 12px;
      cursor: pointer;
    }
    nav {
      text-align: center;
      margin: 20px;
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 10px;
    }
    nav a {
      padding: 10px 20px;
      background: #39b472;
      color: white;
      text-decoration: none;
      border-radius: 20px;
      font-size: 14px;
    }
    section {
      padding: 40px 20px;
      text-align: center;
    }
    .tokenomics, .roadmap, .howtobuy {
      background-color: #ffffff;
      margin: 20px auto;
      border-radius: 20px;
      padding: 30px;
      max-width: 1000px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
    }
    .tokenomics-grid {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 20px;
      margin-top: 30px;
    }
    .tokenomics-card {
      background: linear-gradient(145deg, #c0f7d5, #a8ebc2);
      border-radius: 16px;
      padding: 20px;
      width: 260px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
      text-align: center;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      animation: fadeInUp 0.6s ease forwards;
    }
    .tokenomics-card:hover {
      transform: translateY(-5px);
      box-shadow: 0 8px 16px rgba(0,0,0,0.15);
    }
    .tokenomics-card h3 {
      margin: 0 0 10px;
      font-size: 20px;
      color: #045d56;
    }
    .tokenomics-card p {
      margin: 0;
      font-size: 16px;
    }
    .roadmap ul {
      list-style: none;
      padding: 0;
      display: grid;
      gap: 16px;
    }
    .roadmap li {
      background: #f9fff3;
      padding: 16px 20px;
      border-left: 6px solid #a8ebc2;
      border-radius: 10px;
      text-align: left;
      box-shadow: 0 2px 6px rgba(0,0,0,0.05);
      transition: transform 0.2s;
    }
    .roadmap li:hover {
      transform: translateX(5px);
    }
    .howtobuy ul {
      list-style: none;
      padding: 0;
      display: grid;
      gap: 16px;
    }
    .howtobuy li {
      background: #f9fff3;
      padding: 16px 20px;
      border-left: 6px solid #a8ebc2;
      border-radius: 10px;
      text-align: left;
      box-shadow: 0 2px 6px rgba(0,0,0,0.05);
    }
    footer {
      text-align: center;
      padding: 20px;
      background-color: #6dd47e;
      color: white;
    }
    @keyframes fadeInUp {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }
    .language-switcher {
      position: absolute;
      top: 20px;
      right: 20px;
      z-index: 999;
    }
    .language-switcher button {
      padding: 6px 12px;
      border: none;
      background-color: #2a9d6f;
      color: white;
      font-size: 14px;
      margin-left: 5px;
      border-radius: 8px;
      cursor: pointer;
      transition: background 0.3s;
    }
    .language-switcher button:hover {
      background-color: #218f61;
    }
  </style>
  <script>
    function switchLang(lang) {
      if (lang === 'en') window.location.href = window.location.pathname + '?lang=en';
      if (lang === 'ru') window.location.href = window.location.pathname + '?lang=ru';
    }
  </script>
</head>
<body>
  <div class="language-switcher">
    <button onclick="switchLang('en')">EN</button>
    <button onclick="switchLang('ru')">RU</button>
  </div>

  <header>
    <h1>FROG Token</h1>
    <p class="subtitle">No gas, no taxes — just pure amphibian meme vibes 🐸</p>
    <div class="contract" onclick="navigator.clipboard.writeText('C61ZJ21pC1X9zs2TtRgzd3RxaBi7qqRBLageGXNEdgaa'); this.textContent = '✅ Copied!'; setTimeout(() => this.textContent = '📋 Contract: C61ZJ21pC1X9zs2TtRgzd3RxaBi7qqRBLageGXNEdgaa', 2000);">
      📋 Contract: C61ZJ21pC1X9zs2TtRgzd3RxaBi7qqRBLageGXNEdgaa
    </div>
  </header>

  <nav>
    <a href="#about">About</a>
    <a href="#tokenomics">Tokenomics</a>
    <a href="#roadmap">Roadmap</a>
    <a href="#howtobuy">How to Buy</a>
    <a href="#whatsnext">What's Next?</a>
    <a href="https://twitter.com/@FROG2026s" target="_blank">Twitter</a>
    <a href="https://t.me/+NrTRXfFMJJUyZmZi" target="_blank">Telegram</a>
    <a href="https://raydium.io/swap/?inputCurrency=sol&outputCurrency=C61ZJ21pC1X9zs2TtRgzd3RxaBi7qqRBLageGXNEdgaa" target="_blank">Buy on Raydium</a>
  </nav>

  <section id="about" class="tokenomics">
    <h2>About the Project</h2>
    <p>FROG isn’t just a meme coin. It’s a community, a philosophy, and a digital memory for those who were here from the beginning.</p>
    <p>The project is currently focused on launching a unique NFT collection: 20,000 one-of-a-kind frogs that will be released in phases — starting with 5,000, then 10,000, and so on. To kick things off, 200 NFTs will be airdropped to active Twitter followers.</p>
    <p>We're starting with organic growth and strong community vibes. First NFTs — then everything else. As the audience grows, so will the project. A listing on Raydium is planned later, once we have a strong base of supporters.</p>
    <p>FROG is built for the fans, not just for profit. These NFTs will be a symbol that you were here early. 🐸💚</p>
  </section>

  <section id="tokenomics" class="tokenomics">
    <h2>Tokenomics 🐸</h2>
    <p><strong>Total Supply:</strong> 1,000,000,000 $FROG</p>
    <div class="tokenomics-grid">
      <div class="tokenomics-card">
        <h3>💧 850,000,000</h3>
        <p>Market Allocation<br><small>Phased DEX listing (200M at launch)<br>200M chosen at launch to stop sniper bots and protect the project from the start.</small></p>
      </div>
      <div class="tokenomics-card">
        <h3>🎁 50,000,000</h3>
        <p>Airdrops & Rewards<br><small>For active community members</small></p>
      </div>
      <div class="tokenomics-card">
        <h3>🔒 100,000,000</h3>
        <p>Founder's Reserve<br><small>Locked for growth and stability</small></p>
      </div>
    </div>
  </section>

  <section id="roadmap" class="roadmap">
    <h2>Roadmap</h2>
    <ul>
      <li>📢 Meme raids and Twitter promotion</li>
      <li>🎉 Meme contests and community rewards</li>
      <li>🔧 Add Buy button and tools</li>
      <li>🎨 Launch of FROG NFT collection — exclusive meme frogs on Solana<br><small>20,000 unique NFTs launching in phases. 200 NFTs will be given away to active Twitter followers. Stay tuned and join the giveaway!</small></li>
      <li>🚀 Launch token on Solana network</li>
      <li>📈 Listing on Raydium</li>
      <li>🌐 Listings on CoinGecko & CoinMarketCap</li>
    </ul>
  </section>

  <section id="howtobuy" class="howtobuy">
    <h2>How to Buy</h2>
    <ul>
      <li>📲 Install Phantom wallet on your device</li>
      <li>💸 Buy SOL on your preferred exchange</li>
      <li>🔁 Transfer SOL to Phantom wallet</li>
      <li>🌐 Go to <a href="https://raydium.io" target="_blank">raydium.io</a> and paste the contract address</li>
      <li>🐸 Swap SOL for $FROG and join the community</li>
    </ul>
  </section>

  <section id="whatsnext" class="roadmap">
    <h2>What's Next?</h2>
    <ul>
      <li>💥 Community raids and growth on Telegram and Twitter</li>
      <li>🎁 NFT giveaways and future token distributions via Telegram and Twitter</li>
      <li>🌐 Submit to CoinGecko and CoinMarketCap</li>
      <li>🛠 Launch of dashboard and utilities</li>
    </ul>
  </section>

  <footer>
    <p>Made with 💚 by the FROG community — 2025</p>
  </footer>
</body>
</html>
