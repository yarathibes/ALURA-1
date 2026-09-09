<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Visão para Tecnologia</title>

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, Helvetica, sans-serif;
    }

    body {
      background: #111827;
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
    }

    .slide {
      width: 1280px;
      height: 720px;
      background: linear-gradient(135deg, #071426, #102a4c);
      color: white;
      padding: 55px 70px;
      position: relative;
      overflow: hidden;
    }

    /* Elementos decorativos */
    .circle {
      position: absolute;
      border-radius: 50%;
      filter: blur(2px);
      opacity: .25;
    }

    .circle.one {
      width: 350px;
      height: 350px;
      background: #00bfff;
      right: -120px;
      top: -130px;
    }

    .circle.two {
      width: 280px;
      height: 280px;
      background: #7c3aed;
      left: -120px;
      bottom: -100px;
    }

    /* Cabeçalho */
    .header {
      position: relative;
      z-index: 2;
      margin-bottom: 35px;
    }

    .header h1 {
      font-size: 48px;
      letter-spacing: 2px;
      font-weight: 800;
    }

    .header h1 span {
      color: #22d3ee;
    }

    .header p {
      margin-top: 10px;
      font-size: 21px;
      color: #cbd5e1;
    }

    /* Conteúdo */
    .content {
      display: grid;
      grid-template-columns: 1fr 120px 1fr;
      gap: 25px;
      align-items: center;
      position: relative;
      z-index: 2;
    }

    .box {
      min-height: 390px;
      border-radius: 24px;
      padding: 35px;
      backdrop-filter: blur(10px);
      box-shadow: 0 20px 50px rgba(0,0,0,.25);
    }

    .problem {
      background: linear-gradient(
        145deg,
        rgba(239,68,68,.20),
        rgba(30,41,59,.75)
      );
      border: 1px solid rgba(248,113,113,.35);
    }

    .solution {
      background: linear-gradient(
        145deg,
        rgba(34,211,238,.18),
        rgba(30,41,59,.75)
      );
      border: 1px solid rgba(34,211,238,.35);
    }

    .box h2 {
      font-size: 29px;
      margin-bottom: 28px;
    }

    .problem h2 {
      color: #f87171;
    }

    .solution h2 {
      color: #22d3ee;
    }

    .item {
      display: flex;
      align-items: center;
      gap: 15px;
      margin: 20px 0;
      font-size: 19px;
      color: #e2e8f0;
    }

    .icon {
      width: 40px;
      height: 40px;
      border-radius: 12px;
      display: flex;
      justify-content: center;
      align-items: center;
      font-size: 20px;
      flex-shrink: 0;
    }

    .problem .icon {
      background: rgba(239,68,68,.18);
    }

    .solution .icon {
      background: rgba(34,211,238,.15);
    }

    /* Seta central */
    .arrow {
      width: 90px;
      height: 90px;
      border-radius: 50%;
      background: linear-gradient(135deg, #06b6d4, #7c3aed);
      display: flex;
      justify-content: center;
      align-items: center;
      font-size: 43px;
      box-shadow: 0 0 35px rgba(34,211,238,.35);
    }

    /* Rodapé */
    .footer {
      position: absolute;
      bottom: 45px;
      left: 70px;
      right: 70px;
      z-index: 2;
      background: rgba(15,23,42,.75);
      border: 1px solid rgba(255,255,255,.10);
      border-radius: 18px;
      padding: 20px 30px;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .footer strong {
      color: #22d3ee;
      font-size: 18px;
    }

    .results {
      display: flex;
      gap: 25px;
      color: #cbd5e1;
      font-size: 16px;
    }

    .result {
      display: flex;
      align-items: center;
      gap: 7px;
    }

    .check {
      color: #22c55e;
      font-weight: bold;
    }

    /* Responsividade */
    @media (max-width: 1000px) {
      .slide {
        transform: scale(.75);
        transform-origin: center;
      }
    }
  </style>
</head>

<body>

  <div class="slide">

    <div class="circle one"></div>
    <div class="circle two"></div>

    <!-- Título -->
    <div class="header">
      <h1>VISÃO PARA <span>TECNOLOGIA</span></h1>
      <p>Transformar problemas em soluções inteligentes</p>
    </div>

    <!-- Problema / Solução -->
    <div class="content">

      <!-- PROBLEMA -->
      <div class="box problem">

        <h2>⚠ PROBLEMA</h2>

        <div class="item">
          <div class="icon">🔗</div>
          <span>Sistemas desconectados</span>
        </div>

        <div class="item">
          <div class="icon">📝</div>
          <span>Processos manuais</span>
        </div>

        <div class="item">
          <div class="icon">📊</div>
          <span>Dados dispersos</span>
        </div>

        <div class="item">
          <div class="icon">⏱</div>
          <span>Baixa produtividade</span>
        </div>

      </div>

      <!-- TRANSFORMAÇÃO -->
      <div class="arrow">
        →
      </div>

      <!-- SOLUÇÃO -->
      <div class="box solution">

        <h2>✓ SOLUÇÃO</h2>

        <div class="item">
          <div class="icon">🔄</div>
          <span>Integração de sistemas</span>
        </div>

        <div class="item">
          <div class="icon">⚙</div>
          <span>Automação de processos</span>
        </div>

        <div class="item">
          <div class="icon">☁</div>
          <span>Dados centralizados</span>
        </div>

        <div class="item">
          <div class="icon">💡</div>
          <span>Inteligência e inovação</span>
        </div>

      </div>

    </div>

    <!-- Resultado -->
    <div class="footer">

      <strong>RESULTADO</strong>

      <div class="results">
        <div class="result">
          <span class="check">✓</span>
          Mais agilidade
        </div>

        <div class="result">
          <span class="check">✓</span>
          Eficiência
        </div>

        <div class="result">
          <span class="check">✓</span>
          Produtividade
        </div>

        <div class="result">
          <span class="check">✓</span>
          Inovação
        </div>
      </div>

    </div>

  </div>

</body>
</html>
