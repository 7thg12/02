<!doctype html><html><head><meta charset=utf8><meta name=viewport content="width=device-width,initial-scale=1,viewport-fit=cover"><style>:root{color-scheme:light;box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}html{scroll-padding-top:env(safe-area-inset-top,0px)}body{margin:0;padding:0;font:14px -apple-system,BlinkMacSystemFont,sans-serif;background:#fff;color:#000}img{max-width:100%}[hidden]:not([hidden=until-found i]){display:none!important}</style></head><body>
<title>Chữ Quốc ngữ</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,400;0,500;0,600;1,400;1,500&family=Be+Vietnam+Pro:wght@300;400;500;600&family=JetBrains+Mono:wght@400;500&display=swap">
<style>
/* Layout concept: a fixed fullscreen stage; 12 scenes crossfade as scroll progress drives every element.
   Signature transition: a gold brush stroke carries a giant tone mark (huyền, sắc, hỏi, ngã, nặng) across the frame.
   Palette: chàm (indigo) night, gold leaf, paper, one lacquer-red seal used only for "raw / wrong" text and the seal. */
:root{
  --ink:#0a1020; --indigo:#16233f; --paper:#ece5d2; --mute:#9aa3b5; --gold:#dcb461; --seal:#e5573d;
  --line:rgba(236,229,210,.16); --veil:rgba(10,16,32,.55);
  --display:'Cormorant Garamond','Iowan Old Style','Times New Roman',serif;
  --body:'Be Vietnam Pro',system-ui,-apple-system,'Segoe UI',sans-serif;
  --mono:'JetBrains Mono',ui-monospace,Menlo,Consolas,monospace;
  --g1:#0a1020; --g2:#16233f;
  color-scheme:dark;
}
*{box-sizing:border-box}
body{background:var(--ink);color:var(--paper);font-family:var(--body);font-weight:300;overflow-x:hidden}
#track{position:relative;width:1px;height:2800vh}
#stage{position:fixed;inset:0;overflow:hidden;background:radial-gradient(120% 95% at 72% 8%,var(--g2),var(--g1) 68%)}
#amb{position:absolute;inset:0;width:100%;height:100%}
#grain{position:absolute;inset:-50%;pointer-events:none;opacity:.07;mix-blend-mode:screen;
  background-image:url("data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' width='160' height='160'><filter id='n'><feTurbulence type='fractalNoise' baseFrequency='.9' numOctaves='2' stitchTiles='stitch'/><feColorMatrix values='0 0 0 0 1  0 0 0 0 1  0 0 0 0 1  0 0 0 .9 0'/></filter><rect width='100%' height='100%' filter='url(%23n)'/></svg>");
  animation:gr 1.2s steps(6) infinite}
@keyframes gr{0%{transform:translate(0,0)}20%{transform:translate(-3%,2%)}40%{transform:translate(2%,-3%)}60%{transform:translate(-2%,-1%)}80%{transform:translate(3%,3%)}100%{transform:translate(0,0)}}
#vig{position:absolute;inset:0;pointer-events:none;background:radial-gradient(ellipse at center,transparent 55%,rgba(3,6,14,.62) 100%)}

/* scenes */
.scene{position:absolute;inset:0;display:grid;align-items:center;padding:clamp(70px,11vh,118px) clamp(18px,6vw,100px) clamp(32px,7vh,72px);will-change:opacity}
.wrap{width:100%;max-width:1280px;margin-inline:auto;min-width:0}
.cols{display:grid;grid-template-columns:minmax(0,1fr) minmax(0,1.05fr);gap:clamp(24px,5vw,80px);align-items:center}
.eyebrow{font:500 clamp(.62rem,.9vw,.78rem)/1.4 var(--mono);letter-spacing:.2em;text-transform:uppercase;color:var(--gold);margin:0 0 1.1em}
h2{font:500 clamp(2rem,5vw,4.5rem)/1.02 var(--display);letter-spacing:-.01em;margin:0 0 .5em;text-wrap:balance}
h2 em{font-style:italic;color:var(--gold);font-weight:400}
p{font-size:clamp(.9rem,1.2vw,1.12rem);line-height:1.65;margin:0 0 1em;max-width:54ch;color:rgba(236,229,210,.84)}
.mono{font-family:var(--mono)}
.small{font:400 clamp(.62rem,.85vw,.74rem)/1.5 var(--mono);letter-spacing:.08em;color:var(--mute)}
.line-x{height:1px;background:var(--gold);transform-origin:left;margin:1.2em 0}

/* hero */
.hero .title{font:500 clamp(3.4rem,13.5vw,12.5rem)/.98 var(--display);margin:0;letter-spacing:-.025em;display:flex;flex-wrap:wrap;column-gap:.24em}
.word{display:inline-flex}
.lt{position:relative;display:inline-grid}
.lt>*{grid-area:1/1}
.lt .b{color:rgba(236,229,210,.3)}
.lt .f{opacity:0;color:var(--paper)}
.lt.on .b{opacity:0}
.lt.on .f{opacity:1}
.lt .mk{position:absolute;left:50%;top:-.02em;font:400 .6em/1 var(--display);color:var(--gold);transform:translateX(-50%);opacity:0;pointer-events:none}
.lt .mk.bot{top:auto;bottom:-.1em}
.lt.flash .f{animation:fl .9s ease-out}
@keyframes fl{0%{color:var(--gold);text-shadow:0 0 .4em var(--gold)}100%{color:var(--paper);text-shadow:0 0 0 transparent}}
.lede{font:italic 400 clamp(1.15rem,2.4vw,2rem)/1.3 var(--display);color:var(--paper);margin-top:1.1em;max-width:30ch}
.cue{position:absolute;left:50%;bottom:clamp(18px,4vh,40px);transform:translateX(-50%);display:flex;flex-direction:column;align-items:center;gap:10px;font:400 .66rem/1 var(--mono);letter-spacing:.24em;text-transform:uppercase;color:var(--mute)}
.cue i{display:block;width:1px;height:42px;background:linear-gradient(var(--gold),transparent);animation:cue 2s ease-in-out infinite;transform-origin:top}
@keyframes cue{0%,100%{transform:scaleY(.3);opacity:.4}50%{transform:scaleY(1);opacity:1}}

/* morph rows */
.mrow{display:grid;grid-template-columns:7.5em minmax(0,1fr);gap:1em;align-items:baseline;padding:.8em 0;border-top:1px solid var(--line)}
.mrow:last-child{border-bottom:1px solid var(--line)}
.lbl{font:400 .66rem/1.3 var(--mono);letter-spacing:.14em;text-transform:uppercase;color:var(--mute)}
.morph{font:italic 500 clamp(1.25rem,2.5vw,2.2rem)/1.2 var(--display);min-height:1.2em;transition:color .25s}
.morph[data-s="0"]{color:var(--seal)}
.morph[data-s="1"]{color:var(--gold)}
.morph[data-s="2"]{color:var(--paper)}
.morph.sm{font-size:clamp(1.05rem,1.8vw,1.5rem);min-height:2.5em}

/* timeline */
.tl{position:relative;margin-top:1.4em;padding-left:1.6em}
.tl:before{content:"";position:absolute;left:4px;top:.3em;bottom:.3em;width:1px;background:var(--gold);transform-origin:top;transform:scaleY(var(--d,0))}
.tl div{position:relative;margin-bottom:.9em;font-size:clamp(.82rem,1.05vw,.98rem);line-height:1.45;color:rgba(236,229,210,.84)}
.tl div:before{content:"";position:absolute;left:-1.6em;top:.45em;width:9px;height:9px;border-radius:50%;background:var(--gold)}
.tl b{font:500 .78rem var(--mono);color:var(--gold);margin-right:.7em}

/* tones */
.tones{display:grid;grid-template-columns:repeat(6,minmax(0,1fr));gap:clamp(6px,1.2vw,16px);margin:1.4em 0 1.6em}
.tone{border:1px solid var(--line);text-align:center;padding:clamp(8px,2vh,22px) 0 clamp(6px,1.2vh,12px);transition:border-color .4s,background .4s}
.tone .g{display:block;font:500 clamp(2.2rem,6.4vw,6rem)/1 var(--display);color:rgba(236,229,210,.22);transition:color .4s,text-shadow .4s}
.tone .n{display:block;font:400 clamp(.55rem,.8vw,.72rem)/1 var(--mono);letter-spacing:.14em;text-transform:uppercase;color:var(--mute);margin-top:.8em}
.tone.on{border-color:var(--gold);background:rgba(220,180,97,.07)}
.tone.on .g{color:var(--gold);text-shadow:0 0 .5em rgba(220,180,97,.5)}
.stats{display:grid;grid-template-columns:repeat(4,minmax(0,1fr));gap:clamp(8px,2vw,28px)}
.stat b{display:block;font:500 clamp(2rem,5vw,4.2rem)/1 var(--display);color:var(--paper)}
.stat span{font:400 clamp(.58rem,.82vw,.72rem)/1.3 var(--mono);letter-spacing:.14em;text-transform:uppercase;color:var(--mute)}

/* relay */
.relay div{font:italic 500 clamp(1.4rem,3.2vw,2.8rem)/1.15 var(--display);padding:.35em 0 .1em}
.relay .line-x{margin:.25em 0 0}
.tags{display:flex;flex-wrap:wrap;gap:8px;margin-top:1.6em}
.tag{font:400 clamp(.6rem,.82vw,.72rem)/1 var(--mono);letter-spacing:.08em;border:1px solid var(--line);padding:.7em 1em;color:var(--paper);border-radius:99px}

/* bars */
.brow{display:grid;grid-template-columns:minmax(0,13em) minmax(0,1fr) 4.8em;gap:.9em;align-items:center;padding:.5em 0}
.bl{font-size:clamp(.74rem,.98vw,.9rem);line-height:1.3;color:rgba(236,229,210,.9)}
.bt{height:10px;background:rgba(236,229,210,.09);display:block;position:relative}
.bt i{position:absolute;inset:0 auto 0 0;width:0;background:linear-gradient(90deg,rgba(220,180,97,.55),var(--gold))}
.bv{white-space:nowrap;font:500 clamp(.74rem,.98vw,.9rem) var(--mono);text-align:right;font-variant-numeric:tabular-nums}
.grp{font:500 .68rem var(--mono);letter-spacing:.18em;text-transform:uppercase;color:var(--gold);margin:0 0 .6em}
.grid2{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:clamp(22px,5vw,80px)}
.stamp{display:inline-block;border:1px solid var(--seal);color:var(--seal);font:500 .66rem/1 var(--mono);letter-spacing:.14em;text-transform:uppercase;padding:.7em .9em;transform:rotate(-1.5deg)}

/* chips */
.chips{display:flex;flex-wrap:wrap;gap:8px 8px}
.chip{font-size:clamp(.74rem,1vw,.92rem);line-height:1;padding:.75em 1.05em;border:1px solid var(--line);border-radius:99px;background:var(--veil);color:var(--paper)}
.chip:nth-child(3n+1){border-color:rgba(220,180,97,.5)}

/* rooms */
.rooms{display:grid;grid-template-columns:minmax(0,1fr) minmax(0,1fr);gap:clamp(14px,3vw,40px)}
.room{border:1px solid var(--line);padding:clamp(16px,2.6vw,34px);background:var(--veil);min-height:clamp(180px,34vh,340px)}
.room h3{font:500 .68rem/1.3 var(--mono);letter-spacing:.18em;text-transform:uppercase;margin:0 0 1.4em}
.room.a h3{color:var(--seal)} .room.b h3{color:var(--gold)}
.bub{display:block;width:fit-content;max-width:100%;padding:.6em 1em;margin-bottom:.6em;border-radius:1.1em 1.1em 1.1em .2em;background:rgba(229,87,61,.14);font:400 clamp(.9rem,1.5vw,1.3rem)/1.3 var(--body)}
.mail{font:italic 400 clamp(1.05rem,1.9vw,1.6rem)/1.45 var(--display);color:var(--paper);border-left:2px solid var(--gold);padding-left:1em;margin-bottom:1em}

/* questions */
.q{display:grid;grid-template-columns:3.2rem minmax(0,1fr);gap:1em;align-items:baseline;border-top:1px solid var(--line);padding:clamp(10px,2vh,22px) 0}
.q b{font:500 clamp(2rem,4vw,3.6rem)/1 var(--display);color:var(--gold)}
.q span{font:500 clamp(1.15rem,2.4vw,2.1rem)/1.2 var(--display)}
.ma{display:flex;flex-wrap:wrap;gap:.2em .7em;font:italic 500 clamp(1.4rem,3vw,2.6rem)/1.1 var(--display);color:var(--gold)}

/* activity cards */
.acts{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:clamp(10px,1.8vw,22px)}
.act{border:1px solid var(--line);background:var(--veil);padding:clamp(14px,2vw,26px);min-width:0}
.act h3{font:500 clamp(1.25rem,2.2vw,1.9rem)/1.1 var(--display);margin:0 0 .5em;color:var(--gold)}
.act p{font-size:clamp(.78rem,.98vw,.92rem);line-height:1.5;margin:0 0 .6em}
.act .small{margin:0}

/* dial */
.dialwrap{display:grid;place-items:center;position:relative}
.dialwrap svg{width:min(100%,clamp(240px,48vh,440px));height:auto}
.dialc{position:absolute;text-align:center;pointer-events:none}
.dialc b{display:block;font:500 clamp(3rem,8vw,6.4rem)/1 var(--display);font-variant-numeric:tabular-nums}
.dialc span{font:400 .66rem var(--mono);letter-spacing:.2em;text-transform:uppercase;color:var(--mute)}
.wk{display:grid;grid-template-columns:5.4em minmax(0,1fr);gap:1em;padding:.8em 0;border-top:1px solid var(--line);opacity:.35;transition:opacity .4s}
.wk.on{opacity:1}
.wk b{font:500 .7rem var(--mono);letter-spacing:.14em;text-transform:uppercase;color:var(--gold)}
.wk span{font-size:clamp(.82rem,1.1vw,1rem);line-height:1.45}

/* finale */
.fin{text-align:center}
.fin .title{justify-content:center;font:500 clamp(3.4rem,13vw,11rem)/1 var(--display);display:flex;margin:0 0 .15em;flex-wrap:wrap;column-gap:.24em}
.fin h2{max-width:20ch;margin-inline:auto;font-size:clamp(1.5rem,3.2vw,3rem)}
.fin p{margin-inline:auto;text-align:center}
.src{max-width:70ch;margin:1.6em auto 0}

/* HUD */
#hud{position:fixed;inset:0;pointer-events:none;z-index:5}
.brand{position:absolute;left:clamp(16px,3vw,40px);top:calc(clamp(14px,3vh,30px) + env(safe-area-inset-top,0px));display:flex;gap:12px;align-items:center;font:500 .68rem var(--mono);letter-spacing:.2em;text-transform:uppercase;color:var(--paper)}
.seal{display:grid;place-items:center;width:30px;height:30px;background:var(--seal);color:var(--ink);font:600 1.15rem/1 var(--display);transform:rotate(-3deg)}
#chap{position:absolute;right:clamp(16px,3vw,40px);top:calc(clamp(14px,3vh,30px) + env(safe-area-inset-top,0px) + 8px);font:400 .66rem var(--mono);letter-spacing:.2em;text-transform:uppercase;color:var(--mute);text-align:right}
#bar{position:absolute;left:0;top:0;height:2px;width:100%;background:var(--gold);transform-origin:left;transform:scaleX(0)}
#dots{position:absolute;right:clamp(8px,1.6vw,22px);top:50%;transform:translateY(-50%);display:flex;flex-direction:column;gap:2px;pointer-events:auto}
#dots button{all:unset;cursor:pointer;width:22px;height:18px;display:grid;place-items:center}
#dots button:before{content:"";width:5px;height:5px;border-radius:50%;background:var(--mute);opacity:.5;transition:all .3s}
#dots button.on:before{background:var(--gold);opacity:1;transform:scale(1.7)}
#dots button:focus-visible{outline:2px solid var(--gold)}
#wipe{position:absolute;inset:0;pointer-events:none;z-index:4;overflow:hidden;opacity:0}
#brush{position:absolute;top:-10%;bottom:-10%;left:0;width:56vw;transform:skewX(-14deg) translateX(-130vw);
  background:linear-gradient(90deg,transparent,rgba(220,180,97,.16) 30%,rgba(220,180,97,.34) 52%,rgba(220,180,97,.1) 80%,transparent)}
#bigmark{position:absolute;left:50%;top:50%;font:italic 500 clamp(14rem,46vw,40rem)/1 var(--display);color:var(--gold);transform:translate(-50%,-50%);opacity:.9;text-shadow:0 0 60px rgba(220,180,97,.35)}
#bigname{position:absolute;left:50%;top:calc(50% + clamp(7rem,22vw,19rem));transform:translateX(-50%);font:500 .8rem var(--mono);letter-spacing:.4em;text-transform:uppercase;color:var(--paper)}

@media (max-width:820px){
  .cols,.grid2,.rooms{grid-template-columns:minmax(0,1fr)}
  .acts{grid-template-columns:minmax(0,1fr)}
  .hide-s{display:none}
  .stats{grid-template-columns:repeat(2,minmax(0,1fr))}
  .brow{grid-template-columns:minmax(0,8em) minmax(0,1fr) 4.4em}
  .mrow{grid-template-columns:5.5em minmax(0,1fr)}
  #chap{display:none}
  .scene{padding-top:78px}
  .room{min-height:0}
}
@media (max-height:640px){.hide-h{display:none}}
a:focus-visible,button:focus-visible{outline:2px solid var(--gold);outline-offset:3px}
@media (prefers-reduced-motion:reduce){#grain{animation:none}.cue i{animation:none}}
</style>

<div id="track"></div>
<main id="stage">
  <canvas id="amb" aria-hidden="true"></canvas>
  <div id="grain" aria-hidden="true"></div>

  <!-- 0 Hero -->
  <section class="scene" data-ch="Mở đầu">
    <div class="wrap hero">
      <p class="eyebrow" data-rv="0,0.001">Đề tài nhóm sinh viên · Công tác giữ gìn tiếng Việt</p>
      <h1 class="title" id="title" aria-label="Chữ Quốc ngữ"></h1>
      <div class="line-x" data-draw="0,0.001" style="max-width:min(420px,60vw)"></div>
      <div class="lede">Giữ gìn và phát huy bắt đầu từ cách mình gõ chữ mỗi ngày.</div>
    </div>
    <div class="cue" data-fade="0,0.12"><span>Cuộn để bắt đầu</span><i></i></div>
  </section>

  <!-- 1 Origins -->
  <section class="scene" data-ch="Khởi nguồn">
    <div class="wrap cols">
      <div>
        <p class="eyebrow" data-rv="0.05,0.15">Thế kỷ XVII · Khởi đầu</p>
        <h2 data-rv="0.08,0.22">Một chữ viết sinh ra từ <em>nhiều bàn tay</em></h2>
        <p data-rv="0.18,0.3">Đầu thế kỷ XVII, các giáo sĩ phương Tây người Bồ Đào Nha, Ý, Pháp dùng mẫu tự Latin để ghi âm tiếng Việt, trước hết để hiểu tiếng người bản xứ và truyền đạo. Francisco de Pina được coi là người đặt nền móng.</p>
      </div>
      <div>
        <div class="grp" data-rv="0.2,0.3" style="margin-bottom:.4em">Bản thảo ban đầu → chữ hôm nay</div>
        <div class="mrow" data-rv="0.24,0.34" data-dy="14"><span class="lbl">Quảng Ngãi</span><span class="morph" data-from="Quanmguya" data-to="Quảng Ngãi" data-mt="0.34,0.5"></span></div>
        <div class="mrow" data-rv="0.28,0.38" data-dy="14"><span class="lbl">chữ đ</span><span class="morph" data-from="dj" data-to="đ" data-mt="0.42,0.54"></span></div>
        <div class="mrow" data-rv="0.32,0.42" data-dy="14"><span class="lbl">chữ x</span><span class="morph" data-from="sc" data-to="x" data-mt="0.5,0.62"></span></div>
        <div class="mrow" data-rv="0.36,0.46" data-dy="14"><span class="lbl">chữ v</span><span class="morph" data-from="b" data-to="v" data-mt="0.58,0.7"></span></div>
        <div class="tl hide-s" data-tl="0.55,0.9">
          <div data-rv="0.6,0.68" data-dy="10"><b>1626</b>Chữ viết rời, không còn dính liền nhau.</div>
          <div data-rv="0.7,0.78" data-dy="10"><b>1632</b>Phụ âm, nguyên âm và dấu thanh đã đủ.</div>
          <div data-rv="0.8,0.88" data-dy="10"><b>1651</b>Alexandre de Rhodes in từ điển Việt–Bồ–La.</div>
        </div>
      </div>
    </div>
  </section>

  <!-- 2 Structure -->
  <section class="scene" data-ch="Cấu trúc">
    <div class="wrap">
      <p class="eyebrow" data-rv="0.04,0.12">Chữ Quốc ngữ là gì</p>
      <h2 data-rv="0.06,0.18">Sáu thanh điệu, <em>hai mươi chín</em> chữ cái</h2>
      <div class="tones" id="tones"></div>
      <div class="cols" style="align-items:start">
        <p data-rv="0.45,0.55">Chữ Quốc ngữ ghi âm trực tiếp bằng mẫu tự Latin, thêm dấu phụ và dấu thanh. Học bảng chữ cái và cách ghép vần là đọc, viết được. Chữ Hán và chữ Nôm thì tượng hình, biểu ý.</p>
        <div class="stats">
          <div class="stat" data-rv="0.5,0.6"><b data-count="6" data-ct="0.5,0.62">0</b><span>thanh điệu</span></div>
          <div class="stat" data-rv="0.54,0.64"><b data-count="29" data-ct="0.54,0.68">0</b><span>chữ cái</span></div>
          <div class="stat" data-rv="0.58,0.68"><b data-count="11" data-ct="0.58,0.7">0</b><span>nguyên âm</span></div>
          <div class="stat" data-rv="0.62,0.72"><b data-count="18" data-ct="0.62,0.74">0</b><span>phụ âm</span></div>
        </div>
      </div>
      <p class="small hide-s" data-rv="0.74,0.84" style="max-width:none;margin-top:1.4em">Tiếng nói có trước, chữ viết có sau. Chữ Quốc ngữ chỉ ghi lại tiếng Việt, hai khái niệm này không đồng nhất.</p>
    </div>
  </section>

  <!-- 3 Role -->
  <section class="scene" data-ch="Vai trò">
    <div class="wrap cols">
      <div>
        <p class="eyebrow" data-rv="0.04,0.12">Cuối XIX · đầu XX</p>
        <h2 data-rv="0.06,0.2">Từ công cụ <em>truyền đạo</em> đến vũ khí <em>khai trí</em></h2>
        <p data-rv="0.18,0.3">Chính quyền Pháp thúc đẩy chữ Quốc ngữ trong hành chính và giáo dục vì dễ học, dễ phổ biến, và để giảm ảnh hưởng của tầng lớp Nho sĩ. Người Việt đã biến công cụ ấy thành vũ khí khai trí.</p>
      </div>
      <div>
        <div class="relay">
          <div data-rv="0.3,0.4" data-dx="40" data-dy="0">Đông kinh nghĩa thục<div class="line-x" data-draw="0.34,0.44"></div></div>
          <div data-rv="0.4,0.5" data-dx="40" data-dy="0">Báo chí quốc ngữ<div class="line-x" data-draw="0.44,0.54"></div></div>
          <div data-rv="0.5,0.6" data-dx="40" data-dy="0">Sách giáo khoa<div class="line-x" data-draw="0.54,0.64"></div></div>
          <div data-rv="0.6,0.7" data-dx="40" data-dy="0">Văn học hiện đại<div class="line-x" data-draw="0.64,0.74"></div></div>
        </div>
        <div class="tags hide-h">
          <span class="tag" data-rv="0.72,0.78" data-dy="10">Xóa mù chữ</span>
          <span class="tag" data-rv="0.75,0.81" data-dy="10">Giáo dục đại trà</span>
          <span class="tag" data-rv="0.78,0.84" data-dy="10">Nghiên cứu khoa học</span>
          <span class="tag" data-rv="0.81,0.87" data-dy="10">Thống nhất cộng đồng</span>
          <span class="tag" data-rv="0.84,0.9" data-dy="10">Tương thích môi trường số</span>
        </div>
      </div>
    </div>
  </section>

  <!-- 4 Survey -->
  <section class="scene" data-ch="Khảo sát">
    <div class="wrap">
      <p class="eyebrow" data-rv="0.03,0.1">Thực trạng · sinh viên năm nhất</p>
      <h2 data-rv="0.05,0.16">Biết nhiều hơn <em>làm</em></h2>
      <div class="grid2" id="survey"></div>
      <div style="display:flex;gap:1em;align-items:center;flex-wrap:wrap;margin-top:1.4em" data-rv="0.8,0.9">
        <span class="stamp">Số liệu minh họa</span>
        <span class="small">100 phiếu hợp lệ, khảo sát trực tuyến. Nhận thức đạt 86–94%, hành động từ 55–82%.</span>
      </div>
    </div>
  </section>

  <!-- 5 Causes -->
  <section class="scene" data-ch="Nguyên nhân">
    <div class="wrap cols">
      <div>
        <p class="eyebrow" data-rv="0.04,0.1">Hạn chế · cách viết hằng ngày</p>
        <h2 data-rv="0.05,0.16">Khi gõ nhanh hơn <em>nghĩ</em></h2>
        <div class="mrow" data-rv="0.14,0.22" data-dy="12"><span class="lbl">viết tắt</span><span class="morph sm" data-from="ko mik j r hok" data-to="không, mình, gì, rồi, không" data-mt="0.24,0.4"></span></div>
        <div class="mrow" data-rv="0.2,0.28" data-dy="12"><span class="lbl">nhắn thầy cô</span><span class="morph sm" data-from="Cô ơi, mai em nghỉ nha" data-to="Thưa cô, ngày mai em xin phép nghỉ học ạ" data-mt="0.38,0.56"></span></div>
        <div class="mrow hide-h" data-rv="0.26,0.34" data-dy="12"><span class="lbl">xen ngoại ngữ</span><span class="morph sm" data-from="Deadline của mình sắp tới rồi" data-to="Hạn nộp bài của mình sắp đến rồi" data-mt="0.54,0.7"></span></div>
      </div>
      <div>
        <div class="grp" data-rv="0.3,0.38">Chín nguyên nhân nhóm nhận diện</div>
        <div class="chips" id="chips"></div>
      </div>
    </div>
  </section>

  <!-- 6 Social -->
  <section class="scene" data-ch="Không gian số">
    <div class="wrap cols">
      <div>
        <p class="eyebrow" data-rv="0.04,0.1">Vì sao bắt đầu từ mạng xã hội</p>
        <h2 data-rv="0.05,0.16"><em data-count="79" data-ct="0.08,0.3" data-suf=" triệu">0</em> người dùng</h2>
        <p data-rv="0.14,0.24">Theo Digital 2026, Việt Nam có khoảng 79 triệu người dùng mạng xã hội, tăng 7,2% so với năm trước. Với sinh viên, ô bình luận và tin nhắn là nơi chữ Quốc ngữ được gõ nhiều nhất.</p>
        <div class="grp" data-rv="0.24,0.3" style="margin-top:1.6em">Người dùng đầu năm 2024 (triệu)</div>
        <div id="social"></div>
      </div>
      <div style="display:grid;place-items:center;gap:1em">
        <div class="dialwrap" data-rv="0.3,0.42">
          <svg viewBox="0 0 160 160" aria-label="75,4% trung lập, 3,5% tiêu cực" style="max-width:min(100%,clamp(220px,42vh,380px))">
            <circle cx="80" cy="80" r="62" fill="none" stroke="rgba(236,229,210,.12)" stroke-width="10"/>
            <circle id="ringA" cx="80" cy="80" r="62" fill="none" stroke="#dcb461" stroke-width="10" transform="rotate(-90 80 80)" stroke-dasharray="389.6" stroke-dashoffset="389.6"/>
            <circle id="ringB" cx="80" cy="80" r="62" fill="none" stroke="#e5573d" stroke-width="10" transform="rotate(-90 80 80)" stroke-dasharray="389.6" stroke-dashoffset="389.6"/>
          </svg>
          <div class="dialc"><b style="font-size:clamp(2.4rem,6vw,4.6rem)" data-count="75.4" data-ct="0.4,0.62" data-suf="%">0</b><span>trung lập</span></div>
        </div>
        <p data-rv="0.62,0.72" style="text-align:center;max-width:38ch;font-size:clamp(.82rem,1.05vw,.98rem)">Khảo sát sinh viên các trường đại học ở TP.HCM: 75,4% trung lập với biến thể ngôn ngữ của giới trẻ, chỉ <b style="color:var(--seal);font-weight:500">3,5%</b> đánh giá tiêu cực.</p>
      </div>
    </div>
  </section>

  <!-- 7 Two rooms -->
  <section class="scene" data-ch="Hai căn phòng">
    <div class="wrap">
      <p class="eyebrow" data-rv="0.04,0.1">Giao tiếp phù hợp</p>
      <h2 data-rv="0.05,0.16">Hai căn phòng, <em>hai cách viết</em></h2>
      <div class="rooms">
        <div class="room a" data-rv="0.18,0.34" data-dx="-60" data-dy="0">
          <h3>Phòng riêng · nhắn với bạn thân</h3>
          <span class="bub" data-rv="0.3,0.38" data-dy="10">Hm ni ôkê hơm?</span>
          <span class="bub" data-rv="0.38,0.46" data-dy="10">M đi học chưa?</span>
          <span class="bub" data-rv="0.46,0.54" data-dy="10">mai gặp ở trg nhé</span>
        </div>
        <div class="room b" data-rv="0.18,0.34" data-dx="60" data-dy="0">
          <h3>Phòng chung · email cho giảng viên</h3>
          <div class="mail" data-rv="0.5,0.6" data-dy="10">Dạ em chào thầy/cô, em xin phép hỏi thầy/cô về nội dung bài tập ạ.</div>
          <div class="mail hide-h" data-rv="0.6,0.7" data-dy="10">Thưa cô, ngày mai em xin phép nghỉ học ạ.</div>
        </div>
      </div>
      <p data-rv="0.72,0.82" style="margin-top:1.4em;max-width:64ch">Mục tiêu là giữ khả năng chuyển đổi giữa hai phòng, không ép mọi tin nhắn thành văn bản hành chính.</p>
    </div>
  </section>

  <!-- 8 Three questions -->
  <section class="scene" data-ch="Trước khi đăng">
    <div class="wrap cols">
      <div>
        <p class="eyebrow" data-rv="0.04,0.1">Quy tắc của nhóm</p>
        <h2 data-rv="0.05,0.17">Ba câu hỏi trước khi <em>bấm đăng</em></h2>
        <p data-rv="0.14,0.24">Bỏ dấu dễ khiến người đọc hiểu nhầm. Chỉ một dấu thanh đã đổi cả nghĩa của chữ.</p>
        <div class="ma" data-rv="0.2,0.3"><span>ma</span><span>mà</span><span>má</span><span>mả</span><span>mã</span><span>mạ</span></div>
      </div>
      <div>
        <div class="q" data-rv="0.28,0.4" data-dx="30" data-dy="0"><b>1</b><span>Người đọc có hiểu đúng ý mình không?</span></div>
        <div class="q" data-rv="0.44,0.56" data-dx="30" data-dy="0"><b>2</b><span>Có chỗ nào đổi nghĩa vì thiếu dấu hoặc viết tắt không?</span></div>
        <div class="q" data-rv="0.6,0.72" data-dx="30" data-dy="0"><b>3</b><span>Nếu lời này được in thành bản tin, mình có ngại không?</span></div>
        <p class="small" data-rv="0.78,0.88" style="margin-top:1.2em">Phản biện vào ý kiến, không vào con người.</p>
      </div>
    </div>
  </section>

  <!-- 9 Activities -->
  <section class="scene" data-ch="Hành động">
    <div class="wrap">
      <p class="eyebrow" data-rv="0.03,0.09">Sinh viên tự tổ chức</p>
      <h2 data-rv="0.04,0.14">Bốn việc làm được ngay <em>trong học kỳ này</em></h2>
      <div class="acts">
        <div class="act" data-rv="0.14,0.3" data-dy="40">
          <h3>Mỗi tuần một lỗi tiếng Việt</h3>
          <p class="hide-s">Chọn một lỗi phổ biến từ bài làm đã ẩn danh, giải thích sai ở đâu, cách sửa, mẹo nhớ.</p>
          <p class="small">12 tuần · đăng sáng thứ Hai · 12 bài, 36 câu trắc nghiệm</p>
        </div>
        <div class="act" data-rv="0.26,0.42" data-dy="40">
          <h3>Sổ tay lỗi tiếng Việt</h3>
          <p class="hide-s">Mỗi mục gồm lỗi sai, cách đúng, giải thích, ví dụ, mẹo nhớ; có giảng viên rà lại.</p>
          <p class="small">8–10 tuần · 40–60 mục · bản điện tử và bản in</p>
        </div>
        <div class="act" data-rv="0.38,0.54" data-dy="40">
          <h3>Sản phẩm song ngữ</h3>
          <p class="hide-s">Video, áp phích giới thiệu chữ Quốc ngữ và văn hóa Huế; lớp tiếng Việt cho sinh viên quốc tế.</p>
          <p class="small">Nhã nhạc cung đình Huế · UNESCO ghi danh 11/2003</p>
        </div>
        <div class="act" data-rv="0.5,0.66" data-dy="40">
          <h3>Công nghệ làm trợ lý</h3>
          <p class="hide-s">Dùng công cụ kiểm tra chính tả, xây thư viện số mẫu email; luôn tự đọc lại và kiểm chứng.</p>
          <p class="small">Công cụ và AI chỉ hỗ trợ, không thay con người</p>
        </div>
      </div>
      <p class="small" data-rv="0.76,0.86" style="margin-top:1.2em;max-width:none">Tránh phong trào “bắt lỗi”: dùng giọng khích lệ, ẩn danh, không chế giễu. Mục tiêu là dùng có ý thức, không loại bỏ mọi từ ngoại ngữ.</p>
    </div>
  </section>

  <!-- 10 21 days -->
  <section class="scene" data-ch="21 ngày viết rõ">
    <div class="wrap cols">
      <div class="dialwrap" data-rv="0.03,0.14" data-dy="0">
        <svg viewBox="0 0 400 400" id="dial" aria-hidden="true"></svg>
        <div class="dialc"><b id="dayN">1</b><span>ngày / 21</span></div>
      </div>
      <div>
        <p class="eyebrow" data-rv="0.04,0.1">Mô hình của nhóm</p>
        <h2 data-rv="0.05,0.16">21 ngày <em>viết rõ</em></h2>
        <div id="wk">
          <div class="wk" data-w="0"><b>Tuần 1</b><span>Nhận diện lỗi trong email, bài tập và bài đăng cá nhân.</span></div>
          <div class="wk" data-w="1"><b>Tuần 2</b><span>Luyện viết và sửa chéo theo tiêu chí chính tả, dùng từ, câu, phong cách.</span></div>
          <div class="wk" data-w="2"><b>Tuần 3</b><span>Tạo một bài viết, video, trang sổ tay hoặc sản phẩm song ngữ.</span></div>
        </div>
        <p class="small" data-rv="0.86,0.94" style="margin-top:1.2em;max-width:none">Đo bằng bài kiểm tra trước–sau và số lỗi trên 100 chữ. Mục tiêu tự đặt, ví dụ 30 người tham gia, giảm 20% lỗi, chưa phải kết quả đã đạt.</p>
      </div>
    </div>
  </section>

  <!-- 11 Finale -->
  <section class="scene" data-ch="Khép lại">
    <div class="wrap fin">
      <h1 class="title" id="title2" aria-label="Tiếng Việt"></h1>
      <h2 data-rv="0.55,0.68">Giữ gìn chữ Quốc ngữ bắt đầu từ cách mình <em>gõ chữ</em> mỗi ngày.</h2>
      <p data-rv="0.66,0.78">Đọc lại một lần trước khi bấm gửi. Sinh viên là chủ thể, và mốc 24/11 là dịp để cùng nhìn lại.</p>
      <p class="small src" data-rv="0.8,0.92">Nguồn số liệu: We Are Social, Digital Vietnam 2024; báo cáo Digital 2026; báo Nhân Dân; ĐHQG Hà Nội; báo Văn hóa. Số liệu khảo sát nhóm là số liệu minh họa.</p>
    </div>
  </section>

  <div id="wipe" aria-hidden="true"><div id="brush"></div><div id="bigmark">à</div><div id="bigname">dấu huyền</div></div>
  <div id="vig"></div>
  <div id="hud">
    <div id="bar"></div>
    <div class="brand"><span class="seal">ữ</span><span>Quốc ngữ</span></div>
    <div id="chap"></div>
    <nav id="dots" aria-label="Các cảnh"></nav>
  </div>
</main>

<script>
(function(){
const $=(s,r=document)=>r.querySelector(s), $$=(s,r=document)=>[...r.querySelectorAll(s)];
const clamp=(x,a=0,b=1)=>Math.min(b,Math.max(a,x));
const seg=(t,a,b)=>clamp((t-a)/(b-a));
const sm=(a,b,x)=>{const t=clamp((x-a)/(b-a));return t*t*(3-2*t)};
const ease=x=>1-Math.pow(1-x,3);
const RM=matchMedia('(prefers-reduced-motion: reduce)').matches;
const P=s=>s.split(',').map(Number);

/* ---------- generated content ---------- */
// letters with tone marks (hero + finale)
function buildWord(host,words){
  const out=[];
  words.forEach(w=>{
    const wd=document.createElement('span');wd.className='word';
    w.forEach(l=>{
      const s=document.createElement('span');s.className='lt';
      const base=l[0],full=l[1]||l[0];
      s.innerHTML='<span class="b">'+base+'</span><span class="f">'+full+'</span>'+(l[2]?'<span class="mk '+(l[3]||'')+'">'+l[2]+'</span>':'');
      if(!l[2]) s.classList.add('on');
      wd.appendChild(s);
      if(l[2]) out.push(s);
    });
    host.appendChild(wd);
  });
  return out;
}
const heroMarks=buildWord($('#title'),[
  [['C'],['h'],['u','ữ','˜']],
  [['Q'],['u'],['o','ố','´'],['c']],
  [['n'],['g'],['u','ữ','˜']]
]);
// wrap "Quốc ngữ" as one flex group: restructure words
(function(){const t=$('#title'),w=$$('.word',t);const g=document.createElement('span');g.className='word';g.style.columnGap='.24em';g.style.display='inline-flex';
  // merge Quốc + ngữ into one non-breaking pair
  const a=w[1],b=w[2];const pair=document.createElement('span');pair.style.display='inline-flex';pair.style.columnGap='.24em';a.after(pair);pair.append(a,b);})();
const finMarks=buildWord($('#title2'),[
  [['T'],['i'],['e','ế','´'],['n'],['g']],
  [['V'],['i'],['e','ệ','·','bot'],['t']]
]);
function setLetter(l,f){
  const mk=$('.mk',l);
  const done=f>=1;
  if(done&&!l.classList.contains('on')){l.classList.add('on','flash');setTimeout(()=>l.classList.remove('flash'),950)}
  if(!done&&l.classList.contains('on')){l.classList.remove('on','flash')}
  const e=ease(clamp(f));
  mk.style.opacity=done?0:clamp(f*3);
  mk.style.transform='translate(-50%,'+(-(1-e)*1.8)+'em)';
}

// tones
const TN=[['a','ngang'],['à','huyền'],['á','sắc'],['ả','hỏi'],['ã','ngã'],['ạ','nặng']];
$('#tones').innerHTML=TN.map(t=>'<div class="tone"><span class="g">'+t[0]+'</span><span class="n">'+t[1]+'</span></div>').join('');

// bars
const dec=v=>String(v).includes('.')?1:0;
const barRow=(label,val,a,b,suf,max)=>'<div class="brow" data-rv="'+a+','+(a+.1)+'" data-dy="12"><span class="bl">'+label+'</span><span class="bt"><i data-bar="'+val+'" data-max="'+(max||100)+'" data-bt="'+a+','+b+'"></i></span><b class="bv" data-count="'+val+'" data-dec="'+dec(val)+'" data-ct="'+a+','+b+'" data-suf="'+(suf||'%')+'">0</b></div>';
$('#survey').innerHTML=
 '<div><div class="grp" data-rv="0.14,0.2">Nhận thức: cho là cần thiết</div>'+
  [['Dùng tiếng Việt có dấu',94],['Vai trò của chữ Quốc ngữ',92],['Viết đúng chính tả',90],['Viết hoa đúng quy tắc',88],['Dùng dấu câu đúng',86]].map((r,i)=>barRow(r[0],r[1],.2+i*.07,.4+i*.07)).join('')+'</div>'+
 '<div><div class="grp" data-rv="0.46,0.52">Hành động: thường xuyên làm</div>'+
  [['Dùng tiếng Việt đầy đủ trong email, bài tập',82],['Kiểm tra chính tả trước khi nộp',78],['Đọc sách, tài liệu tiếng Việt',70],['Tra từ điển khi chưa chắc',65],['Từng viết, thuyết trình, hùng biện',55]].map((r,i)=>barRow(r[0],r[1],.52+i*.05,.66+i*.05)).join('')+'</div>';
$('#social').innerHTML=[['Facebook',72.7],['TikTok (từ 18 tuổi)',67.7],['YouTube',63]].map((r,i)=>barRow(r[0],r[1],.28+i*.06,.5+i*.06,' tr',80)).join('');

// chips
const CH=['Mạng xã hội','Viết nhanh, viết tắt','Chạy theo xu hướng','Tiếng lóng','Xen ngoại ngữ','Ít đọc sách','Ít rà soát lỗi','Lẫn thân mật với trang trọng','Xem nhẹ lỗi nhỏ'];
$('#chips').innerHTML=CH.map((c,i)=>'<span class="chip" data-rv="'+(.36+i*.055)+','+(.44+i*.055)+'" data-dy="14">'+c+'</span>').join('');

// dial
(function(){let h='<circle cx="200" cy="200" r="120" fill="none" stroke="rgba(236,229,210,.1)"/>';
 for(let i=0;i<21;i++){const a=(i/21)*Math.PI*2-Math.PI/2,r1=140,r2=184;
  h+='<line class="tk" data-i="'+i+'" x1="'+(200+Math.cos(a)*r1)+'" y1="'+(200+Math.sin(a)*r1)+'" x2="'+(200+Math.cos(a)*r2)+'" y2="'+(200+Math.sin(a)*r2)+'" stroke="rgba(236,229,210,.2)" stroke-width="6" stroke-linecap="round"/>'}
 $('#dial').innerHTML=h})();
const ticks=$$('.tk'),wks=$$('.wk'),dayN=$('#dayN');

// nav dots
const scenes=$$('.scene',$('#stage'));
const N=scenes.length;
const dots=scenes.map((s,i)=>{const b=document.createElement('button');b.setAttribute('aria-label','Cảnh '+(i+1)+': '+s.dataset.ch);b.title=s.dataset.ch;b.onclick=()=>goTo(i);$('#dots').appendChild(b);return b});

/* ---------- parse reactive elements ---------- */
const S=scenes.map((el,i)=>({
  el,i,
  rv:$$('[data-rv]',el).map(n=>({n,r:P(n.dataset.rv),dx:+(n.dataset.dx||0),dy:n.dataset.dy!==undefined?+n.dataset.dy:26})),
  draw:$$('[data-draw]',el).map(n=>({n,r:P(n.dataset.draw)})),
  bars:$$('[data-bar]',el).map(n=>({n,v:+n.dataset.bar,m:+n.dataset.max,r:P(n.dataset.bt)})),
  counts:$$('[data-count]',el).map(n=>({n,v:+n.dataset.count,d:+(n.dataset.dec||dec(n.dataset.count)),suf:n.dataset.suf||'',r:P(n.dataset.ct)})),
  morphs:$$('.morph',el).map(n=>({n,f:n.dataset.from,t:n.dataset.to,r:P(n.dataset.mt)})),
  fades:$$('[data-fade]',el).map(n=>({n,r:P(n.dataset.fade)})),
  tl:$('[data-tl]',el)
}));
const fmt=(v,d)=>v.toLocaleString('vi-VN',{minimumFractionDigits:d,maximumFractionDigits:d});

/* ---------- background tint per scene ---------- */
const TINT=[['#0a1020','#16233f'],['#140f0a','#34230f'],['#0a1020','#1b2c52'],['#08181b','#12383e'],['#0a1020','#16233f'],['#160c18','#35183a'],['#0a1020','#17294c'],['#0e1118','#26272f'],['#0a1020','#1a2a4d'],['#0b1713','#143528'],['#0a1020','#2a2410'],['#0a1020','#1d2b52']];
const hx=h=>[1,3,5].map(i=>parseInt(h.slice(i,i+2),16));
const mixc=(a,b,w)=>a.map((v,i)=>Math.round(v+(b[i]-v)*w));
const TC=TINT.map(p=>p.map(hx));
const stage=$('#stage');

/* ---------- ambient canvas ---------- */
const cv=$('#amb'),cx=cv.getContext('2d');let W=0,H=0,DPR=1,L=1;
const GL='aăâeêioôơuưyđàáảãạằắẳẵặầấẩẫậèéẻẽẹềếểễệìíỉĩịòóỏõọồốổỗộờớởỡợùúủũụừứửữự'.split('');
const parts=Array.from({length:46},()=>({c:GL[Math.random()*GL.length|0],x:Math.random(),y:Math.random(),z:.2+Math.random()*.8,r:Math.random()*6.28,sp:.005+Math.random()*.012}));
let mx=0,my=0,sNow=0;
function drawAmb(time){
  cx.clearRect(0,0,W,H);
  for(const p of parts){
    const y=((p.y-(time*p.sp*p.z)-sNow*p.z*.28)%1+1)%1;
    const x=p.x+Math.sin(time*.1+p.r)*.015+mx*.02*p.z;
    cx.font='italic '+(14+p.z*58)+'px "Cormorant Garamond",serif';
    cx.fillStyle='rgba(220,180,97,'+(.04+p.z*.13)+')';
    cx.fillText(p.c,x*W,y*(H+120)-60+my*10*p.z);
  }
}
function resize(){DPR=Math.min(devicePixelRatio||1,2);W=innerWidth;H=innerHeight;cv.width=W*DPR;cv.height=H*DPR;cx.setTransform(DPR,0,0,DPR,0,0);L=H*2.3;$('#track').style.height=(N*L+H)+'px';onScroll();drawAmb(0)}
addEventListener('resize',resize);
addEventListener('pointermove',e=>{mx=e.clientX/W-.5;my=e.clientY/H-.5},{passive:true});

/* ---------- scroll ---------- */
let target=0,cur=0,lastRender=-1;
function onScroll(){target=clamp(scrollY/L,0,N)}
addEventListener('scroll',onScroll,{passive:true});
function goTo(i){scrollTo({top:i===0?0:(i+.6)*L,behavior:RM?'auto':'smooth'})}

/* ---------- transition overlay ---------- */
const WM=[['à','dấu huyền'],['á','dấu sắc'],['ả','dấu hỏi'],['ã','dấu ngã'],['ạ','dấu nặng']];
const wipe=$('#wipe'),brush=$('#brush'),bigm=$('#bigmark'),bign=$('#bigname');
let lastK=-1;
function doWipe(s){
  const k=Math.round(s);
  if(k<1||k>N-1){wipe.style.opacity=0;return}
  const x=(s-k)/.1;
  if(Math.abs(x)>=1){wipe.style.opacity=0;return}
  if(k!==lastK){const m=WM[(k-1)%5];bigm.textContent=m[0];bign.textContent=m[1];lastK=k}
  const bell=Math.cos(x*Math.PI/2);
  wipe.style.opacity=bell;
  brush.style.transform='skewX(-14deg) translateX('+((x*.5+.5)*230-130)+'vw)';
  bigm.style.transform='translate(calc(-50% + '+(-x*8)+'vw),-50%) scale('+(0.92+bell*.12)+')';
}

/* ---------- render ---------- */
function render(s){
  sNow=s;
  S.forEach(sc=>{
    const i=sc.i;
    const op=(i===0?1:sm(i-.07,i+.07,s))*(i===N-1?1:1-sm(i+1-.07,i+1+.07,s));
    const el=sc.el;
    if(op<.003){if(el.style.visibility!=='hidden'){el.style.visibility='hidden';el.style.opacity=0}return}
    el.style.visibility='visible';el.style.opacity=op;
    el.style.pointerEvents=op>.5?'auto':'none';
    el.style.filter=op<.99?'blur('+((1-op)*9).toFixed(1)+'px)':'none';
    const t=clamp(s-i);
    sc.rv.forEach(o=>{const p=ease(seg(t,o.r[0],o.r[1]));o.n.style.opacity=p;o.n.style.transform=p>=1?'none':'translate('+(o.dx*(1-p)).toFixed(1)+'px,'+(o.dy*(1-p)).toFixed(1)+'px)'});
    sc.draw.forEach(o=>{o.n.style.transform='scaleX('+ease(seg(t,o.r[0],o.r[1]))+')'});
    sc.fades.forEach(o=>{o.n.style.opacity=1-seg(t,o.r[0],o.r[1])});
    sc.bars.forEach(o=>{o.n.style.width=(o.v/o.m*100*ease(seg(t,o.r[0],o.r[1]))).toFixed(1)+'%'});
    sc.counts.forEach(o=>{o.n.textContent=fmt(o.v*ease(seg(t,o.r[0],o.r[1])),o.d)+o.suf});
    sc.morphs.forEach(o=>{
      const k=seg(t,o.r[0],o.r[1]),len=Math.max(o.f.length,o.t.length),n=Math.floor(k*len);
      o.n.textContent=k>=1?o.t:o.t.slice(0,n)+o.f.slice(Math.min(n,o.f.length));
      o.n.dataset.s=k<=0?0:k>=1?2:1;
    });
    if(sc.tl)sc.tl.style.setProperty('--d',seg(t,...P(sc.tl.dataset.tl)));
    if(i===0){const e=seg(t,.1,.9);$('#title').style.transform='translateY('+(-e*50)+'px) scale('+(1+e*.08)+')';$('#title').style.opacity=1-e*.9}
    if(i===2){$$('.tone').forEach((n,k)=>n.classList.toggle('on',t>.16+k*.05))}
    if(i===6){const c=389.6,a=.754*ease(seg(t,.4,.62)),b=.035*ease(seg(t,.58,.7));
      $('#ringA').style.strokeDashoffset=c*(1-a);
      const rb=$('#ringB');rb.setAttribute('transform','rotate('+(-90+360*.754)+' 80 80)');rb.style.strokeDashoffset=c*(1-b)}
    if(i===10){const d=Math.max(1,Math.ceil(21*seg(t,.2,.82)));dayN.textContent=d;
      ticks.forEach((tk,k)=>{const on=k<d;tk.setAttribute('stroke',on?(k<7?'#ece5d2':k<14?'#dcb461':'#e5573d'):'rgba(236,229,210,.2)')});
      wks.forEach((w,k)=>w.classList.toggle('on',Math.floor((d-1)/7)>=k&&t>.14))}
    if(i===11){finMarks.forEach((l,k)=>setLetter(l,seg(t,.04+k*.14,.18+k*.14)))}
  });
  // tint
  let c=TC[0].map(x=>x);let c2=TC[0][1];c=TC[0][0];
  let g1=TC[0][0],g2=TC[0][1];
  for(let k=1;k<N;k++){const w=sm(k-.12,k+.12,s);g1=mixc(g1,TC[k][0],w);g2=mixc(g2,TC[k][1],w)}
  stage.style.setProperty('--g1','rgb('+g1+')');stage.style.setProperty('--g2','rgb('+g2+')');
  const ci=Math.min(N-1,Math.floor(s+.1));
  $('#chap').textContent=(ci+1)+' / '+N+'  ·  '+scenes[ci].dataset.ch;
  dots.forEach((d,k)=>d.classList.toggle('on',k===ci));
  $('#bar').style.transform='scaleX('+(s/N)+')';
  doWipe(s);
}

/* ---------- hero intro (time based, rests on final title) ---------- */
let t0=performance.now(),introDone=false;
function intro(now){
  const f=RM?9:(now-t0-350)/1000;
  heroMarks.forEach((l,k)=>setLetter(l,clamp((f-k*.38)/.7)));
  if(f>2.4)introDone=true;
}

/* ---------- loop ---------- */
function frame(now){
  cur+=(target-cur)*(RM?1:.12);
  if(Math.abs(target-cur)<.0005)cur=target;
  if(cur!==lastRender){render(cur);lastRender=cur}
  if(!introDone)intro(now);
  if(!RM||lastRender===cur)drawAmb(now/1000);
  requestAnimationFrame(frame);
}
resize();
if(document.fonts&&document.fonts.ready)document.fonts.ready.then(()=>{lastRender=-1});
heroMarks.forEach(l=>setLetter(l,RM?1:0));
render(0);
if(RM){introDone=false;intro(0)}
requestAnimationFrame(frame);
})();
</script>

</body></html>
