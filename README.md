<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Guia de Resumos de Veterinária | Organize seus estudos</title>
<meta name="description" content="Guia completo de resumos de Fisiologia, Criação Animal, Enfermidades, Fisiopatologia Básica e Farmacologia para estudantes de Medicina Veterinária.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800;900&display=swap" rel="stylesheet">
<style>
  :root{
    --aqua:#3EC6B8;
    --aqua-deep:#1F8E85;
    --blue:#2D6FE0;
    --blue-deep:#1B3E8C;
    --ink:#151A19;
    --gray:#5B6B6A;
    --gray-light:#8AA0A0;
    --paper:#FAFDFC;
    --card:#FFFFFF;
    --line:#E1EEEC;
    --radius:16px;
    --shadow: 0 10px 30px -12px rgba(20,60,60,0.15);
  }
  *{margin:0;padding:0;box-sizing:border-box;}
  html{scroll-behavior:smooth;}
  body{
    font-family:'Inter',-apple-system,BlinkMacSystemFont,sans-serif;
    color:var(--ink);
    background:var(--paper);
    line-height:1.6;
    -webkit-font-smoothing:antialiased;
    overflow-x:hidden;
  }
  img,svg{max-width:100%;display:block;}
  a{text-decoration:none;color:inherit;}
  .wrap{max-width:1080px;margin:0 auto;padding:0 24px;}
  .eyebrow{
    display:inline-flex;align-items:center;gap:8px;
    font-size:13px;font-weight:700;letter-spacing:.08em;text-transform:uppercase;
    color:var(--aqua-deep);
    background:rgba(62,198,184,0.1);
    border:1px solid rgba(62,198,184,0.25);
    padding:6px 14px;border-radius:999px;
    margin-bottom:18px;
  }
  h1,h2,h3{font-weight:800;letter-spacing:-0.02em;color:var(--ink);}
  h2{font-size:clamp(26px,4vw,38px);margin-bottom:14px;}
  h3{font-size:20px;margin-bottom:8px;}
  p{color:var(--gray);font-size:16px;}
  section{padding:76px 0;position:relative;}

  /* divider strip motif — a "prontuário" tab edge, reused as the section signature */
  .tab-divider{
    height:10px;width:100%;
    background:linear-gradient(90deg,var(--aqua) 0%,var(--aqua) 18%,transparent 18%,transparent 22%,var(--blue) 22%,var(--blue) 40%,transparent 40%,transparent 44%,var(--aqua) 44%,var(--aqua) 62%,transparent 62%,transparent 66%,var(--blue) 66%,var(--blue) 84%,transparent 84%);
    opacity:.55;
  }

  /* ===== HEADER / HERO ===== */
  header.hero{
    background:
      radial-gradient(1200px 500px at 15% -10%, rgba(62,198,184,0.16), transparent 60%),
      radial-gradient(900px 500px at 100% 0%, rgba(45,111,224,0.13), transparent 55%),
      var(--paper);
    padding:56px 0 70px;
  }
  .hero-grid{max-width:640px;}
  .hero h1{font-size:clamp(30px,4.4vw,46px);line-height:1.14;margin-bottom:20px;}
  .hero h1 .accent{
    background:linear-gradient(90deg,var(--aqua-deep),var(--blue));
    -webkit-background-clip:text;background-clip:text;color:transparent;
  }
  .hero p.lead{font-size:18px;color:var(--gray);max-width:520px;margin-bottom:32px;}
  .btn{
    display:inline-flex;align-items:center;justify-content:center;gap:10px;
    font-weight:700;font-size:16px;
    padding:17px 30px;border-radius:12px;
    background:linear-gradient(90deg,var(--aqua-deep),var(--blue));
    color:#fff;border:none;cursor:pointer;
    box-shadow:0 14px 28px -10px rgba(31,142,133,0.45);
    transition:transform .18s ease, box-shadow .18s ease;
  }
  .btn:hover{transform:translateY(-2px);box-shadow:0 18px 34px -10px rgba(31,142,133,0.55);}
  .btn:focus-visible{outline:3px solid var(--blue-deep);outline-offset:3px;}
  .btn-sub{font-size:13px;color:var(--gray-light);margin-top:14px;}

  /* ===== PROBLEM ===== */
  .problem{background:var(--card);}
  .problem-grid{display:grid;grid-template-columns:1fr 1fr;gap:48px;align-items:start;}
  .problem ul{list-style:none;display:flex;flex-direction:column;gap:16px;margin-top:8px;}
  .problem li{
    display:flex;gap:12px;align-items:flex-start;
    font-size:16px;color:var(--gray);
    background:var(--paper);border:1px solid var(--line);border-radius:12px;padding:14px 16px;
  }
  .problem li .ic{font-size:20px;flex-shrink:0;}

  /* ===== CONTENTS (5 record cards, tab-file motif) ===== */
  .contents{background:var(--paper);}
  .contents .head{max-width:640px;margin:0 auto 40px;text-align:center;}
  .record-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:18px;}
  .record{
    position:relative;
    background:var(--card);border:1px solid var(--line);border-radius:var(--radius);
    padding:26px 22px 22px;box-shadow:var(--shadow);
    transition:transform .2s ease, box-shadow .2s ease;
  }
  .record:hover{transform:translateY(-4px);}
  .record::before{
    content:attr(data-tab);
    position:absolute;top:-11px;left:22px;
    font-size:11px;font-weight:800;letter-spacing:.08em;
    color:#fff;background:var(--blue-deep);
    padding:4px 10px;border-radius:6px;
  }
  .record .ic{font-size:26px;margin-bottom:12px;display:block;}
  .record h3{font-size:17px;margin-bottom:6px;}
  .record p{font-size:14px;color:var(--gray);}
  .record.wide{grid-column:span 1;}

  /* ===== BENEFITS ===== */
  .benefits{background:var(--card);}
  .benefit-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:20px;margin-top:36px;}
  .benefit{
    padding:26px 22px;border-radius:var(--radius);
    background:var(--paper);border:1px solid var(--line);
  }
  .benefit .ic{font-size:24px;margin-bottom:10px;}
  .benefit h3{font-size:16px;}
  .benefit p{font-size:14px;}
/* ===== TESTIMONIAL ===== */
  .testimonial{background:var(--card);}
  .quote-box{
    max-width:720px;margin:0 auto;text-align:center;
    background:linear-gradient(160deg,#EAFBF8,#EAF1FE);
    border-radius:20px;padding:44px 36px;position:relative;
  }
  .quote-box .ic{font-size:30px;margin-bottom:14px;}
  .quote-box p{font-size:18px;color:var(--ink);font-style:italic;line-height:1.7;}
  .quote-box .who{margin-top:20px;font-size:14px;font-weight:700;color:var(--aqua-deep);font-style:normal;}

  /* ===== PRICING ===== */
  .pricing{
    background:linear-gradient(160deg,var(--blue-deep),var(--aqua-deep));
    color:#fff;
  }
  .pricing .wrap{text-align:center;}
  .pricing h2{color:#fff;}
  .pricing p.lead{color:rgba(255,255,255,0.85);max-width:520px;margin:0 auto 30px;}
  .price-card{
    max-width:420px;margin:0 auto;background:rgba(255,255,255,0.08);
    border:1px solid rgba(255,255,255,0.25);border-radius:20px;
    padding:36px 30px;backdrop-filter:blur(6px);
  }
  .price-old{font-size:14px;color:rgba(255,255,255,0.7);}
  .price-main{font-size:44px;font-weight:900;margin:6px 0 2px;}
  .price-installments{font-size:14px;color:rgba(255,255,255,0.85);margin-bottom:22px;}
  .price-list{list-style:none;text-align:left;display:flex;flex-direction:column;gap:10px;margin-bottom:26px;font-size:14px;}
  .price-list li{display:flex;gap:8px;align-items:center;}
  .pricing .btn{width:100%;background:#fff;color:var(--blue-deep);box-shadow:0 14px 28px -10px rgba(0,0,0,0.35);}
  .pricing .btn:hover{background:#F4FDFC;}

  /* ===== GUARANTEE ===== */
  .guarantee{background:var(--paper);}
  .guarantee-box{
    max-width:640px;margin:0 auto;text-align:center;
    background:var(--card);border:1px solid var(--line);border-radius:20px;
    padding:40px 32px;box-shadow:var(--shadow);
  }
  .guarantee-box .ic{font-size:40px;margin-bottom:14px;}

  /* ===== FAQ ===== */
  .faq{background:var(--card);}
  .faq-list{max-width:760px;margin:36px auto 0;display:flex;flex-direction:column;gap:12px;}
  .faq-item{border:1px solid var(--line);border-radius:12px;overflow:hidden;background:var(--paper);}
  .faq-q{
    width:100%;text-align:left;background:none;border:none;cursor:pointer;
    padding:18px 20px;font-size:16px;font-weight:600;color:var(--ink);
    display:flex;justify-content:space-between;align-items:center;gap:12px;
    font-family:inherit;
  }
  .faq-q:focus-visible{outline:2px solid var(--blue-deep);outline-offset:-2px;}
  .faq-q .plus{font-size:20px;color:var(--aqua-deep);transition:transform .2s ease;flex-shrink:0;}
  .faq-item.open .faq-q .plus{transform:rotate(45deg);}
  .faq-a{
    max-height:0;overflow:hidden;transition:max-height .25s ease;
  }
  .faq-a p{padding:0 20px 18px;font-size:15px;}

  /* ===== FINAL CTA ===== */
  .final-cta{
    background:
      radial-gradient(900px 400px at 50% 0%, rgba(62,198,184,0.18), transparent 60%),
      var(--paper);
    text-align:center;
  }
  .final-cta h2{max-width:620px;margin:0 auto 10px;}
  .final-cta p.lead{max-width:520px;margin:0 auto 30px;}

  footer{padding:32px 0;text-align:center;font-size:13px;color:var(--gray-light);background:var(--paper);border-top:1px solid var(--line);}

  @media (max-width:860px){
    .problem-grid{grid-template-columns:1fr;}
    .record-grid{grid-template-columns:1fr 1fr;}
    .benefit-grid{grid-template-columns:1fr 1fr;}
    .aud-grid{grid-template-columns:1fr;}
  }
  @media (max-width:520px){
    section{padding:56px 0;}
    .record-grid{grid-template-columns:1fr;}
    .benefit-grid{grid-template-columns:1fr;}
    .nav{padding-bottom:32px;}
    .btn{width:100%;padding:16px 22px;}
  }

  @media (prefers-reduced-motion: reduce){
    *{transition:none !important;animation:none !important;}
    html{scroll-behavior:auto;}
  }
</style>
</head>
<body>

<header class="hero">
  <div class="wrap">
    <div class="hero-grid">
      <div>
        <h1>Pare de perder horas juntando materiais de <span class="accent">Veterinária</span></h1>
        <p class="lead">Tenha os principais conteúdos organizados em um só lugar: resumos de Fisiologia, Criação Animal, Enfermidades, Fisiopatologia Básica e Farmacologia — pensados para quem precisa estudar muito conteúdo sem pular entre dezenas de materiais.</p>
        <a href="https://pay.kiwify.com.br/k75g8Pb" class="btn">💉 Quero organizar meus estudos</a>
        <p class="btn-sub">Acesso imediato após a compra · Garantia de 7 dias</p>
      </div>
    </div>
  </div>
</header>
<div class="tab-divider"></div>
<section class="problem">
  <div class="wrap">
    <div class="problem-grid">
      <div>
        <span class="eyebrow">O cenário</span>
        <h2>Você sente que estuda, estuda e ainda parece que falta alguma coisa?</h2>
        <p>Na metade do curso de Veterinária, a quantidade de conteúdo começa a ficar cada vez maior. Você precisa revisar uma matéria, procura um material. Precisa lembrar de outro assunto, abre outro PDF.</p>
        <p style="margin-top:14px;">No fim, uma parte do seu tempo vai embora só tentando encontrar e organizar o que precisa estudar — antes mesmo de abrir o caderno.</p>
      </div>
      <ul>
        <li><span class="ic">📄</span> Aparece uma informação importante em uma aula, outra em uma apostila e outra em uma pesquisa.</li>
        <li><span class="ic">🗂️</span> Materiais espalhados, em formatos diferentes, sem uma organização clara.</li>
        <li><span class="ic">⏳</span> Menos tempo estudando de fato, mais tempo procurando onde está cada conteúdo.</li>
      </ul>
    </div>
  </div>
</section>

<section class="contents">
  <div class="wrap">
    <div class="head">
      <span class="eyebrow">🐾 O que você recebe</span>
      <h2>Um lugar só para organizar sua revisão em Veterinária</h2>
      <p>Em vez de começar cada estudo procurando onde está cada conteúdo, você encontra os principais temas reunidos em um material organizado e visualmente agradável.</p>
    </div>
    <div class="record-grid">
      <div class="record" data-tab="01"><span class="ic">🫀</span><h3>Fisiologia</h3><p>Para revisar os principais conteúdos de forma mais organizada.</p></div>
      <div class="record" data-tab="02"><span class="ic">🐄</span><h3>Criação Animal</h3><p>Conteúdos reunidos para facilitar sua consulta e revisão.</p></div>
      <div class="record" data-tab="03"><span class="ic">🩹</span><h3>Enfermidades</h3><p>Um material estruturado para encontrar e revisar com mais praticidade.</p></div>
      <div class="record" data-tab="04"><span class="ic">🧬</span><h3>Fisiopatologia Básica</h3><p>Para ajudar na compreensão e revisão dos fundamentos.</p></div>
      <div class="record" data-tab="05"><span class="ic">💊</span><h3>Farmacologia</h3><p>Conteúdo organizado para facilitar seus momentos de estudo e revisão.</p></div>
      <div class="record" data-tab="tudo junto"><span class="ic">📚</span><h3>Um único guia</h3><p>Todas as áreas reunidas num só material, com organização pensada para a sua rotina.</p></div>
    </div>
  </div>
</section>

<section class="benefits">
  <div class="wrap">
    <div class="head" style="max-width:640px;margin:0 auto;text-align:center;">
      <span class="eyebrow">Por que funciona</span>
      <h2>Menos tempo procurando. Mais tempo estudando.</h2>
      <p>A proposta do guia é simples: tirar parte da desorganização do caminho para você se concentrar no que realmente importa.</p>
    </div>
    <div class="benefit-grid">
      <div class="benefit"><span class="ic">📚</span><h3>Organização</h3><p>Os conteúdos ficam reunidos em um único material, facilitando a consulta.</p></div>
      <div class="benefit"><span class="ic">⏱️</span><h3>Mais praticidade</h3><p>Menos tempo procurando informações em diferentes lugares antes de começar a estudar.</p></div>
      <div class="benefit"><span class="ic">🧠</span><h3>Revisão direcionada</h3><p>Você consegue voltar aos assuntos de forma mais organizada quando precisar revisar.</p></div>
      <div class="benefit"><span class="ic">📖</span><h3>Conteúdo variado</h3><p>O guia reúne diferentes áreas importantes da formação em Medicina Veterinária.</p></div>
      <div class="benefit"><span class="ic">✨</span><h3>Visualmente organizado</h3><p>A apresentação foi pensada para tornar o estudo mais agradável e fácil de navegar.</p></div>
      <div class="benefit"><span class="ic">🐾</span><h3>Feito por quem vive a rotina</h3><p>Pensado por dentro do curso, para quem também precisa revisar muito conteúdo.</p></div>
    </div>
  </div>
</section>
<section class="audience">
  <div class="wrap">
    <div class="head" style="max-width:640px;margin:0 auto 30px;text-align:center;">
      <span class="eyebrow">Para quem é</span>
      <h2>Este guia é para você?</h2>
    </div>
    <div class="aud-grid">
      <div class="aud-card yes">
        <h3>🩺 É para você que</h3>
        <ul>
          <li>Está cursando Medicina Veterinária, principalmente a partir da metade do curso.</li>
          <li>Sente dificuldade para organizar tantos conteúdos diferentes.</li>
          <li>Perde tempo procurando materiais para estudar.</li>
          <li>Quer ter diferentes assuntos reunidos em um só lugar.</li>
          <li>Gosta de estudar com materiais organizados e visualmente agradáveis.</li>
          <li>Precisa de mais praticidade na hora de revisar.</li>
        </ul>
      </div>
      <div class="aud-card no">
        <h3>🚫 Talvez não seja para você se</h3>
        <ul>
          <li>Você procura um curso completo com aulas ao vivo.</li>
          <li>Você espera que o material substitua todas as aulas e referências da graduação.</li>
          <li>Você não tem interesse em utilizar resumos como apoio aos estudos.</li>
        </ul>
      </div>
    </div>
  </div>
</section>

<section class="testimonial">
  <div class="wrap">
    <div class="quote-box">
      <span class="ic">🧑‍⚕️</span>
      <p>"Sou estudante de Medicina Veterinária, estou no último período e tenho experiência hospitalar em centro cirúrgico. Criei este guia porque conheço de perto a dificuldade de estudar quando os materiais ficam espalhados e você precisa procurar informação em vários lugares para conseguir organizar uma revisão. A ideia foi reunir os conteúdos de uma forma mais prática, organizada e visualmente agradável, ajudando outros estudantes a gastarem menos energia procurando materiais e mais tempo estudando."</p>
      <p class="who">— Nina Neves (@meuestudovivo)<br>Criadora do Guia</p>
    </div>
  </div>
</section>

<section class="pricing">
  <div class="wrap">
    <span class="eyebrow" style="background:rgba(255,255,255,0.15);border-color:rgba(255,255,255,0.3);color:#fff;">🐾 Seu investimento</span>
    <h2>Comece a estudar com tudo organizado</h2>
    <p class="lead">Um material completo e variado, pensado para facilitar sua rotina de estudos na graduação.</p>
    <div class="price-card">
      <div class="price-old">12x de R$ 10,00 ou</div>
      <div class="price-main">R$ 97,00</div>
      <div class="price-installments">à vista</div>
      <ul class="price-list">
        <li>✅ Fisiologia</li>
        <li>✅ Criação Animal</li>
        <li>✅ Enfermidades</li>
        <li>✅ Fisiopatologia Básica</li>
        <li>✅ Farmacologia</li>
      </ul>
      <a href="https://pay.kiwify.com.br/k75g8Pb" class="btn">🐾 Quero ter o guia</a>
    </div>
  </div>
</section>

<section class="guarantee">
  <div class="wrap">
    <div class="guarantee-box">
      <span class="ic">🛡️</span>
      <h2>Garantia de 7 dias</h2>
      <p>Você tem 7 dias de garantia para conhecer o material. A decisão de adquirir o guia fica mais tranquila porque você tem esse período para avaliar se ele faz sentido para sua rotina de estudos.</p>
    </div>
  </div>
</section>

<section class="faq">
  <div class="wrap">
    <div class="head" style="max-width:640px;margin:0 auto;text-align:center;">
      <span class="eyebrow">Dúvidas</span>
      <h2>Perguntas frequentes</h2>
    </div>
    <div class="faq-list" id="faqList">
      <div class="faq-item">
        <button class="faq-q">O guia substitui as aulas da faculdade?<span class="plus">+</span></button>
        <div class="faq-a"><p>Não. O guia funciona como material de apoio para estudo e revisão e não substitui aulas, professores ou outras referências acadêmicas indicadas pela sua instituição.</p></div>
      </div>
      <div class="faq-item">
        <button class="faq-q">Para quem o guia foi feito?<span class="plus">+</span></button>
        <div class="faq-a"><p>Principalmente para estudantes de Medicina Veterinária, especialmente aqueles que já estão na metade do curso e começaram a lidar com uma quantidade maior de conteúdos para revisar.</p></div>
      </div>
      <div class="faq-item">
        <button class="faq-q">Quais conteúdos estão no guia?<span class="plus">+</span></button>
        <div class="faq-a"><p>O material reúne cinco áreas: Fisiologia, Criação Animal, Enfermidades, Fisiopatologia Básica e Farmacologia.</p></div>
      </div>
      <div class="faq-item">
        <button class="faq-q">Como vou receber o material?<span class="plus">+</span></button>
        <div class="faq-a"><p>O acesso é feito pela área de membros da plataforma, enviado imediatamente após a compra para o e-mail informado na compra, e por lá você já visualiza todo o conteúdo.</p></div>
      </div>
      <div class="faq-item">
        <button class="faq-q">Preciso comprar vários materiais diferentes?<span class="plus">+</span></button>
        <div class="faq-a"><p>A proposta do guia é justamente reunir esses conteúdos em um único material, trazendo mais praticidade para sua organização e revisão.</p></div>
      </div>
      <div class="faq-item">
        <button class="faq-q">Tenho quanto tempo de garantia?<span class="plus">+</span></button>
        <div class="faq-a"><p>Você tem 7 dias de garantia.</p></div>
      </div>
      <div class="faq-item">
        <button class="faq-q">Qual é o valor?<span class="plus">+</span></button>
        <div class="faq-a"><p>O investimento é de R$ 97,00 à vista, ou em 12x de R$ 10,00 pela plataforma.</p></div>
      </div>
    </div>
  </div>
</section>

<section class="final-cta">
  <div class="wrap">
    <span class="eyebrow">🐕‍🦺 Última chamada</span>
    <h2>Organize seus estudos. Simplifique sua revisão.</h2>
    <p class="lead">Você já tem conteúdo suficiente para estudar. Agora pode ter os principais temas deste guia organizados em um só lugar.</p>
    <a href="https://pay.kiwify.com.br/k75g8Pb" class="btn">🩺 Quero meu guia de resumos de Veterinária</a>
  </div>
</section>

<footer>
  <div class="wrap">Guia de Resumos de Veterinária · Material de apoio aos estudos, não substitui a graduação.</div>
</footer>

<script>
  document.querySelectorAll('.faq-item').forEach(function(item){
    var q = item.querySelector('.faq-q');
    var a = item.querySelector('.faq-a');
    q.addEventListener('click', function(){
      var isOpen = item.classList.contains('open');
      document.querySelectorAll('.faq-item.open').forEach(function(openItem){
        if(openItem !== item){
          openItem.classList.remove('open');
          openItem.querySelector('.faq-a').style.maxHeight = null;
        }
      });
      if(isOpen){
        item.classList.remove('open');
        a.style.maxHeight = null;
      } else {
        item.classList.add('open');
        a.style.maxHeight = a.scrollHeight + 'px';
      }
    });
  });
</script>

</body>
</html>