<!DOCTYPE html>
<html lang="ms">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Royal Flow Scalper — XAUUSD Dashboard</title>
<style>
  :root{
    --bg:#0b0e14;
    --panel:#11151f;
    --line:#232938;
    --gold:#e8b84b;
    --teal:#3ad6a0;
    --red:#ef5350;
    --blue:#4ea1f0;
    --text:#e8e9ee;
    --muted:#8a90a3;
  }
  *{box-sizing:border-box;}
  body{
    margin:0;
    background:var(--bg);
    color:var(--text);
    font-family:-apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,sans-serif;
    padding:16px;
  }
  .wrap{max-width:480px;margin:0 auto;}
  .title{
    display:flex;justify-content:space-between;align-items:center;
    margin-bottom:14px;
  }
  .title h1{font-size:17px;font-weight:600;letter-spacing:.5px;margin:0;color:var(--gold);}
  .badge{
    font-size:11px;padding:3px 8px;border-radius:5px;
    background:rgba(58,214,160,.12);color:var(--teal);border:1px solid rgba(58,214,160,.3);
  }
  .badge.off{background:rgba(239,83,80,.12);color:var(--red);border-color:rgba(239,83,80,.3);}
  .card{
    background:var(--panel);border:1px solid var(--line);border-radius:10px;
    margin-bottom:12px;overflow:hidden;
  }
  .row{
    display:flex;justify-content:space-between;align-items:center;
    padding:11px 14px;border-bottom:1px solid var(--line);font-size:14px;
  }
  .row:last-child{border-bottom:none;}
  .row .k{color:var(--muted);}
  .row .v{font-weight:600;}
  .v.sell{color:var(--red);}
  .v.buy{color:var(--teal);}
  .v.gold{color:var(--gold);}
  .v.blue{color:var(--blue);}
  .price-big{
    text-align:center;padding:18px 14px;
  }
  .price-big .p{font-size:34px;font-weight:700;font-variant-numeric:tabular-nums;}
  .price-big .meta{font-size:12px;color:var(--muted);margin-top:4px;}
  .up{color:var(--teal);}
  .down{color:var(--red);}
  .nfp-banner{
    display:none;
    background:rgba(232,184,75,.1);
    border:1px solid rgba(232,184,75,.4);
    color:var(--gold);
    padding:10px 14px;border-radius:10px;
    font-size:13px;margin-bottom:12px;
    text-align:center;font-weight:600;
  }
  .nfp-banner.show{display:block;}
  .section-label{
    font-size:11px;color:var(--muted);letter-spacing:1px;text-transform:uppercase;
    padding:9px 14px;background:rgba(255,255,255,.02);
  }
  .footer-note{
    font-size:11px;color:var(--muted);text-align:center;margin-top:6px;line-height:1.5;
  }
  button{
    width:100%;padding:10px;border-radius:8px;border:1px solid var(--line);
    background:var(--panel);color:var(--text);font-size:13px;cursor:pointer;margin-bottom:12px;
  }
  button:active{transform:scale(.98);}
</style>
</head>
<body>
<div class="wrap">

  <div class="title">
    <h1>ROYAL FLOW SCALPER</h1>
    <span class="badge" id="connBadge">CONNECTING</span>
  </div>

  <div class="nfp-banner" id="nfpBanner"></div>

  <div class="card">
    <div class="price-big">
      <div class="p" id="priceVal">--.--</div>
      <div class="meta" id="priceMeta">Pair: XAUUSD &middot; menunggu data...</div>
    </div>
  </div>

  <button id="notifBtn">Aktifkan notifikasi NFP &amp; alert harga</button>

  <div class="card">
    <div class="section-label">Signal</div>
    <div class="row"><span class="k">Signal Type</span><span class="v" id="sigType">--</span></div>
    <div class="row"><span class="k">Market Trend</span><span class="v" id="sigTrend">--</span></div>
    <div class="row"><span class="k">Status</span><span class="v gold" id="sigStatus">ACTIVE</span></div>
  </div>

  <div class="card">
    <div class="section-label">Levels (auto-kira dari harga semasa)</div>
    <div class="row"><span class="k">Entry</span><span class="v" id="lvlEntry">--</span></div>
    <div class="row"><span class="k">SL</span><span class="v" id="lvlSL">--</span></div>
    <div class="row"><span class="k">TP1</span><span class="v" id="lvlTP1">--</span></div>
    <div class="row"><span class="k">TP2</span><span class="v" id="lvlTP2">--</span></div>
    <div class="row"><span class="k">TP3</span><span class="v" id="lvlTP3">--</span></div>
  </div>

  <div class="card">
    <div class="section-label">Multi-timeframe (M15 &middot; M30 &middot; H1 &middot; H4 &middot; Daily &middot; Weekly)</div>
    <table id="tfTable" style="width:100%;border-collapse:collapse;font-size:12.5px;">
      <thead>
        <tr style="color:var(--muted);text-align:right;">
          <th style="text-align:left;font-weight:500;padding:8px 10px;">TF</th>
          <th style="font-weight:500;padding:8px 6px;">Open</th>
          <th style="font-weight:500;padding:8px 6px;">High</th>
          <th style="font-weight:500;padding:8px 6px;">Low</th>
          <th style="font-weight:500;padding:8px 10px;">Trend</th>
        </tr>
      </thead>
      <tbody id="tfBody"></tbody>
    </table>
  </div>

  <div class="card">
    <div class="section-label">NFP / Berita Ekonomi</div>
    <div class="row"><span class="k">Next NFP (jangkaan)</span><span class="v blue" id="nfpDate">--</span></div>
    <div class="row"><span class="k">Countdown</span><span class="v" id="nfpCountdown">--</span></div>
  </div>

  <div class="footer-note">
    Harga emas live dari gold-api.com (percuma, no key). Candle M15-Weekly dibina sendiri
    dari tick harga semasa app ini dibuka (disimpan dalam browser awak) — sebab tu candle
    Daily/Weekly akan ambil masa untuk "lengkap" sehingga genap satu sesi/minggu; bukan data
    sejarah sebenar dari broker. Tarikh NFP dikira automatik (Jumaat pertama setiap bulan,
    8:30am New York) — bukan dari calendar rasmi. Signal/SL/TP contoh formula ringkas
    (ATR-style), BUKAN nasihat kewangan — sila uji dulu di akaun demo sebelum guna duit sebenar.
  </div>

</div>

<script>
const priceVal = document.getElementById('priceVal');
const priceMeta = document.getElementById('priceMeta');
const connBadge = document.getElementById('connBadge');
const sigType = document.getElementById('sigType');
const sigTrend = document.getElementById('sigTrend');
const lvlEntry = document.getElementById('lvlEntry');
const lvlSL = document.getElementById('lvlSL');
const lvlTP1 = document.getElementById('lvlTP1');
const lvlTP2 = document.getElementById('lvlTP2');
const lvlTP3 = document.getElementById('lvlTP3');
const nfpDate = document.getElementById('nfpDate');
const nfpCountdown = document.getElementById('nfpCountdown');
const nfpBanner = document.getElementById('nfpBanner');
const notifBtn = document.getElementById('notifBtn');

let priceHistory = [];
let lastPrice = null;
let notifEnabled = false;
let notifiedThisEvent = false;

const TIMEFRAMES = [
  {key:'M15', label:'M15', ms:15*60*1000},
  {key:'M30', label:'M30', ms:30*60*1000},
  {key:'H1',  label:'H1',  ms:60*60*1000},
  {key:'H4',  label:'H4',  ms:4*60*60*1000},
  {key:'D1',  label:'Daily', ms:24*60*60*1000},
  {key:'W1',  label:'Weekly', ms:7*24*60*60*1000}
];

const STORE_KEY = 'rfs_candles_v1';
let candles = {};
try{
  const saved = JSON.parse(localStorage.getItem(STORE_KEY) || '{}');
  candles = saved;
}catch(e){ candles = {}; }

function periodStart(tfMs, weekly){
  const now = Date.now();
  if(weekly){
    const d = new Date(now);
    const day = d.getUTCDay();
    const diffToMonday = (day === 0 ? 6 : day - 1);
    d.setUTCHours(0,0,0,0);
    d.setUTCDate(d.getUTCDate() - diffToMonday);
    return d.getTime();
  }
  return Math.floor(now / tfMs) * tfMs;
}

function updateCandles(price){
  TIMEFRAMES.forEach(tf=>{
    const start = periodStart(tf.ms, tf.key === 'W1');
    let c = candles[tf.key];
    if(!c || c.start !== start){
      c = { start, o:price, h:price, l:price, c:price };
      candles[tf.key] = c;
    } else {
      c.h = Math.max(c.h, price);
      c.l = Math.min(c.l, price);
      c.c = price;
    }
  });
  try{ localStorage.setItem(STORE_KEY, JSON.stringify(candles)); }catch(e){}
  renderTFTable();
}

function renderTFTable(){
  const body = document.getElementById('tfBody');
  body.innerHTML = '';
  TIMEFRAMES.forEach(tf=>{
    const c = candles[tf.key];
    const tr = document.createElement('tr');
    tr.style.borderTop = '1px solid var(--line)';
    if(!c){
      tr.innerHTML = '<td style="padding:8px 10px;">'+tf.label+'</td><td colspan="4" style="padding:8px 10px;text-align:right;color:var(--muted);">mengumpul data...</td>';
      body.appendChild(tr);
      return;
    }
    const up = c.c >= c.o;
    const trendTxt = up ? 'BULLISH' : 'BEARISH';
    const trendClass = up ? 'buy' : 'sell';
    tr.innerHTML =
      '<td style="padding:8px 10px;color:var(--text);">'+tf.label+'</td>'+
      '<td style="padding:8px 6px;text-align:right;color:var(--muted);">'+fmt(c.o)+'</td>'+
      '<td style="padding:8px 6px;text-align:right;color:var(--teal);">'+fmt(c.h)+'</td>'+
      '<td style="padding:8px 6px;text-align:right;color:var(--red);">'+fmt(c.l)+'</td>'+
      '<td style="padding:8px 10px;text-align:right;" class="v '+trendClass+'">'+trendTxt+'</td>';
    body.appendChild(tr);
  });
}
renderTFTable();

function fmt(n){ return n.toLocaleString('en-US',{minimumFractionDigits:3,maximumFractionDigits:3}); }

async function fetchPrice(){
  try{
    const res = await fetch('https://api.gold-api.com/price/XAU');
    if(!res.ok) throw new Error('bad response');
    const data = await res.json();
    const price = data.price;
    connBadge.textContent = 'LIVE';
    connBadge.classList.remove('off');
    updatePrice(price);
  }catch(e){
    connBadge.textContent = 'OFFLINE';
    connBadge.classList.add('off');
    priceMeta.textContent = 'Tak dapat capai data harga sekarang, cuba lagi...';
  }
}

function updatePrice(price){
  priceHistory.push(price);
  if(priceHistory.length > 30) priceHistory.shift();

  const dir = lastPrice === null ? '' : (price > lastPrice ? 'up' : price < lastPrice ? 'down' : '');
  priceVal.textContent = fmt(price);
  priceVal.className = 'p ' + dir;
  priceMeta.textContent = 'Pair: XAUUSD · update setiap 10s · ' + new Date().toLocaleTimeString();
  lastPrice = price;

  updateCandles(price);
  computeSignal(price);
}

function computeSignal(price){
  if(priceHistory.length < 5){
    sigType.textContent = 'MENGUMPUL DATA';
    sigType.className = 'v';
    return;
  }
  const avg = priceHistory.slice(0,-1).reduce((a,b)=>a+b,0)/(priceHistory.length-1);
  const isSell = price < avg;
  const atr = Math.max(...priceHistory) - Math.min(...priceHistory) || price*0.001;

  sigType.textContent = isSell ? 'SELL' : 'BUY';
  sigType.className = 'v ' + (isSell ? 'sell' : 'buy');

  const trendStrong = Math.abs(price-avg) > atr*0.3;
  sigTrend.textContent = isSell
    ? (trendStrong ? 'BEARISH' : 'BEARISH (lemah)')
    : (trendStrong ? 'BULLISH' : 'BULLISH (lemah)');
  sigTrend.className = 'v ' + (isSell ? 'sell' : 'buy');

  const slMult = 1.5, tp1Mult = 1.0, tp2Mult = 2.0, tp3Mult = 3.0;
  const entry = price;
  const sl = isSell ? price + atr*slMult : price - atr*slMult;
  const tp1 = isSell ? price - atr*tp1Mult : price + atr*tp1Mult;
  const tp2 = isSell ? price - atr*tp2Mult : price + atr*tp2Mult;
  const tp3 = isSell ? price - atr*tp3Mult : price + atr*tp3Mult;

  lvlEntry.textContent = fmt(entry);
  lvlSL.textContent = fmt(sl);
  lvlTP1.textContent = fmt(tp1);
  lvlTP2.textContent = fmt(tp2);
  lvlTP3.textContent = fmt(tp3);
}

function firstFridayDateOnly(y,m){
  const d = new Date(Date.UTC(y,m,1,12,0));
  let day = d.getUTCDay();
  let offset = (5 - day + 7) % 7;
  return 1 + offset;
}

function nyOffsetHours(y,m,day){
  const probe = new Date(Date.UTC(y,m,day,12,0));
  const parts = new Intl.DateTimeFormat('en-US',{
    timeZone:'America/New_York', timeZoneName:'shortOffset', hour:'2-digit'
  }).formatToParts(probe);
  const tzPart = parts.find(p=>p.type==='timeZoneName');
  const match = tzPart && tzPart.value.match(/GMT([+-]\d+)/);
  return match ? parseInt(match[1],10) : -5;
}

function getNextNFP(){
  const now = new Date();
  let year = now.getUTCFullYear();
  let month = now.getUTCMonth();

  function nfpCandidate(y,m){
    const fridayDate = firstFridayDateOnly(y,m);
    const offset = nyOffsetHours(y,m,fridayDate);
    const utcHour = 8 - offset;
    return new Date(Date.UTC(y,m,fridayDate,utcHour,30));
  }

  let candidate = nfpCandidate(year, month);
  if(candidate.getTime() < now.getTime()){
    month += 1;
    if(month > 11){ month = 0; year += 1; }
    candidate = nfpCandidate(year, month);
  }
  return candidate;
}

function updateNFP(){
  const next = getNextNFP();
  const now = new Date();
  const diffMs = next - now;
  const diffMin = Math.floor(diffMs/60000);
  const days = Math.floor(diffMin/1440);
  const hours = Math.floor((diffMin%1440)/60);
  const mins = diffMin%60;

  nfpDate.textContent = next.toLocaleString('en-US',{
    weekday:'short', month:'short', day:'numeric', hour:'2-digit', minute:'2-digit', timeZone:'America/New_York'
  }) + ' (ET)';

  nfpCountdown.textContent = days+'h ' + hours+'j ' + mins+'m';

  if(diffMin <= 60 && diffMin >= 0){
    nfpBanner.classList.add('show');
    nfpBanner.textContent = 'NFP akan release dalam ' + diffMin + ' minit — jangka volatiliti tinggi pada XAUUSD.';
    if(notifEnabled && !notifiedThisEvent){
      notifiedThisEvent = true;
      try{
        new Notification('NFP akan release dalam ' + diffMin + ' minit', {
          body: 'XAUUSD — sedia untuk volatiliti tinggi.'
        });
      }catch(e){}
    }
  } else {
    nfpBanner.classList.remove('show');
    if(diffMin > 65) notifiedThisEvent = false;
  }
}

notifBtn.addEventListener('click', async ()=>{
  if(!('Notification' in window)){
    notifBtn.textContent = 'Notifikasi browser tak disokong';
    return;
  }
  const perm = await Notification.requestPermission();
  if(perm === 'granted'){
    notifEnabled = true;
    notifBtn.textContent = 'Notifikasi NFP diaktifkan';
  } else {
    notifBtn.textContent = 'Notifikasi ditolak — boleh aktifkan dalam setting browser';
  }
});

fetchPrice();
updateNFP();
setInterval(fetchPrice, 10000);
setInterval(updateNFP, 15000);
</script>
</body>
</html>
