!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <title>Smartfx Option Trade — Clone (Demo)</title>
  <style>
    :root{--accent:#0b61ff;--dark:#0b1220;--muted:#6b7280}
    body{font-family:Inter,system-ui,Arial,Helvetica,sans-serif;margin:0;color:var(--dark);line-height:1.4}
    header{display:flex;justify-content:space-between;align-items:center;padding:20px 32px;border-bottom:1px solid #eee}
    .brand{display:flex;gap:12px;align-items:center}
    .brand img{width:42px;height:42px;object-fit:cover;border-radius:6px}
    nav a{margin-left:16px;color:var(--dark);text-decoration:none;font-weight:600}
    .cta{background:var(--accent);color:#fff;padding:8px 14px;border-radius:8px;text-decoration:none}

    .hero{padding:60px 32px;background:linear-gradient(180deg,#f6f9ff,white)}
    .hero .wrap{max-width:1100px;margin:0 auto;display:flex;gap:32px;align-items:center}
    .hero h1{font-size:34px;margin:0 0 12px}
    .hero p{color:var(--muted);margin:0 0 20px}
    .hero .buttons a{margin-right:12px;padding:10px 16px;border-radius:8px;text-decoration:none;font-weight:700}
    .primary{background:var(--accent);color:#fff}
    .secondary{border:1px solid #ddd;background:#fff;color:var(--dark)}

    .features{max-width:1100px;margin:36px auto;display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:18px;padding:0 18px}
    .card{background:#fff;border-radius:12px;padding:18px;border:1px solid #f0f0f0}
    .card h3{margin:0 0 8px}
    .trust{display:flex;gap:18px;align-items:center;max-width:1100px;margin:32px auto;padding:0 18px}
    .reviews{max-width:1100px;margin:18px auto;padding:0 18px}
    footer{border-top:1px solid #eee;padding:24px 32px;color:var(--muted);display:flex;justify-content:space-between;align-items:center}

    /* responsive */
    @media (max-width:800px){.hero .wrap{flex-direction:column;text-align:center}.hero h1{font-size:26px}}

    /* chat bubble */
    .chat{position:fixed;right:18px;bottom:18px;background:var(--accent);color:#fff;padding:12px 16px;border-radius:999px;box-shadow:0 6px 18px rgba(11,97,255,0.18);cursor:pointer}
  </style>
</head>
<body>
  <header>
    <div class="brand">
      <img src="data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' width='64' height='64'><rect rx='12' width='100%' height='100%' fill='%230b61ff'/><text x='50%' y='55%' font-size='28' text-anchor='middle' fill='white' font-family='Arial' font-weight='700'>S</text></svg>" alt="logo">
      <div>
        <div style="font-weight:800">Smartfx Option Trade</div>
        <div style="font-size:12px;color:var(--muted)">Online Forex ECN/STP Broker</div>
      </div>
    </div>
    <nav>
      <a href="#">Platforms</a>
      <a href="#">Funding</a>
      <a href="#">Legal</a>
      <a class="cta" href="#">Open an account</a>
    </nav>
  </header>

  <section class="hero">
    <div class="wrap">
      <div style="flex:1">
        <h1>Trade Stocks, Forex, Options and Crypto</h1>
        <p>Join thousands who use our platform to trade across multiple asset classes with fast execution and 24/7 support.</p>
        <div class="buttons">
          <a class="primary" href="#">Trade Now</a>
          <a class="secondary" href="#">Practice Account</a>
        </div>
      </div>
      <div style="width:360px">
        <img src="https://via.placeholder.com/360x240?text=Chart+Preview" alt="chart" style="width:100%;border-radius:12px;display:block">
      </div>
    </div>
  </section>

  <section class="features">
    <div class="card">
      <h3>Stocks & ETFs</h3>
      <p>Access global stocks and ETFs. Competitive commissions and wide coverage.</p>
      <a href="#">Invest in Stocks</a>
    </div>
    <div class="card">
      <h3>Crypto</h3>
      <p>Buy, sell and store Bitcoin and other leading cryptocurrencies.</p>
      <a href="#">Buy Crypto</a>
    </div>
    <div class="card">
      <h3>CFD Trading</h3>
      <p>Trade FX, commodities and indices with flexible leverage and tight spreads.</p>
      <a href="#">Trade Now</a>
    </div>
  </section>

  <section class="trust">
    <div style="flex:1;">
      <h3>Regulated</h3>
      <p style="margin:6px 0;color:var(--muted)">Our company is regulated by major authorities.</p>
    </div>
    <div style="flex:1;">
      <h3>Swift & Reliable</h3>
      <p style="margin:6px 0;color:var(--muted)">Fast APIs and multi-platform support.</p>
    </div>
    <div style="flex:1;">
      <h3>Privacy</h3>
      <p style="margin:6px 0;color:var(--muted)">We will never share your private data without permission.</p>
    </div>
  </section>

  <section class="reviews">
    <div style="max-width:1100px;margin:0 auto;padding:0 18px">
      <h3>What our clients say</h3>
      <blockquote style="border-left:3px solid #eee;padding-left:12px;color:var(--muted)">"Great platform for starting traders. Great selection and transparent fee system." — Bryce C.</blockquote>
      <div style="margin-top:12px;color:var(--muted)">7,665,635 Open Trades</div>
    </div>
  </section>

  <footer>
    <div>
      © <span id="year"></span> Smartfx Option Trade — Demo. Not an official site.
    </div>
    <div style="text-align:right">
      <div>Support: <a href="mailto:support@example.com">support@example.com</a></div>
    </div>
  </footer>

  <div class="chat" onclick="openChat()">24/7 Live Chat</div>

  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
    function openChat(){ alert('This demo implements a placeholder chat — integrate your live-chat provider (e.g., Smartsupp) here.'); }
  </script>
</body>
</html>
