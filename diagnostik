<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>English Diagnostic Test — Grade 11</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Special+Elite&family=Libre+Franklin:wght@400;500;600;700;800&display=swap" rel="stylesheet">
<style>
  :root{
    --paper:#EFE6CC;
    --paper-deep:#E4D9B8;
    --rule:#C9BB93;
    --ink:#20303A;
    --chalk:#2F4A3E;
    --chalk-dark:#233A30;
    --pencil:#D9A441;
    --pen-red:#B23A2E;
    --correct:#3F7A5A;
    --paper-shadow: rgba(32,48,58,0.18);
  }
  *{box-sizing:border-box;}
  html,body{margin:0;padding:0;}
  body{
    background:
      repeating-linear-gradient(0deg, transparent, transparent 27px, var(--rule) 28px),
      var(--paper);
    color:var(--ink);
    font-family:'Libre Franklin', sans-serif;
    min-height:100vh;
    display:flex;
    align-items:flex-start;
    justify-content:center;
    padding:32px 16px;
  }
  .sheet{
    width:100%;
    max-width:720px;
    background:var(--paper-deep);
    border:1px solid var(--rule);
    border-radius:4px;
    box-shadow:0 18px 40px var(--paper-shadow), 0 2px 0 var(--rule);
    position:relative;
    overflow:hidden;
  }
  .sheet::before{
    content:"";
    position:absolute;
    left:38px; top:0; bottom:0;
    width:2px;
    background:var(--pen-red);
    opacity:0.35;
  }
  .content{ padding:28px 30px 30px 58px; }
  header.top{
    display:flex;
    align-items:baseline;
    justify-content:space-between;
    border-bottom:2px solid var(--ink);
    padding-bottom:10px;
    margin-bottom:20px;
  }
  .brand{
    font-family:'Special Elite', monospace;
    font-size:13px;
    letter-spacing:2px;
    text-transform:uppercase;
    color:var(--chalk-dark);
  }
  .brand small{display:block; font-size:10px; letter-spacing:1px; opacity:0.7; margin-top:2px;}
  .page-tag{
    font-family:'Special Elite', monospace;
    font-size:12px;
    color:var(--ink);
    opacity:0.65;
  }
  h1.title{
    font-family:'Special Elite', monospace;
    font-size:26px;
    line-height:1.35;
    margin:0 0 6px 0;
    color:var(--chalk-dark);
  }
  p.sub{
    margin:0 0 22px 0;
    font-size:14.5px;
    color:var(--ink);
    opacity:0.85;
  }
  .field{ margin-bottom:16px; }
  .field label{
    display:block;
    font-size:12px;
    text-transform:uppercase;
    letter-spacing:1.5px;
    font-weight:700;
    margin-bottom:6px;
    color:var(--chalk-dark);
  }
  .field input{
    width:100%;
    font-family:'Libre Franklin', sans-serif;
    font-size:16px;
    padding:10px 12px;
    border:none;
    border-bottom:2px dashed var(--ink);
    background:transparent;
    color:var(--ink);
    outline:none;
  }
  .field input:focus{ border-bottom-color:var(--pen-red); }
  .btn{
    font-family:'Special Elite', monospace;
    font-size:14px;
    letter-spacing:1px;
    text-transform:uppercase;
    background:var(--chalk);
    color:var(--paper);
    border:none;
    padding:13px 22px;
    border-radius:3px;
    cursor:pointer;
    transition:transform .12s ease, background .15s ease;
    box-shadow:0 3px 0 var(--chalk-dark);
  }
  .btn:hover{ background:var(--chalk-dark); }
  .btn:active{ transform:translateY(2px); box-shadow:0 1px 0 var(--chalk-dark); }
  .btn.secondary{
    background:transparent;
    color:var(--chalk-dark);
    box-shadow:none;
    border:2px solid var(--chalk-dark);
    padding:11px 20px;
  }
  .btn.secondary:hover{ background:rgba(47,74,62,0.08); }
  .btn:disabled{ opacity:.4; cursor:not-allowed; box-shadow:none; }
  .row{ display:flex; gap:12px; justify-content:flex-end; margin-top:6px; flex-wrap:wrap; }
  .row.between{ justify-content:space-between; align-items:center; }

  /* progress */
  .progress-wrap{ margin-bottom:22px; }
  .progress-label{
    font-family:'Special Elite', monospace;
    font-size:11.5px;
    color:var(--chalk-dark);
    margin-bottom:6px;
    display:flex; justify-content:space-between;
  }
  .progress-track{
    height:8px;
    background:rgba(32,48,58,0.12);
    border-radius:4px;
    overflow:hidden;
  }
  .progress-fill{
    height:100%;
    background:var(--pencil);
    border-radius:4px;
    transition:width .3s ease;
  }

  /* question card */
  .qnum{
    font-family:'Special Elite', monospace;
    font-size:15px;
    color:var(--pen-red);
    margin-bottom:8px;
  }
  .qtext{
    font-size:18px;
    line-height:1.5;
    font-weight:600;
    margin-bottom:6px;
  }
  .passage{
    background:rgba(255,255,255,0.35);
    border-left:3px solid var(--chalk);
    padding:12px 14px;
    font-size:14.5px;
    line-height:1.6;
    margin-bottom:14px;
    border-radius:2px;
  }
  .options{ margin-top:18px; display:flex; flex-direction:column; gap:12px; }
  .option{
    display:flex;
    align-items:center;
    gap:14px;
    cursor:pointer;
    padding:8px 6px;
    border-radius:4px;
    transition:background .12s ease;
  }
  .option:hover{ background:rgba(47,74,62,0.06); }
  .bubble{
    flex:0 0 auto;
    width:26px; height:26px;
    border-radius:50%;
    border:2px solid var(--ink);
    position:relative;
    display:flex; align-items:center; justify-content:center;
    font-family:'Special Elite', monospace;
    font-size:12px;
  }
  .option.selected .bubble{
    background:var(--chalk-dark);
    border-color:var(--chalk-dark);
    color:var(--paper);
  }
  .option .otext{ font-size:15.5px; }

  .quiz-footer{ margin-top:26px; }

  /* results */
  .stamp{
    display:inline-block;
    font-family:'Special Elite', monospace;
    border:3px solid var(--pen-red);
    color:var(--pen-red);
    padding:10px 18px;
    border-radius:6px;
    transform:rotate(-4deg);
    text-transform:uppercase;
    letter-spacing:2px;
    font-size:18px;
    margin-bottom:18px;
  }
  .score-big{
    font-family:'Special Elite', monospace;
    font-size:54px;
    color:var(--chalk-dark);
    line-height:1;
    margin:6px 0 2px 0;
  }
  .score-sub{ font-size:14px; opacity:0.75; margin-bottom:20px;}
  table.breakdown{ width:100%; border-collapse:collapse; margin:18px 0 24px 0; font-size:14px;}
  table.breakdown th, table.breakdown td{
    text-align:left; padding:8px 6px; border-bottom:1px solid var(--rule);
  }
  table.breakdown th{ font-family:'Special Elite', monospace; font-size:12px; text-transform:uppercase; letter-spacing:1px;}
  .tag-ok{ color:var(--correct); font-weight:700; }
  .tag-no{ color:var(--pen-red); font-weight:700; }
  .hidden{ display:none !important; }
  footer.note{ margin-top:18px; font-size:12px; opacity:0.6; }
  @media(max-width:480px){
    .content{ padding:22px 16px 24px 34px; }
    .sheet::before{ left:20px; }
    h1.title{ font-size:21px; }
    .score-big{ font-size:42px; }
  }
</style>
</head>
<body>

<div class="sheet">
  <div class="content">

    <header class="top">
      <div class="brand">English Diagnostic Test<small>Grade 11 · SMK / SMA</small></div>
      <div class="page-tag" id="pageTag">Form A</div>
    </header>

    <!-- SCREEN 1: START -->
    <section id="screen-start">
      <h1 class="title">Before you begin…</h1>
      <p class="sub">This test has 30 questions covering grammar, vocabulary, and reading. Answer every item as best you can — there is no time limit, but try not to look anything up. Let's see where you stand.</p>

      <div class="field">
        <label for="inputName">Full Name</label>
        <input type="text" id="inputName" placeholder="e.g. Andi Pratama" autocomplete="off">
      </div>
      <div class="field">
        <label for="inputClass">Class</label>
        <input type="text" id="inputClass" placeholder="e.g. XI TKJ 2" autocomplete="off">
      </div>

      <div class="row">
        <button class="btn" id="btnStart">Start Test</button>
      </div>
    </section>

    <!-- SCREEN 2: QUIZ -->
    <section id="screen-quiz" class="hidden">
      <div class="progress-wrap">
        <div class="progress-label">
          <span id="progressText">Question 1 of 30</span>
          <span id="progressPercent">0%</span>
        </div>
        <div class="progress-track"><div class="progress-fill" id="progressFill" style="width:0%"></div></div>
      </div>

      <div class="qnum" id="qNum">No. 01</div>
      <div class="passage hidden" id="passageBox"></div>
      <div class="qtext" id="qText"></div>

      <div class="options" id="optionsBox"></div>

      <div class="row between quiz-footer">
        <button class="btn secondary" id="btnPrev">← Back</button>
        <button class="btn" id="btnNext" disabled>Next →</button>
      </div>
    </section>

    <!-- SCREEN 3: RESULT -->
    <section id="screen-result" class="hidden">
      <div class="stamp">Graded</div>
      <p class="sub" style="margin-bottom:2px;">Result for <strong id="resName"></strong> — Class <strong id="resClass"></strong></p>
      <div class="score-big"><span id="resScore">0</span>/30</div>
      <div class="score-sub" id="resPercent"></div>
      <h1 class="title" id="resLevel" style="font-size:20px;"></h1>
      <p class="sub" id="resLevelDesc"></p>

      <table class="breakdown" id="breakdownTable">
        <thead><tr><th>Skill Area</th><th>Score</th></tr></thead>
        <tbody id="breakdownBody"></tbody>
      </table>

      <div class="row between">
        <button class="btn secondary" id="btnReview">Review Answers</button>
        <button class="btn" id="btnDownload">⬇ Download Result</button>
      </div>
      <footer class="note">Taken on <span id="resDate"></span> · English Diagnostic Test, Grade 11</footer>
    </section>

    <!-- SCREEN 4: REVIEW -->
    <section id="screen-review" class="hidden">
      <h1 class="title" style="font-size:20px;">Answer Review</h1>
      <div id="reviewList"></div>
      <div class="row" style="justify-content:flex-start; margin-top:20px;">
        <button class="btn secondary" id="btnBackToResult">← Back to Result</button>
      </div>
    </section>

  </div>
</div>

<script>
const QUESTIONS = [
  {cat:"Tenses", q:"She ___ to school every day.", opts:["go","goes","going","gone"], a:1},
  {cat:"Tenses", q:"They ___ dinner when I arrived.", opts:["were having","have","had","has"], a:0},
  {cat:"Tenses", q:"I ___ my homework already.", opts:["finish","finished","have finished","had finished"], a:2},
  {cat:"Tenses", q:"By next year, she ___ from university.", opts:["will graduate","will have graduated","graduates","is graduating"], a:1},
  {cat:"Tenses", q:"Look! It ___ outside.", opts:["rains","rained","is raining","has rained"], a:2},
  {cat:"Tenses", q:"Yesterday, we ___ to the museum.", opts:["go","went","gone","goes"], a:1},

  {cat:"Vocabulary", q:"Choose the word closest in meaning to 'huge'.", opts:["tiny","enormous","quiet","simple"], a:1},
  {cat:"Vocabulary", q:"Choose the word opposite in meaning to 'increase'.", opts:["decrease","expand","grow","rise"], a:0},
  {cat:"Vocabulary", q:"The manager will ___ the new schedule tomorrow.", opts:["announce","announcement","announcing","announced"], a:0},
  {cat:"Vocabulary", q:"Please fill ___ this form before the interview.", opts:["in","on","at","for"], a:0},

  {cat:"Prepositions", q:"The meeting starts ___ 9 a.m.", opts:["in","on","at","for"], a:2},
  {cat:"Prepositions", q:"She has been working here ___ 2019.", opts:["since","for","from","at"], a:0},
  {cat:"Prepositions", q:"He is good ___ solving problems.", opts:["in","at","on","with"], a:1},
  {cat:"Prepositions", q:"We will discuss it ___ the meeting.", opts:["during","while","for","since"], a:0},

  {cat:"Modals", q:"You ___ wear a helmet when riding a motorbike.", opts:["can","might","must","could"], a:2},
  {cat:"Modals", q:"___ I open the window?", opts:["Must","Should","May","Will"], a:2},
  {cat:"Modals", q:"Students ___ submit their assignments by Friday.", opts:["should","would","might","could"], a:0},

  {cat:"Passive Voice", q:"The report ___ by the secretary yesterday.", opts:["wrote","was written","is written","writes"], a:1},
  {cat:"Passive Voice", q:"New employees ___ trained every month.", opts:["are","is","was","were"], a:0},
  {cat:"Passive Voice", q:"The machine ___ repaired next week.", opts:["will be","will","is being","was"], a:0},

  {cat:"Conditionals", q:"If it rains, we ___ the trip.", opts:["will cancel","cancel","would cancel","cancelled"], a:0},
  {cat:"Conditionals", q:"If I ___ more time, I would learn French.", opts:["have","had","has","having"], a:1},

  {cat:"Comparatives", q:"This laptop is ___ than that one.", opts:["cheap","cheaper","cheapest","more cheap"], a:1},
  {cat:"Comparatives", q:"He is ___ student in the class.", opts:["the most diligent","most diligent","diligent","more diligent"], a:0},

  {cat:"Reading", passage:"Rani is a student at a vocational high school. Last semester, she did an internship at a local hotel's front office. During the three-month program, she learned how to greet guests, handle phone calls, and manage bookings. At first, she felt nervous because she had to speak English with foreign guests. However, her supervisor was patient and gave her helpful feedback every week. By the end of the internship, Rani felt more confident and even received a certificate of excellent performance.",
   q:"Where did Rani do her internship?", opts:["At a school library","At a hotel's front office","At a travel agency","At a restaurant kitchen"], a:1},
  {cat:"Reading", passage:"Rani is a student at a vocational high school. Last semester, she did an internship at a local hotel's front office. During the three-month program, she learned how to greet guests, handle phone calls, and manage bookings. At first, she felt nervous because she had to speak English with foreign guests. However, her supervisor was patient and gave her helpful feedback every week. By the end of the internship, Rani felt more confident and even received a certificate of excellent performance.",
   q:"Why did Rani feel nervous at first?", opts:["She disliked her supervisor","She had to speak English with foreign guests","She arrived late every day","She did not like hotels"], a:1},
  {cat:"Reading", passage:"Rani is a student at a vocational high school. Last semester, she did an internship at a local hotel's front office. During the three-month program, she learned how to greet guests, handle phone calls, and manage bookings. At first, she felt nervous because she had to speak English with foreign guests. However, her supervisor was patient and gave her helpful feedback every week. By the end of the internship, Rani felt more confident and even received a certificate of excellent performance.",
   q:"What did Rani receive at the end of the internship?", opts:["A full-time job offer","A salary bonus","A certificate of excellent performance","A scholarship"], a:2},

  {cat:"Workplace English", q:"The customer complained about the ___ service.", opts:["efficient","poor","available","technical"], a:1},
  {cat:"Workplace English", q:"Please ___ me know if you need any help.", opts:["let","allow","make","give"], a:0},
  {cat:"Workplace English", q:"It's important to ___ good communication with colleagues.", opts:["maintain","maintenance","maintained","maintaining"], a:0},
];

let current = 0;
let answers = new Array(QUESTIONS.length).fill(null);
let studentName = "";
let studentClass = "";

const screenStart = document.getElementById('screen-start');
const screenQuiz = document.getElementById('screen-quiz');
const screenResult = document.getElementById('screen-result');
const screenReview = document.getElementById('screen-review');
const pageTag = document.getElementById('pageTag');

document.getElementById('btnStart').addEventListener('click', () => {
  const nameVal = document.getElementById('inputName').value.trim();
  const classVal = document.getElementById('inputClass').value.trim();
  if(!nameVal || !classVal){
    alert("Please fill in both your name and class before starting.");
    return;
  }
  studentName = nameVal;
  studentClass = classVal;
  screenStart.classList.add('hidden');
  screenQuiz.classList.remove('hidden');
  pageTag.textContent = "Form A · In Progress";
  renderQuestion();
});

function renderQuestion(){
  const item = QUESTIONS[current];
  document.getElementById('qNum').textContent = "No. " + String(current+1).padStart(2,'0');
  document.getElementById('qText').textContent = item.q;

  const passageBox = document.getElementById('passageBox');
  if(item.passage){
    passageBox.textContent = item.passage;
    passageBox.classList.remove('hidden');
  } else {
    passageBox.classList.add('hidden');
  }

  const optionsBox = document.getElementById('optionsBox');
  optionsBox.innerHTML = "";
  item.opts.forEach((opt, idx) => {
    const div = document.createElement('div');
    div.className = 'option' + (answers[current]===idx ? ' selected' : '');
    div.innerHTML = `<span class="bubble">${String.fromCharCode(65+idx)}</span><span class="otext">${opt}</span>`;
    div.addEventListener('click', () => {
      answers[current] = idx;
      renderQuestion();
    });
    optionsBox.appendChild(div);
  });

  document.getElementById('progressText').textContent = `Question ${current+1} of ${QUESTIONS.length}`;
  const pct = Math.round(((current+1)/QUESTIONS.length)*100);
  document.getElementById('progressPercent').textContent = pct + "%";
  document.getElementById('progressFill').style.width = pct + "%";

  document.getElementById('btnPrev').disabled = current===0;
  const nextBtn = document.getElementById('btnNext');
  nextBtn.disabled = answers[current]===null;
  nextBtn.textContent = current === QUESTIONS.length-1 ? "Finish Test" : "Next →";
}

document.getElementById('btnPrev').addEventListener('click', () => {
  if(current>0){ current--; renderQuestion(); }
});

document.getElementById('btnNext').addEventListener('click', () => {
  if(answers[current]===null) return;
  if(current < QUESTIONS.length-1){
    current++;
    renderQuestion();
  } else {
    showResult();
  }
});

function levelFor(pct){
  if(pct >= 91) return {label:"Advanced", desc:"Excellent! You have a strong command of English grammar and vocabulary at an upper-secondary level."};
  if(pct >= 76) return {label:"Upper-Intermediate", desc:"Very good. You understand most grammar structures well, with only minor gaps to polish."};
  if(pct >= 61) return {label:"Intermediate", desc:"Good progress. You have a solid foundation but should review a few grammar areas."};
  if(pct >= 41) return {label:"Elementary", desc:"You know the basics, but need more practice with tenses, prepositions, and vocabulary."};
  return {label:"Beginner", desc:"It's a good time to build up your core English grammar and vocabulary step by step."};
}

function showResult(){
  screenQuiz.classList.add('hidden');
  screenResult.classList.remove('hidden');
  pageTag.textContent = "Form A · Graded";

  let score = 0;
  const catStats = {};
  QUESTIONS.forEach((item, idx) => {
    if(!catStats[item.cat]) catStats[item.cat] = {correct:0, total:0};
    catStats[item.cat].total++;
    if(answers[idx] === item.a){ score++; catStats[item.cat].correct++; }
  });
  const pct = Math.round((score/QUESTIONS.length)*100);
  const lvl = levelFor(pct);

  document.getElementById('resName').textContent = studentName;
  document.getElementById('resClass').textContent = studentClass;
  document.getElementById('resScore').textContent = score;
  document.getElementById('resPercent').textContent = pct + "% correct";
  document.getElementById('resLevel').textContent = "Level: " + lvl.label;
  document.getElementById('resLevelDesc').textContent = lvl.desc;
  document.getElementById('resDate').textContent = new Date().toLocaleDateString('en-GB', {day:'numeric', month:'long', year:'numeric'});

  const tbody = document.getElementById('breakdownBody');
  tbody.innerHTML = "";
  Object.keys(catStats).forEach(cat => {
    const s = catStats[cat];
    const tr = document.createElement('tr');
    tr.innerHTML = `<td>${cat}</td><td>${s.correct}/${s.total}</td>`;
    tbody.appendChild(tr);
  });

  window._lastResult = {score, pct, lvl, catStats};
}

document.getElementById('btnReview').addEventListener('click', () => {
  screenResult.classList.add('hidden');
  screenReview.classList.remove('hidden');
  const list = document.getElementById('reviewList');
  list.innerHTML = "";
  QUESTIONS.forEach((item, idx) => {
    const isCorrect = answers[idx] === item.a;
    const div = document.createElement('div');
    div.style.borderBottom = "1px solid var(--rule)";
    div.style.padding = "12px 0";
    div.innerHTML = `
      <div class="qnum" style="margin-bottom:4px;">No. ${String(idx+1).padStart(2,'0')} — <span class="${isCorrect?'tag-ok':'tag-no'}">${isCorrect?'Correct':'Incorrect'}</span></div>
      <div style="font-weight:600; margin-bottom:4px;">${item.q}</div>
      <div style="font-size:13.5px;">Your answer: <strong>${answers[idx]!==null ? item.opts[answers[idx]] : '(no answer)'}</strong></div>
      ${!isCorrect ? `<div style="font-size:13.5px; color:var(--correct);">Correct answer: <strong>${item.opts[item.a]}</strong></div>` : ""}
    `;
    list.appendChild(div);
  });
});

document.getElementById('btnBackToResult').addEventListener('click', () => {
  screenReview.classList.add('hidden');
  screenResult.classList.remove('hidden');
});

document.getElementById('btnDownload').addEventListener('click', () => {
  const r = window._lastResult;
  const dateStr = new Date().toLocaleDateString('en-GB', {day:'numeric', month:'long', year:'numeric'});
  let breakdownRows = "";
  Object.keys(r.catStats).forEach(cat => {
    const s = r.catStats[cat];
    breakdownRows += `<tr><td style="padding:6px 8px;border-bottom:1px solid #C9BB93;">${cat}</td><td style="padding:6px 8px;border-bottom:1px solid #C9BB93;">${s.correct}/${s.total}</td></tr>`;
  });
  let reviewRows = "";
  QUESTIONS.forEach((item, idx) => {
    const isCorrect = answers[idx] === item.a;
    reviewRows += `
      <tr>
        <td style="padding:6px 8px;border-bottom:1px solid #C9BB93;">${idx+1}</td>
        <td style="padding:6px 8px;border-bottom:1px solid #C9BB93;">${item.q}</td>
        <td style="padding:6px 8px;border-bottom:1px solid #C9BB93;">${answers[idx]!==null ? item.opts[answers[idx]] : '-'}</td>
        <td style="padding:6px 8px;border-bottom:1px solid #C9BB93;">${item.opts[item.a]}</td>
        <td style="padding:6px 8px;border-bottom:1px solid #C9BB93; color:${isCorrect?'#3F7A5A':'#B23A2E'}; font-weight:700;">${isCorrect?'Correct':'Incorrect'}</td>
      </tr>`;
  });

  const html = `<!DOCTYPE html>
<html lang="en"><head><meta charset="UTF-8"><title>English Diagnostic Result - ${studentName}</title>
<style>
  body{font-family:Georgia, serif; background:#EFE6CC; color:#20303A; padding:36px; max-width:800px; margin:0 auto;}
  h1{font-size:22px; border-bottom:2px solid #20303A; padding-bottom:10px;}
  .stamp{display:inline-block; border:3px solid #B23A2E; color:#B23A2E; padding:8px 16px; border-radius:6px; transform:rotate(-4deg); text-transform:uppercase; letter-spacing:2px; font-weight:bold; margin-bottom:16px;}
  table{width:100%; border-collapse:collapse; margin:16px 0;}
  th{text-align:left; padding:6px 8px; border-bottom:2px solid #20303A; font-size:12px; text-transform:uppercase; letter-spacing:1px;}
  .score{font-size:40px; font-weight:bold;}
  .meta{font-size:14px; opacity:0.8;}
</style></head>
<body>
  <div class="stamp">Graded</div>
  <h1>English Diagnostic Test Result — Grade 11</h1>
  <p class="meta">Name: <strong>${studentName}</strong> &nbsp;|&nbsp; Class: <strong>${studentClass}</strong> &nbsp;|&nbsp; Date: ${dateStr}</p>
  <p class="score">${r.score}/30 <span style="font-size:16px; font-weight:normal;">(${r.pct}%)</span></p>
  <p><strong>Level: ${r.lvl.label}</strong><br>${r.lvl.desc}</p>

  <h2 style="font-size:16px;">Score by Skill Area</h2>
  <table><tr><th>Skill Area</th><th>Score</th></tr>${breakdownRows}</table>

  <h2 style="font-size:16px;">Answer Details</h2>
  <table>
    <tr><th>No.</th><th>Question</th><th>Your Answer</th><th>Correct Answer</th><th>Status</th></tr>
    ${reviewRows}
  </table>
  <p class="meta" style="margin-top:24px;">Generated by the English Diagnostic Test tool, Grade 11 SMK/SMA.</p>
</body></html>`;

  const blob = new Blob([html], {type: "text/html"});
  const url = URL.createObjectURL(blob);
  const a = document.createElement('a');
  a.href = url;
  const safeName = studentName.replace(/[^a-z0-9]+/gi, '_');
  const safeClass = studentClass.replace(/[^a-z0-9]+/gi, '_');
  a.download = `English_Diagnostic_Result_${safeName}_${safeClass}.html`;
  document.body.appendChild(a);
  a.click();
  document.body.removeChild(a);
  URL.revokeObjectURL(url);
});
</script>
</body>
</html>
