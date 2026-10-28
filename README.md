<!DOCTYPE html>
<html lang="uz"><head><meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Slayd Crok</title>
<style>
:root{--bg:#f4f5f7;--card:#fff;--tx:#161a22;--mu:#667085;--bd:#e1e4ea;--ac:#6d4aff;box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
@media (prefers-color-scheme:dark){:root:not([data-theme="light"]){--bg:#0f1117;--card:#181b24;--tx:#eef0f5;--mu:#98a0b3;--bd:#2a2f3c}}
:root[data-theme="dark"]{--bg:#0f1117;--card:#181b24;--tx:#eef0f5;--mu:#98a0b3;--bd:#2a2f3c}
*{box-sizing:border-box}
html{scroll-padding-top:env(safe-area-inset-top,0px)}
body{margin:0;background:var(--bg);color:var(--tx);font-family:system-ui,-apple-system,"Segoe UI",Roboto,sans-serif}
header{display:flex;align-items:center;justify-content:space-between;padding:14px 20px}
header b{font-size:18px}header b span{color:var(--ac)}
.pill{font-size:12px;color:var(--mu);border:1px solid var(--bd);border-radius:99px;padding:4px 10px;background:var(--card)}
main{display:grid;grid-template-columns:minmax(0,1fr) 340px;gap:16px;padding:0 20px 20px;max-width:1200px;margin:auto}
@media(max-width:860px){main{grid-template-columns:1fr}}
.card{background:var(--card);border:1px solid var(--bd);border-radius:14px}
.stage{position:relative;aspect-ratio:16/9;overflow:hidden;border-radius:14px;background:#000;perspective:1200px}
.slide{position:absolute;inset:0;display:flex;gap:4%;align-items:center;padding:5% 6%;color:#fff;background:linear-gradient(135deg,var(--c1),var(--c2))}
.slide .tx{flex:1;min-width:0}
.slide h1{margin:0 0 2.5%;font-size:clamp(16px,3.6vw,40px);line-height:1.1}.fact{margin-top:3%;display:inline-block;background:#ffffff26;border-radius:10px;padding:.5em .8em;font-size:clamp(9px,1.5vw,18px);line-height:1.4;animation:up .5s ease 1.6s both}
.slide ul{margin:0;padding-left:1.1em;font-size:clamp(9px,1.6vw,20px);line-height:1.45}
.slide li{opacity:0;animation:up .5s ease forwards}
.slide img{width:38%;max-height:90%;object-fit:cover;border-radius:14px;box-shadow:0 10px 30px #0006;animation:zin .6s ease both}
.num{position:absolute;right:14px;bottom:10px;font-size:12px;opacity:.7;color:#fff}
.in-fade{animation:fade .6s ease}.in-slide{animation:slide .6s cubic-bezier(.2,.8,.2,1)}
.in-zoom{animation:zoom .6s cubic-bezier(.2,.8,.2,1)}.in-flip{animation:flip .7s ease;transform-origin:center}
@keyframes fade{from{opacity:0}}@keyframes slide{from{transform:translateX(100%)}}
@keyframes zoom{from{transform:scale(.6);opacity:0}}@keyframes flip{from{transform:rotateY(90deg);opacity:0}}
@keyframes up{from{opacity:0;transform:translateY(14px)}to{opacity:1;transform:none}}
@keyframes zin{from{opacity:0;transform:scale(.85)}}
.bar{display:flex;gap:8px;flex-wrap:wrap;align-items:center;padding:10px}
button,select{font:inherit;font-size:13px;color:var(--tx);background:var(--bg);border:1px solid var(--bd);border-radius:9px;padding:7px 11px;cursor:pointer}
button.p{background:var(--ac);border-color:var(--ac);color:#fff}
.thumbs{display:flex;gap:8px;overflow-x:auto;padding:0 10px 12px}
.th{flex:0 0 96px;aspect-ratio:16/9;border-radius:8px;border:2px solid transparent;color:#fff;font-size:10px;padding:5px;overflow:hidden;cursor:pointer;background:linear-gradient(135deg,var(--c1),var(--c2))}
.th.on{border-color:var(--ac)}
.chat{display:flex;flex-direction:column;height:100%;min-height:360px}
.msgs{flex:1;overflow-y:auto;padding:12px;display:flex;flex-direction:column;gap:8px;max-height:430px}
.m{padding:8px 11px;border-radius:12px;font-size:13.5px;line-height:1.45;max-width:90%}
.u{align-self:flex-end;background:var(--ac);color:#fff}.b{background:var(--bg);border:1px solid var(--bd)}
.in{display:flex;gap:6px;padding:10px;border-top:1px solid var(--bd)}
.in input{flex:1;min-width:0;font:inherit;font-size:14px;padding:9px 11px;border-radius:9px;border:1px solid var(--bd);background:var(--bg);color:var(--tx)}
.hint{font-size:12px;color:var(--mu);padding:0 12px 10px}
.ov{position:fixed;inset:0;background:#000b;display:flex;align-items:center;justify-content:center;z-index:50;padding:16px}
.box{background:var(--card);color:var(--tx);border:1px solid var(--bd);border-radius:16px;padding:24px;max-width:380px;width:100%;text-align:center;max-height:92vh;overflow:auto}.box.wide{max-width:660px}
.plans{display:grid;grid-template-columns:1fr 1fr;gap:12px;text-align:left;margin:14px 0}@media(max-width:600px){.plans{grid-template-columns:1fr}}
.pc{border:1px solid var(--bd);border-radius:12px;padding:14px;font-size:13px}.pp{border-color:var(--ac);box-shadow:0 0 0 2px var(--ac) inset}
.pr{font-size:20px;font-weight:700;margin:6px 0}.pc ul{padding-left:18px;line-height:1.7;margin:8px 0}
.g{width:100%;padding:12px;font-size:15px;background:#fff;color:#222;border:1px solid #ccc}
.acc{display:flex;gap:10px;align-items:center;padding:10px;border:1px solid var(--bd);border-radius:10px;margin:8px 0;cursor:pointer;text-align:left;font-size:13px}
.av{width:34px;height:34px;border-radius:50%;background:var(--ac);color:#fff;display:flex;align-items:center;justify-content:center;font-weight:700;flex:none}
.s{font-size:12px;color:var(--mu)}h2 span{color:var(--ac)}
.wm{position:absolute;left:14px;bottom:10px;display:flex;align-items:center;gap:5px;font-size:clamp(9px,1.4vw,14px);font-weight:600;color:#fff;background:#00000040;padding:3px 9px 3px 5px;border-radius:99px;opacity:.9;letter-spacing:.2px;pointer-events:none}.wm svg{width:1.5em;height:1.5em}
.kp{display:grid;grid-template-columns:repeat(4,1fr);gap:10px;margin:14px 0}@media(max-width:600px){.kp{grid-template-columns:1fr 1fr}}
.k{border:1px solid var(--bd);border-radius:12px;padding:10px;background:var(--bg)}.k span{display:block;font-size:11px;color:var(--mu)}.k b{font-size:18px}
.bars{display:flex;align-items:flex-end;gap:8px;height:90px;margin-bottom:10px}.bars div{flex:1;background:linear-gradient(var(--ac),#06b6d4);border-radius:6px 6px 0 0}
#adm table{width:100%;border-collapse:collapse;font-size:13px}#adm td,#adm th{padding:6px 8px;border-bottom:1px solid var(--bd);text-align:left}
.set{display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-bottom:10px}.set label{font-size:12px;color:var(--mu);display:flex;flex-direction:column;gap:4px}.set input{font:inherit;padding:8px;border-radius:8px;border:1px solid var(--bd);background:var(--bg);color:var(--tx)}
</style></head>
<body>
<svg width="0" height="0" style="position:absolute"><symbol id="logo" viewBox="0 0 40 40"><defs><linearGradient id="lg" x1="0" y1="0" x2="1" y2="1"><stop offset="0" stop-color="#7c3aed"/><stop offset="1" stop-color="#06b6d4"/></linearGradient></defs><rect width="40" height="40" rx="10" fill="url(#lg)"/><rect x="8" y="9" width="24" height="17" rx="3" fill="#fff"/><path d="M17 13.5v8l7-4z" fill="#7c3aed"/><rect x="12" y="30" width="16" height="3" rx="1.5" fill="#fff" opacity=".75"/></symbol></svg>
<header><b style="display:flex;align-items:center;gap:8px"><svg width="32" height="32"><use href="#logo"/></svg><span style="color:inherit">Slayd&nbsp;<span style="color:var(--ac)">Crok</span></span></b><span style="display:flex;gap:8px;align-items:center"><span class="pill" id="plan"></span><button id="openadm" style="display:none">🛠 Kabinet</button><button class="p" id="openpro">⭐ Pro</button><button id="out" style="display:none">Chiqish</button></span></header>
<div id="login" class="ov"><div class="box"><svg width="64" height="64"><use href="#logo"/></svg><h2>Slayd <span>Crok</span></h2><p class="s" style="font-size:14px">Mavzuni yozing — slaydlar soniyalarda tayyor.</p><div id="l1"><button class="g" id="gbtn">Google bilan davom etish</button><p class="s" id="lerr">Google akkauntingiz bilan kiring, parol soʻralmaydi.</p></div></div></div>
<div id="adm" class="ov" style="display:none"><div class="box wide" style="text-align:left"><div style="display:flex;align-items:center;gap:10px"><svg width="40" height="40"><use href="#logo"/></svg><div><h2 style="margin:0">Slayd <span>Crok</span> · Kabinet</h2><span class="s">Sayt egasi: <b>Siz</b> · faqat siz koʻra olasiz (demo)</span></div></div><div class="kp"><div class="k"><span>Foydalanuvchilar</span><b>1 248</b></div><div class="k"><span>Pro obunachilar</span><b>86</b></div><div class="k"><span>Bugungi taqdimotlar</span><b>412</b></div><div class="k"><span>Oylik daromad (soʻm)</span><b id="krev"></b></div></div><p class="s">Oxirgi 7 kun: yaratilgan taqdimotlar</p><div class="bars" id="bars"></div><h3>Oxirgi foydalanuvchilar</h3><table><tr><th>Ism</th><th>Tarif</th><th>Bugun</th></tr><tr><td>Ali K.</td><td>⭐ Pro</td><td>7 ta</td></tr><tr><td>Dilnoza S.</td><td>Tekin</td><td>3 ta</td></tr><tr><td>Jasur M.</td><td>Tekin</td><td>1 ta</td></tr><tr><td>Madina R.</td><td>⭐ Pro</td><td>12 ta</td></tr></table><h3>Sozlamalar</h3><div class="set"><label>Pro narxi (soʻm/oy)<input type="number" id="sprice" value="30000"></label><label>Tekin limit (kuniga)<input type="number" id="slim" value="3"></label></div><p class="s">Bu demo maʻlumotlar. Haqiqiy saytda raqamlar Firebase’dan keladi.</p><button id="acl">Yopish</button></div></div>
<div id="pro" class="ov" style="display:none"><div class="box wide"><h2>Slayd <span>Crok</span> Pro</h2><div class="plans"><div class="pc"><h3>Tekin</h3><div class="pr">0 soʻm</div><ul><li>Kuniga 3 ta taqdimot</li><li>20 varoqgacha</li><li>Kichik “Slayd Crok” belgisi</li><li>Qoʻlda tahrirlash va fon</li></ul></div><div class="pc pp"><h3>⭐ Pro</h3><div class="pr">30 000 soʻm/oy</div><ul><li>Kuniga 20 ta taqdimot</li><li>40 varoqgacha</li><li>Belgisiz yuklab olish</li><li>Premium fon va shablonlar</li><li>Birinchi navbat</li></ul><button class="p" id="pay1">Payme orqali (tez orada)</button> <button id="pay2">Click orqali (tez orada)</button></div></div><button id="cl">Yopish</button></div></div>
<main>
<section>
<div class="stage" id="stage"></div>
<div class="card" style="margin-top:12px">
<div class="bar">
<button id="prev">◀</button><button id="next">▶</button>
<select id="tr"><option value="fade">Oʻtish: fade</option><option value="slide">Oʻtish: slide</option><option value="zoom">Oʻtish: zoom</option><option value="flip">Oʻtish: flip</option></select>
<label class="pill" style="cursor:pointer">🖼 Rasm qoʻshish<input type="file" id="file" accept="image/*" hidden></label>
<button class="p" id="full">▶ Taqdimot</button>
</div>
<div class="thumbs" id="thumbs"></div>
</div>
</section>
<aside class="card chat">
<div class="msgs" id="msgs"></div>
<div class="hint">Masalan: <i>“Sunʼiy intellekt haqida 10 ta slayd qil”</i>, <i>“sarlavhani Mening loyiham qil”</i>, <i>“oʻtish zoom”</i>, <i>“rang yashil”</i>, <i>“slayd qoʻsh”</i></div>
<div class="in"><input id="q" placeholder="Buyruq yozing…"><button class="p" id="send">Yuborish</button></div>
</aside>
</main>
<script>
const COL={ko:['#1d4ed8','#6d28d9'],qizil:['#be123c','#f97316'],yashil:['#047857','#0e7490'],binafsha:['#6d28d9','#db2777'],qora:['#111827','#374151'],sariq:['#b45309','#ca8a04']};
let S0=[
{t:"Quyosh tizimi",b:["Bizning kosmik uyimiz","8 ta sayyora, 1 ta yulduz","Taxminan 4,6 mlrd yoshda"]},
{t:"Quyosh",b:["Tizimning 99,8% massasi","Yuzasi harorati ≈ 5500 °C","Vodorod geliyga aylanadi"]},
{t:"Merkuriy",b:["Quyoshga eng yaqin sayyora","Yili atigi 88 kun","Atmosferasi deyarli yoʻq"]},
{t:"Venera",b:["Eng issiq sayyora (≈ 465 °C)","Qalin karbonat angidrid qatlami","Teskari yoʻnalishda aylanadi"]},
{t:"Yer",b:["Hayot mavjud yagona sayyora","Yuzasining ≈ 71% suv","Bitta tabiiy yoʻldosh: Oy"]},
{t:"Mars",b:["Qizil sayyora","Quyosh tizimidagi eng baland togʻ: Olimp","Ikki yoʻldosh: Fobos va Deymos"]},
{t:"Yupiter",b:["Eng katta sayyora","Katta Qizil Dogʻ — ulkan boʻron","90 dan ortiq yoʻldoshi bor"]},
{t:"Saturn",b:["Mashhur halqalari","Zichligi suvdan kam","Titan — qalin atmosferali yoʻldosh"]},
{t:"Uran va Neptun",b:["Muz gigantlari","Uran yon tomoni bilan aylanadi","Neptunda eng kuchli shamollar"]},
{t:"Xulosa",b:["Har bir sayyora oʻziga xos","Kosmosni oʻrganish davom etmoqda","Savollaringiz bormi?"]}];
let i=0,tr='fade',pal=COL.ko,imgs={};
const ST=Array.from({length:45},(_,k)=>'<circle cx="'+(k*97%400)+'" cy="'+((k*53+k*k*7)%300)+'" r="'+(k%5?0.8:1.5)+'" fill="#fff" opacity=".7"/>').join('');
const svg=x=>'data:image/svg+xml;utf8,'+encodeURIComponent('<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 400 300"><rect width="400" height="300" fill="#0b1026"/>'+ST+x+'</svg>');
const pl=(a,b,r,x=200,y=150,id='g')=>'<defs><radialGradient id="'+id+'" cx=".35" cy=".35"><stop offset="0" stop-color="'+a+'"/><stop offset="1" stop-color="'+b+'"/></radialGradient></defs><circle cx="'+x+'" cy="'+y+'" r="'+r+'" fill="url(#'+id+')"/>';
const dots=(a,c,r,o)=>a.map(([x,y,rr,f])=>'<circle cx="'+x+'" cy="'+y+'" r="'+rr+'" fill="'+f+'" opacity="'+o+'"/>').join('');
const RING=(front)=>'<g transform="rotate(-20 200 150)"><'+(front?'path d="M50 150 A150 38 0 0 0 350 150"':'ellipse cx="200" cy="150" rx="150" ry="38"')+' fill="none" stroke="#e7d3a0" stroke-width="14" opacity=".85"/></g>';
const bands=(cols)=>'<defs><clipPath id="c"><circle cx="200" cy="150" r="85"/></clipPath></defs><g clip-path="url(#c)" opacity=".6">'+cols.map((c,k)=>'<rect x="100" y="'+(70+k*22)+'" width="200" height="14" fill="'+c+'"/>').join('')+'</g>';
const orb=()=>{let o='';[55,90,130,170,225,285].forEach(r=>o+='<circle cx="50" cy="150" r="'+r+'" fill="none" stroke="#fff" opacity=".2"/>');const P=[[55,25,4,'#9ca3af'],[90,-20,6,'#fcd34d'],[130,15,7,'#3b82f6'],[170,-25,6,'#ef4444'],[225,12,13,'#d6a56b'],[285,-12,11,'#e7d3a0']];P.forEach(([r,a,s,f])=>{a=a*Math.PI/180;o+='<circle cx="'+(50+r*Math.cos(a))+'" cy="'+(150+r*Math.sin(a))+'" r="'+s+'" fill="'+f+'"/>'});return pl('#fde68a','#f97316',34,50,150,'s')+o};
const emo=(e,c='#6d28d9')=>'data:image/svg+xml;utf8,'+encodeURIComponent('<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 400 300"><defs><linearGradient id="l" x1="0" y1="0" x2="1" y2="1"><stop offset="0" stop-color="'+c+'"/><stop offset="1" stop-color="#0ea5e9"/></linearGradient></defs><rect width="400" height="300" rx="20" fill="url(#l)"/><circle cx="60" cy="50" r="90" fill="#fff" opacity=".08"/><circle cx="360" cy="270" r="110" fill="#fff" opacity=".08"/><text x="200" y="195" font-size="140" text-anchor="middle">'+e+'</text></svg>');
const EM={'Kirish':'👋','Tarixi':'📜','Asosiy tushunchalar':'🧩','Turlari':'🗂️','Afzalliklari':'✅','Muammolari':'⚠️','Amaliy misollar':'🛠️','Statistika':'📊','Kelajagi':'🚀'};
function te(t){t=t.toLowerCase().replace(/[‘’ʻ`´ʼ]/g,"'");const m=[[/sun'iy|intellekt|robot|\bai\b/,'🤖'],[/kosmos|sayyora|quyosh|yulduz/,'🪐'],[/tarix|urush/,'📜'],[/sog'liq|tibbiyot|salomat/,'🩺'],[/iqlim|ekologiya|tabiat|suv/,'🌍'],[/dasturlash|kompyuter|internet|texnolog/,'💻'],[/iqtisod|biznes|pul|bank/,'💼'],[/ta'lim|talim|maktab|universitet/,'🎓'],[/sport|futbol/,'⚽']];for(const [r,e] of m)if(r.test(t))return e;return '💡'}
let S=[
{t:"Quyosh tizimi",img:svg(orb()),f:"Quyosh nuri Yergacha taxminan 8 daqiqa 20 soniyada yetib keladi.",b:["Bizning kosmik uyimiz","8 ta sayyora va 1 ta yulduz — Quyosh","Yoshi taxminan 4,6 mlrd yil","Tosh sayyoralar: Merkuriy, Venera, Yer, Mars","Gigantlar: Yupiter, Saturn, Uran, Neptun"]},
{t:"Quyosh",img:svg('<circle cx="200" cy="150" r="125" fill="#f59e0b" opacity=".14"/><circle cx="200" cy="150" r="100" fill="#f59e0b" opacity=".25"/>'+pl('#fef08a','#ea580c',75)),f:"Quyoshning ichiga taxminan 1,3 million Yer sigʻadi.",b:["Tizim massasining 99,8% i shu yerda","Diametri ≈ 1,39 mln km (Yernikidan 109 marta katta)","Yuzasi harorati ≈ 5500 °C, yadrosida ≈ 15 mln °C","Vodorod yadro reaksiyasida geliyga aylanadi","Yer uchun yorugʻlik va issiqlik manbai"]},
{t:"Merkuriy",img:svg(pl('#e5e7eb','#6b7280',72)+dots([[170,120,10,'#6b7280'],[225,160,14,'#6b7280'],[190,190,7,'#6b7280'],[235,115,6,'#6b7280']],0,0,.55)),f:"Bir Quyosh kuni Yer hisobida ≈ 176 sutkaga teng.",b:["Quyoshga eng yaqin sayyora","Diametri ≈ 4879 km — eng kichigi","Yili atigi 88 Yer kuni","Kunduz ≈ +430 °C, tunda ≈ −180 °C","Yoʻldoshi va deyarli atmosferasi yoʻq"]},
{t:"Venera",img:svg(pl('#fde68a','#b45309',80)+'<ellipse cx="200" cy="125" rx="70" ry="9" fill="#fff" opacity=".25"/><ellipse cx="205" cy="160" rx="72" ry="10" fill="#fff" opacity=".2"/><ellipse cx="195" cy="195" rx="55" ry="8" fill="#fff" opacity=".2"/>'),f:"Veneraning kuni (243 sutka) uning yilidan (225 sutka) uzunroq.",b:["Yerning “egizagi” — oʻlchami yaqin","Eng issiq sayyora: ≈ 465 °C","Atmosfera bosimi Yerdagidan ≈ 92 marta katta","Qalin karbonat angidrid va oltingugurt bulutlari","Boshqalarga teskari yoʻnalishda aylanadi"]},
{t:"Yer",img:svg(pl('#60a5fa','#1e3a8a',82)+'<ellipse cx="170" cy="125" rx="30" ry="20" fill="#22c55e"/><ellipse cx="225" cy="175" rx="26" ry="32" fill="#22c55e"/><ellipse cx="205" cy="108" rx="20" ry="9" fill="#16a34a"/>'+pl('#f3f4f6','#9ca3af',17,325,70,'m')),f:"Yer Quyosh atrofida ≈ 30 km/s tezlik bilan harakatlanadi.",b:["Hayot mavjud yagona maʼlum sayyora","Quyoshdan ≈ 149,6 mln km uzoqlikda","Yuzasining ≈ 71% i suv bilan qoplangan","Oʻz oʻqi atrofida 24 soatda aylanadi, yili 365,25 kun","Tabiiy yoʻldoshi — Oy (≈ 384 400 km)"]},
{t:"Mars",img:svg(pl('#fdba74','#9a3412',65)+dots([[180,130,12,'#7c2d12'],[225,165,16,'#7c2d12'],[190,180,8,'#7c2d12']],0,0,.4)+'<ellipse cx="200" cy="92" rx="22" ry="6" fill="#fff" opacity=".75"/>'+pl('#d1d5db','#6b7280',8,320,90,'p')+pl('#d1d5db','#6b7280',5,85,210,'q')),f:"Marsdagi Olimp togʻi ≈ 22 km — Everestdan deyarli 2,5 marta baland.",b:["“Qizil sayyora” — tuprogʻida temir oksidi","Kun ≈ 24 soat 37 daqiqa, yil ≈ 687 sutka","Oʻrtacha harorat ≈ −60 °C","Yupqa atmosfera, asosan karbonat angidrid","Ikki yoʻldoshi bor: Fobos va Deymos"]},
{t:"Yupiter",img:svg(pl('#f3d9a8','#7c4a1f',85)+bands(['#a8703d','#e8c48a','#8b5a2b','#d9a066','#9c6b3c','#e8c48a','#8b5a2b'])+'<ellipse cx="235" cy="182" rx="20" ry="11" fill="#b91c1c" opacity=".85"/>'),f:"Yupiter massasi qolgan barcha sayyoralar yigʻindisidan ≈ 2,5 marta katta.",b:["Eng katta sayyora, diametri ≈ 140 000 km","Asosan vodorod va geliydan iborat gaz giganti","Katta Qizil Dogʻ — 300 yildan ortiq davom etayotgan boʻron","Kuni atigi ≈ 10 soat — eng tez aylanuvchi","90 dan ortiq yoʻldoshi bor (Io, Yevropa, Ganimed, Kallisto)"]},
{t:"Saturn",img:svg(RING(0)+pl('#f5e3b0','#a07a3c',62)+RING(1)),f:"Saturn zichligi suvnikidan kam: uni ulkan suvga solsa, suzib yurardi.",b:["Eng mashhur halqalar tizimi","Halqalar muz va tosh boʻlaklaridan iborat","Kengligi ≈ 280 000 km, qalinligi esa juda yupqa","140 dan ortiq yoʻldoshi bor","Titan — Yerdan qalinroq atmosferali yoʻldosh"]},
{t:"Uran va Neptun",img:svg(pl('#a5f3fc','#0e7490',52,115,150,'a')+'<ellipse cx="115" cy="150" rx="8" ry="75" fill="none" stroke="#cffafe" opacity=".5"/>'+pl('#93c5fd','#1d4ed8',50,285,150,'b')),f:"Neptun 1846-yilda avval hisob-kitob bilan “topilgan”, keyin teleskopda koʻrilgan.",b:["Ikkalasi ham muz gigantlari","Uran oʻqi ≈ 98° ogʻgan — “yonboshlab” aylanadi","Uran yili ≈ 84, Neptun yili ≈ 165 Yer yili","Neptunda shamol tezligi 2000 km/soatgacha yetadi","Triton (Neptun yoʻldoshi) teskari orbitada aylanadi"]},
{t:"Xulosa",img:svg(orb()+pl('#60a5fa','#1e3a8a',12,330,90,'e')),f:"Voyager-1 zondi 1977-yilda uchirilgan va hozir yulduzlararo fazoda.",b:["4 ta tosh va 4 ta gigant sayyora","Har birining oʻz iqlimi, yoʻldoshlari va sirlari","Pluton 2006-yildan mitti sayyora hisoblanadi","Yerdan tashqari hayot izlash davom etmoqda","Savollaringiz bormi?"]}];
const $=id=>document.getElementById(id);
function cols(el){el.style.setProperty('--c1',pal[0]);el.style.setProperty('--c2',pal[1])}
function render(anim=true){
 const s=S[i],st=$('stage');
 st.innerHTML='';const d=document.createElement('div');d.className='slide'+(anim?' in-'+tr:'');cols(d);
 const tx=document.createElement('div');tx.className='tx';
 const h=document.createElement('h1');h.textContent=s.t;tx.appendChild(h);
 const ul=document.createElement('ul');
 s.b.forEach((x,k)=>{const li=document.createElement('li');li.textContent=x;li.style.animationDelay=(.3+k*.25)+'s';ul.appendChild(li)});
 tx.appendChild(ul);if(s.f){const f=document.createElement('div');f.className='fact';f.textContent='💡 '+s.f;tx.appendChild(f)}d.appendChild(tx);
 if(s.img){const im=document.createElement('img');im.src=s.img;d.appendChild(im)}
 const n=document.createElement('div');n.className='num';n.textContent=(i+1)+' / '+S.length;d.appendChild(n);
 st.appendChild(d);
 const th=$('thumbs');th.innerHTML='';
 S.forEach((x,k)=>{const e=document.createElement('div');e.className='th'+(k==i?' on':'');cols(e);e.textContent=(k+1)+'. '+x.t;e.onclick=()=>{i=k;render()};th.appendChild(e)});
}
function go(k){i=Math.max(0,Math.min(S.length-1,k));render()}
$('prev').onclick=()=>go(i-1);$('next').onclick=()=>go(i+1);
$('tr').onchange=e=>{tr=e.target.value;render()};
$('full').onclick=()=>$('stage').requestFullscreen&&$('stage').requestFullscreen();
document.addEventListener('keydown',e=>{if(e.target.id==='q')return;if(e.key==='ArrowRight')go(i+1);if(e.key==='ArrowLeft')go(i-1)});
$('file').onchange=e=>{const f=e.target.files[0];if(!f)return;const r=new FileReader();r.onload=()=>{S[i].img=r.result;render();say('Rasm '+(i+1)+'-slaydga qoʻshildi.')};r.readAsDataURL(f)};
function msg(t,c){const m=document.createElement('div');m.className='m '+c;m.textContent=t;$('msgs').appendChild(m);$('msgs').scrollTop=1e9}
function say(t){msg(t,'b')}
function gen(topic,n){
 const T=topic.charAt(0).toUpperCase()+topic.slice(1);
 const base=[["Kirish","Mavzu bilan tanishuv","Nima uchun muhim?","Asosiy savollar"],["Tarixi","Paydo boʻlishi","Muhim bosqichlar","Hozirgi holat"],["Asosiy tushunchalar","Asosiy atamalar","Qanday ishlaydi","Misollar"],["Turlari","Asosiy turlari","Farqlari","Qoʻllanilish sohalari"],["Afzalliklari","Samaradorlik","Qulaylik","Tejamkorlik"],["Muammolari","Mavjud cheklovlar","Xavflar","Yechim yoʻllari"],["Amaliy misollar","Real hayotdagi holat","Muvaffaqiyatli tajriba","Xulosalar"],["Statistika","Asosiy raqamlar","Oʻsish tendensiyasi","Prognoz"],["Kelajagi","Yangi imkoniyatlar","Rivojlanish yoʻnalishlari","Bizni nima kutmoqda"]];
 const out=[{t:T,img:emo(te(topic),'#7c3aed'),f:'Maslahat: har slaydga bitta aniq misol qoʻshing.',b:["Taqdimot mavzusi","Muallif: siz","Sana: "+new Date().toLocaleDateString('uz'),"Reja: kirish, asosiy qism, xulosa"]}];
 for(let k=0;k<n-2;k++){const x=base[k%base.length];out.push({t:x[0],img:emo(EM[x[0]]||'💡',k%2?'#0891b2':'#7c3aed'),f:'Maslahat: bu slaydga oʻz maʼlumot va raqamlaringizni qoʻshing.',b:x.slice(1).concat(['Misol: '+T+' bilan bogʻliq real holat','Savol: auditoriya buni qanday baholaydi?'])})}
 out.push({t:"Xulosa",img:emo('🎯','#be123c'),f:'Yaxshi taqdimot — qisqa, aniq va koʻrgazmali.',b:[T+" haqida asosiy fikrlar","Keyingi qadamlar","Eʼtiboringiz uchun rahmat!"]});
 return out.slice(0,Math.max(n,2));
}
function cmd(raw){
 const q=raw.toLowerCase().replace(/[‘’ʻ`´ʼ]/g,"'").trim();let m;
 if(m=q.match(/^(.+?)\s+haqida(?:\s+(\d+)\s*(?:ta|varoq\w*|slayd\w*))?/)){
  const n=+(m[2]||(q.match(/(\d+)\s*(?:ta|varoq|slayd)/)||[])[1]||10);
  const topic=raw.trim().slice(0,m[1].length);
  S=gen(topic,Math.min(Math.max(n,2),20));i=0;render();return say(S.length+" ta slayd tayyor: “"+topic+"”. Endi tahrirlashingiz mumkin. (Bu namunada matn shablon; haqiqiy AI ulanganda kontent oʻzi yoziladi.)")}
 if(m=raw.trim().match(/(?:ism|sarlavha|nom)\w*\s+(.+?)\s+(?:qil|deb\s+o.zgartir\w*|ga\s+o.zgartir\w*)$/i)){
  S[i].t=m[1];render(false);return say(i+1+"-slayd sarlavhasi oʻzgardi: “"+m[1]+"”.")}
 if(m=q.match(/o'tish\w*\s*:?\s*(fade|slide|zoom|flip)/)){tr=m[1];$('tr').value=tr;render();return say("Oʻtish effekti: "+tr)}
 if(m=q.match(/rang\w*\s*:?\s*(ko'k|qizil|yashil|binafsha|qora|sariq)/)){const k=m[1].replace("'",'').replace('kok','ko');pal=COL[k]||COL.ko;render(false);return say("Rang oʻzgardi: "+m[1])}
 if(/slayd\s+qo'sh/.test(q)){S.splice(i+1,0,{t:"Yangi slayd",b:["Matn yozing","Fikrni qoʻshing"]});go(i+1);return say("Yangi slayd qoʻshildi.")}
 if(/(o'chir)/.test(q)&&S.length>1){S.splice(i,1);go(Math.min(i,S.length-1));return say("Slayd oʻchirildi.")}
 if(/keyingi/.test(q))return go(i+1);if(/oldingi/.test(q))return go(i-1);
 say("Tushunmadim. Sinab koʻring: “… haqida 10 ta slayd qil”, “sarlavhani … qil”, “oʻtish zoom”, “rang qizil”, “slayd qoʻsh”.");
}
function send(){const v=$('q').value.trim();if(!v)return;msg(v,'u');$('q').value='';cmd(v)}
$('send').onclick=send;$('q').onkeydown=e=>{if(e.key==='Enter')send()};
say("Salom! 10 varoqli namuna tayyor (Quyosh tizimi). Mavzu yozing, masalan: “Sunʼiy intellekt haqida 10 ta slayd qil”, yoki sarlavhani oʻzgartiring.");
render();
</script>
<script>
(function(){
const $=id=>document.getElementById(id);
let plan='free',used=0;const LIM={free:3,pro:20};
function upd(){const p=$('plan');p.textContent=plan==='pro'?'⭐ Pro · '+used+'/'+LIM.pro:'Tekin · '+used+'/'+LIM.free+' bugun';p.style.background=plan==='pro'?'var(--ac)':'';p.style.color=plan==='pro'?'#fff':''}
function openPro(){$('pro').style.display='flex'}
$('openpro').onclick=openPro;$('cl').onclick=()=>$('pro').style.display='none';
$('pro').onclick=e=>{if(e.target.id==='pro')$('pro').style.display='none'};
['pay1','pay2'].forEach(id=>$(id).onclick=()=>{$('pro').style.display='none';say('Toʻlov tizimi hali ulanmagan. Pro olish uchun sayt egasi bilan bogʻlaning.')});
document.addEventListener('keydown',e=>{if(e.target.isContentEditable)e.stopImmediatePropagation()},true);
const _r=render;
render=function(a){_r(a);const s=S[i],sl=document.querySelector('.slide');if(s.bg)sl.style.background=s.bg;
const wm=document.createElement('div');wm.className='wm';wm.innerHTML='<svg><use href="#logo"/></svg>Slayd Crok';sl.appendChild(wm);
const h=sl.querySelector('h1');h.contentEditable=true;h.spellcheck=false;h.oninput=()=>{s.t=h.textContent};h.onkeydown=e=>{if(e.key==='Enter')e.preventDefault()};
sl.querySelectorAll('li').forEach((li,k)=>{li.contentEditable=true;li.spellcheck=false;li.oninput=()=>{s.b[k]=li.textContent};li.onkeydown=e=>{if(e.key==='Enter')e.preventDefault()}})};
function setBg(v){if($('all').checked)S.forEach(s=>s.bg=v);else S[i].bg=v;render(false)}
const p=document.createElement('div');p.className='bar';p.style.borderTop='1px solid var(--bd)';p.innerHTML='<span class="pill">🎨 Fon</span>';
[['#1d4ed8','#6d28d9'],['#be123c','#f97316'],['#047857','#0e7490'],['#111827','#374151'],['#b45309','#ca8a04'],['#db2777','#7c3aed']].forEach(c=>{const g='linear-gradient(135deg,'+c[0]+','+c[1]+')';const b=document.createElement('button');b.style.cssText='width:30px;height:30px;padding:0;border-radius:50%;background:'+g;b.onclick=()=>setBg(g);p.appendChild(b)});
const lb=document.createElement('label');lb.className='pill';lb.style.cursor='pointer';lb.innerHTML='🖼 Oʻz rasmim<input type="file" accept="image/*" hidden>';
lb.querySelector('input').onchange=e=>{const f=e.target.files[0];if(!f)return;const r=new FileReader();r.onload=()=>setBg('linear-gradient(#0007,#0007),url("'+r.result+'") center/cover');r.readAsDataURL(f)};
const al=document.createElement('label');al.className='pill';al.innerHTML='<input type="checkbox" id="all"> Hamma slaydga';
const cp=document.createElement('label');cp.className='pill';cp.style.cursor='pointer';cp.innerHTML='🎨 Istalgan rang <input type="color" value="#1d4ed8" style="width:26px;height:22px;border:0;padding:0;vertical-align:middle;background:none">';cp.querySelector('input').oninput=e=>{const c=e.target.value;setBg('linear-gradient(135deg,'+c+','+c+'cc)')};
p.appendChild(cp);p.appendChild(lb);p.appendChild(al);const card=document.querySelector('main section .card');card.insertBefore(p,$('thumbs'));
const _c=cmd;
const API='https://slayd-api.gulshankucharova441-8d1.workers.dev';
window.setUsage=function(p,u,l){plan=p==='pro'?'pro':'free';used=u;if(l)LIM[plan]=l;upd()};
let busy=false;
async function aiGen(raw){
 if(busy)return say('Oldingi soʻrov hali bajarilmoqda, biroz kuting…');
 const q=raw.toLowerCase().replace(/[‘’ʻ`´ʼ]/g,"'").trim();
 const m=q.match(/^(.+?)\s+haqida/);
 const topic=m?raw.trim().slice(0,m[1].length):raw.trim();
 const n=+((q.match(/(\d+)\s*(?:ta|varoq|slayd)/)||[])[1]||10);
 const tok=window.getToken&&await window.getToken();
 if(!tok){$('login').style.display='flex';return say('Avval Google bilan kiring.')}
 busy=true;say('⏳ “'+topic+'” boʻyicha slaydlar yozilmoqda…');
 try{
  const r=await fetch(API+'/generate',{method:'POST',headers:{'Content-Type':'application/json','Authorization':'Bearer '+tok},body:JSON.stringify({topic:topic,n:n})});
  const d=await r.json().catch(()=>({}));
  if(r.status===429){window.setUsage(d.plan,d.used,d.limit);say('Bugungi limit tugadi ('+d.limit+' ta taqdimot). Pro bilan kuniga koʻproq yaratishingiz mumkin.');openPro();return}
  if(!r.ok)return say(d.error||'Xatolik yuz berdi. Qayta urinib koʻring.');
  S=d.slides.map((s,k)=>({t:s.title,b:s.bullets,f:s.fact,img:emo(s.emoji||'💡',k%2?'#0891b2':'#7c3aed')}));
  i=0;render();window.setUsage(d.plan,d.used,d.limit);
  say(S.length+' ta slayd tayyor: “'+topic+'”. Matn ustiga bosib tahrirlashingiz mumkin.');
 }catch(e){say('Internet yoki server bilan muammo. Qayta urinib koʻring.')}
 finally{busy=false}
}
cmd=function(raw){if(/haqida/i.test(raw)){aiGen(raw);return}_c(raw)};
const nf=n=>n.toString().replace(/\B(?=(\d{3})+(?!\d))/g,' ');let price=30000;const proN=86;
function rev(){$('krev').textContent=nf(proN*price)}
$('openadm').onclick=()=>$('adm').style.display='flex';$('acl').onclick=()=>$('adm').style.display='none';
$('adm').onclick=e=>{if(e.target.id==='adm')$('adm').style.display='none'};
[40,55,48,70,62,85,90].forEach(h=>{const d=document.createElement('div');d.style.height=h+'%';$('bars').appendChild(d)});
$('sprice').oninput=e=>{price=+e.target.value||0;rev();document.querySelector('.pp .pr').textContent=nf(price)+' soʻm/oy'};
$('slim').oninput=e=>{LIM.free=Math.max(1,+e.target.value||1);upd()};
rev();upd();render(false);
})();
</script>
<script type="module">
import {initializeApp} from "https://www.gstatic.com/firebasejs/10.12.2/firebase-app.js";
import {getAuth,GoogleAuthProvider,signInWithPopup,onAuthStateChanged,signOut} from "https://www.gstatic.com/firebasejs/10.12.2/firebase-auth.js";
const firebaseConfig={
 apiKey:"AIzaSyBXyvHCOhytSODqIp6wNsH8y8eiERYrp9w",
 authDomain:"slayd-crok.firebaseapp.com",
 projectId:"slayd-crok",
 storageBucket:"slayd-crok.firebasestorage.app",
 messagingSenderId:"188206286614",
 appId:"1:188206286614:web:1388b64af8ba4c8ad37237"
};
const API='https://slayd-api.gulshankucharova441-8d1.workers.dev';
const ADMIN='burxonovman@gmail.com';
const auth=getAuth(initializeApp(firebaseConfig));
const $=id=>document.getElementById(id);
window.getToken=async()=>auth.currentUser?await auth.currentUser.getIdToken():null;
$('gbtn').onclick=async()=>{
 $('lerr').textContent='Kutilmoqda…';
 try{await signInWithPopup(auth,new GoogleAuthProvider())}
 catch(e){$('lerr').textContent='Kirib boʻlmadi: '+(e.code||e.message)}
};
$('out').onclick=()=>signOut(auth);
onAuthStateChanged(auth,async u=>{
 if(!u){$('login').style.display='flex';$('out').style.display='none';$('openadm').style.display='none';$('lerr').textContent='Google akkauntingiz bilan kiring, parol soʻralmaydi.';return}
 $('login').style.display='none';$('out').style.display='';
 $('openadm').style.display=(u.email||'').toLowerCase()===ADMIN?'':'none';
 try{
  const r=await fetch(API+'/me',{method:'POST',headers:{'Authorization':'Bearer '+await u.getIdToken()}});
  const d=await r.json();if(r.ok)window.setUsage(d.plan,d.used,d.limit);
 }catch(e){}
 const say=window.say||null;
 document.dispatchEvent(new CustomEvent('slayd-login',{detail:u}));
});
</script>
</body></html>
