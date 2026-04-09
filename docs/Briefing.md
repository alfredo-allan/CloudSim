📋 BRIEFING TÉCNICO - CloudSim Lab
🔧 CDNs Necessários (colar no <head>)
html

<!-- Bootstrap 5 CSS -->
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet" />

<!-- Font Awesome 6 -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" />

<!-- Anime.js (opcional, usado no script.js) -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/animejs/3.2.1/anime.min.js"></script>

<!-- Bootstrap JS (colar antes do fechamento do </body>) -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>

🎨 Cores do Tema (Variáveis CSS)
css

:root {
--bg-primary: #0f0f0f;
--bg-secondary: #1a1a1a;
--bg-darker: #0a0a0a;
--text-primary: #ffffff;
--text-secondary: #e0e0e0;
--text-gray: #a0a0a0;
--accent-primary: #6c5ce7;
--accent-secondary: #a29bfe;
--border-color: #2a2a2a;
--card-hover: #252525;
}

📁 Estrutura de Arquivos
text

projeto/
├── index.html
├── css/
│ ├── styles.css
│ └── header.css
├── js/
│ ├── script.js
│ └── header.js
└── CloudSim.pdf

🧩 Classes CSS Principais
Classe Uso
.section-padding padding: 100px 0 (60px no mobile)
.bg-darker fundo #0a0a0a para seções alternadas
.card fundo #1a1a1a, borda, border-radius 16px
.concept-tip caixa de dica com ícone e fundo roxo claro
.answer-box.correct caixa de resposta correta (fundo verde claro)
.gradient-text texto com gradiente roxo
.badge.bg-primary badge com gradiente linear
.section-title título com linha inferior colorida
.text-gray cor de texto #a0a0a0
.btn-primary botão com gradiente e hover
📝 Estrutura Padrão de uma Section
html

<section id="nome-da-sessao" class="section-padding bg-darker">
  <div class="container">
    <h2 class="section-title">
      <i class="fas fa-icone me-3"></i>Título da Seção
    </h2>
    <div class="row g-4">
      <div class="col-lg-10 mx-auto">
        <div class="card">
          <div class="card-body">
            <!-- CONTEÚDO AQUI -->
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

🧠 Estrutura de Card Interno
html

<div class="card">
  <div class="card-body">
    <span class="badge bg-primary mb-3">TAG</span>
    <h3><i class="fas fa-icone text-primary me-2"></i>Título</h3>
    <p class="text-gray">Texto descritivo</p>
    
    <div class="concept-tip">
      <i class="fas fa-lightbulb"></i>
      <span>Conteúdo da dica</span>
    </div>
  </div>
</div>

🎯 Ícones Font Awesome Mais Usados
Ícone Classe
Nuvem fa-cloud-upload-alt
Linux fa-linux
Java fa-java
Código fa-code
Terminal fa-terminal
Livro fa-book-open
Engrenagens fa-cogs
Gráfico fa-chart-bar
Bandeira fa-flag-checkered
Pergunta fa-question-circle
Lâmpada fa-lightbulb
Cérebro fa-brain
Banco de dados fa-database
Construção fa-building
🖥️ Scripts Necessários (colar antes do </body>)
html

<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
<script src="./js/script.js"></script>
<script src="./js/header.js"></script>
<script>
  // Progress bar scroll
  window.addEventListener('scroll', function () {
    const winScroll = document.body.scrollTop || document.documentElement.scrollTop
    const height = document.documentElement.scrollHeight - document.documentElement.clientHeight
    const scrolled = (winScroll / height) * 100
    const progressBar = document.querySelector('.reading-progress .progress-bar')
    if (progressBar) progressBar.style.width = scrolled + '%'
  })
</script>

📱 Breakpoints Responsivos
Tela Comportamento
Desktop (>992px) Layout normal
Tablet (768px-992px) Padding reduzido
Mobile (<768px) Padding: 60px 0, fontes menores
✅ Checklist para Nova Seção

    Usar <section> com id único

    Adicionar classe section-padding

    Opcional: bg-darker para fundo alternado

    Título com section-title e ícone

    Conteúdo dentro de .card > .card-body

    Textos com classe .text-gray

    Ícones com cor text-primary

🔗 Links de Referência

    Bootstrap 5: https://getbootstrap.com/docs/5.3

    Font Awesome 6: https://fontawesome.com/icons

    Anime.js: https://animejs.com
