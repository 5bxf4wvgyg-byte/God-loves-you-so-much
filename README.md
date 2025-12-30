# God-loves-you-so-much
A safe place to learn and meet 
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>God Loves You</title>
  <meta name="description" content="A safe place to find hope in God and submit anonymous prayer requests." />

  <style>
    :root {
      --bg-main: #fbfaf8;
      --bg-card: #ffffff;
      --primary: #6b8cff;
      --primary-dark: #4e6ee6;
      --accent: #f3c969;
      --accent-soft: #fff2cf;
      --lavender: #b9a7e8;
      --text-main: #2b2b2b;
      --text-muted: #5a5a5a;
      --border-soft: #e6e2da;
      --max: 1100px;
    }

    * { box-sizing: border-box; }

    body {
      margin: 0;
      font-family: system-ui, -apple-system, Segoe UI, Roboto, Arial, sans-serif;
      background: var(--bg-main);
      color: var(--text-main);
      line-height: 1.6;
    }

    a { color: var(--primary); text-decoration: none; }

    .wrap {
      max-width: var(--max);
      margin: auto;
      padding: 24px;
    }

    header {
      background: linear-gradient(135deg, #6b8cff, #b9a7e8);
      color: #fff;
    }

    nav {
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
    }

    nav a {
      color: #fff;
      margin-left: 14px;
      font-weight: 500;
    }

    .brand {
      font-weight: 800;
      letter-spacing: 0.5px;
    }

    .hero {
      padding: 60px 0;
    }

    .tag {
      background: rgba(255,255,255,.25);
      padding: 6px 12px;
      border-radius: 999px;
      font-size: 13px;
      display: inline-block;
      margin-bottom: 12px;
    }

    h1 {
      font-size: clamp(36px, 5vw, 56px);
      margin: 0 0 12px;
    }

    .sub {
      max-width: 65ch;
      font-size: 18px;
      opacity: .95;
    }

    main section {
      padding: 36px 0;
    }

    .card {
      background: var(--bg-card);
      border-radius: 20px;
      padding: 22px;
      border: 1px solid var(--border-soft);
      box-shadow: 0 12px 30px rgba(0,0,0,.05);
      margin-bottom: 24px;
    }

    .pill {
      display: inline-block;
      background: var(--accent-soft);
      color: #6a4b00;
      padding: 8px 14px;
      border-radius: 999px;
      font-size: 13px;
      margin: 6px 6px 0 0;
    }

    label {
      font-weight: 600;
      margin-top: 14px;
      display: block;
    }

    input, textarea, select {
      width: 100%;
      padding: 12px;
      border-radius: 14px;
      border: 1px solid var(--border-soft);
      margin-top: 6px;
      font: inherit;
    }

    textarea {
      min-height: 150px;
    }

    button {
      margin-top: 16px;
      padding: 12px 18px;
      border-radius: 16px;
      border: none;
      background: var(--primary);
      color: #fff;
      font-weight: 600;
      cursor: pointer;
    }

    button:hover {
      background: var(--primary-dark);
    }

    .notice {
      background: #f2f0ff;
      border-left: 4px solid var(--lavender);
      padding: 14px;
      border-radius: 14px;
      margin-top: 16px;
    }

    footer {
      text-align: center;
      padding: 30px 0;
      font-size: 13px;
      color: var(--text-muted);
      border-top: 1px solid var(--border-soft);
    }
  </style>
</head>

<body>

<header>
  <div class="wrap">
    <nav>
      <div class="brand">GOD LOVES YOU</div>
      <div>
        <a href="#about">About</a>
        <a href="#prayer">Prayer</a>
        <a href="#verse">Verse</a>
      </div>
    </nav>

    <div class="hero">
      <span class="tag">Faith • Hope • Anonymous Prayer</span>
      <h1>You are deeply loved.</h1>
      <p class="sub">
        This is a safe place to learn about God and submit an anonymous prayer request.
        You don’t have to carry everything by yourself.
      </p>
    </div>
  </div>
</header>

<main>
  <div class="wrap">

    <section id="about">
      <div class="card">
        <h2>Why this page exists</h2>
        <p>
          Life can be heavy. God sees you, hears you, and cares deeply about what you’re facing.
          You can submit a prayer request anonymously — no names, no pressure.
        </p>
        <div class="notice">
          Please don’t include names, addresses, or identifying details.
        </div>
      </div>
    </section>

    <section id="prayer">
      <div class="card">
        <h2>Anonymous Prayer Request</h2>
        <p>
          Share only what you’re comfortable sharing. We will pray over your request.
        </p>

        <!-- 🔁 REPLACE YOUR_FORM_ID WITH YOUR FORMSPREE ID -->
        <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
          <label>Category (optional)</label>
          <select name="category">
            <option value="">Select one</option>
            <option>Peace</option>
            <option>Healing</option>
            <option>Family</option>
            <option>Guidance</option>
            <option>Faith</option>
            <option>Provision</option>
          </select>

          <label>Your prayer request</label>
          <textarea name="prayer_request" required placeholder="Write your prayer here..."></textarea>

          <!-- Honeypot for spam protection -->
          <input type="text" name="_gotcha" style="display:none">

          <button type="submit">Submit Prayer</button>
        </form>
      </div>
    </section>

    <section id="verse">
      <div class="card">
        <h2>Verse of Encouragement</h2>
        <p style="font-size:18px;">
          “Come to me, all who labor and are heavy laden, and I will give you rest.”
        </p>
        <p><strong>— Matthew 11:28</strong></p>
      </div>
    </section>

  </div>
</main>

<footer>
  © <span id="year"></span> God Loves You • Built with prayer 🤍
</footer>

<script>
  document.getElementById("year").textContent = new Date().getFullYear();
</script>

</body>
</html>
