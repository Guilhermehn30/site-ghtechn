[index (3).html](https://github.com/user-attachments/files/33918509/index.3.html)
<!doctype html>
<html lang="pt-BR">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>GHTECHN | Suporte de TI, CFTV e controle de acesso em São Paulo</title>
<meta name="description" content="Suporte de TI remoto com atendimento presencial, gerenciamento de Microsoft 365, CFTV, controle de acesso e infraestrutura de rede para pequenas e médias empresas em São Paulo.">
<meta property="og:title" content="GHTECHN | TI, CFTV e controle de acesso para empresas">
<meta property="og:description" content="Suporte de TI remoto com atendimento presencial quando precisar. Para pequenas e médias empresas em São Paulo.">
<meta property="og:type" content="website">
<meta property="og:url" content="https://ghtechn.com.br">
<link rel="icon" href="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 64 64'%3E%3Crect width='64' height='64' rx='12' fill='%230F2233'/%3E%3Ccircle cx='20' cy='32' r='6' fill='%232BB673'/%3E%3Crect x='32' y='26' width='16' height='12' rx='2' fill='%23EDF0F2'/%3E%3C/svg%3E">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Familjen+Grotesk:wght@500;600;700&family=Instrument+Sans:wght@400;500;600&display=swap" rel="stylesheet">

<!--
  ANTES DE PUBLICAR: confira o e-mail de contato no rodapé (contato@ghtechn.com.br).
  O número do WhatsApp fica na variável WA_NUMBER (no fim do arquivo): 55 + DDD + número, só dígitos.
-->

<style>
  :root {
    --paper: #EDF0F2;
    --panel: #FFFFFF;
    --ink: #0F2233;
    --ink-soft: #46586A;
    --line: #CBD3DB;
    --cable: #1F5FBF;
    --led: #1E9E5E;
    --led-glow: #2BB673;
    --radius: 10px;
    --max: 1080px;
  }
  * { box-sizing: border-box; }
  html { scroll-behavior: smooth; }
  body {
    margin: 0;
    background: var(--paper);
    color: var(--ink);
    font-family: "Instrument Sans", system-ui, sans-serif;
    font-size: 17px;
    line-height: 1.6;
    -webkit-font-smoothing: antialiased;
  }
  h1, h2, h3 { font-family: "Familjen Grotesk", system-ui, sans-serif; line-height: 1.1; margin: 0; letter-spacing: -0.02em; }
  p { margin: 0; }
  a { color: inherit; }
  :focus-visible { outline: 3px solid var(--cable); outline-offset: 3px; border-radius: 4px; }
  .wrap { width: min(var(--max), 100% - 32px); margin-inline: auto; }

  /* Topo */
  header.top { padding: 18px 0; }
  header.top .wrap { display: flex; align-items: center; justify-content: space-between; gap: 16px; }
  .brand { font-family: "Familjen Grotesk", sans-serif; font-weight: 700; font-size: 1.35rem; letter-spacing: -0.03em; text-decoration: none; display: inline-flex; align-items: center; gap: 10px; }
  .brand i { width: 12px; height: 12px; border-radius: 50%; background: var(--led-glow); box-shadow: 0 0 0 4px rgba(43,182,115,.2); display: inline-block; }
  .btn {
    display: inline-flex; align-items: center; justify-content: center; gap: 10px;
    background: var(--ink); color: #fff; text-decoration: none; font-weight: 600;
    padding: 13px 22px; border-radius: 999px; border: 0; cursor: pointer; font-size: 1rem;
    transition: background .2s, transform .2s;
  }
  .btn:hover { background: #1a3550; transform: translateY(-1px); }
  .btn.wa { background: var(--led); }
  .btn.wa:hover { background: #17884f; }
  .btn.small { padding: 9px 16px; font-size: .95rem; }
  .btn svg { width: 20px; height: 20px; fill: currentColor; }

  /* Hero */
  .hero { padding: clamp(40px, 8vw, 96px) 0 clamp(48px, 8vw, 88px); }
  .hero .wrap { display: grid; grid-template-columns: 1.1fr .9fr; gap: clamp(32px, 6vw, 72px); align-items: center; }
  .hero h1 { font-size: clamp(2.3rem, 5.4vw, 4rem); font-weight: 700; max-width: 14ch; }
  .hero p.lead { margin-top: 22px; font-size: 1.15rem; color: var(--ink-soft); max-width: 46ch; }
  .hero .actions { margin-top: 32px; display: flex; flex-wrap: wrap; gap: 14px; align-items: center; }
  .hero .actions span { color: var(--ink-soft); font-size: .95rem; }

  /* Painel de patch: o elemento memorável */
  .rack {
    background: var(--ink); border-radius: 14px; padding: 22px 22px 26px;
    box-shadow: 0 24px 40px -24px rgba(15,34,51,.55);
  }
  .rack .rack-head { display: flex; justify-content: space-between; align-items: center; color: #9FB3C6; font-size: .85rem; margin-bottom: 18px; }
  .rack .rack-head b { color: #fff; font-family: "Familjen Grotesk", sans-serif; font-size: 1rem; font-weight: 600; }
  .ports { display: grid; grid-template-columns: repeat(6, 1fr); gap: 10px; }
  .port {
    aspect-ratio: 1 / 1.05; background: #0A1722; border: 2px solid #284257; border-radius: 6px; position: relative;
  }
  .port::before { content: ""; position: absolute; inset: 24% 18% 18%; border: 2px solid #1c3347; border-top: 0; border-radius: 0 0 4px 4px; }
  .port::after {
    content: ""; position: absolute; top: 8px; right: 8px; width: 7px; height: 7px; border-radius: 50%;
    background: var(--led-glow); box-shadow: 0 0 8px var(--led-glow);
  }
  .port.off::after { background: #284257; box-shadow: none; }
  .port.slow::after { animation: pulse 3.2s ease-in-out infinite; }
  .port.slow.d2::after { animation-delay: 1.1s; }
  .port.slow.d3::after { animation-delay: 2.1s; }
  @keyframes pulse { 0%, 100% { opacity: 1; } 50% { opacity: .25; } }
  .rack .rack-foot { margin-top: 18px; display: flex; gap: 8px; flex-wrap: wrap; }
  .rack .tag { color: #C9D6E2; font-size: .85rem; border: 1px solid #284257; border-radius: 999px; padding: 4px 12px; }

  /* Seções */
  section { padding: clamp(44px, 7vw, 80px) 0; }
  .sec-head { max-width: 640px; margin-bottom: 36px; }
  .sec-head h2 { font-size: clamp(1.7rem, 3.4vw, 2.5rem); font-weight: 700; }
  .sec-head p { margin-top: 14px; color: var(--ink-soft); }

  /* Serviços: lista em linhas, não cards */
  .services { background: var(--panel); border-block: 1px solid var(--line); }
  .svc { display: grid; grid-template-columns: 260px 1fr; gap: 12px 40px; padding: 26px 0; border-top: 1px solid var(--line); }
  .svc:first-of-type { border-top: 0; padding-top: 0; }
  .svc h3 { font-size: 1.4rem; font-weight: 600; }
  .svc p { color: var(--ink-soft); max-width: 62ch; }
  .svc ul { margin: 12px 0 0; padding-left: 18px; color: var(--ink); }
  .svc li { margin: 4px 0; }

  /* Como funciona: sequência real */
  .steps { list-style: none; padding: 0; margin: 0; display: grid; grid-template-columns: repeat(4, 1fr); gap: 20px; counter-reset: s; }
  .steps li { counter-increment: s; border-top: 3px solid var(--cable); padding-top: 14px; }
  .steps li::before { content: counter(s); font-family: "Familjen Grotesk", sans-serif; font-weight: 700; color: var(--cable); font-size: 1.1rem; }
  .steps h3 { font-size: 1.15rem; margin: 6px 0 8px; font-weight: 600; }
  .steps p { color: var(--ink-soft); font-size: .98rem; }

  /* Para quem */
  .fit { background: var(--ink); color: #fff; }
  .fit .sec-head p { color: #B7C6D4; }
  .fit-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 28px; }
  .fit-grid h3 { font-size: 1.15rem; font-weight: 600; margin-bottom: 8px; }
  .fit-grid p { color: #B7C6D4; font-size: .98rem; }

  /* Contato */
  .contact .box { background: var(--panel); border: 1px solid var(--line); border-radius: 16px; padding: clamp(26px, 5vw, 48px); display: grid; grid-template-columns: 1.2fr .8fr; gap: 32px; align-items: center; }
  .contact h2 { font-size: clamp(1.7rem, 3.4vw, 2.4rem); font-weight: 700; }
  .contact p { margin-top: 12px; color: var(--ink-soft); }
  .contact .right { display: grid; gap: 12px; justify-items: start; }
  .contact .right small { color: var(--ink-soft); }

  footer { padding: 28px 0 48px; color: var(--ink-soft); font-size: .92rem; }
  footer .wrap { display: flex; flex-wrap: wrap; justify-content: space-between; gap: 10px; }

  @media (max-width: 860px) {
    .hero .wrap { grid-template-columns: 1fr; }
    .svc { grid-template-columns: 1fr; }
    .steps { grid-template-columns: 1fr 1fr; }
    .fit-grid { grid-template-columns: 1fr; }
    .contact .box { grid-template-columns: 1fr; }
  }
  @media (max-width: 520px) {
    body { font-size: 16px; }
    .steps { grid-template-columns: 1fr; }
    header.top .btn.small span { display: none; }
  }
  @media (prefers-reduced-motion: reduce) {
    html { scroll-behavior: auto; }
    .port.slow::after { animation: none; }
    .btn { transition: none; }
  }
</style>
</head>
<body>

<header class="top">
  <div class="wrap">
    <a class="brand" href="#topo" aria-label="GHTECHN, início"><i></i>GHTECHN</a>
    <a class="btn wa small" data-wa href="https://wa.me/5511974455720">
      <svg viewBox="0 0 24 24" aria-hidden="true"><path d="M12.04 2a9.9 9.9 0 0 0-8.5 14.9L2 22l5.25-1.4A9.9 9.9 0 1 0 12.04 2zm5.8 14.1c-.25.7-1.45 1.35-2 1.4-.52.06-1.17.08-1.9-.12a16 16 0 0 1-5.7-3.5 8.5 8.5 0 0 1-2-3.4c-.2-1 .2-1.8.45-2.1.25-.3.55-.37.74-.37h.52c.17 0 .4-.06.62.48.24.57.8 1.97.87 2.1.07.15.12.32.02.5-.1.2-.15.32-.3.5l-.45.5c-.15.15-.3.3-.13.6.17.3.77 1.27 1.65 2.05 1.13 1 2.1 1.32 2.4 1.47.3.15.47.12.65-.07.17-.2.75-.87.95-1.17.2-.3.4-.25.67-.15.27.1 1.72.8 2.02.97.3.15.5.22.57.35.07.12.07.7-.18 1.4z"/></svg>
      <span>Falar no WhatsApp</span>
    </a>
  </div>
</header>

<main id="topo">
  <div class="hero">
    <div class="wrap">
      <div>
        <h1>Sua empresa funcionando, sem parar por problema de TI.</h1>
        <p class="lead">Suporte de TI remoto com atendimento presencial quando for preciso. Também instalamos câmeras, controle de acesso e a rede da sua empresa, em São Paulo.</p>
        <div class="actions">
          <a class="btn wa" data-wa href="https://wa.me/5511974455720">
            <svg viewBox="0 0 24 24" aria-hidden="true"><path d="M12.04 2a9.9 9.9 0 0 0-8.5 14.9L2 22l5.25-1.4A9.9 9.9 0 1 0 12.04 2zm5.8 14.1c-.25.7-1.45 1.35-2 1.4-.52.06-1.17.08-1.9-.12a16 16 0 0 1-5.7-3.5 8.5 8.5 0 0 1-2-3.4c-.2-1 .2-1.8.45-2.1.25-.3.55-.37.74-.37h.52c.17 0 .4-.06.62.48.24.57.8 1.97.87 2.1.07.15.12.32.02.5-.1.2-.15.32-.3.5l-.45.5c-.15.15-.3.3-.13.6.17.3.77 1.27 1.65 2.05 1.13 1 2.1 1.32 2.4 1.47.3.15.47.12.65-.07.17-.2.75-.87.95-1.17.2-.3.4-.25.67-.15.27.1 1.72.8 2.02.97.3.15.5.22.57.35.07.12.07.7-.18 1.4z"/></svg>
            Pedir uma conversa
          </a>
          <span>Resposta pelo WhatsApp, sem formulário.</span>
        </div>
      </div>

      <div class="rack" role="img" aria-label="Ilustração de um painel de rede com portas ativas">
        <div class="rack-head"><b>Rede da sua empresa</b><span>tudo no ar</span></div>
        <div class="ports" aria-hidden="true">
          <div class="port slow"></div><div class="port"></div><div class="port slow d2"></div><div class="port"></div><div class="port slow d3"></div><div class="port"></div>
          <div class="port"></div><div class="port slow d3"></div><div class="port"></div><div class="port off"></div><div class="port slow"></div><div class="port"></div>
        </div>
        <div class="rack-foot" aria-hidden="true">
          <span class="tag">Computadores</span><span class="tag">Microsoft 365</span><span class="tag">Câmeras</span><span class="tag">Acesso</span><span class="tag">Wi-Fi</span>
        </div>
      </div>
    </div>
  </div>

  <section class="services" id="servicos">
    <div class="wrap">
      <div class="sec-head">
        <h2>O que a GHTECHN faz pela sua empresa</h2>
        <p>Cinco frentes, com um único responsável. Você fala com uma pessoa só, em vez de correr atrás de vários fornecedores.</p>
      </div>

      <div class="svc">
        <h3>Suporte de TI (service desk)</h3>
        <div>
          <p>Atendimento remoto para a equipe resolver o dia a dia sem esperar, com visita presencial quando o problema exige.</p>
          <ul>
            <li>Computadores, impressoras, e-mail e acessos de usuários</li>
            <li>Backup, antivírus e manutenção preventiva</li>
            <li>Plano mensal combinado conforme o tamanho da equipe</li>
          </ul>
        </div>
      </div>

      <div class="svc">
        <h3>Gerenciamento de Microsoft 365</h3>
        <div>
          <p>Administração do ambiente Microsoft da sua empresa, para a equipe trabalhar de qualquer lugar com segurança e sem perder arquivos.</p>
          <ul>
            <li>Office 365: contas de usuários, licenças e e-mail</li>
            <li>SharePoint e OneDrive: pastas, permissões e compartilhamento organizados</li>
            <li>Intune: gerenciamento e proteção de computadores e celulares da empresa</li>
            <li>Políticas de segurança e suporte aos usuários no dia a dia</li>
          </ul>
        </div>
      </div>

      <div class="svc">
        <h3>CFTV e câmeras</h3>
        <div>
          <p>Projeto e instalação de câmeras para você acompanhar a empresa de onde estiver.</p>
          <ul>
            <li>Visualização pelo celular</li>
            <li>Gravação com armazenamento dimensionado para o seu caso</li>
            <li>Manutenção e ajustes depois da instalação</li>
          </ul>
        </div>
      </div>

      <div class="svc">
        <h3>Controle de acesso</h3>
        <div>
          <p>Saiba quem entra e quando, com portas liberadas só para quem precisa.</p>
          <ul>
            <li>Leitores de cartão, biometria ou senha</li>
            <li>Cadastro e bloqueio de pessoas de forma simples</li>
            <li>Integração com o restante da segurança da empresa</li>
          </ul>
        </div>
      </div>

      <div class="svc">
        <h3>Infraestrutura de rede</h3>
        <div>
          <p>Cabeamento, Wi-Fi e organização do rack para a internet parar de cair no meio do expediente.</p>
          <ul>
            <li>Cabeamento estruturado e pontos de rede</li>
            <li>Wi-Fi bem distribuído pelo ambiente</li>
            <li>Rack organizado e identificado</li>
          </ul>
        </div>
      </div>
    </div>
  </section>

  <section id="como-funciona">
    <div class="wrap">
      <div class="sec-head">
        <h2>Como começamos</h2>
        <p>Sem contrato longo e sem proposta genérica. Primeiro entendemos o que a sua empresa precisa.</p>
      </div>
      <ol class="steps">
        <li><h3>Conversa rápida</h3><p>Você conta no WhatsApp como é a empresa e qual é o problema.</p></li>
        <li><h3>Diagnóstico</h3><p>Levantamos o que existe hoje: equipamentos, rede e pontos de risco.</p></li>
        <li><h3>Proposta clara</h3><p>Você recebe o que será feito e quanto custa, antes de qualquer cobrança.</p></li>
        <li><h3>Atendimento contínuo</h3><p>Suporte remoto no dia a dia e visita presencial quando necessário.</p></li>
      </ol>
    </div>
  </section>

  <section class="fit">
    <div class="wrap">
      <div class="sec-head">
        <h2>Feito para pequenas e médias empresas</h2>
        <p>Quem tem equipe enxuta e não precisa (nem quer pagar) um departamento de TI inteiro.</p>
      </div>
      <div class="fit-grid">
        <div><h3>Escritórios e consultórios</h3><p>Computadores, impressoras, e-mail e rede funcionando todo dia.</p></div>
        <div><h3>Comércio e lojas</h3><p>Câmeras, controle de entrada e internet estável para o caixa e o estoque.</p></div>
        <div><h3>Empresas em crescimento</h3><p>Rede e segurança organizadas para acompanhar a abertura de novas salas e filiais.</p></div>
      </div>
    </div>
  </section>

  <section class="contact" id="contato">
    <div class="wrap">
      <div class="box">
        <div>
          <h2>Conte o que a sua empresa precisa</h2>
          <p>Mande uma mensagem com o tipo de negócio, o número de pessoas e o problema. Respondemos pelo WhatsApp.</p>
        </div>
        <div class="right">
          <a class="btn wa" data-wa href="https://wa.me/5511974455720">
            <svg viewBox="0 0 24 24" aria-hidden="true"><path d="M12.04 2a9.9 9.9 0 0 0-8.5 14.9L2 22l5.25-1.4A9.9 9.9 0 1 0 12.04 2zm5.8 14.1c-.25.7-1.45 1.35-2 1.4-.52.06-1.17.08-1.9-.12a16 16 0 0 1-5.7-3.5 8.5 8.5 0 0 1-2-3.4c-.2-1 .2-1.8.45-2.1.25-.3.55-.37.74-.37h.52c.17 0 .4-.06.62.48.24.57.8 1.97.87 2.1.07.15.12.32.02.5-.1.2-.15.32-.3.5l-.45.5c-.15.15-.3.3-.13.6.17.3.77 1.27 1.65 2.05 1.13 1 2.1 1.32 2.4 1.47.3.15.47.12.65-.07.17-.2.75-.87.95-1.17.2-.3.4-.25.67-.15.27.1 1.72.8 2.02.97.3.15.5.22.57.35.07.12.07.7-.18 1.4z"/></svg>
            Chamar no WhatsApp
          </a>
          <small>Ou escreva para <a href="mailto:contato@ghtechn.com.br">contato@ghtechn.com.br</a></small>
        </div>
      </div>
    </div>
  </section>
</main>

<footer>
  <div class="wrap">
    <span>© <span id="ano">2026</span> GHTECHN. São Paulo, SP.</span>
    <span>Suporte de TI, CFTV, controle de acesso e redes.</span>
  </div>
</footer>

<script>
  // Troque aqui pelo seu número: 55 + DDD + número, só dígitos.
  var WA_NUMBER = "5511974455720";
  var WA_TEXT = "Olá! Vi o site da GHTECHN e gostaria de conversar sobre TI para a minha empresa.";
  var link = "https://wa.me/" + WA_NUMBER + "?text=" + encodeURIComponent(WA_TEXT);
  document.querySelectorAll("[data-wa]").forEach(function (a) { a.href = link; a.target = "_blank"; a.rel = "noopener"; });
  document.getElementById("ano").textContent = new Date().getFullYear();
</script>
</body>
</html>
