<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<title>Happy Birthday — Flip Card Surprise</title>
<style>
:root{
  --bg:#fff0f6; --card:#ffffff; --accent:#ff6fa8; --soft:#ffd6e8; --text:#3a2a33;
}
*{box-sizing:border-box}
body{margin:0; font-family: 'Poppins', system-ui, -apple-system, 'Segoe UI', Roboto; background:linear-gradient(180deg,var(--bg),#fff6f9 60%); min-height:100vh; display:flex; align-items:center; justify-content:center; padding:30px}

/* Stage */
.stage{width:100%; max-width:900px; display:grid; grid-template-columns:1fr 420px; gap:24px; align-items:start}

/* Left - story / pages */
.viewer{background:transparent}
.page{background:transparent; border-radius:18px; padding:24px; min-height:380px; display:flex; align-items:center; justify-content:center;}

/* Flip card container */
.flip-wrap{perspective:1400px}
.flip-card{width:380px; height:240px; position:relative; transform-style:preserve-3d; transition:transform 900ms cubic-bezier(.2,.9,.26,1); margin:auto}
.flip-card.is-flipped{transform:rotateY(180deg)}

.face{position:absolute; inset:0; backface-visibility:hidden; border-radius:18px; box-shadow:0 10px 30px rgba(0,0,0,0.08); display:flex; flex-direction:column; padding:20px}

/* front */
.front{background:linear-gradient(180deg,#fff,#fff0); border:4px dashed rgba(255,111,168,0.12)}
.front .title{font-size:24px; color:var(--text); font-weight:700}
.front .subtitle{color:#8b6b78; margin-top:8px}
.sticker{position:absolute; left:18px; top:18px; font-size:13px; background:var(--soft); padding:6px 10px; border-radius:12px; box-shadow:0 6px 18px rgba(255,111,168,0.08)}

/* back */
.back{transform:rotateY(180deg); background:linear-gradient(180deg,#fff7fb,#fff); border:1px solid rgba(255,111,168,0.06)}
.back .message{flex:1; display:flex; align-items:center; justify-content:center; padding:8px; text-align:center}
.message p{font-size:16px; line-height:1.5; color:var(--text)}

/* controls */
.controls{display:flex; gap:12px; justify-content:center; margin-top:12px}
.btn{background:var(--accent); color:white; border:none; padding:10px 16px; border-radius:10px; cursor:pointer; font-weight:600}
.btn.ghost{background:transparent; color:var(--accent); border:2px solid rgba(255,111,168,0.12)}

/* Right - cake stage */
.panel{background:var(--card); border-radius:18px; padding:18px; box-shadow:0 10px 30px rgba(0,0,0,0.06)}
.panel h3{margin:6px 0 10px 0; color:var(--text)}
.cake-area{min-height:320px; display:flex; align-items:center; justify-content:center; flex-direction:column}

/* ROUND cake styling - updated visually */
.cake{
  width:240px; height:180px; 
  background: linear-gradient(to bottom, #ffe9f5 0%, #ffd6ec 100%);
  border-radius:50% / 25%; /* subtle 3D ellipse look */
  position:relative; 
  padding-top:20px; /* space for candles */
  opacity:0; 
  transform:scale(0.8); 
  transition:all 0.8s ease;
  box-shadow:0 10px 20px rgba(0,0,0,0.1), inset 0 -5px 10px rgba(0,0,0,0.05);
}
.cake.show{
  opacity:1; 
  transform:scale(1);
}
.cake-plate{
  width:280px; height:20px; 
  background:#fff6ff; 
  border-radius:50%; 
  margin-top:-10px; 
  box-shadow:0 2px 6px rgba(0,0,0,0.1);
}
.candles{
  display:flex; gap:8px; justify-content:center; position:absolute; top:12px; left:50%; transform:translateX(-50%);
}
.candle{
  width:10px; height:46px; background:#f9d85c; border-radius:4px; position:relative; box-shadow:0 2px 6px rgba(0,0,0,0.08); 
  transform:translateY(-20px); opacity:0; transition:all 0.5s ease;
}
.candle.show{
  opacity:1; transform:translateY(0);
}
.flame{
  position:absolute; left:50%; transform:translateX(-50%); top:-12px; width:12px; height:16px; border-radius:50%; background:linear-gradient(180deg,#ffd27a,#ff8c42); animation:flick 240ms infinite alternate;
}
@keyframes flick{0%{transform:translateX(-50%) scaleY(1)}100%{transform:translateX(-50%) scaleY(1.25)}}

/* confetti canvas */
#confetti{position:fixed; inset:0; pointer-events:none; z-index:999}

/* small helpers */
.muted{color:#8b6b78; font-size:13px}
.hidden{display:none}

/* responsive */
@media(max-width:900px){.stage{grid-template-columns:1fr; padding:0} .flip-card{width:320px}}
</style>
</head>
<body>
<div class="stage">
  <div class="viewer">
    <div class="page flip-wrap">
      <div id="flip" class="flip-card" aria-live="polite">
        <div class="face front">
          <div class="sticker">For my favorite person ✨</div>
          <div style="flex:1; display:flex; flex-direction:column; align-items:center; justify-content:center">
            <div class="title">Happy Birthday! 🎉</div>
            <div class="subtitle">A tiny surprise made just for you — tap to flip</div>
          </div>
          <div style="display:flex; gap:8px; justify-content:center">
            <button id="flipBtn" class="btn">Flip Card</button>
            <button id="peekBtn" class="btn ghost">Peek</button>
          </div>
        </div>
        <div class="face back">
          <div class="message">
            <p id="customMsg">Happy Birthday, my favorite person! 🥳💖 You make my heart so happy just by being you. I hope your day is as sweet, sparkly, and amazing as you are. Can’t wait to hug you tight and spoil you today! 😘✨</p>
          </div>
          <div style="display:flex; gap:8px; justify-content:center">
            <button id="openCake" class="btn">Open Cake 🎂</button>
            <button id="unflip" class="btn ghost">Close</button>
          </div>
        </div>
      </div>
    </div>
    <div style="text-align:center; margin-top:18px">
      <div class="muted">Tip: Flip the card, read the message, then open the cake. Play the song and celebrate! 💕</div>
    </div>
  </div>

  <div class="panel">
    <h3>Birthday Cake & Candles</h3>
    <div class="cake-area">
      <div id="cakeCard" class="cake">
        <div class="candles" id="candlesContainer"></div>
        <div class="cake-plate"></div>
      </div>

      <div id="controls" style="margin-top:12px; display:flex; gap:8px">
        <button id="playSong" class="btn">Play Song ▶</button>
        <button id="startBlow" class="btn">Start Microphone 🎤</button>
        <button id="resetAll" class="btn ghost">Reset</button>
      </div>

      <div style="margin-top:10px">
        <div id="status" class="muted">Candles lit: <span id="litCount">19</span></div>
      </div>
    </div>
  </div>
</div>

<canvas id="confetti"></canvas>

<script>
// ---------- SETTINGS ----------
const TOTAL_CANDLES = 19;
const BLOW_THRESHOLD = 55;
const COOLDOWN_MS = 900;

// ---------- FLIP CARD ----------
const flip = document.getElementById('flip');
document.getElementById('flipBtn').addEventListener('click', ()=> flip.classList.add('is-flipped'));
document.getElementById('peekBtn').addEventListener('click', ()=>{ flip.classList.toggle('is-flipped'); setTimeout(()=>flip.classList.remove('is-flipped'),2200)});
document.getElementById('unflip').addEventListener('click', ()=> flip.classList.remove('is-flipped'));
document.getElementById('openCake').addEventListener('click', ()=> showCake());

// ---------- CAKE + CANDLES ----------
const cakeCard = document.getElementById('cakeCard');
const candlesContainer = document.getElementById('candlesContainer');
const litCountEl = document.getElementById('litCount');
let lit = TOTAL_CANDLES;
let blowCooldown = false;

function createCandles(){
  candlesContainer.innerHTML = '';
  for(let i=0;i<TOTAL_CANDLES;i++){
    const c = document.createElement('div');
    c.className='candle';
    c.dataset.index = i;
    c.innerHTML = '<div class="flame"></div>';
    candlesContainer.appendChild(c);
    setTimeout(()=> c.classList.add('show'), i*80);
  }
  lit = TOTAL_CANDLES;
  litCountEl.textContent = lit;
}

function showCake(){
  createCandles();
  cakeCard.classList.add('show');
}

function extinguishOne(){
  if(lit<=0) return;
  const flames = document.querySelectorAll('.candle .flame');
  if(flames.length===0) return;
  const f = flames[flames.length-1];
  f.style.transition='transform 400ms ease, opacity 400ms ease';
  f.style.transform='scale(0.2) translateY(-6px)';
  f.style.opacity='0';
  setTimeout(()=>{ f.remove(); },500);
  lit--;
  litCountEl.textContent = lit;
  if(lit===0) onAllBlown();
}

function onAllBlown(){
  launchConfetti();
  speakText('All candles are blown! Happy Birthday!');
}

// ---------- MICROPHONE ----------
let audioCtx, analyser, micStream, dataArr;
async function startMic(){
  if(audioCtx) return;
  try{
    const stream = await navigator.mediaDevices.getUserMedia({audio:true});
    audioCtx = new (window.AudioContext || window.webkitAudioContext)();
    micStream = audioCtx.createMediaStreamSource(stream);
    analyser = audioCtx.createAnalyser();
    analyser.fftSize = 256;
    micStream.connect(analyser);
    dataArr = new Uint8Array(analyser.frequencyBinCount);
    monitorBlow();
  }catch(e){ alert('Microphone access is required to blow out the candles.'); }
}
function monitorBlow(){
  function loop(){
    analyser.getByteFrequencyData(dataArr);
    let sum = 0; for(let i=0;i<dataArr.length;i++) sum += dataArr[i];
    const avg = sum / dataArr.length;
    if(avg > BLOW_THRESHOLD && !blowCooldown){
      blowCooldown = true;
      const strength = Math.min(5, Math.round((avg - BLOW_THRESHOLD)/8)+1);
      for(let i=0;i<strength;i++) extinguishOne();
      setTimeout(()=> blowCooldown=false, COOLDOWN_MS);
    }
    if(lit>0) requestAnimationFrame(loop);
  }
  loop();
}

// ---------- PLAY HAPPY BIRTHDAY (WebAudio simple) ----------
const playSongBtn = document.getElementById('playSong');
function playMelody(){
  const ctx = new (window.AudioContext || window.webkitAudioContext)();
  const notes = [
    [660, 300], [660,300], [740,600], [660,600], [880,600], [740,1200],
    [660,300], [660,300], [740,600], [660,600], [988,600], [880,1200],
    [660,300], [660,300], [1320,600], [1047,600], [880,600], [740,600], [988,1200]
  ];
  let t = ctx.currentTime + 0.05;
  notes.forEach(n =>{
    const osc = ctx.createOscillator();
    const gain = ctx.createGain();
    osc.type='sine'; osc.frequency.value = n[0];
    gain.gain.value = 0.0001;
    osc.connect(gain); gain.connect(ctx.destination);
    osc.start(t);
    gain.gain.linearRampToValueAtTime(0.12, t+0.01);
    gain.gain.linearRampToValueAtTime(0.0001, t + n[1]/1000);
    osc.stop(t + n[1]/1000 + 0.02);
    t += n[1]/1000;
  });
}
playSongBtn.addEventListener('click', playMelody);

// ---------- CONFETTI ----------
const confettiCanvas = document.getElementById('confetti');
const confettiCtx = confettiCanvas.getContext('2d');
let confettiPieces = [];
function resizeCanvas(){ confettiCanvas.width = innerWidth; confettiCanvas.height = innerHeight; }
window.addEventListener('resize', resizeCanvas); resizeCanvas();
function random(min,max){return Math.random()*(max-min)+min}
function launchConfetti(){
  const count = 140;
  confettiPieces = [];
  for(let i=0;i<count;i++){
    confettiPieces.push({
      x: random(0, confettiCanvas.width),
      y: random(-confettiCanvas.height,0),
      w: random(6,12), h: random(8,16),
      vx: random(-0.8,0.8), vy: random(2,6),
      r: random(0,360), vr: random(-6,6),
      color: `hsl(${Math.floor(random(0,360))},70%,60%)`
    });
  }
  requestAnimationFrame(confettiLoop);
}
function confettiLoop(){
  confettiCtx.clearRect(0,0,confettiCanvas.width, confettiCanvas.height);
  for(let p of confettiPieces){
    p.x += p.vx; p.y += p.vy; p.r += p.vr;
    confettiCtx.save();
    confettiCtx.translate(p.x,p.y); confettiCtx.rotate(p.r*Math.PI/180);
    confettiCtx.fillStyle = p.color; confettiCtx.fillRect(-p.w/2, -p.h/2, p.w, p.h);
    confettiCtx.restore();
  }
  confettiPieces = confettiPieces.filter(p => p.y < confettiCanvas.height + 40);
  if(confettiPieces.length>0) requestAnimationFrame(confettiLoop);
}

// ---------- VOICE FEEDBACK ----------
function speakText(txt){
  if('speechSynthesis' in window){
    const s = new SpeechSynthesisUtterance(txt);
    s.lang = 'en-GB';
    window.speechSynthesis.cancel();
    window.speechSynthesis.speak(s);
  }
}

// ---------- UI HOOKS ----------
document.getElementById('startBlow').addEventListener('click', ()=>{ startMic(); speakText('Ready! Blow on the mic to make a wish.'); });
document.getElementById('resetAll').addEventListener('click', ()=>{
  createCandles(); 
  cakeCard.classList.remove('show');
  litCountEl.textContent = lit; 
  speakText('Reset. Flip again when you are ready.');
});

// Auto-create initial UI state
createCandles();
setTimeout(()=>{ flip.classList.add('is-flipped'); setTimeout(()=>flip.classList.remove('is-flipped'),1100); }, 800);
window.addEventListener('click', ()=>{ if(audioCtx && audioCtx.state==='suspended') audioCtx.resume(); });
</script>
</body>
</html>
