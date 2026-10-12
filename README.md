
                        <!DOCTYPE html>
                        <html lang="en">
                        <head>
                            <meta charset="UTF-8">
                            <meta name="viewport" content="width=device-width, initial-scale=1.0">
              <style>
                body {
                  background-color: white; /* Ensure the iframe has a white background */
                }

                @import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700&family=Roboto:wght@400;500&display=swap');

body {
  background-color: #050505;
  color: #e0e0e0;
  font-family: 'Roboto', sans-serif;
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
  margin: 0;
}

.generator-container {
  width: 100%;
  max-width: 420px;
  background: linear-gradient(145deg, #1a1a1a, #0d0d0d);
  border-radius: 20px;
  box-shadow: 0 20px 50px rgba(0,0,0,0.8), 0 0 0 1px #333;
  overflow: hidden;
  border-top: 2px solid #ff3333;
}

.header {
  background: #111;
  padding: 30px 20px;
  text-align: center;
  border-bottom: 1px solid #333;
  position: relative;
}

.logo-icon {
  width: 50px;
  height: 50px;
  margin: 0 auto 10px;
  color: #ff3333;
  filter: drop-shadow(0 0 10px rgba(255, 51, 51, 0.6));
}

.title {
  font-family: 'Orbitron', sans-serif;
  font-size: 1.8rem;
  margin: 0;
  color: #fff;
  letter-spacing: 2px;
  text-transform: uppercase;
}

.subtitle {
  font-size: 0.7rem;
  color: #666;
  margin-top: 5px;
  letter-spacing: 3px;
}

.content {
  padding: 25px;
}

.control-group {
  margin-bottom: 25px;
}

label {
  display: block;
  font-size: 0.8rem;
  color: #888;
  margin-bottom: 8px;
  font-weight: bold;
  text-transform: uppercase;
}

/* Custom Select */
.select-wrapper {
  position: relative;
}

select {
  width: 100%;
  background: #222;
  border: 1px solid #444;
  color: #fff;
  padding: 12px;
  border-radius: 8px;
  font-size: 1rem;
  appearance: none;
  cursor: pointer;
  transition: 0.3s;
}

select:focus {
  outline: none;
  border-color: #ff3333;
  box-shadow: 0 0 10px rgba(255, 51, 51, 0.2);
}

.select-arrow {
  position: absolute;
  right: 15px;
  top: 50%;
  transform: translateY(-50%);
  color: #666;
  pointer-events: none;
}

/* Preset Grid */
.preset-grid {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 10px;
}

.preset-btn {
  background: #222;
  border: 1px solid #444;
  color: #aaa;
  padding: 10px;
  border-radius: 6px;
  cursor: pointer;
  font-weight: bold;
  transition: all 0.2s;
}

.preset-btn:hover {
  background: #333;
  color: #fff;
}

.preset-btn.active {
  background: #ff3333;
  color: #fff;
  border-color: #ff3333;
  box-shadow: 0 0 15px rgba(255, 51, 51, 0.4);
}

.preset-btn.danger.active {
  background: #ff0000;
  animation: pulse-danger 1.5s infinite;
}

/* Volume Slider */
.volume-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

#volumeValue {
  font-family: 'Orbitron', sans-serif;
  color: #ff3333;
}

input[type=range] {
  width: 100%;
  height: 6px;
  background: #333;
  border-radius: 5px;
  outline: none;
  -webkit-appearance: none;
}

input[type=range]::-webkit-slider-thumb {
  -webkit-appearance: none;
  width: 20px;
  height: 20px;
  background: #ff3333;
  border-radius: 50%;
  cursor: pointer;
  box-shadow: 0 0 10px rgba(255, 51, 51, 0.5);
  margin-top: -7px;
}

input[type=range]::-webkit-slider-runnable-track {
  height: 6px;
  background: #333;
  border-radius: 5px;
}

/* Action Buttons */
.action-buttons {
  display: flex;
  gap: 15px;
  margin-top: 30px;
}

button {
  flex: 1;
  padding: 15px;
  border: none;
  border-radius: 8px;
  font-size: 1rem;
  font-weight: bold;
  cursor: pointer;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 8px;
  transition: 0.2s;
}

button svg {
  width: 20px;
  height: 20px;
}

.btn-stop {
  background: #333;
  color: #fff;
}

.btn-stop:hover:not(:disabled) {
  background: #444;
}

.btn-start {
  background: #ff3333;
  color: #fff;
  box-shadow: 0 5px 20px rgba(255, 51, 51, 0.3);
}

.btn-start:hover:not(:disabled) {
  background: #ff1a1a;
  transform: translateY(-2px);
}

button:disabled {
  opacity: 0.5;
  cursor: not-allowed;
  transform: none !important;
}

.footer-note {
  text-align: center;
  font-size: 0.7rem;
  color: #555;
  margin-top: 20px;
}

@keyframes pulse-danger {
  0% { box-shadow: 0 0 0 0 rgba(255, 0, 0, 0.7); }
  70% { box-shadow: 0 0 0 10px rgba(255, 0, 0, 0); }
  100% { box-shadow: 0 0 0 0 rgba(255, 0, 0, 0); }
}


              </style>
                        </head>
                        <body>
                            <div class="generator-container">
  <!-- Header -->
  <div class="header">
    <div class="logo-icon">
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor">
        <path d="M12 2L2 22h20L12 2zm0 3.5L18.5 20H5.5L12 5.5zM11 10v4h2v-4h-2zm0 6v2h2v-2h-2z"/>
      </svg>
    </div>
    <h1 class="title">爆音ジェネレーター</h1>
    <p class="subtitle">40 TYPES OF WARNING SOUNDS</p>
  </div>

  <div class="content">
    <!-- Sound Selector -->
    <div class="control-group">
      <label>警告音の種類 (40種類)</label>
      <div class="select-wrapper">
        <select id="soundSelect"></select>
        <span class="select-arrow">▼</span>
      </div>
    </div>

    <!-- Preset Buttons -->
    <div class="control-group">
      <label>モード選択</label>
      <div class="preset-grid">
        <button id="presetBass" class="preset-btn">低音</button>
        <button id="presetNormal" class="preset-btn active">通常</button>
        <button id="presetLoud" class="preset-btn danger">爆音</button>
      </div>
    </div>

    <!-- Volume Slider -->
    <div class="control-group">
      <div class="volume-header">
        <label>音量調整</label>
        <span id="volumeValue">75%</span>
      </div>
      <input type="range" id="volumeSlider" min="0" max="100" value="75">
    </div>

    <!-- Main Controls -->
    <div class="action-buttons">
      <button id="stopBtn" disabled class="btn-stop">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor"><path d="M6 6h12v12H6z"/></svg>
        ストップ
      </button>
      <button id="startBtn" class="btn-start">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor"><path d="M8 5v14l11-7z"/></svg>
        再生
      </button>
    </div>
    
    <div class="footer-note">
      ⚠️ 周囲の状況に配慮してご利用ください
    </div>
  </div>
</div>


              <script>
                              // 40種類の警告音データ
const sounds = [
  { name: "1. 標準警報", type: "square", freq: 800, modFreq: 10, modDepth: 200 },
  { name: "2. サイレン", type: "sine", freq: 600, modFreq: 0.5, modDepth: 400 },
  { name: "3. 救急車", type: "sawtooth", freq: 700, modFreq: 2, modDepth: 300 },
  { name: "4. 火災警報", type: "square", freq: 3000, modFreq: 4, modDepth: 0 },
  { name: "5. 核警報", type: "sine", freq: 400, modFreq: 0.1, modDepth: 100 },
  { name: "6. ピップ音", type: "sine", freq: 1000, modFreq: 3, modDepth: 0, duty: 0.1 },
  { name: "7. 低周波", type: "sawtooth", freq: 50, modFreq: 5, modDepth: 20 },
  { name: "8. 高周波", type: "square", freq: 4000, modFreq: 0, modDepth: 0 },
  { name: "9. 警察", type: "triangle", freq: 600, modFreq: 3, modDepth: 200 },
  { name: "10. 機械故障", type: "sawtooth", freq: 100, modFreq: 15, modDepth: 50 },
  { name: "11. 潜水艦", type: "sine", freq: 200, modFreq: 0.2, modDepth: 50 },
  { name: "12. ゲームオーバー", type: "square", freq: 400, modFreq: 10, modDepth: -100 },
  { name: "13. UFO", type: "sine", freq: 1000, modFreq: 8, modDepth: 500 },
  { name: "14. レーザー", type: "sawtooth", freq: 100, modFreq: 20, modDepth: 800 },
  { name: "15. 心臓モニター", type: "sine", freq: 800, modFreq: 1.2, modDepth: 0, duty: 0.05 },
  { name: "16. 工場", type: "square", freq: 500, modFreq: 0.8, modDepth: 100 },
  { name: "17. タイマー", type: "triangle", freq: 1200, modFreq: 5, modDepth: 0 },
  { name: "18. エレベーター", type: "sine", freq: 1500, modFreq: 0, modDepth: 0 },
  { name: "19. レーダー", type: "sine", freq: 2000, modFreq: 1, modDepth: 0, duty: 0.02 },
  { name: "20. 怪獣", type: "sawtooth", freq: 80, modFreq: 3, modDepth: 40 },
  { name: "21. 宇宙船", type: "sawtooth", freq: 100, modFreq: 0.5, modDepth: 20 },
  { name: "22. デジタルError", type: "square", freq: 1500, modFreq: 20, modDepth: 500 },
  { name: "23. 霧笛", type: "sawtooth", freq: 150, modFreq: 0.3, modDepth: 10 },
  { name: "24. チャイム", type: "sine", freq: 800, modFreq: 2, modDepth: 100 },
  { name: "25. ブザー", type: "sawtooth", freq: 200, modFreq: 0, modDepth: 0 },
  { name: "26. 高速回転", type: "square", freq: 200, modFreq: 30, modDepth: 100 },
  { name: "27. 下降", type: "sine", freq: 1000, modFreq: 2, modDepth: -400 },
  { name: "28. 上昇", type: "sine", freq: 200, modFreq: 2, modDepth: 400 },
  { name: "29. 鼓動", type: "sine", freq: 400, modFreq: 2, modDepth: 200 },
  { name: "30. 静電気", type: "sawtooth", freq: 1000, modFreq: 50, modDepth: 1000 },
  { name: "31. 消防車", type: "sine", freq: 820, modFreq: 2.2, modDepth: 360 },
  { name: "32. 地震警報", type: "triangle", freq: 1200, modFreq: 6, modDepth: 420 },
  { name: "33. 津波警報", type: "sawtooth", freq: 980, modFreq: 2.8, modDepth: 340 },
  { name: "34. 防災ベル", type: "square", freq: 1300, modFreq: 5, modDepth: 220 },
  { name: "35. パルス", type: "square", freq: 1200, modFreq: 7, modDepth: 380 },
  { name: "36. 連続音", type: "sine", freq: 1000, modFreq: 0, modDepth: 0 },
  { name: "37. 警告ビープ", type: "square", freq: 900, modFreq: 4, modDepth: 0, duty: 0.2 },
  { name: "38. 深海", type: "sine", freq: 100, modFreq: 0.1, modDepth: 20 },
  { name: "39. 接近警告", type: "sawtooth", freq: 600, modFreq: 10, modDepth: 100 },
  { name: "40. システムダウン", type: "square", freq: 200, modFreq: 5, modDepth: -50 }
];

const presets = {
  normal: { gainMult: 0.5, freqShift: 0, depthMult: 1.0 },
  loud: { gainMult: 1.2, freqShift: 0, depthMult: 1.5 }, // 爆音は歪みやすいためGainは控えめに、Depthで迫力を出す
  bass: { gainMult: 0.8, freqShift: -300, depthMult: 1.2 }
};

let audioCtx;
let isPlaying = false;
let activeNodes = [];
let timers = [];
let currentPreset = 'normal';

const els = {
  select: document.getElementById('soundSelect'),
  start: document.getElementById('startBtn'),
  stop: document.getElementById('stopBtn'),
  vol: document.getElementById('volumeSlider'),
  volVal: document.getElementById('volumeValue'),
  pNormal: document.getElementById('presetNormal'),
  pLoud: document.getElementById('presetLoud'),
  pBass: document.getElementById('presetBass')
};

// 初期化
sounds.forEach((s, i) => {
  const opt = document.createElement('option');
  opt.value = i;
  opt.textContent = s.name;
  els.select.appendChild(opt);
});

// プリセット切り替え
function setPreset(p) {
  currentPreset = p;
  [els.pNormal, els.pLoud, els.pBass].forEach(b => b.classList.remove('active'));
  if(p === 'normal') els.pNormal.classList.add('active');
  if(p === 'loud') els.pLoud.classList.add('active');
  if(p === 'bass') els.pBass.classList.add('active');
  if(isPlaying) playSound();
}

[els.pNormal, els.pLoud, els.pBass].forEach(btn => {
  btn.addEventListener('click', () => {
    if(btn.id === 'presetNormal') setPreset('normal');
    if(btn.id === 'presetLoud') setPreset('loud');
    if(btn.id === 'presetBass') setPreset('bass');
  });
});

els.vol.addEventListener('input', (e) => {
  els.volVal.textContent = e.target.value + '%';
});

// 音声生成ロジック
function initAudio() {
  if (!audioCtx) audioCtx = new (window.AudioContext || window.webkitAudioContext)();
  if (audioCtx.state === 'suspended') audioCtx.resume();
}

function clearAll() {
  timers.forEach(clearInterval);
  timers = [];
  activeNodes.forEach(n => {
    try {
      if(n.osc) n.osc.stop();
      if(n.lfo) n.lfo.stop();
      n.osc?.disconnect();
      n.lfo?.disconnect();
      n.gain?.disconnect();
    } catch(e){}
  });
  activeNodes = [];
}

function playSound() {
  initAudio();
  clearAll();
  isPlaying = true;
  updateUI();

  const cfg = sounds[Number(els.select.value)];
  const pre = presets[currentPreset];
  const vol = Number(els.vol.value) / 100;

  const osc = audioCtx.createOscillator();
  const gain = audioCtx.createGain();
  
  osc.type = cfg.type;
  osc.frequency.value = Math.max(20, cfg.freq + pre.freqShift);
  
  // 爆音モードでもクリッピングしないよう調整
  const baseGain = 0.4 * pre.gainMult; 
  gain.gain.value = Math.min(1.0, baseGain * vol);

  osc.connect(gain);
  gain.connect(audioCtx.destination);
  
  const now = audioCtx.currentTime;
  osc.start(now);
  activeNodes.push({ osc, gain });

  // モジュレーション（サイレン効果）
  if (cfg.modFreq > 0 && cfg.modDepth !== 0) {
    const lfo = audioCtx.createOscillator();
    const lfoGain = audioCtx.createGain();
    lfo.type = 'sine';
    lfo.frequency.value = cfg.modFreq;
    lfoGain.gain.value = Math.abs(cfg.modDepth) * pre.depthMult;
    
    lfo.connect(lfoGain);
    lfoGain.connect(osc.frequency);
    lfo.start(now);
    activeNodes.push({ lfo, gain: lfoGain });
  } 
  // パルス効果（Beepなど）
  else if (cfg.duty) {
    const interval = setInterval(() => {
      if(!isPlaying) return clearInterval(interval);
      const t = audioCtx.currentTime;
      gain.gain.setValueAtTime(Math.min(1.0, baseGain * vol), t);
      gain.gain.setValueAtTime(0, t + (1/cfg.modFreq * cfg.duty));
    }, 1000 / cfg.modFreq);
    timers.push(interval);
  }
}

function stopSound() {
  clearAll();
  isPlaying = false;
  updateUI();
}

function updateUI() {
  els.start.disabled = isPlaying;
  els.stop.disabled = !isPlaying;
  els.select.disabled = isPlaying;
  [els.pNormal, els.pLoud, els.pBass].forEach(b => b.disabled = isPlaying);
}

els.start.addEventListener('click', playSound);
els.stop.addEventListener('click', stopSound);


              </script>
                        </body>
                        </html>
                    
