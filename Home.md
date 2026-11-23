<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Project Sendiri</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,500;0,600;1,500&family=Poppins:wght@300;400;500&display=swap" rel="stylesheet">
<style>
  :root {
    --cream: #fbf6f1;
    --blush: #f3dcd6;
    --rose: #c98f8a;
    --sage: #dfe8df;
    --ink: #4a3f3f;
    --muted: #8b7c7a;
    --card: rgba(255, 255, 255, 0.7);
  }

  * { box-sizing: border-box; margin: 0; padding: 0; }

  body {
    font-family: 'Poppins', sans-serif;
    font-weight: 300;
    color: var(--ink);
    background:
      radial-gradient(circle at 15% 10%, var(--blush) 0%, transparent 45%),
      radial-gradient(circle at 85% 90%, var(--sage) 0%, transparent 45%),
      var(--cream);
    background-attachment: fixed;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
  }

  main {
    flex: 1;
    width: 100%;
    max-width: 640px;
    margin: 0 auto;
    padding: 72px 24px 32px;
  }

  .hero { text-align: center; margin-bottom: 48px; }

  .eyebrow {
    font-size: 0.75rem;
    letter-spacing: 0.3em;
    text-transform: uppercase;
    color: var(--rose);
    margin-bottom: 18px;
  }

  h1 {
    font-family: 'Cormorant Garamond', serif;
    font-weight: 600;
    font-size: clamp(2.6rem, 11vw, 4rem);
    line-height: 1.1;
    margin-bottom: 16px;
  }

  h1 em { font-style: italic; color: var(--rose); font-weight: 500; }

  .divider {
    width: 56px;
    height: 1px;
    background: var(--rose);
    margin: 22px auto;
    opacity: 0.7;
  }

  .subtitle {
    color: var(--muted);
    font-size: 0.95rem;
    line-height: 1.8;
    max-width: 420px;
    margin: 0 auto;
  }

  .section-label {
    font-size: 0.7rem;
    letter-spacing: 0.25em;
    text-transform: uppercase;
    color: var(--muted);
    margin-bottom: 14px;
    padding-left: 4px;
  }

  .card {
    display: flex;
    align-items: center;
    gap: 18px;
    padding: 22px;
    background: var(--card);
    backdrop-filter: blur(8px);
    -webkit-backdrop-filter: blur(8px);
    border: 1px solid rgba(255, 255, 255, 0.9);
    border-radius: 22px;
    text-decoration: none;
    color: inherit;
    box-shadow: 0 10px 30px rgba(201, 143, 138, 0.15);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }

  .card:hover, .card:focus-visible {
    transform: translateY(-3px);
    box-shadow: 0 16px 38px rgba(201, 143, 138, 0.25);
    outline: none;
  }

  .icon {
    flex: 0 0 54px;
    height: 54px;
    border-radius: 16px;
    background: linear-gradient(135deg, var(--blush), var(--sage));
    display: grid;
    place-items: center;
    font-size: 1.5rem;
  }

  .card-body { flex: 1; min-width: 0; }

  .card-title {
    font-family: 'Cormorant Garamond', serif;
    font-size: 1.45rem;
    font-weight: 600;
    margin-bottom: 2px;
  }

  .card-desc { font-size: 0.85rem; color: var(--muted); }

  .arrow {
    color: var(--rose);
    font-size: 1.4rem;
    transition: transform 0.3s ease;
  }

  .card:hover .arrow { transform: translateX(4px); }

  footer {
    text-align: center;
    padding: 28px 24px 36px;
    font-size: 0.78rem;
    color: var(--muted);
    letter-spacing: 0.05em;
  }

  .fade { animation: fade 0.9s ease both; }
  .fade.d2 { animation-delay: 0.2s; }
  @keyframes fade {
    from { opacity: 0; transform: translateY(14px); }
    to   { opacity: 1; transform: none; }
  }
</style>
</head>
<body>
  <main>
    <section class="hero fade">
      <p class="eyebrow">Selamat Datang</p>
      <h1>Project <em>Sendiri</em></h1>
      <div class="divider"></div>
      <p class="subtitle">Kumpulan tools pribadi yang dibuat dengan sederhana, rapi, dan sepenuh hati.</p>
    </section>

    <section class="fade d2">
      <p class="section-label">Halaman</p>
      <a class="card" href="https://pelitaonline.github.io/projectsendiri/timeline-felicia.html">
        <div class="icon">🌸</div>
        <div class="card-body">
          <div class="card-title">Timeline Felicia</div>
          <div class="card-desc">Buka halaman timeline</div>
        </div>
        <span class="arrow">→</span>
      </a>
    </section>
  </main>

  <footer>© 2026 Project Sendiri</footer>
</body>
</html>
