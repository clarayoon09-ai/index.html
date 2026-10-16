<!doctype html>
<html lang="ko">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<title>오늘의 영어 · 2000개 단어 + 유의어/다의어/반의어/발음기호</title>
<meta name="theme-color" content="#f6f7fb" />
<style>
:root{
  --bg:#f6f7fb; --paper:#fff; --ink:#22283a; --muted:#6f7688;
  --accent:#6259d9; --light:#efedff; --line:#e8eaf2;
  --green:#e2f7eb; --red:#ffeded; --radius:14px;
}
*{box-sizing:border-box}
html,body{height:100%;margin:0;font-family:system-ui,-apple-system,"Noto Sans KR",sans-serif;background:var(--bg);color:var(--ink)}
.header{display:flex;align-items:center;justify-content:space-between;padding:10px 18px;background:#fff;border-bottom:1px solid var(--line);position:sticky;top:0;z-index:40}
.brand{font-weight:900;font-size:18px}
.nav{display:flex;gap:8px;align-items:center}
.tab{background:transparent;border:0;padding:8px 12px;border-radius:9px;color:var(--muted);font-weight:800;cursor:pointer}
.tab.active{background:var(--light);color:var(--accent)}
.container{max-width:1180px;margin:20px auto;padding:0 18px}
.toolbar{display:flex;gap:10px;align-items:center;flex-wrap:wrap;margin-bottom:12px}
.input{padding:10px;border-radius:10px;border:1px solid var(--line);flex:1;min-width:220px}
.small{padding:8px 10px;border-radius:8px;border:1px solid var(--line);background:#fff;color:var(--accent);cursor:pointer;font-weight:800}
.exportBtn{background:var(--accent);color:#fff;border:0;padding:8px 12px;border-radius:9px;font-weight:800;cursor:pointer}

/* grid */
.view { background:transparent; min-height:60vh; }
.grid {
  display:grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap:14px;
  align-items:start;
}

/* card */
.card {
  background:var(--paper);
  border:1px solid var(--line);
  border-radius:12px;
  padding:12px;
  display:flex;flex-direction:column;gap:8px;
  min-height:180px;
}
.card .img {
  height:110px;border-radius:10px;background:#f2f2f7;background-position:center;background-size:cover;
  display:block;
}
.meta {display:flex;justify-content:space-between;align-items:center;gap:8px}
.en {font-weight:900;font-size:16px}
.ko {color:var(--muted);font-weight:700}
.ex {color:var(--muted);font-size:13px;flex:1}
.actions{display:flex;gap:8px;margin-top:auto}
.smallBtn{padding:8px 10px;border-radius:8px;border:1px solid var(--line);background:#fff;color:var(--accent);cursor:pointer;font-weight:800}

/* today list */
.today-list{display:grid;gap:8px}
.today-row{display:flex;justify-content:space-between;align-items:center;padding:10px;border-radius:10px;background:#fff;border:1px solid var(--line)}

/* panel */
.panel {
  position:fixed;
  width:420px;
  min-height:120px;
  background:#fff;
  border:1px solid rgba(0,0,0,0.08);
  box-shadow:0 8px 30px rgba(10,12,30,0.08);
  border-radius:10px;
  z-index:80;
  overflow:hidden;
  display:flex;flex-direction:column;
}
.panel .head {background:var(--accent);color:#fff;padding:8px;cursor:move;display:flex;justify-content:space-between;align-items:center}
.panel .body {padding:12px;overflow:auto;max-height:62vh}
.closePanel{background:transparent;border:0;color:#fff;font-weight:900;cursor:pointer}

/* responsive */
@media(max-width:760px){
  .card .img{height:90px}
  .panel{width:92%}
}
</style>
</head>
<body>
<header class="header">
  <div class="brand">오늘의 <span style="color:var(--accent)">영어</span></div>
  <nav class="nav" aria-label="메뉴">
    <button class="tab active" data-view="vocab">단어 카드</button>
    <button class="tab" data-view="today">오늘의 20</button>
    <button class="tab" data-view="quiz">퀴즈</button>
    <button class="tab" data-view="sentences">회화 예문</button>
    <button class="exportBtn" id="exportView">Export view</button>
  </nav>
</header>

<main class="container">
  <div class="toolbar" id="toolbar">
    <input id="globalSearch" class="input" placeholder="검색: 영어/한국어/예문/유의어/반의어/다의어" />
    <label style="display:flex;align-items:center;gap:6px;color:var(--muted)"><input type="checkbox" id="allowDupChk"> 오늘 중복 허용</label>
    <label style="display:flex;align-items:center;gap:6px;color:var(--muted)"><input type="checkbox" id="enableTTS" checked> 스피커 켜기</label>
    <button class="small" id="openListPanel">목록 창 열기</button>
    <button class="small" id="openQuizPanel">퀴즈 창 열기</button>
  </div>
  <section id="vocab" class="view">
    <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:10px">
      <h2>단어 카드</h2>
      <div style="color:var(--muted)">표시되는 카드 수는 화면 크기에 맞춰 자동 조정</div>
    </div>
    <div id="vocabGrid" class="grid" aria-live="polite"></div>
  </section>

  <section id="today" class="view" style="display:none">
    <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:10px">
      <h2>오늘의 20단어</h2>
      <div style="display:flex;gap:8px;align-items:center">
        <button class="small" id="regenTodayBtn">다시 생성</button>
        <button class="small" id="openTodayPanel">오늘 창 열기</button>
      </div>
    </div>
    <div id="todayList" class="today-list"></div>
  </section>

  <section id="quiz" class="view" style="display:none">
    <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:10px">
      <h2>퀴즈</h2>
      <div style="color:var(--muted)">패널 창으로 별도 연습</div>
    </div>
    <div id="quizArea" style="background:#fff;border:1px solid var(--line);padding:14px;border-radius:10px">
      <div id="mcQuestion" style="font-weight:900;font-size:20px">퀴즈를 시작하세요</div>
      <div id="mcAnswers" style="display:grid;grid-template-columns:repeat(2,1fr);gap:8px;margin-top:12px"></div>
      <div style="margin-top:10px;display:flex;gap:8px">
        <button class="small" id="mcNext" disabled>다음</button>
        <button class="small" id="mcStart">시작</button>
      </div>
      <div id="mcFeedback" style="margin-top:10px;font-weight:800;color:var(--muted)"></div>
    </div>
  </section>

  <section id="sentences" class="view" style="display:none">
    <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:10px">
      <h2>회화 예문</h2>
      <div style="color:var(--muted)">예문 듣기 / 창 열기</div>
    </div>
    <div id="sentList" style="display:grid;gap:8px"></div>
  </section>
</main>

<div id="panelsRoot"></div>

<script>
/* ---------------------------------------------------------------
   2000개 단어 생성 (자동 생성 기반, 유의어/반의어/다의어/관련 단어 포함)
   --------------------------------------------------------------- */
const seedWords = [
  "accept","access","achieve","acknowledge","act","add","admire","admit","advise","afford","agree","allow","announce","appear","apply","approach","approve","argue","arrange","arrive","ask","assess","assist","assume","attach","attempt","attend","attract","avoid","balance","ban","become","begin","believe","belong","benefit","bind","bite","blame","blend","bless","block","blow","boost","borrow","bounce","break","breathe","bring","build","burn","bury","buy","calculate","call","calm","cancel","capture","care","carry","catch","celebrate","change","charge","chase","chat","check","choose","claim","clarify","clean","clear","climb","close","collect","combine","comfort","comment","commit","communicate","compare","compete","complain","complete","concern","conclude","conduct","confirm","connect","consider","construct","consult","consume","contain","continue","contract","control","convert","convince","cook","copy","correct","cost","count","create","cross","cry","cut","dance","date","deal","decide","declare","decorate","delay","deliver","demand","deny","depend","describe","deserve","design","desire","destroy","determine","develop","die","dig","direct","discuss","display","disturb","divide","do","double","drag","draw","dream","dress","drink","drive","drop","earn","eat","edit","educate","effect","elaborate","eliminate","embrace","emerge","employ","enable","encourage","endure","enforce","engage","enhance","enjoy","ensure","enter","entertain","escape","establish","estimate","evaluate","examine","excel","exchange","excite","exercise","exhibit","exist","expand","expect","explain","explore","express","extend","face","fail","fall","fashion","favor","feed","feel","fight","fill","finance","find","finish","fit","fix","focus","force","form","found","frame","freeze","gather","generate","get","give","go","grab","grant","grasp","grow","guard","guess","guide","handle","happen","harm","hate","have","heal","hear","help","hide","highlight","hire","hold","hope","identify","ignore","imagine","imitate","impact","implement","improve","include","increase","indicate","influence","inform","inherit","initiate","inject","injure","inspect","install","instruct","intend","interest","interpret","introduce","invent","invest","invite","involve","issue","judge","jump","justify","keep","kick","kill","knock","label","land","launch","lead","learn","leave","lecture","lend","let","lift","light","like","limit","link","listen","live","load","locate","lock","look","lose","love","maintain","manage","match","measure","meet","mention","merge","mind","miss","mix","move","murmur","name","need","negotiate","notice","obey","object","observe","obtain","occupy","offer","open","operate","order","organize","overcome","owe","own","paint","park","participate","pass","pay","perform","permit","persuade","place","plan","play","please","point","polish","possess","post","pour","practice","praise","prefer","prepare","preserve","present","press","prevent","print","produce","progress","promise","protect","prove","provide","publish","pull","purchase","push","put","qualify","question","quickly","quit","raise","reach","read","realize","receive","recognize","recommend","record","recover","reduce","refer","reflect","refuse","regain","regard","register","regret","relate","release","rely","remain","remember","remind","remove","repair","repeat","replace","reply","report","represent","request","require","rescue","research","reserve","resist","resolve","respond","restore","retain","retire","return","reveal","review","revise","reward","rid","ride","ring","risk","roll","rule","run","rush","satisfy","save","say","search","secure","see","seek","seem","select","sell","send","sense","serve","set","settle","share","shine","ship","shoot","shop","show","shut","sign","signal","speak","specify","spend","spill","spread","spring","stand","start","state","stay","steal","step","stick","stop","store","stress","study","submit","succeed","suggest","supply","support","suppose","survive","switch","talk","target","teach","tell","test","thank","think","throw","touch","trade","train","transfer","translate","travel","treat","trust","turn","understand","unite","update","upgrade","use","utilize","validate","value","vary","view","visit","vote","wait","walk","want","warn","wash","watch","wave","wear","weigh","welcome","whisper","win","wonder","work","worry","wrap","write","yield"
];

const lexiconSeed = {
  "accept":["receive","take","approve","admit"],
  "achieve":["attain","accomplish","realize","complete"],
  "avoid":["evade","shun","bypass","skip"],
  "build":["construct","assemble","create","forge"],
  "confident":["assured","self-assured","sure","bold"],
  "consider":["reflect","ponder","review","weigh"],
  "convince":["persuade","induce","win over","assure"],
  "decide":["choose","determine","resolve","select"],
  "discover":["find","uncover","locate","detect"],
  "efficient":["productive","effective","capable","streamlined"],
  "encourage":["support","motivate","boost","inspire"],
  "improve":["enhance","upgrade","refine","better"],
  "learn":["study","master","acquire","grasp"],
  "reliable":["dependable","trustworthy","stable","sound"],
  "recommend":["suggest","advise","propose","endorse"],
  "solve":["resolve","address","fix","answer"],
  "understand":["comprehend","grasp","decode","know"],
  "value":["appreciate","esteem","cherish","respect"],
  "care":["concern","attention","nurture","watch"],
  "danger":["risk","hazard","threat","peril"],
  "final":["last","ultimate","closing","terminal"],
  "happy":["cheerful","joyful","glad","pleased"],
  "important":["significant","crucial","major","essential"],
  "increase":["grow","expand","boost","raise"],
  "reduce":["decrease","cut","lessen","shrink"]
};

const relatedSeed = {
  "accept":{"noun":"acceptance","adj":"acceptable","verb":"accept","adv":"acceptably"},
  "build":{"noun":"builder","adj":"buildable","verb":"build","adv":"build-wise"},
  "decide":{"noun":"decision","adj":"decisive","verb":"decide","adv":"decisively"},
  "happy":{"noun":"happiness","adj":"happy","verb":"happen","adv":"happily"},
  "improve":{"noun":"improvement","adj":"improved","verb":"improve","adv":"improvingly"},
  "increase":{"noun":"increase","adj":"increased","verb":"increase","adv":"increasingly"},
  "reduce":{"noun":"reduction","adj":"reduced","verb":"reduce","adv":"reducibly"},
  "trust":{"noun":"trust","adj":"trustworthy","verb":"trust","adv":"trustfully"},
  "value":{"noun":"value","adj":"valuable","verb":"value","adv":"valuably"},
  "succeed":{"noun":"success","adj":"successful","verb":"succeed","adv":"successfully"}
};

const sensesSeed = {
  "accept":["to receive or agree to something","to consider something valid"],
  "build":["to construct something","to develop gradually"],
  "decide":["to make a choice","to settle a matter"],
  "value":["to appreciate the worth of something","to consider important"],
  "reduce":["to make smaller","to bring down in amount"],
  "increase":["to become larger","to make larger"],
  "trust":["to believe in someone","to rely on someone"],
  "solve":["to find an answer","to work out a problem"]
};

const antonymSeed = {
  "accept":["reject","refuse","decline"],
  "avoid":["face","encounter","meet"],
  "build":["destroy","demolish","ruin"],
  "confident":["insecure","timid","nervous"],
  "consider":["ignore","dismiss","neglect"],
  "decide":["hesitate","delay","doubt"],
  "discover":["lose","hide","miss"],
  "efficient":["inefficient","wasteful","slow"],
  "encourage":["discourage","deter","weaken"],
  "improve":["worsen","decline","damage"],
  "learn":["forget","ignore","neglect"],
  "reliable":["unreliable","unstable","doubtful"],
  "recommend":["discourage","warn","oppose"],
  "solve":["create","worsen","complicate"],
  "understand":["misunderstand","confuse","misread"],
  "value":["ignore","disregard","undervalue"],
  "happy":["sad","unhappy","miserable"],
  "increase":["decrease","reduce","lessen"],
  "reduce":["increase","expand","raise"]
};

function generatePron(w){
  const letters = w.toLowerCase().split('');
  let accented = '';
  for (let i=0;i<letters.length;i++){
    const ch = letters[i];
    if (ch === 'a') accented += 'ə';
    else if (ch === 'e') accented += 'iː';
    else if (ch === 'i') accented += 'ɪ';
    else if (ch === 'o') accented += 'əʊ';
    else if (ch === 'u') accented += 'juː';
    else if (ch === 'c') accented += 'k';
    else accented += ch;
  }
  return "/" + accented.replace(/aa/g,'ɑ').replace(/ee/g,'iː').replace(/oo/g,'uː') + "/";
}
function simpleKo(word){
  const lower = word.toLowerCase();
  if (lower.endsWith("ing")) return lower.replace(/ing$/,'하는');
  if (lower.endsWith("ed")) return lower.replace(/ed$/,'된');
  if (lower.endsWith("s")) return lower.replace(/s$/,'들');
  if (lower.endsWith("ly")) return lower.replace(/ly$/,'하게');
  if (lower.endsWith("tion")) return lower.replace(/tion$/,'션');
  return lower + "하다";
}
function sampleSense(word){
  const lower = word.toLowerCase();
  if (sensesSeed[word]) return sensesSeed[word];
  const base = lower.replace(/ly$/,'').replace(/ing$/,'').replace(/ed$/,'').replace(/s$/,'');
  return [`to ${base} something`, `the act of ${base}`];
}
function genRelated(word){
  const key = word.toLowerCase();
  const rel = relatedSeed[key] || {};
  const out = [];
  for (const k in rel) {
    if (rel[k]) out.push(rel[k]);
  }
  if (!out.length) {
    const base = key.replace(/ing$/,'').replace(/ed$/,'').replace(/s$/,'');
    out.push(base + "er", base + "ment", base + "ing", base + "ed");
  }
  return [...new Set(out)].slice(0,4);
}
function getAnt(word){
  const lower = word.toLowerCase();
  if (antonymSeed[lower]) return antonymSeed[lower];
  return ["opposite", "contrast", "inverse"];
}
function getSyn(word){
  const lower = word.toLowerCase();
  if (lexiconSeed[lower]) return lexiconSeed[lower];
  const base = lower.replace(/ing$/,'').replace(/ed$/,'').replace(/s$/,'');
  return [base + "ing", base + "ed", base + "able", base + "ness"];
}

let generated = [];
const used = new Set();

function addWord(word){
  const key = String(word).trim();
  if (!key || used.has(key.toLowerCase())) return;
  used.add(key.toLowerCase());
  const lower = key.toLowerCase();
  const en = key.charAt(0).toUpperCase() + key.slice(1);
  const pron = generatePron(en);
  const ko = simpleKo(en);
  const senses = sampleSense(en);
  const synonyms = getSyn(lower).slice(0,5);
  const antonyms = getAnt(lower).slice(0,5);
  const related = genRelated(lower).slice(0,4);
  generated.push({
    en, ko, pron,
    synonyms, antonyms, senses, related, cat: "동사",
    ex: `I ${en.toLowerCase()} it every day.`, tr: `매일 그것을 ${ko} 생각해요.`
  });
}
for (const seed of seedWords) addWord(seed);
let i = 0;
while (generated.length < 2000 && i < 20000){
  // create around 2000 total
  const seed = seedWords[i % seedWords.length];
  const variant = seed + (i % 7 === 0 ? "ly" : i % 5 === 0 ? "ness" : i % 3 === 0 ? "ing" : "");
  addWord(variant);
  i++;
}
let words = generated.slice(0, 2000);
words = words.map((w, idx) => ({...w, id: idx + 1, cat: idx % 5 === 0 ? "명사" : idx % 3 === 0 ? "형용사" : "동사"}));
words = words.slice(0, 2000);

/* ---------------------------------------------------------------
   UI logic
   --------------------------------------------------------------- */
const TTS_KEY = "enableTTS";
function speak(text){
  if(!("speechSynthesis" in window)) return;
  const enabled = document.getElementById('enableTTS').checked;
  if(!enabled) return;
  speechSynthesis.cancel();
  const u = new SpeechSynthesisUtterance(text);
  u.lang = "en-US";
  u.rate = 0.9;
  const voices = speechSynthesis.getVoices();
  const v = voices.find(x=>x.lang==="en-US") || voices.find(x=>x.lang && x.lang.startsWith("en"));
  if(v) u.voice = v;
  speechSynthesis.speak(u);
}
window.speak = speak;

const TODAY_KEY = "oneul_today_v2000";
function shuffle(a){ const b=[...a]; for(let i=b.length-1;i>0;i--){const j=Math.floor(Math.random()*(i+1));[b[i],b[j]]=[b[j],b[i]];} return b; }
function sampleToday(count=20, allowDup=false){
  if(allowDup){
    const out=[]; for(let i=0;i<count;i++) out.push(words[Math.floor(Math.random()*words.length)]);
    return out;
  }
  const arr = shuffle(words);
  return arr.slice(0, count);
}
function regenerateToday(){
  const allowDup = document.getElementById('allowDupChk').checked;
  const list = sampleToday(20, allowDup);
  try{ localStorage.setItem(TODAY_KEY, JSON.stringify({date:new Date().toISOString().slice(0,10), list})); }catch(e){}
  renderToday();
}
function getTodayList(){
  try{
    const raw = localStorage.getItem(TODAY_KEY);
    const today = new Date().toISOString().slice(0,10);
    if(!raw){ regenerateToday(); return JSON.parse(localStorage.getItem(TODAY_KEY)).list; }
    const parsed = JSON.parse(raw);
    if(parsed.date !== today){ regenerateToday(); return JSON.parse(localStorage.getItem(TODAY_KEY)).list; }
    return parsed.list;
  }catch(e){
    regenerateToday();
    return [];
  }
}
function renderToday(){
  const root = $('todayList');
  if(!root) return;
  root.innerHTML = '';
  const list = getTodayList();
  list.forEach((w,i)=>{
    const row = document.createElement('div'); row.className='today-row';
    row.innerHTML = `<div><strong>${i+1}. ${w.en}</strong><div style="color:var(--muted)">${w.ko}</div></div>`;
    const right = document.createElement('div'); right.style.display='flex'; right.style.gap='8px';
    const play = document.createElement('button'); play.className='small'; play.textContent='🔊'; play.onclick=()=>speak(w.en);
    const open = document.createElement('button'); open.className='small'; open.textContent='상세'; open.onclick=()=>openPanelForWord(w);
    right.append(play,open);
    row.appendChild(right);
    root.appendChild(row);
  });
}
document.getElementById('regenTodayBtn').addEventListener('click', ()=>regenerateToday());

/* adaptive grid sizing */
let currentPageSize = 12;
function calcPageSize(){
  const grid = $('vocabGrid');
  if(!grid) return 12;
  const rowHeight = 220;
  const availHeight = Math.max(240, window.innerHeight - grid.getBoundingClientRect().top - 140);
  const rows = Math.max(1, Math.floor(availHeight / rowHeight));
  const gridWidth = grid.clientWidth || (window.innerWidth - 40);
  const colWidth = 240;
  const cols = Math.max(1, Math.floor(gridWidth / colWidth));
  return rows * cols;
}
function renderVocabPage(){
  const q = ($('globalSearch').value||'').trim().toLowerCase();
  const grid = $('vocabGrid');
  if(!grid) return;
  const filtered = words.filter(w=>{
    if(!q) return true;
    const searchText = [
      w.en, w.ko, w.pron, w.ex, w.tr, (w.synonyms||[]).join(' '), (w.antonyms||[]).join(' '), (w.related||[]).join(' '), (w.senses||[]).join(' ')
    ].join(' ').toLowerCase();
    return searchText.includes(q);
  });
  const pageSize = currentPageSize;
  const start = 0;
  const pageItems = filtered.slice(start, start + pageSize);
  grid.innerHTML = '';
  if(pageItems.length === 0){
    grid.innerHTML = '<div style="grid-column:1/-1;padding:20px;background:#fff;border:1px solid var(--line);border-radius:10px;color:var(--muted)">검색 결과가 없습니다.</div>';
    return;
  }
  pageItems.forEach(w=>{
    const c = document.createElement('div'); c.className='card';
    const img = document.createElement('div'); img.className='img';
    img.style.backgroundImage = `url('${imageForWord(w.en)}')`;
    const meta = document.createElement('div'); meta.className='meta';
    const en = document.createElement('div'); en.className='en'; en.textContent = w.en;
    const cat = document.createElement('div'); cat.style.color='var(--muted)'; cat.style.fontWeight='800'; cat.textContent = w.cat || '동사';
    meta.append(en,cat);
    const ko = document.createElement('div'); ko.className='ko'; ko.textContent = w.ko || '';
    const ex = document.createElement('div'); ex.className='ex'; ex.textContent = w.ex || '';
    const actions = document.createElement('div'); actions.className='actions';
    const btnSpeak = document.createElement('button'); btnSpeak.className='smallBtn'; btnSpeak.textContent='🔊'; btnSpeak.title='발음 듣기'; btnSpeak.onclick=(ev)=>{ev.stopPropagation(); speak(w.en);}
    const btnOpen = document.createElement('button'); btnOpen.className='smallBtn'; btnOpen.textContent='상세'; btnOpen.onclick=(ev)=>{ev.stopPropagation(); openPanelForWord(w);}
    actions.append(btnSpeak, btnOpen);
    c.append(img, meta, ko, ex, actions);
    c.onclick = ()=>{ openPanelForWord(w); if(document.getElementById('enableTTS').checked) speak(w.en); };
    grid.appendChild(c);
  });
}
function layoutAndRender(){ currentPageSize = calcPageSize(); renderVocabPage(); renderToday(); renderSentences(); }
window.addEventListener('resize', ()=>layoutAndRender());

/* ---------------------------
   Sentences render
   --------------------------- */
function renderSentences(){
  const root = $('sentList');
  if(!root) return;
  root.innerHTML = '';
  const base = [
    {en:"I can't wait to hear from you.",ko:"너의 소식을 기다리고 있어."},
    {en:"That really helps.",ko:"그거 정말 도움이 돼요."},
    {en:"I have a lot on my plate.",ko:"할 일이 많이 있어요."},
    {en:"It was worth it.",ko:"그만한 가치가 있었어요."},
    {en:"I am looking forward to it.",ko:"그것을 기대하고 있어요."}
  ];
  base.forEach((s,i)=>{
    const el = document.createElement('div'); el.style.background='#fff'; el.style.border='1px solid var(--line)'; el.style.padding='12px'; el.style.borderRadius='10px';
    el.innerHTML = `<div style="font-weight:800">${s.en}</div><div style="color:var(--muted)">${s.ko}</div>`;
    const btn = document.createElement('button'); btn.className='small'; btn.textContent='창 열기'; btn.style.marginTop='8px'; btn.onclick=()=>openPanelForSentence(s);
    el.appendChild(btn);
    root.appendChild(el);
  });
}

/* ---------------------------
   Panels
   --------------------------- */
const panelsRoot = document.getElementById('panelsRoot');
let panelCounter = 0;
function openPanel(opts){
  const id = 'panel-'+(panelCounter++);
  const panel = document.createElement('div'); panel.className='panel'; panel.id=id;
  panel.style.left = (60 + panelCounter*18) + 'px';
  panel.style.top = (60 + panelCounter*12) + 'px';
  panel.innerHTML = `<div class="head"><div>${opts.title}</div><div><button class="closePanel">✕</button></div></div><div class="body">${opts.html}</div>`;
  panelsRoot.appendChild(panel);
  panel.querySelector('.closePanel').addEventListener('click', ()=>panel.remove());
  makeDraggable(panel);
}
function openPanelForWord(w){
  const html = `
    <div style="display:flex;gap:10px">
      <div style="width:120px;height:80px;background-image:url('${imageForWord(w.en)}');background-size:cover;border-radius:8px"></div>
      <div style="flex:1">
        <div style="font-weight:900">${w.en}</div>
        <div style="color:var(--muted)">${w.ko}</div>
        <div style="margin-top:8px">${w.ex||''}</div>
      </div>
    </div>
    <div style="margin-top:12px">
      <div><strong>발음기호:</strong> ${w.pron || '/' + w.en + '/'}</div>
      <div><strong>유의어:</strong> ${(w.synonyms||[]).join(', ') || '없음'}</div>
      <div><strong>반의어:</strong> ${(w.antonyms||[]).join(', ') || '없음'}</div>
      <div><strong>다의어:</strong> ${(w.senses||[]).join(' / ') || '없음'}</div>
      <div><strong>관련 단어:</strong> ${(w.related||[]).join(', ') || '없음'}</div>
    </div>
    <div style="margin-top:10px"><button class="small" onclick="window.speak('${escapeForInline(w.en)}')">🔊 발음</button></div>
  `;
  openPanel({title:w.en, html});
  if(document.getElementById('enableTTS').checked) speak(w.en);
}
function openPanelForSentence(s){ const html = `<div style="font-weight:900">${s.en}</div><div style="color:var(--muted);margin-top:8px">${s.ko}</div><div style="margin-top:8px"><button class="small" onclick="window.speak('${escapeForInline(s.en)}')">🔊 듣기</button></div>`; openPanel({title:'문장', html}); }
function openQuizPanel(){ const html = `<div id="panelQuizArea"><div style="font-weight:900" id="pqQuestion">퀴즈 준비...</div><div id="pqAnswers" style="display:grid;grid-template-columns:repeat(2,1fr);gap:8px;margin-top:8px"></div><div style="margin-top:8px"><button class="small" id="pqNext" disabled>다음</button><button class="small" id="pqStart">시작</button></div><div id="pqFeedback" style="margin-top:8px;font-weight:800;color:var(--muted)"></div></div>`; openPanel({title:'퀴즈', html}); setTimeout(()=>initPanelQuiz(),60); }
function openListPanel(){ const listHtml = words.map(w=>`<div style="padding:8px;border-bottom:1px solid #f0f0f5"><strong>${w.en}</strong><div style="color:var(--muted)">${w.ko}</div></div>`).join(''); openPanel({title:'전체 목록', html:`<div style="max-height:60vh;overflow:auto">${listHtml}</div>`}); }
function makeDraggable(panel){
  const head = panel.querySelector('.head');
  if(!head) return;
  head.onmousedown = function(e){
    e.preventDefault();
    let shiftX = e.clientX - panel.getBoundingClientRect().left;
    let shiftY = e.clientY - panel.getBoundingClientRect().top;
    function moveAt(pageX,pageY){ panel.style.left = pageX - shiftX + 'px'; panel.style.top = pageY - shiftY + 'px'; }
    function onMouseMove(e){ moveAt(e.pageX,e.pageY); }
    document.addEventListener('mousemove', onMouseMove);
    document.onmouseup = function(){ document.removeEventListener('mousemove', onMouseMove); document.onmouseup = null; };
  };
  head.ondragstart = ()=>false;
}

/* panel quiz */
function initPanelQuiz(){
  const panel = panelsRoot.querySelector('.panel:last-child');
  if(!panel) return;
  const qEl = panel.querySelector('#pqQuestion');
  const aEl = panel.querySelector('#pqAnswers');
  const fb = panel.querySelector('#pqFeedback');
  const startBtn = panel.querySelector('#pqStart');
  const nextBtn = panel.querySelector('#pqNext');
  let deck = [], pIdx=0, pAnswered=false;
  function start(){
    deck = shuffle(words).slice(0,8);
    pIdx=0; pAnswered=false; fb.textContent=''; nextBtn.disabled=true; show();
  }
  function show(){
    const w = deck[pIdx];
    qEl.textContent = w.en;
    aEl.innerHTML = '';
    const choices = shuffle([w, ...shuffle(words.filter(x=>x.en!==w.en)).slice(0,3)]);
    choices.forEach(c=>{
      const b = document.createElement('button'); b.className='smallBtn'; b.style.width='100%'; b.textContent = c.ko;
      b.onclick = ()=>{ if(pAnswered) return; pAnswered=true; nextBtn.disabled=false; if(c.en===w.en){ b.style.background='#e6fbf0'; fb.textContent='정답!'; } else { b.style.background='#fff0f0'; fb.textContent='오답'; } };
      aEl.appendChild(b);
    });
    if(document.getElementById('enableTTS').checked) speak(w.en);
  }
  startBtn.onclick = start;
  nextBtn.onclick = ()=>{ if(!pAnswered) return; pIdx++; if(pIdx >= deck.length){ fb.textContent='퀴즈 완료!'; qEl.textContent='완료'; aEl.innerHTML=''; nextBtn.disabled=true; } else { pAnswered=false; nextBtn.disabled=true; fb.textContent=''; show(); } };
}

/* export */
document.getElementById('exportView').addEventListener('click', ()=>{
  const activeTab = document.querySelector('.tab.active');
  const viewId = activeTab ? activeTab.dataset.view : 'vocab';
  const viewEl = document.getElementById(viewId);
  if(!viewEl) return alert('뷰를 찾을 수 없습니다.');
  const html = `<!doctype html><html><head><meta charset="utf-8"><title>Exported - ${viewId}</title><style>body{font-family:system-ui;margin:20px;background:#f6f7fb;color:#222} .card{background:#fff;padding:12px;border-radius:8px;border:1px solid #eee;margin-bottom:12px}</style></head><body>${viewEl.outerHTML}</body></html>`;
  const blob = new Blob([html],{type:'text/html'});
  const url = URL.createObjectURL(blob);
  const a = document.createElement('a'); a.href = url; a.download = `${viewId}.html`; document.body.appendChild(a); a.click(); a.remove(); URL.revokeObjectURL(url);
});

/* panel/event bindings */
document.querySelectorAll('.tab').forEach(tab=>{
  tab.addEventListener('click', ()=> {
    document.querySelectorAll('.tab').forEach(t=>t.classList.remove('active'));
    tab.classList.add('active');
    const view = tab.dataset.view;
    document.querySelectorAll('.view').forEach(v=>v.style.display='none');
    const el = document.getElementById(view);
    if(el) el.style.display = '';
    layoutAndRender();
  });
});

$('globalSearch').addEventListener('input', ()=>{ renderVocabPage(); });
document.getElementById('openListPanel').addEventListener('click', openListPanel);
document.getElementById('openQuizPanel').addEventListener('click', openQuizPanel);
document.getElementById('openTodayPanel').addEventListener('click', ()=>openPanel({title:'오늘의 단어', html: document.getElementById('todayList').innerHTML}));
document.getElementById('allowDupChk').addEventListener('change', ()=>regenerateToday());
document.getElementById('enableTTS').checked = true;

function escapeForInline(s){ return (s||'').replace(/'/g,"\\'").replace(/"/g,'\\"'); }

layoutAndRender();
renderToday();
renderSentences();
</script>
</body>
</html>
