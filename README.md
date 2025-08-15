<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Sathler — Site oficial</title>

  <!-- Tipografia (Google Fonts) -->
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;800&display=swap" rel="stylesheet">

  <!-- Metadados sociais -->
  <meta name="description" content="Bem-vindo ao site da Sathler. Serviços, portfólio e contato.">
  <meta property="og:title" content="Sathler — Site oficial">
  <meta property="og:description" content="Bem-vindo ao site da Sathler. Serviços, portfólio e contato.">
  <meta property="og:type" content="website">
  <meta property="og:url" content="https://www.sathler.com.br/">

  <style>
    :root{
      --bg: #0b0c10;
      --card: #12131a;
      --text: #e8e8ee;
      --muted:#a8adbd;
      --accent:#7c5cff;
    }
    *{box-sizing:border-box}
    html,body{margin:0}
    body{
      font-family: Inter, system-ui, -apple-system, Segoe UI, Roboto, Arial, sans-serif;
      background: radial-gradient(1200px 600px at 10% -10%, #1c1d26 10%, transparent 50%) , var(--bg);
      color: var(--text);
      line-height: 1.6;
    }
    a{color:inherit;text-decoration:none}
    .container{max-width: 1080px; margin: 0 auto; padding: 24px}
    header{
      position: sticky; top:0; backdrop-filter: blur(6px);
      border-bottom: 1px solid #22232e; background: rgba(11,12,16,.65);
    }
    .nav{
      display:flex; align-items:center; justify-content:space-between;
    }
    .brand{font-weight:800; letter-spacing:.4px}
    .nav a{
      padding:10px 12px; border-radius:8px;
    }
    .nav a:hover{background:#1b1c25}

    .hero{
      padding: 72px 0 36px;
      display:grid; gap:16px;
    }
    .kicker{
      display:inline-block; font-size:.85rem; color: var(--muted);
      border:1px solid #2a2b3a; padding:6px 10px; border-radius:999px;
    }
    h1{
      margin:8px 0 4px; font-size: clamp(36px, 5vw, 56px); line-height: 1.1;
    }
    .lead{color:var(--muted); font-size: clamp(16px, 2.2vw, 18px); max-width: 60ch}

    .actions{display:flex; gap:12px; margin-top: 16px; flex-wrap: wrap}
    .btn{
      display:inline-block; padding:12px 18px; border-radius:12px; font-weight:600;
      border:1px solid #2a2b3a; background:#1a1b24;
    }
    .btn.primary{background: linear-gradient(120deg, #8468ff, #5f8bff); border:none}
    .btn:hover{transform: translateY(-1px)}

    .section{padding: 36px 0}
    .cards{
      display:grid; gap:16px;
      grid-template-columns: repeat(auto-fit,minmax(240px,1fr));
    }
    .card{
      background: var(--card); border:1px solid #22232e; border-radius:16px;
      padding:18px;
    }
    .card h3{margin:0 0 6px}
    footer{
      border-top: 1px solid #22232e; color:var(--muted);
    }
    .small{font-size:.9rem; color:var(--muted)}
  </style>
</head>
<body>
  <header>
    <div class="container nav">
      <div class="brand">Sathler</div>
      <nav>
        <a href="#servicos">Serviços</a>
        <a href="#sobre">Sobre</a>
        <a href="#contato">Contato</a>
      </nav>
    </div>
  </header>

  <main class="container">
    <section class="hero">
      <span class="kicker">Bem-vindo(a)</span>
      <h1>Resultados claros, sem complicação.</h1>
      <p class="lead">Este é um modelo inicial para você colocar seu conteúdo. Edite os textos, adicione seu portfólio e publique em poucos cliques.</p>
      <div class="actions">
        <a class="btn primary" href="#contato">Fale comigo</a>
        <a class="btn" href="#servicos">Ver serviços</a>
      </div>
    </section>

    <section id="servicos" class="section">
      <h2>Serviços</h2>
      <div class="cards">
        <article class="card">
          <h3>Consultoria</h3>
          <p>Diagnóstico rápido e plano de ação objetivo para seu projeto.</p>
        </article>
        <article class="card">
          <h3>Desenvolvimento</h3>
          <p>Sites rápidos, responsivos e fáceis de manter.</p>
        </article>
        <article class="card">
          <h3>Suporte & Evolução</h3>
          <p>Acompanhamento contínuo para manter tudo no ar e atualizado.</p>
        </article>
      </div>
    </section>

    <section id="sobre" class="section">
      <h2>Sobre</h2>
      <p class="small">Escreva um parágrafo curto sobre quem você é, sua experiência e o que te diferencia.</p>
    </section>

    <section id="contato" class="section">
      <h2>Contato</h2>
      <p class="small">Preferências de contato:</p>
      <p>
        <a class="btn" href="mailto:seuemail@sathler.com.br">📧 Enviar e-mail</a>
        <a class="btn" href="https://wa.me/55SEUNUMERO" target="_blank" rel="noopener">💬 WhatsApp</a>
      </p>
      <p class="small">Substitua o e-mail e o número acima pelos seus.</p>
    </section>
  </main>

  <footer>
    <div class="container">
      <p class="small">© <span id="y"></span> Sathler — Todos os direitos reservados.</p>
    </div>
  </footer>

  <script>
    // Atualiza o ano automaticamente
    document.getElementById('y').textContent = new Date().getFullYear();
  </script>
</body>
</html>
