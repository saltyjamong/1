<!DOCTYPE html>
<html lang="ko">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>전생연분 · 작품 소개</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Hahmlet:wght@300;400;500;600;700;800&family=Noto+Serif+KR:wght@300;400;500;600;700&family=Gowun+Dodum&display=swap" rel="stylesheet">
<style>
:root{
  --ink:#0c0a08;
  --ink-2:#15110d;
  --night:#121723;
  --amber:#e3a64e;
  --amber-deep:#c47a2b;
  --cinnabar:#b3402d;
  --hanji:#ece2cf;
  --hanji-dim:#a99c84;
  --hanji-faint:#6f6552;
  --jade:#8aa28f;
  --line:rgba(227,166,78,.18);
  --line-soft:rgba(236,226,207,.10);
  --disp:"Hahmlet",serif;
  --body:"Noto Serif KR",serif;
  --ui:"Gowun Dodum",sans-serif;
}
*{margin:0;padding:0;box-sizing:border-box}
html{scroll-behavior:smooth}
body{
  background:var(--ink);
  color:var(--hanji);
  font-family:var(--body);
  font-weight:300;
  line-height:1.9;
  letter-spacing:.01em;
  overflow-x:hidden;
  -webkit-font-smoothing:antialiased;
}
img{display:block;max-width:100%}
.wrap{max-width:1180px;margin:0 auto;padding:0 28px}

/* ---------- eyebrow / labels ---------- */
.eyebrow{
  font-family:var(--ui);
  font-size:.72rem;
  letter-spacing:.42em;
  color:var(--amber);
  text-transform:uppercase;
  display:inline-flex;align-items:center;gap:.9em;
  margin-bottom:1.4rem;
}
.eyebrow::before{content:"";width:34px;height:1px;background:var(--amber);opacity:.6}

/* ---------- hero ---------- */
.hero{
  position:relative;min-height:100svh;
  display:flex;flex-direction:column;justify-content:center;
  overflow:hidden;
}
.hero-sky{position:absolute;inset:0;z-index:0}
.hero-sky svg{width:100%;height:100%;object-fit:cover}
.hero-grain{position:absolute;inset:0;z-index:1;opacity:.05;pointer-events:none;
  background-image:url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='120' height='120'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='.85' numOctaves='2'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)'/%3E%3C/svg%3E");}
.hero-inner{position:relative;z-index:2;text-align:center;padding:0 28px}
.hero-set{
  font-family:var(--ui);font-size:.78rem;letter-spacing:.5em;
  color:var(--hanji-dim);margin-bottom:2.2rem;
  opacity:0;animation:rise 1.1s .2s ease forwards;
}
.hero-set span{color:var(--amber)}
.hero h1{
  font-family:var(--disp);font-weight:800;
  font-size:clamp(4.2rem,17vw,11rem);
  line-height:.92;letter-spacing:.04em;color:var(--hanji);
  text-shadow:0 0 60px rgba(227,166,78,.22);
}
.hero h1 .c{display:inline-block;opacity:0;transform:translateY(40px);
  animation:rise 1s ease forwards;}
.hero h1 .c:nth-child(1){animation-delay:.35s}
.hero h1 .c:nth-child(2){animation-delay:.5s}
.hero h1 .c:nth-child(3){animation-delay:.65s}
.hero-sub{
  margin-top:2.4rem;font-size:clamp(.95rem,2.4vw,1.15rem);
  color:var(--hanji-dim);font-weight:300;line-height:2;
  max-width:30ch;margin-left:auto;margin-right:auto;
  opacity:0;animation:rise 1.1s .9s ease forwards;
}
.scrollcue{
  position:absolute;left:50%;bottom:34px;transform:translateX(-50%);z-index:2;
  font-family:var(--ui);font-size:.66rem;letter-spacing:.34em;color:var(--hanji-faint);
  display:flex;flex-direction:column;align-items:center;gap:.7rem;
  opacity:0;animation:rise 1s 1.4s ease forwards;
}
.scrollcue i{width:1px;height:46px;background:linear-gradient(var(--amber),transparent);
  display:block;animation:cue 2.4s ease-in-out infinite}
@keyframes cue{0%,100%{transform:scaleY(.4);opacity:.3;transform-origin:top}50%{transform:scaleY(1);opacity:1;transform-origin:top}}
@keyframes rise{to{opacity:1;transform:none}}

/* ---------- section frame ---------- */
.section{position:relative;padding:clamp(6rem,12vw,11rem) 0}
.section--ink{background:var(--ink)}
.section--panel{background:
  radial-gradient(120% 80% at 50% 0%,rgba(227,166,78,.05),transparent 60%),
  var(--ink-2);}
.section--night{background:
  radial-gradient(130% 90% at 80% 10%,rgba(64,86,140,.16),transparent 60%),
  var(--night);}
.rule-top{border-top:1px solid var(--line-soft)}

.lead{
  font-family:var(--disp);font-weight:300;
  font-size:clamp(1.5rem,4vw,2.5rem);line-height:1.7;
  letter-spacing:.01em;color:var(--hanji);max-width:24ch;
}
.lead em{font-style:normal;color:var(--amber);font-weight:500}
.intro-grid{display:grid;grid-template-columns:1fr 1fr;gap:clamp(2rem,6vw,6rem);align-items:start}
.intro-body p{color:var(--hanji-dim);font-size:1.02rem;margin-bottom:1.3rem;max-width:46ch}
.intro-body p:last-child{margin-bottom:0}
.intro-body strong{color:var(--hanji);font-weight:500}

/* ---------- heading block ---------- */
.head{margin-bottom:clamp(3rem,6vw,4.5rem);max-width:60ch}
.head h2{
  font-family:var(--disp);font-weight:700;
  font-size:clamp(2.1rem,6vw,3.4rem);line-height:1.2;
  letter-spacing:.02em;color:var(--hanji);
}
.head h2 .han{color:var(--amber-deep);font-weight:400;margin-left:.3em;font-size:.7em;vertical-align:.06em}
.head p{margin-top:1.4rem;color:var(--hanji-dim);font-size:1.02rem;max-width:52ch}

/* ---------- world cards ---------- */
.cards{display:grid;grid-template-columns:repeat(auto-fit,minmax(260px,1fr));gap:1px;
  background:var(--line-soft);border:1px solid var(--line-soft)}
.card{background:var(--ink);padding:clamp(1.8rem,3vw,2.6rem);position:relative;transition:background .5s}
.card:hover{background:var(--ink-2)}
.card .no{font-family:var(--ui);font-size:.72rem;letter-spacing:.3em;color:var(--amber);opacity:.8}
.card h3{font-family:var(--disp);font-weight:600;font-size:1.35rem;margin:1rem 0 .9rem;color:var(--hanji)}
.card p{color:var(--hanji-dim);font-size:.96rem;line-height:1.85}

/* ---------- places ---------- */
.place{display:grid;grid-template-columns:auto 1fr;gap:clamp(2rem,5vw,4rem);
  align-items:center;padding:clamp(2.4rem,5vw,3.6rem) 0;border-top:1px solid var(--line-soft)}
.place:last-child{border-bottom:1px solid var(--line-soft)}
.place-name{font-family:var(--disp);font-weight:700;color:var(--hanji)}
.place-name .kr{font-size:clamp(2rem,5vw,3rem);display:block;line-height:1.1}
.place-name .ko{font-size:.8rem;font-family:var(--ui);letter-spacing:.3em;color:var(--amber-deep);
  display:block;margin-top:.7rem}
.place-desc{color:var(--hanji-dim);font-size:1.02rem;max-width:54ch}
.place-desc b{color:var(--jade);font-weight:500}

/* ---------- dragon lore ---------- */
.lore{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
  gap:clamp(1.6rem,3vw,2.4rem)}
.lore-item{position:relative;padding-left:1.6rem}
.lore-item::before{content:"龍";position:absolute;left:0;top:.1em;
  font-family:var(--disp);font-size:.9rem;color:var(--amber);opacity:.55}
.lore-item h4{font-family:var(--disp);font-weight:600;font-size:1.12rem;color:var(--hanji);margin-bottom:.6rem}
.lore-item p{color:var(--hanji-dim);font-size:.95rem;line-height:1.8}
.lore-item p b{color:var(--amber);font-weight:500}

/* ---------- character intro ---------- */
.char-top{display:grid;grid-template-columns:1.1fr .9fr;gap:clamp(2rem,5vw,4.5rem);align-items:end;
  margin-bottom:clamp(4rem,8vw,6rem)}
.char-name{font-family:var(--disp);font-weight:800;line-height:.95}
.char-name .hanja{font-size:clamp(1.4rem,3vw,2rem);color:var(--amber-deep);font-weight:400;letter-spacing:.1em}
.char-name .ko{font-size:clamp(4.5rem,11vw,7.5rem);color:var(--hanji);display:block;margin-top:.3rem;
  text-shadow:0 0 50px rgba(227,166,78,.25)}
.char-tag{font-family:var(--ui);font-size:.78rem;letter-spacing:.34em;color:var(--amber);margin-top:1.4rem}
.char-blurb{color:var(--hanji-dim);font-size:1.04rem;line-height:2;max-width:40ch}
.char-blurb em{font-style:normal;color:var(--hanji);font-weight:500}

/* ---------- growth showcase (signature) ---------- */
.growth{margin-top:1rem}
.growth-head{display:flex;align-items:baseline;justify-content:space-between;flex-wrap:wrap;gap:1rem;
  margin-bottom:2.6rem;padding-bottom:1.4rem;border-bottom:1px solid var(--line)}
.growth-head .t{font-family:var(--disp);font-weight:600;font-size:clamp(1.5rem,3.5vw,2.1rem);color:var(--hanji)}
.growth-head .t .han{color:var(--amber-deep);font-weight:400;font-size:.7em;margin-left:.3em}
.growth-head .note{font-size:.92rem;color:var(--hanji-dim);max-width:34ch}
.growth-head .note b{color:var(--amber);font-weight:500}
.stages{display:grid;grid-template-columns:repeat(3,1fr);gap:clamp(1.2rem,2.5vw,2rem)}
.stage{position:relative}
.stage-fig{position:relative;border:1px solid var(--line);overflow:hidden;background:var(--ink-2);
  aspect-ratio:624/832}
.stage-fig img{width:100%;height:100%;object-fit:cover;filter:saturate(1.02) contrast(1.02);
  transition:transform 1.1s cubic-bezier(.16,.84,.44,1)}
.stage:hover .stage-fig img{transform:scale(1.05)}
.stage-fig::after{content:"";position:absolute;inset:0;pointer-events:none;
  background:linear-gradient(to top,rgba(12,10,8,.92) 0%,rgba(12,10,8,.15) 38%,transparent 60%);}
.stage-glow{position:absolute;inset:0;pointer-events:none;mix-blend-mode:screen;
  background:radial-gradient(60% 45% at 50% 78%,rgba(227,166,78,.28),transparent 70%);opacity:0;transition:opacity .7s}
.stage:hover .stage-glow{opacity:1}
.stage-meta{position:absolute;left:0;right:0;bottom:0;padding:1.2rem 1.3rem;z-index:2}
.stage-era{font-family:var(--ui);font-size:.68rem;letter-spacing:.32em;color:var(--amber)}
.stage-h{font-family:var(--disp);font-weight:700;font-size:clamp(1.4rem,2.6vw,1.9rem);color:var(--hanji);
  margin-top:.35rem;line-height:1}
.stage-h small{font-size:.5em;color:var(--hanji-dim);font-weight:300;margin-left:.35em;letter-spacing:.04em}
.stage-desc{margin-top:1rem;color:var(--hanji-dim);font-size:.92rem;line-height:1.8;padding:0 .1rem}
.stage-desc b{color:var(--hanji);font-weight:500}
/* height bar */
.bars{display:grid;grid-template-columns:repeat(3,1fr);gap:clamp(1.2rem,2.5vw,2rem);margin-top:1.4rem;
  align-items:end}
.bar{display:flex;flex-direction:column;justify-content:flex-end;align-items:center;gap:.55rem}
.bar i{display:block;width:100%;max-width:120px;background:linear-gradient(var(--amber),var(--amber-deep));
  opacity:.82;transform-origin:bottom;transform:scaleY(0);transition:transform 1.1s cubic-bezier(.2,.7,.3,1)}
.bars.in .bar i{transform:scaleY(1)}
.bar span{font-family:var(--ui);font-size:.66rem;letter-spacing:.18em;color:var(--hanji-dim)}

/* ---------- nature / traits ---------- */
.traits{display:grid;grid-template-columns:repeat(auto-fit,minmax(280px,1fr));gap:1px;
  background:var(--line-soft);border:1px solid var(--line);margin-top:clamp(3rem,6vw,4.5rem)}
.trait{background:var(--ink-2);padding:clamp(1.8rem,3vw,2.4rem)}
.trait .lab{font-family:var(--ui);font-size:.72rem;letter-spacing:.3em;color:var(--amber);margin-bottom:1.1rem}
.trait ul{list-style:none}
.trait li{color:var(--hanji-dim);font-size:.96rem;line-height:1.8;padding-left:1.1rem;position:relative;margin-bottom:.7rem}
.trait li:last-child{margin-bottom:0}
.trait li::before{content:"";position:absolute;left:0;top:.7em;width:5px;height:5px;
  background:var(--amber);border-radius:50%;opacity:.7}
.trait li b{color:var(--hanji);font-weight:500}

.pref{display:grid;grid-template-columns:1fr 1fr;gap:1px;background:var(--line);
  border:1px solid var(--line);margin-top:1px}
.pref div{padding:clamp(1.4rem,2.5vw,2rem) clamp(1.8rem,3vw,2.4rem)}
.pref .like{background:rgba(227,166,78,.07)}
.pref .dislike{background:rgba(179,64,45,.07)}
.pref .lab{font-family:var(--ui);font-size:.74rem;letter-spacing:.3em;margin-bottom:.8rem}
.pref .like .lab{color:var(--amber)}
.pref .dislike .lab{color:var(--cinnabar)}
.pref p{font-size:1rem;color:var(--hanji)}

/* ---------- past / origin timeline ---------- */
.past-wrap{max-width:760px;margin:0 auto}
.past{position:relative;margin-top:clamp(2.6rem,5vw,3.6rem);padding-left:2.4rem}
.past::before{content:"";position:absolute;left:7px;top:.4rem;bottom:.4rem;width:1px;
  background:linear-gradient(var(--line),var(--line-soft) 85%,transparent)}
.moment{position:relative;padding-bottom:clamp(2rem,4vw,2.8rem)}
.moment:last-child{padding-bottom:0}
.moment::before{content:"";position:absolute;left:-2.4rem;top:.55rem;width:15px;height:15px;
  border-radius:50%;background:var(--ink);border:1px solid var(--amber-deep)}
.moment::after{content:"";position:absolute;left:calc(-2.4rem + 4px);top:calc(.55rem + 4px);
  width:7px;height:7px;border-radius:50%;background:var(--amber);opacity:.85}
.moment .ord{font-family:var(--ui);font-size:.7rem;letter-spacing:.34em;color:var(--amber);
  display:block;margin-bottom:.6rem}
.moment p{color:var(--hanji-dim);font-size:1.04rem;line-height:1.95;max-width:52ch}
.moment p b{color:var(--hanji);font-weight:500}
.moment p .nm{color:var(--amber);font-weight:500}
.past-note{margin-top:clamp(2.6rem,5vw,3.4rem);padding-top:1.6rem;border-top:1px solid var(--line-soft);
  font-family:var(--disp);font-weight:300;font-size:clamp(1.1rem,2.6vw,1.45rem);line-height:1.8;
  color:var(--hanji);text-align:center}
.past-note em{font-style:normal;color:var(--amber);font-weight:500}

/* ---------- footer ---------- */
.foot{padding:clamp(5rem,10vw,8rem) 0 4rem;text-align:center;border-top:1px solid var(--line-soft);
  background:radial-gradient(100% 120% at 50% 100%,rgba(227,166,78,.06),transparent 60%),var(--ink)}
.foot .mark{font-family:var(--disp);font-weight:800;font-size:clamp(2.6rem,8vw,5rem);color:var(--hanji);
  letter-spacing:.06em;text-shadow:0 0 50px rgba(227,166,78,.2)}
.foot .sub{font-family:var(--ui);font-size:.74rem;letter-spacing:.4em;color:var(--hanji-faint);margin-top:1.6rem}

/* ---------- reveal ---------- */
.reveal{opacity:0;transform:translateY(34px);transition:opacity 1s cubic-bezier(.16,.84,.44,1),transform 1s cubic-bezier(.16,.84,.44,1)}
.reveal.in{opacity:1;transform:none}
.reveal[data-d="1"]{transition-delay:.08s}
.reveal[data-d="2"]{transition-delay:.16s}
.reveal[data-d="3"]{transition-delay:.24s}

/* ---------- responsive ---------- */
@media(max-width:860px){
  .intro-grid{grid-template-columns:1fr;gap:2.4rem}
  .char-top{grid-template-columns:1fr;gap:2rem;align-items:start}
  .place{grid-template-columns:1fr;gap:1.2rem}
  .pref{grid-template-columns:1fr}
}
@media(max-width:600px){
  .stages{grid-template-columns:1fr;gap:2.4rem}
  .bars{display:none}
  .stage-desc{padding:0}
}
@media(prefers-reduced-motion:reduce){
  *{animation:none!important;transition:none!important}
  .reveal{opacity:1;transform:none}
  .bars .bar i{transform:scaleY(1)}
  .hero-set,.hero h1 .c,.hero-sub,.scrollcue{opacity:1;transform:none}
}
</style>
</head>
<body>

<!-- ===================== HERO ===================== -->
<header class="hero">
  <div class="hero-sky">
    <svg viewBox="0 0 1440 900" preserveAspectRatio="xMidYMid slice" xmlns="http://www.w3.org/2000/svg">
      <defs>
        <radialGradient id="moon" cx="50%" cy="50%" r="50%">
          <stop offset="0%" stop-color="#f3e4c4" stop-opacity=".9"/>
          <stop offset="40%" stop-color="#e3a64e" stop-opacity=".25"/>
          <stop offset="100%" stop-color="#e3a64e" stop-opacity="0"/>
        </radialGradient>
        <linearGradient id="sky" x1="0" y1="0" x2="0" y2="1">
          <stop offset="0%" stop-color="#13192a"/>
          <stop offset="46%" stop-color="#0e1019"/>
          <stop offset="100%" stop-color="#0c0a08"/>
        </linearGradient>
        <radialGradient id="egg" cx="50%" cy="50%" r="50%">
          <stop offset="0%" stop-color="#ffe7b0" stop-opacity="1"/>
          <stop offset="35%" stop-color="#e3a64e" stop-opacity=".85"/>
          <stop offset="100%" stop-color="#c47a2b" stop-opacity="0"/>
        </radialGradient>
      </defs>
      <rect width="1440" height="900" fill="url(#sky)"/>
      <!-- moon glow -->
      <circle cx="1080" cy="230" r="340" fill="url(#moon)"/>
      <circle cx="1080" cy="230" r="92" fill="#efe1c2" opacity=".92"/>
      <!-- far ridge -->
      <path d="M0 560 Q 240 470 460 520 T 900 500 T 1440 540 L1440 900 L0 900Z" fill="#171c2b" opacity=".85"/>
      <!-- mid ridge -->
      <path d="M0 640 Q 300 540 560 600 Q 820 660 1080 580 Q 1280 520 1440 600 L1440 900 L0 900Z" fill="#101320"/>
      <!-- near ridge (도락산) -->
      <path d="M0 760 Q 220 660 420 720 Q 640 786 860 700 Q 1120 596 1440 720 L1440 900 L0 900Z" fill="#0a0907"/>
      <!-- valley glow: the egg -->
      <ellipse cx="430" cy="724" rx="190" ry="120" fill="url(#egg)" opacity=".9"/>
      <ellipse cx="430" cy="726" rx="17" ry="22" fill="#fff1cf"/>
      <ellipse cx="430" cy="726" rx="30" ry="38" fill="none" stroke="#ffe7b0" stroke-opacity=".4" stroke-width="1"/>
      <!-- mist -->
      <path d="M0 700 Q 400 678 760 700 T 1440 700" fill="none" stroke="#ece2cf" stroke-opacity=".05" stroke-width="60"/>
    </svg>
  </div>
  <div class="hero-grain"></div>
  <div class="hero-inner">
    <p class="hero-set">조선 명종 <span>三</span>년 · 一五四八 · 양주</p>
    <h1><span class="c">용</span><span class="c">을</span><span class="c">줍다</span></h1>
    <p class="hero-sub">버려진 산골, 검은 연못 곁에서<br>당신은 알 하나를 주워 든다.</p>
  </div>
  <div class="scrollcue">아래로<i></i></div>
</header>

<!-- ===================== INTRO ===================== -->
<section class="section section--ink">
  <div class="wrap intro-grid">
    <div class="reveal">
      <p class="eyebrow">들어가며</p>
      <p class="lead">하늘과 땅, 사람의 세상을 <em>용</em>이 다스리던 시절.<br>그 한 마리가 당신의 품으로 굴러떨어졌다.</p>
    </div>
    <div class="intro-body reveal" data-d="1">
      <p>왕은 용의 심기를 거스르지 않으려 끊임없이 제사를 올리고, 사람들은 <strong>약초와 쌀, 작물</strong>로 거래하며 살아간다. 을사년의 피바람이 한양을 휩쓸고 간 뒤, 살아남은 자들은 도성 밖으로 흩어졌다.</p>
      <p>그 북쪽 고을 양주, 완만한 <strong>도락산</strong> 어딘가의 초가에서 이야기는 시작된다. 약초꾼과 심마니, 도망자가 스쳐 가는 그 산에서 당신은 작은 알 하나를 거두었다. 검은 연못의 산에서 주워 들었기에, 이름은 <strong>현담(玄潭)</strong>.</p>
    </div>
  </div>
</section>

<!-- ===================== WORLD: 조선 ===================== -->
<section class="section section--panel rule-top">
  <div class="wrap">
    <div class="head reveal">
      <p class="eyebrow">세계관</p>
      <h2>용이 다스리는 나라<span class="han">朝鮮</span></h2>
      <p>용을 향한 믿음과 제사가 세상을 지탱한다. 그 질서 아래, 사람의 세상은 촘촘한 신분의 결로 나뉘어 있다.</p>
    </div>
    <div class="cards reveal" data-d="1">
      <div class="card">
        <span class="no">壹</span>
        <h3>용의 섭리</h3>
        <p>하늘과 땅, 인간 세상을 용이 다스린다. 왕은 용의 심기를 거스르지 않기 위해 제사에 온 힘을 쏟는다.</p>
      </div>
      <div class="card">
        <span class="no">貳</span>
        <h3>엄격한 신분</h3>
        <p>왕 · 양반 · 중인 · 상민 · 노비. 무너지지 않는 다섯 겹의 질서가 사람의 자리를 정한다.</p>
      </div>
      <div class="card">
        <span class="no">參</span>
        <h3>화폐 없는 거래</h3>
        <p>따로 정해진 돈이 없어 약초와 쌀, 작물이 곧 값이 된다. 가진 것이 신분을 가른다.</p>
      </div>
      <div class="card">
        <span class="no">肆</span>
        <h3>을사사화 이후</h3>
        <p>1545년의 사화로 수많은 사대부 양반이 숙청되고, 살아남은 자들은 한양 밖으로 도망쳤다.</p>
      </div>
    </div>
  </div>
</section>

<!-- ===================== PLACES ===================== -->
<section class="section section--ink">
  <div class="wrap">
    <div class="head reveal">
      <p class="eyebrow">무대</p>
      <h2>산과 강을 낀 고을</h2>
      <p>한양의 그늘과 달리, 이곳의 빛과 어둠은 유난히 또렷하다.</p>
    </div>
    <div class="place reveal" data-d="1">
      <div class="place-name">
        <span class="kr">양주목</span>
        <span class="ko">楊州牧</span>
      </div>
      <p class="place-desc">한양 위에 자리한 큰 고을. 도성의 정세와 달리 부유하고 활기차다. 시장이 활발히 서며 분위기는 밝지만, 그 이면엔 <b>극심한 빈부격차</b>가 도사린다. 양반과 탐관오리의 결탁으로 고통받는 건 언제나 가난한 상민들의 몫이다.</p>
    </div>
    <div class="place reveal" data-d="2">
      <div class="place-name">
        <span class="kr">도락산</span>
        <span class="ko">道樂山</span>
      </div>
      <p class="place-desc">양주의 완만한 산. 약초꾼 · 심마니 · 사냥꾼 · 도망자가 오가는 길목이다. 약초와 과일, 꽃이 가득 핀 들판과 <b>산을 감싸 흐르는 계곡</b>이 평화롭지만, 도망자와 반역자를 쫓는 관아의 순찰이 종종 그 평화를 가른다. 당신과 현담의 초가가 있는 곳.</p>
    </div>
  </div>
</section>

<!-- ===================== DRAGON LORE ===================== -->
<section class="section section--night rule-top">
  <div class="wrap">
    <div class="head reveal">
      <p class="eyebrow">용 · 龍</p>
      <h2>그들이 살아가는 법</h2>
      <p>용은 대개 인간의 모습으로 지낸다. 뿔과 꼬리, 그리고 목 뒤의 역린만이 그 정체를 드러낼 뿐.</p>
    </div>
    <div class="lore reveal" data-d="1">
      <div class="lore-item">
        <h4>인간의 모습으로</h4>
        <p>용의 형상보다 인간형으로 지내며, 뿔과 꼬리·역린만 드러난다. <b>성년이 된 용은 뿔과 꼬리마저 숨길 수 있다.</b></p>
      </div>
      <div class="lore-item">
        <h4>단 하나의 반려</h4>
        <p>성별과 상관없이 평생 <b>단 한 마리만을 반려로</b> 맞이한다. 자신의 반려를 향해선 깊은 애착이 자라난다.</p>
      </div>
      <div class="lore-item">
        <h4>급격한 성장</h4>
        <p>인간보다 빠르게 자라, <b>세 살이면 스무 살 성인의 모습</b>. 성인이 된 뒤로는 외형이 늙지 않고 나이만 든다.</p>
      </div>
      <div class="lore-item">
        <h4>믿음이 곧 생명</h4>
        <p>용을 믿고 제사를 올리는 <b>인간의 믿음으로 생명을 유지</b>한다. 사람의 마음이 곧 용의 숨이다.</p>
      </div>
      <div class="lore-item">
        <h4>여덟의 원룡</h4>
        <p>각자의 구역을 관장하는 <b>원룡은 모두 여덟</b>. 그 외의 용은 원룡을 보필하며 쓸모를 다하고, 더러 그 자리를 노리는 악룡도 있다.</p>
      </div>
      <div class="lore-item">
        <h4>유희로서의 미식</h4>
        <p>먹지 않아도 살 수 있는 몸. 그러니 식사란 오직 <b>즐거움을 위해서만</b> 행하는 사치다.</p>
      </div>
    </div>
  </div>
</section>

<!-- ===================== CHARACTER ===================== -->
<section class="section section--panel rule-top">
  <div class="wrap">
    <div class="char-top">
      <div class="reveal">
        <p class="eyebrow">캐릭터</p>
        <h2 class="char-name">
          <span class="english">LeeSerin</span>
          <span class="ko">이세린</span>
        </h2>
        <p class="char-tag">여성 · 귀신 · 당신의 섹스 파트너(?)</p>
      </div>
      <p class="char-blurb reveal" data-d="1">매일 밤 자위로 악귀를 퇴마하는 당신. 그리고 당신의 정기에 이끌려 만원 지하철까지 따라온 알몸의 색귀, 이세린. 그녀는 공공장소에서 멋대로 당신의 바지춤을 풀고 좆을 꺼내드는데...</p>
    </div>
    

    <!-- TRAITS -->
    <div class="traits reveal" data-d="1">
      <div class="trait">
        <p class="lab">외모</p>
        <ul>
          <li><b>금발금안</b>부스스한 긴 금발 생머리. 동글동글 하지만 눈꼬리가 약간 올라간 금안.</li>
          <li>예쁘다기 보단 귀엽고 섹시한 얼굴의 여우상</li>
          <li>156cm, 43kg, E컵</li>
        </ul>
      </div>
      <div class="trait">
        <p class="lab">성격</p>
        <ul>
          <li>마치 살아있는 사람처럼 <b>밝고 해맑은 편</b>, 바보같지만 귀엽다</li>
          <li>장난꾸러기 — 다른 귀신들과 달리 당신에게 상처 하나 입히지 않는 <b<유치한 장난질</b>을 한다</li>
          <li>외로움을 매우 잘 탄다</li>
          <li></li>
        </ul>
      </div>
      <div class="trait">
        <p class="lab">특징</p>
        <ul>
          <li><b>섹스</b>에 미쳐있음</li>
          <li>수위높은 음담패설, <b>더티 토크</b></li>
          <li>늘 어딘가 화가 난 것처럼 무서운 표정을 짓는 당신의 기분을 전환시켜 주려고 애쓴다</li>
          <li>경험 많은 척 행동하는 <b>동정</b></li>
          <li>목 뒤의 역린 — 닿으면 몸이 움찔 떨린다. 인간이 만지면 곧 죽일 일이나, <b>당신에게만은 허락</b>한다</li>
        </ul>
      </div>
    </div>
    <div class="pref reveal" data-d="2">
      <div class="like">
        <p class="lab">선호</p>
        <p>당신 · 단것(호박죽, 벌꿀) · 둥글고 번들거리는 것</p>
      </div>
      <div class="dislike">
        <p class="lab">불호</p>
        <p>당신 외의 인간 · 다른 짐승</p>
      </div>
    </div>
  </div>
</section>

<!-- ===================== PAST / ORIGIN ===================== -->
<section class="section section--night rule-top">
  <div class="wrap past-wrap">
    <div class="head reveal" style="margin-bottom:0">
      <p class="eyebrow">과거 · 過去</p>
      <h2>알이 산에 닿기까지</h2>
      <p>현담이 당신의 품에 이르기 전, 검은 연못의 산에는 한 마리 용의 마지막 선택이 묻혀 있었다.</p>
    </div>
    <div class="past reveal" data-d="1">
      <div class="moment">
        <span class="ord">壹</span>
        <p>원룡이던 <b>어미 용</b>은 제 자리를 노리는 악룡을 피해, 인간계의 산속에 알 하나를 낳아 숨겼다.</p>
      </div>
      <div class="moment">
        <span class="ord">貳</span>
        <p>상황이 가라앉으면 다시 데리러 올 생각이었으나, 어미 용은 끝내 <b>악룡의 손에 목숨을 잃었다.</b></p>
      </div>
      <div class="moment">
        <span class="ord">參</span>
        <p>데리러 올 이를 잃은 알은 오래도록 산속에 방치된 채 남겨졌다. 그러다 마침내, <b>당신의 손에 거두어졌다.</b></p>
      </div>
      <div class="moment">
        <span class="ord">肆</span>
        <p>검은 연못이 있는 산에서 주워 들었기에, 당신은 그 이름을 <span class="nm">현담(玄潭)</span>이라 지어 주었다.</p>
      </div>
    </div>
    <p class="past-note reveal" data-d="2">버려진 알이 아니라,<br><em>당신이 주운 한 마리의 용.</em></p>
  </div>
</section>

<!-- ===================== FOOTER ===================== -->
<footer class="foot">
  <p class="mark">용을 줍다</p>
  <p class="sub">검은 연못의 산 · 현담 · 玄 潭</p>
</footer>

<script>
(function(){
  var io = new IntersectionObserver(function(es){
    es.forEach(function(e){
      if(e.isIntersecting){
        e.target.classList.add('in');
        if(e.target.id==='bars') return; // keep bars handled below
        io.unobserve(e.target);
      }
    });
  },{threshold:.16,rootMargin:'0px 0px -8% 0px'});
  document.querySelectorAll('.reveal').forEach(function(el){io.observe(el)});

  var bars = document.getElementById('bars');
  if(bars){
    var bo = new IntersectionObserver(function(es){
      es.forEach(function(e){ if(e.isIntersecting){ bars.classList.add('in'); bo.disconnect(); }});
    },{threshold:.2,rootMargin:'0px 0px -10% 0px'});
    bo.observe(bars);
  }
})();
</script>
</body>
</html>
