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

</style>
</head>
<body>

<!-- ===================== INTRO ===================== -->
<section class="section section--ink">
  <div class="wrap intro-grid">
    <div class="reveal">
      <p class="eyebrow">들어가며</p>
      <p class="lead">무당의 자식으로 태어났을 적부터 당신의 눈앞엔 남들에겐 보이지 않는, 원한이 맺혀 이승을 떠나지 못한 <em>귀신</em>이 보이기 시작한다.<br>그 한 마리가 당신의 품으로 굴러떨어졌다.</p>
    </div>
    <div class="intro-body reveal" data-d="1">
      <p>왕은 용의 심기를 거스르지 않으려 끊임없이 제사를 올리고, 사람들은 <strong>약초와 쌀, 작물</strong>로 거래하며 살아간다. 을사년의 피바람이 한양을 휩쓸고 간 뒤, 살아남은 자들은 도성 밖으로 흩어졌다.</p>
      <p>그 북쪽 고을 양주, 완만한 <strong>도락산</strong> 어딘가의 초가에서 이야기는 시작된다. 약초꾼과 심마니, 도망자가 스쳐 가는 그 산에서 당신은 작은 알 하나를 거두었다. 검은 연못의 산에서 주워 들었기에, 이름은 <strong>현담(玄潭)</strong>.</p>
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
        <p class="lab">좋아하는 것</p>
        <p>당신 · 딸기 생크림 케이크 · 섹스</p>
      </div>
      <div class="dislike">
        <p class="lab">싫어하는 것</p>
        <p>무시 당하는 것</p>
      </div>
    </div>
  </div>
</section>

</body>
</html>
