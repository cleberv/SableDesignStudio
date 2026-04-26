# SableDesignStudio
<style>
*{box-sizing:border-box;margin:0;padding:0;}
.g{font-family:var(--font-sans);padding:0 0 2.5rem;}
.cover{background:#0D0D12;border-radius:16px;padding:36px 32px 32px;margin-bottom:2rem;position:relative;overflow:hidden;}
.orb1{position:absolute;width:280px;height:280px;border-radius:50%;background:#7B2FFF;opacity:0.13;top:-80px;right:-40px;pointer-events:none;}
.orb2{position:absolute;width:180px;height:180px;border-radius:50%;background:#00D4E8;opacity:0.09;bottom:-30px;left:30px;pointer-events:none;}
.orb3{position:absolute;width:120px;height:120px;border-radius:50%;background:#F54E6E;opacity:0.07;bottom:20px;right:120px;pointer-events:none;}
.logo-lockup{display:flex;align-items:center;gap:12px;margin-bottom:22px;}
.logo-ring{width:44px;height:44px;border-radius:50%;border:2px solid #7B2FFF;display:flex;align-items:center;justify-content:center;}
.logo-core{width:14px;height:14px;border-radius:50%;background:#7B2FFF;}
.logo-wm{color:#fff;font-size:22px;font-weight:500;letter-spacing:0.12em;text-transform:uppercase;}
.logo-sub{color:#C4A0FF;font-size:9px;letter-spacing:0.24em;text-transform:uppercase;}
.cover-eye{color:rgba(255,255,255,0.35);font-size:10px;letter-spacing:0.18em;text-transform:uppercase;margin-bottom:5px;}
.cover-title{color:#fff;font-size:20px;font-weight:500;line-height:1.3;}
.cover-ver{display:inline-flex;align-items:center;gap:6px;margin-top:12px;}
.ver-badge{background:#7B2FFF;color:#E8D5FF;border-radius:20px;padding:3px 10px;font-size:10px;font-weight:500;letter-spacing:0.06em;}
.updated-badge{background:#00D4E8;color:#003A40;border-radius:20px;padding:3px 10px;font-size:10px;font-weight:500;letter-spacing:0.06em;}

.section{margin-bottom:2.25rem;}
.sl{font-size:10px;letter-spacing:0.2em;text-transform:uppercase;font-weight:500;color:var(--color-text-secondary);margin-bottom:14px;padding-bottom:8px;border-bottom:0.5px solid var(--color-border-tertiary);}
.divider{height:0.5px;background:var(--color-border-tertiary);margin:2rem 0;}

.color-chapter{margin-bottom:24px;}
.chapter-title{font-size:11px;font-weight:500;letter-spacing:0.12em;text-transform:uppercase;color:var(--color-text-secondary);margin-bottom:10px;}
.swatch-row{display:grid;grid-template-columns:repeat(5,1fr);gap:10px;}
.swatch-row-4{display:grid;grid-template-columns:repeat(4,1fr);gap:10px;}
.sw{display:flex;flex-direction:column;gap:5px;}
.sc{height:60px;border-radius:12px;position:relative;}
.sc-tall{height:80px;}
.hero-swatch{height:100px;border-radius:14px;display:flex;align-items:flex-end;padding:10px 12px;}
.sn{font-size:12px;font-weight:500;color:var(--color-text-primary);line-height:1.3;}
.sx{font-size:10px;color:var(--color-text-secondary);font-family:var(--font-mono);}
.sr{font-size:10px;color:var(--color-text-secondary);line-height:1.4;}
.new-pill{display:inline-block;background:#00D4E8;color:#003A40;border-radius:20px;padding:1px 7px;font-size:9px;font-weight:500;vertical-align:middle;margin-left:4px;}
.replaced-pill{display:inline-block;background:#FEF3E2;color:#7A4A0A;border-radius:20px;padding:1px 7px;font-size:9px;font-weight:500;vertical-align:middle;margin-left:4px;text-decoration:line-through;}

.color-story{display:grid;grid-template-columns:1fr 1fr;gap:12px;margin-bottom:16px;}
.story-card{border-radius:14px;padding:20px;display:flex;flex-direction:column;gap:10px;}
.story-clinic{background:#F5F5F0;border:0.5px solid #E0E0D8;}
.story-events{background:#0D0D12;}
.story-label{font-size:9px;letter-spacing:0.18em;text-transform:uppercase;font-weight:500;}
.story-clinic .story-label{color:#999;}
.story-events .story-label{color:rgba(255,255,255,0.3);}
.story-h{font-size:18px;font-weight:500;line-height:1.2;margin-bottom:2px;}
.story-clinic .story-h{color:#0B1A40;}
.story-events .story-h{color:#fff;}
.story-p{font-size:11px;line-height:1.5;}
.story-clinic .story-p{color:#555;}
.story-events .story-p{color:rgba(255,255,255,0.4);}
.btn-pill{border-radius:100px;padding:7px 16px;font-size:12px;font-weight:500;display:inline-block;cursor:pointer;border:none;}
.btn-purple{background:#7B2FFF;color:#fff;}
.btn-teal-light{background:#D4F9FC;color:#003A40;}
.btn-eteal{background:#00D4E8;color:#002A30;}
.btn-eteal-outline{background:transparent;color:#00D4E8;border:1.5px solid #00D4E8;}
.btn-purple-dark{background:#7B2FFF;color:#E8D5FF;}
.story-btns{display:flex;gap:7px;flex-wrap:wrap;}
.bar{height:2px;border-radius:1px;margin-top:6px;}

.tints-row{display:grid;grid-template-columns:repeat(5,1fr);gap:8px;margin-bottom:16px;}
.tint-sw{display:flex;flex-direction:column;gap:4px;}
.tint-sc{height:40px;border-radius:8px;}

.usage-grid{display:grid;grid-template-columns:1fr 1fr;gap:12px;}
.usage-card{background:var(--color-background-secondary);border-radius:12px;padding:16px;}
.usage-title{font-size:12px;font-weight:500;color:var(--color-text-primary);margin-bottom:10px;}
.dot-item{display:flex;align-items:center;gap:8px;margin-bottom:6px;}
.dot{width:10px;height:10px;border-radius:50%;flex-shrink:0;}
.dot-label{font-size:12px;color:var(--color-text-secondary);}

.pairing-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:10px;}
.pair-card{border-radius:12px;overflow:hidden;}
.pair-top{padding:20px 16px;display:flex;flex-direction:column;gap:6px;}
.pair-bottom{padding:10px 16px;font-size:11px;line-height:1.4;}

.motif-showcase{display:grid;grid-template-columns:repeat(3,1fr);gap:10px;}
.motif-panel{background:var(--color-background-secondary);border-radius:12px;padding:16px;display:flex;flex-direction:column;gap:8px;}
.motif-vis{height:64px;display:flex;align-items:center;justify-content:center;}
.motif-title{font-size:12px;font-weight:500;color:var(--color-text-primary);}
.motif-desc{font-size:11px;color:var(--color-text-secondary);line-height:1.5;}

.type-stack{display:flex;flex-direction:column;gap:8px;}
.type-row{display:flex;align-items:baseline;gap:14px;padding:12px;background:var(--color-background-secondary);border-radius:10px;}
.type-meta{min-width:130px;flex-shrink:0;}
.type-role{font-size:10px;text-transform:uppercase;letter-spacing:0.12em;color:var(--color-text-secondary);font-weight:500;}
.type-name{font-size:11px;color:var(--color-text-secondary);margin-top:2px;}

.dos-donts{display:grid;grid-template-columns:1fr 1fr;gap:10px;}
.do-card{background:#F0F9E8;border:0.5px solid #B5D98A;border-radius:12px;padding:15px;}
.dont-card{background:#FEF2EE;border:0.5px solid #F4B8A0;border-radius:12px;padding:15px;}
.do-card .clbl{color:#2F6B12;font-size:10px;letter-spacing:0.15em;text-transform:uppercase;font-weight:500;margin-bottom:9px;}
.dont-card .clbl{color:#8B2C10;font-size:10px;letter-spacing:0.15em;text-transform:uppercase;font-weight:500;margin-bottom:9px;}
.do-card li{font-size:11px;line-height:1.7;color:#2A5C0F;}
.dont-card li{font-size:11px;line-height:1.7;color:#7A2A10;}
ul{list-style:none;padding:0;}
ul li::before{content:'— ';opacity:0.45;}

.logo-ctx-grid{display:grid;grid-template-columns:1fr 1fr;gap:12px;}
.lctx{border-radius:14px;padding:24px;display:flex;flex-direction:column;align-items:center;gap:10px;}
.lctx-light{background:#F5F5F0;border:0.5px solid #E0E0D8;}
.lctx-dark{background:#0D0D12;}
.ctx-mark{display:flex;align-items:center;gap:9px;}
.ctx-ring{width:32px;height:32px;border-radius:50%;border:2px solid;display:flex;align-items:center;justify-content:center;}
.ctx-core{width:10px;height:10px;border-radius:50%;}
.ctx-p .ctx-ring{border-color:#7B2FFF;}.ctx-p .ctx-core{background:#7B2FFF;}.ctx-p .ctx-wm{color:#0B1A40;font-size:16px;font-weight:500;letter-spacing:0.1em;text-transform:uppercase;}.ctx-p .ctx-sub{font-size:9px;letter-spacing:0.2em;text-transform:uppercase;color:#7B2FFF;}
.ctx-e .ctx-ring{border-color:#00D4E8;}.ctx-e .ctx-core{background:#00D4E8;}.ctx-e .ctx-wm{color:#fff;font-size:16px;font-weight:500;letter-spacing:0.1em;text-transform:uppercase;}.ctx-e .ctx-sub{font-size:9px;letter-spacing:0.2em;text-transform:uppercase;color:#00D4E8;}
.ctx-lbl{font-size:11px;font-weight:500;}
.lctx-light .ctx-lbl{color:#888;}.lctx-dark .ctx-lbl{color:rgba(255,255,255,0.35);}
.lctx p{font-size:11px;text-align:center;line-height:1.5;}
.lctx-light p{color:#666;}.lctx-dark p{color:rgba(255,255,255,0.35);}

.photo-grid{display:grid;grid-template-columns:repeat(4,1fr);gap:8px;}
.photo-block{border-radius:10px;display:flex;align-items:center;justify-content:center;height:70px;position:relative;overflow:hidden;}
.photo-label{position:absolute;bottom:6px;left:0;right:0;text-align:center;font-size:10px;font-weight:500;}
.photo-ok{border:1.5px solid #0F6E56;}
.photo-no{border:1.5px solid #A32D2D;position:relative;}
.photo-no::after{content:'';position:absolute;inset:0;background:rgba(163,45,45,0.08);}
.ok-label{color:#0F6E56;}.no-label{color:#A32D2D;}

.spacing-row{display:flex;align-items:flex-end;gap:12px;flex-wrap:wrap;}
.space-unit{display:flex;flex-direction:column;align-items:center;gap:5px;}
.space-block{background:#7B2FFF;border-radius:4px;width:100%;}
.space-label{font-size:10px;color:var(--color-text-secondary);text-align:center;}
.space-val{font-size:11px;font-weight:500;color:var(--color-text-primary);}

@media(max-width:480px){
  .swatch-row{grid-template-columns:repeat(3,1fr);}
  .swatch-row-4{grid-template-columns:repeat(2,1fr);}
  .color-story,.logo-ctx-grid,.usage-grid,.dos-donts,.motif-showcase,.pairing-grid{grid-template-columns:1fr;}
  .photo-grid{grid-template-columns:repeat(2,1fr);}
  .type-row{flex-direction:column;gap:4px;}
  .tints-row{grid-template-columns:repeat(3,1fr);}
}
@media(prefers-color-scheme:dark){
  .story-clinic{background:#1C1E26;border-color:#2E3040;}
  .story-clinic .story-label{color:rgba(255,255,255,0.3);}
  .story-clinic .story-h{color:#E8EAF2;}
  .story-clinic .story-p{color:rgba(255,255,255,0.4);}
  .btn-teal-light{background:#002A30;color:#00D4E8;}
  .lctx-light{background:#1C1E26;border-color:#2E3040;}
  .lctx-light .ctx-lbl{color:rgba(255,255,255,0.35);}
  .ctx-p .ctx-wm{color:#E8EAF2;}
  .lctx-light p{color:rgba(255,255,255,0.35);}
  .do-card{background:#1A2E10;border-color:#2F5020;}
  .dont-card{background:#2E1510;border-color:#5A2510;}
  .do-card .clbl{color:#8FD46A;}.dont-card .clbl{color:#F4896A;}
  .do-card li{color:#A8E085;}.dont-card li{color:#F4A080;}
}
</style>

<h2 class="sr-only">Neonova brand visual guidelines v3 — full identity system with updated electric teal replacing volt</h2>

<div class="g">

<div class="cover">
  <div class="orb1"></div><div class="orb2"></div><div class="orb3"></div>
  <div class="logo-lockup">
    <div class="logo-ring"><div class="logo-core"></div></div>
    <div><div class="logo-wm">Neonova</div><div class="logo-sub">PrEP Clinic &amp; Community</div></div>
  </div>
  <div class="cover-eye">Brand visual guidelines</div>
  <div class="cover-title">The complete Neonova<br>visual identity system</div>
  <div class="cover-ver">
    <span class="ver-badge">v3.0</span>
    <span class="updated-badge">Electric Teal update</span>
  </div>
</div>

<div class="section">
  <div class="sl">01 — Logo system</div>
  <div class="logo-ctx-grid">
    <div class="lctx lctx-light">
      <div class="ctx-mark ctx-p">
        <div class="ctx-ring"><div class="ctx-core"></div></div>
        <div><div class="ctx-wm">Neonova</div><div class="ctx-sub">PrEP Clinic</div></div>
      </div>
      <span class="ctx-lbl">Clinic — light context</span>
      <p>Electric Purple ring on Cloud. Trustworthy, clean, medically credible. Used on platform UI, telehealth, packaging, and all official communications.</p>
    </div>
    <div class="lctx lctx-dark">
      <div class="ctx-mark ctx-e">
        <div class="ctx-ring"><div class="ctx-core"></div></div>
        <div><div class="ctx-wm">Neonova</div><div class="ctx-sub">Events</div></div>
      </div>
      <span class="ctx-lbl">Events — dark context</span>
      <p>Electric Teal ring on Deep Space. Signals energy, nightlife, and cultural presence. Used on flyers, merch, wristbands, and social graphics.</p>
    </div>
  </div>
  <p style="font-size:12px;color:var(--color-text-secondary);line-height:1.6;margin-top:10px;">The nova ring gap sits at top-right — never alter it. In the clinic context, Electric Purple anchors the mark. In events, Electric Teal takes over, connecting to the palette's energy. The wordmark is always DM Sans, tracked uppercase. No effects, no recoloring outside these two approved treatments.</p>
</div>

<div class="divider"></div>

<div class="section">
  <div class="sl">02 — Color system</div>

  <div class="color-chapter">
    <div class="chapter-title">Hero colors — the backbone of both palettes</div>
    <div class="swatch-row" style="grid-template-columns:repeat(2,1fr);gap:12px;margin-bottom:4px;">
      <div class="sw">
        <div class="hero-swatch sc-tall" style="background:#7B2FFF;">
          <div>
            <div style="font-size:13px;font-weight:500;color:#E8D5FF;">Electric Purple</div>
            <div style="font-size:11px;color:rgba(255,255,255,0.5);font-family:var(--font-mono);">#7B2FFF</div>
          </div>
        </div>
        <div class="sr">Primary identity color. Logo, CTAs, active states, badges. The connective thread across both clinic and events.</div>
      </div>
      <div class="sw">
        <div class="hero-swatch sc-tall" style="background:#00D4E8;">
          <div>
            <div style="font-size:13px;font-weight:500;color:#002A30;">Electric Teal</div>
            <div style="font-size:11px;color:rgba(0,42,48,0.6);font-family:var(--font-mono);">#00D4E8</div>
          </div>
        </div>
        <div class="sr">Events lead color. Replaces Volt. Carries the energy of nightlife and community celebration with a cooler, more electric edge. <span class="new-pill">New</span></div>
      </div>
    </div>
  </div>

  <div class="color-chapter">
    <div class="chapter-title">Clinic palette — light context</div>
    <div class="swatch-row">
      <div class="sw"><div class="sc" style="background:#0B1A40;"></div><div class="sn">Midnight Navy</div><div class="sx">#0B1A40</div><div class="sr">Authority, primary text</div></div>
      <div class="sw"><div class="sc" style="background:#1A3A8C;"></div><div class="sn">Nova Blue</div><div class="sx">#1A3A8C</div><div class="sr">Headings, links</div></div>
      <div class="sw"><div class="sc" style="background:#7B2FFF;"></div><div class="sn">Electric Purple</div><div class="sx">#7B2FFF</div><div class="sr">CTAs, logo, badges</div></div>
      <div class="sw"><div class="sc" style="background:#4FC8A0;"></div><div class="sn">Vitality Teal</div><div class="sx">#4FC8A0</div><div class="sr">Health indicators</div></div>
      <div class="sw"><div class="sc" style="background:#F5F5F0;border:0.5px solid #E0E0D8;"></div><div class="sn">Cloud</div><div class="sx">#F5F5F0</div><div class="sr">Page background</div></div>
    </div>
  </div>

  <div class="color-chapter">
    <div class="chapter-title">Events palette — dark context</div>
    <div class="swatch-row">
      <div class="sw"><div class="sc" style="background:#0D0D12;border:0.5px solid #222;"></div><div class="sn">Deep Space</div><div class="sx">#0D0D12</div><div class="sr">Canvas, stage</div></div>
      <div class="sw">
        <div class="sc" style="background:#00D4E8;position:relative;">
          <span style="position:absolute;top:6px;right:6px;background:#002A30;color:#00D4E8;border-radius:10px;padding:1px 6px;font-size:9px;font-weight:500;">new</span>
        </div>
        <div class="sn">Electric Teal <span class="new-pill">New</span></div>
        <div class="sx">#00D4E8</div>
        <div class="sr">Primary events energy</div>
      </div>
      <div class="sw"><div class="sc" style="background:#7B2FFF;"></div><div class="sn">Electric Purple</div><div class="sx">#7B2FFF</div><div class="sr">Identity, depth</div></div>
      <div class="sw"><div class="sc" style="background:#F54E6E;"></div><div class="sn">Pulse Pink</div><div class="sx">#F54E6E</div><div class="sr">Passion, pride</div></div>
      <div class="sw"><div class="sc" style="background:#1A0A2E;"></div><div class="sn">Dusk Plum</div><div class="sx">#1A0A2E</div><div class="sr">Surface on dark</div></div>
    </div>
  </div>

  <div class="color-chapter">
    <div class="chapter-title">Electric Teal — tint scale</div>
    <div class="tints-row">
      <div class="tint-sw"><div class="tint-sc" style="background:#00D4E8;"></div><div class="sx">#00D4E8</div><div class="sr">Primary</div></div>
      <div class="tint-sw"><div class="tint-sc" style="background:#33DDF0;"></div><div class="sx">#33DDF0</div><div class="sr">Hover</div></div>
      <div class="tint-sw"><div class="tint-sc" style="background:#99EEF7;"></div><div class="sx">#99EEF7</div><div class="sr">Light accent</div></div>
      <div class="tint-sw"><div class="tint-sc" style="background:#D4F9FC;"></div><div class="sx">#D4F9FC</div><div class="sr">Tint / surface</div></div>
      <div class="tint-sw"><div class="tint-sc" style="background:#001A1E;border:0.5px solid #222;"></div><div class="sx">#001A1E</div><div class="sr">Dark surface</div></div>
    </div>
  </div>

  <div class="color-chapter">
    <div class="chapter-title">Electric Purple — tint scale</div>
    <div class="tints-row">
      <div class="tint-sw"><div class="tint-sc" style="background:#7B2FFF;"></div><div class="sx">#7B2FFF</div><div class="sr">Primary</div></div>
      <div class="tint-sw"><div class="tint-sc" style="background:#9B5FFF;"></div><div class="sx">#9B5FFF</div><div class="sr">Hover</div></div>
      <div class="tint-sw"><div class="tint-sc" style="background:#C4A0FF;"></div><div class="sx">#C4A0FF</div><div class="sr">On dark text</div></div>
      <div class="tint-sw"><div class="tint-sc" style="background:#EFE5FF;"></div><div class="sx">#EFE5FF</div><div class="sr">Tint / surface</div></div>
      <div class="tint-sw"><div class="tint-sc" style="background:#1A0A2E;"></div><div class="sx">#1A0A2E</div><div class="sr">Dark surface</div></div>
    </div>
  </div>
</div>

<div class="divider"></div>

<div class="section">
  <div class="sl">03 — Color in context</div>
  <div class="color-story">
    <div class="story-card story-clinic">
      <div class="story-label">Clinic — light</div>
      <div class="story-h">Your health,<br>your terms.</div>
      <div class="story-p">Start PrEP online in minutes. Our clinicians handle everything — no judgment.</div>
      <div class="story-btns">
        <button class="btn-pill btn-purple">Get started</button>
        <button class="btn-pill btn-teal-light">Learn more</button>
      </div>
      <div style="display:flex;align-items:center;gap:5px;"><span style="width:7px;height:7px;border-radius:50%;background:#4FC8A0;display:inline-block;"></span><span style="font-size:10px;color:#666;">Covered by most insurance</span></div>
    </div>
    <div class="story-card story-events">
      <div class="story-label">Events — dark</div>
      <div class="story-h">After Dark<br>Vol. 4</div>
      <div class="story-p">One night. The whole community. Presented by Neonova.</div>
      <div class="story-btns">
        <button class="btn-pill btn-eteal">Get tickets</button>
        <button class="btn-pill btn-purple-dark">RSVP free</button>
      </div>
      <div class="bar" style="background:linear-gradient(90deg,#00D4E8,#7B2FFF,#F54E6E);"></div>
    </div>
  </div>

  <div class="usage-grid">
    <div class="usage-card">
      <div class="usage-title">Clinic palette — usage roles</div>
      <div class="dot-item"><div class="dot" style="background:#0B1A40;"></div><div class="dot-label">Midnight Navy — primary text, structure</div></div>
      <div class="dot-item"><div class="dot" style="background:#1A3A8C;"></div><div class="dot-label">Nova Blue — headings, interactive links</div></div>
      <div class="dot-item"><div class="dot" style="background:#7B2FFF;"></div><div class="dot-label">Electric Purple — CTAs, logo, key actions</div></div>
      <div class="dot-item"><div class="dot" style="background:#4FC8A0;"></div><div class="dot-label">Vitality Teal — health status, success</div></div>
      <div class="dot-item"><div class="dot" style="background:#F5F5F0;border:0.5px solid #ccc;"></div><div class="dot-label">Cloud — page and surface background</div></div>
    </div>
    <div class="usage-card">
      <div class="usage-title">Events palette — usage roles</div>
      <div class="dot-item"><div class="dot" style="background:#0D0D12;"></div><div class="dot-label">Deep Space — base canvas, backgrounds</div></div>
      <div class="dot-item"><div class="dot" style="background:#00D4E8;"></div><div class="dot-label">Electric Teal — lead CTA, logo on dark</div></div>
      <div class="dot-item"><div class="dot" style="background:#7B2FFF;"></div><div class="dot-label">Electric Purple — secondary action, depth</div></div>
      <div class="dot-item"><div class="dot" style="background:#F54E6E;"></div><div class="dot-label">Pulse Pink — warmth, passion, pride</div></div>
      <div class="dot-item"><div class="dot" style="background:#1A0A2E;"></div><div class="dot-label">Dusk Plum — cards and surfaces on dark</div></div>
    </div>
  </div>
</div>

<div class="divider"></div>

<div class="section">
  <div class="sl">04 — Color pairings</div>
  <div class="pairing-grid">
    <div class="pair-card">
      <div class="pair-top" style="background:#0D0D12;">
        <div style="font-size:16px;font-weight:500;color:#00D4E8;">Electric Teal</div>
        <div style="font-size:12px;color:rgba(255,255,255,0.35);">on Deep Space</div>
        <div style="height:1.5px;background:#00D4E8;border-radius:1px;margin-top:4px;"></div>
      </div>
      <div class="pair-bottom" style="background:var(--color-background-secondary);color:var(--color-text-secondary);">Primary events pairing. Maximum contrast, maximum energy.</div>
    </div>
    <div class="pair-card">
      <div class="pair-top" style="background:#7B2FFF;">
        <div style="font-size:16px;font-weight:500;color:#fff;">Electric Purple</div>
        <div style="font-size:12px;color:rgba(255,255,255,0.5);">on itself</div>
        <div style="height:1.5px;background:#C4A0FF;border-radius:1px;margin-top:4px;"></div>
      </div>
      <div class="pair-bottom" style="background:var(--color-background-secondary);color:var(--color-text-secondary);">Use white or Lavender (#C4A0FF) text only on Purple fills.</div>
    </div>
    <div class="pair-card">
      <div class="pair-top" style="background:#F5F5F0;border-bottom:0.5px solid #E0E0D8;">
        <div style="font-size:16px;font-weight:500;color:#7B2FFF;">Electric Purple</div>
        <div style="font-size:12px;color:#999;">on Cloud</div>
        <div style="height:1.5px;background:#7B2FFF;border-radius:1px;margin-top:4px;opacity:0.4;"></div>
      </div>
      <div class="pair-bottom" style="background:var(--color-background-secondary);color:var(--color-text-secondary);">The core clinic pairing. Clean, accessible, credible.</div>
    </div>
    <div class="pair-card">
      <div class="pair-top" style="background:#1A0A2E;">
        <div style="font-size:16px;font-weight:500;color:#00D4E8;">Electric Teal</div>
        <div style="font-size:12px;color:#7B2FFF;">+ Dusk Plum</div>
        <div style="height:1.5px;background:linear-gradient(90deg,#00D4E8,#7B2FFF);border-radius:1px;margin-top:4px;"></div>
      </div>
      <div class="pair-bottom" style="background:var(--color-background-secondary);color:var(--color-text-secondary);">Event card surfaces. Depth without pure black.</div>
    </div>
    <div class="pair-card">
      <div class="pair-top" style="background:#D4F9FC;border-bottom:0.5px solid #99EEF7;">
        <div style="font-size:16px;font-weight:500;color:#003A40;">Electric Teal</div>
        <div style="font-size:12px;color:#005A66;">tint on light</div>
        <div style="height:1.5px;background:#00D4E8;border-radius:1px;margin-top:4px;opacity:0.5;"></div>
      </div>
      <div class="pair-bottom" style="background:var(--color-background-secondary);color:var(--color-text-secondary);">Teal surface in clinic UI — info banners, secondary CTAs.</div>
    </div>
    <div class="pair-card">
      <div class="pair-top" style="background:#0D0D12;">
        <div style="display:flex;gap:8px;align-items:center;">
          <div style="width:28px;height:16px;background:#00D4E8;border-radius:8px;"></div>
          <div style="width:28px;height:16px;background:#7B2FFF;border-radius:8px;"></div>
          <div style="width:28px;height:16px;background:#F54E6E;border-radius:8px;"></div>
        </div>
        <div style="font-size:12px;color:rgba(255,255,255,0.35);margin-top:6px;">Teal · Purple · Pink</div>
      </div>
      <div class="pair-bottom" style="background:var(--color-background-secondary);color:var(--color-text-secondary);">The three-way events accent. Never use all three in one element — sequence across sections.</div>
    </div>
  </div>
</div>

<div class="divider"></div>

<div class="section">
  <div class="sl">05 — Visual motifs</div>
  <div class="motif-showcase">
    <div class="motif-panel">
      <div class="motif-vis">
        <svg width="60" height="60" viewBox="0 0 60 60" fill="none">
          <circle cx="30" cy="30" r="22" stroke="#7B2FFF" stroke-width="2" stroke-dasharray="126 10" stroke-dashoffset="4"/>
          <circle cx="30" cy="30" r="11" stroke="#7B2FFF" stroke-width="1.5" opacity="0.3"/>
          <circle cx="30" cy="30" r="4" fill="#7B2FFF"/>
        </svg>
      </div>
      <div class="motif-title">Nova ring</div>
      <div class="motif-desc">Concentric circles with an open gap. The primary motif — appears in backgrounds, dividers, and framing. Always becoming, never closed.</div>
    </div>
    <div class="motif-panel">
      <div class="motif-vis">
        <svg width="60" height="60" viewBox="0 0 60 60" fill="none">
          <line x1="12" y1="48" x2="30" y2="10" stroke="#00D4E8" stroke-width="1.5" stroke-linecap="round"/>
          <line x1="48" y1="48" x2="30" y2="10" stroke="#7B2FFF" stroke-width="1.5" stroke-linecap="round" opacity="0.7"/>
          <line x1="12" y1="48" x2="48" y2="48" stroke="#F54E6E" stroke-width="1.5" stroke-linecap="round" opacity="0.5"/>
          <circle cx="30" cy="10" r="3" fill="#00D4E8"/>
        </svg>
      </div>
      <div class="motif-title">Light burst</div>
      <div class="motif-desc">Radiating lines from a central point. Evokes a nova, a signal, energy spreading outward. Event graphics and hero treatments.</div>
    </div>
    <div class="motif-panel">
      <div class="motif-vis">
        <svg width="60" height="60" viewBox="0 0 60 60" fill="none">
          <rect x="6" y="22" width="20" height="16" rx="8" fill="#1A3A8C" opacity="0.9"/>
          <rect x="20" y="22" width="20" height="16" rx="8" fill="#7B2FFF" opacity="0.85"/>
          <rect x="34" y="22" width="20" height="16" rx="8" fill="#00D4E8" opacity="0.9"/>
        </svg>
      </div>
      <div class="motif-title">Layered pills</div>
      <div class="motif-desc">Overlapping capsule forms in brand colors. Represents community, diversity, and the people Neonova serves.</div>
    </div>
    <div class="motif-panel">
      <div class="motif-vis">
        <svg width="60" height="60" viewBox="0 0 60 60" fill="none">
          <circle cx="16" cy="28" r="10" fill="#F54E6E" opacity="0.65"/>
          <circle cx="30" cy="18" r="10" fill="#7B2FFF" opacity="0.65"/>
          <circle cx="44" cy="28" r="10" fill="#00D4E8" opacity="0.65"/>
          <circle cx="30" cy="38" r="10" fill="#4FC8A0" opacity="0.65"/>
        </svg>
      </div>
      <div class="motif-title">Community dots</div>
      <div class="motif-desc">Overlapping circles in accent colors. Chosen family, constellation of community. Pattern work and illustration.</div>
    </div>
    <div class="motif-panel">
      <div class="motif-vis">
        <svg width="60" height="60" viewBox="0 0 60 60" fill="none">
          <rect x="6" y="8" width="22" height="10" rx="2" fill="#EFE5FF"/>
          <rect x="6" y="22" width="48" height="10" rx="2" fill="#7B2FFF" opacity="0.6"/>
          <rect x="6" y="36" width="34" height="10" rx="2" fill="#D4F9FC"/>
          <rect x="6" y="50" width="18" height="6" rx="2" fill="#00D4E8" opacity="0.4"/>
        </svg>
      </div>
      <div class="motif-title">Editorial grid</div>
      <div class="motif-desc">Asymmetric bold layout with accent bars. Full-width headlines, single accent color. Magazine energy, not brochure.</div>
    </div>
    <div class="motif-panel">
      <div class="motif-vis">
        <svg width="60" height="60" viewBox="0 0 60 60" fill="none">
          <circle cx="30" cy="30" r="24" stroke="#00D4E8" stroke-width="0.75" stroke-dasharray="4 3" opacity="0.4"/>
          <circle cx="30" cy="30" r="16" stroke="#7B2FFF" stroke-width="0.75" stroke-dasharray="3 3" opacity="0.5"/>
          <circle cx="30" cy="30" r="8" stroke="#00D4E8" stroke-width="1" opacity="0.6"/>
          <circle cx="30" cy="30" r="3" fill="#7B2FFF"/>
          <circle cx="54" cy="30" r="3" fill="#00D4E8" opacity="0.7"/>
          <circle cx="6" cy="30" r="2" fill="#F54E6E" opacity="0.6"/>
          <circle cx="30" cy="6" r="2" fill="#00D4E8" opacity="0.5"/>
        </svg>
      </div>
      <div class="motif-title">Orbital system</div>
      <div class="motif-desc">Dashed concentric rings with orbiting nodes. Used in hero backgrounds and data illustrations. Evokes the nova, the solar, the living system.</div>
    </div>
  </div>
</div>

<div class="divider"></div>

<div class="section">
  <div class="sl">06 — Photography direction</div>
  <div class="photo-grid">
    <div class="photo-block photo-ok" style="background:#E8F0FF;flex-direction:column;gap:4px;">
      <svg width="24" height="24" viewBox="0 0 24 24" fill="none"><circle cx="12" cy="8" r="4" stroke="#1A3A8C" stroke-width="1.5"/><path d="M4 20c0-4 3.6-7 8-7s8 3 8 7" stroke="#1A3A8C" stroke-width="1.5" stroke-linecap="round"/></svg>
      <span class="photo-label ok-label">Real people, warm light</span>
    </div>
    <div class="photo-block photo-ok" style="background:#D4F9FC;flex-direction:column;gap:4px;">
      <svg width="24" height="24" viewBox="0 0 24 24" fill="none"><path d="M12 3C7 3 3 7 3 12s4 9 9 9 9-4 9-9-4-9-9-9z" stroke="#003A40" stroke-width="1.5"/><path d="M8 14s1.5 2 4 2 4-2 4-2" stroke="#003A40" stroke-width="1.5" stroke-linecap="round"/></svg>
      <span class="photo-label ok-label">Joy and community</span>
    </div>
    <div class="photo-block photo-no" style="background:#F5F0F0;flex-direction:column;gap:4px;">
      <svg width="24" height="24" viewBox="0 0 24 24" fill="none"><rect x="4" y="6" width="16" height="12" rx="2" stroke="#A32D2D" stroke-width="1.5"/><path d="M9 12h6M12 9v6" stroke="#A32D2D" stroke-width="1.5" stroke-linecap="round"/></svg>
      <span class="photo-label no-label">Medical stock imagery</span>
    </div>
    <div class="photo-block photo-no" style="background:#F5F0F0;flex-direction:column;gap:4px;">
      <svg width="24" height="24" viewBox="0 0 24 24" fill="none"><path d="M12 3l2.5 5 5.5.8-4 3.9.9 5.5L12 15.5l-4.9 2.7.9-5.5-4-3.9 5.5-.8L12 3z" stroke="#A32D2D" stroke-width="1.5" fill="none"/></svg>
      <span class="photo-label no-label">Pride-flag tokenism</span>
    </div>
  </div>
  <p style="font-size:12px;color:var(--color-text-secondary);line-height:1.6;margin-top:10px;">Clinic photography: warm natural light, everyday life, diverse bodies and expressions. Events photography: bold contrast, high energy, night-lit crowds. Never clinical stock, never performative diversity. People should look like they belong in the world Neonova is building.</p>
</div>

<div class="divider"></div>

<div class="section">
  <div class="sl">08 — Spacing &amp; shape language</div>
  <div style="background:var(--color-background-secondary);border-radius:12px;padding:18px;margin-bottom:14px;">
    <div class="chapter-title" style="margin-bottom:12px;">Spacing scale</div>
    <div class="spacing-row">
      <div class="space-unit" style="flex:1;max-width:40px;"><div class="space-block" style="height:4px;"></div><div class="space-label">4px</div><div class="space-val">xs</div></div>
      <div class="space-unit" style="flex:1;max-width:50px;"><div class="space-block" style="height:8px;"></div><div class="space-label">8px</div><div class="space-val">sm</div></div>
      <div class="space-unit" style="flex:1;max-width:60px;"><div class="space-block" style="height:12px;"></div><div class="space-label">12px</div><div class="space-val">md</div></div>
      <div class="space-unit" style="flex:1;max-width:70px;"><div class="space-block" style="height:16px;"></div><div class="space-label">16px</div><div class="space-val">lg</div></div>
      <div class="space-unit" style="flex:1;max-width:80px;"><div class="space-block" style="height:24px;"></div><div class="space-label">24px</div><div class="space-val">xl</div></div>
      <div class="space-unit" style="flex:1;max-width:90px;"><div class="space-block" style="height:32px;"></div><div class="space-label">32px</div><div class="space-val">2xl</div></div>
      <div class="space-unit" style="flex:1;max-width:110px;"><div class="space-block" style="height:48px;"></div><div class="space-label">48px</div><div class="space-val">3xl</div></div>
    </div>
  </div>
  <div style="background:var(--color-background-secondary);border-radius:12px;padding:18px;">
    <div class="chapter-title" style="margin-bottom:12px;">Border radius</div>
    <div style="display:flex;gap:14px;flex-wrap:wrap;align-items:center;">
      <div style="display:flex;flex-direction:column;align-items:center;gap:6px;"><div style="width:48px;height:48px;background:#7B2FFF;opacity:0.15;border:1.5px solid #7B2FFF;border-radius:6px;"></div><div style="font-size:10px;color:var(--color-text-secondary);">6px<br>small</div></div>
      <div style="display:flex;flex-direction:column;align-items:center;gap:6px;"><div style="width:48px;height:48px;background:#7B2FFF;opacity:0.15;border:1.5px solid #7B2FFF;border-radius:10px;"></div><div style="font-size:10px;color:var(--color-text-secondary);">10px<br>default</div></div>
      <div style="display:flex;flex-direction:column;align-items:center;gap:6px;"><div style="width:48px;height:48px;background:#7B2FFF;opacity:0.15;border:1.5px solid #7B2FFF;border-radius:14px;"></div><div style="font-size:10px;color:var(--color-text-secondary);">14px<br>cards</div></div>
      <div style="display:flex;flex-direction:column;align-items:center;gap:6px;"><div style="width:48px;height:48px;background:#7B2FFF;opacity:0.15;border:1.5px solid #7B2FFF;border-radius:24px;"></div><div style="font-size:10px;color:var(--color-text-secondary);">24px<br>large</div></div>
      <div style="display:flex;flex-direction:column;align-items:center;gap:6px;"><div style="width:64px;height:36px;background:#7B2FFF;border-radius:100px;"></div><div style="font-size:10px;color:var(--color-text-secondary);">100px<br>pill / CTA</div></div>
    </div>
  </div>
</div>

<div class="divider"></div>

<div class="section">
  <div class="sl">07 — Brand do's &amp; don'ts</div>
  <div class="dos-donts">
    <div class="do-card">
      <div class="clbl">Do</div>
      <ul>
        <li>Use Electric Teal as the lead events color on dark</li>
        <li>Use Electric Purple as the primary clinic action color</li>
        <li>Keep the nova ring gap at top-right — never alter it</li>
        <li>Pair Teal with Deep Space or Dusk Plum on dark</li>
        <li>Pair Purple with Cloud or Deep Space only</li>
        <li>Sequence Teal, Purple, and Pink across sections — never stack all three on one element</li>
        <li>Use pill-shaped buttons and inputs across all UI</li>
        <li>Apply Space Grotesk only in events contexts</li>
        <li>Use real, diverse photography with warmth and life</li>
        <li>Give the logo clear space equal to the ring height on all sides</li>
      </ul>
    </div>
    <div class="dont-card">
      <div class="clbl">Don't</div>
      <ul>
        <li>Pair Electric Teal and Electric Purple on the same button or element — they compete</li>
        <li>Pair Electric Purple with Midnight Navy on the same element</li>
        <li>Mix clinic and events palettes on a single asset</li>
        <li>Use rainbow gradients as a brand system element</li>
        <li>Use red anywhere except semantic error states</li>
        <li>Use medical stock photography — pills, syringes, clinical settings</li>
        <li>Apply multiple accent colors in a single headline</li>
        <li>Add drop shadows, glows, or blur to the logo mark</li>
        <li>Write "patients" or "at-risk" — speak to people directly</li>
        <li>Use Space Grotesk in the clinic platform or official communications</li>
      </ul>
    </div>
  </div>
</div>

<div style="border-top:0.5px solid var(--color-border-tertiary);padding-top:14px;display:flex;justify-content:space-between;align-items:center;margin-top:0.5rem;">
  <div style="font-size:11px;color:var(--color-text-secondary);">Neonova visual brand guidelines — v3.0</div>
  <div style="display:flex;align-items:center;gap:7px;">
    <div style="width:14px;height:14px;border-radius:50%;border:1.5px solid #7B2FFF;display:flex;align-items:center;justify-content:center;"><div style="width:5px;height:5px;border-radius:50%;background:#7B2FFF;"></div></div>
    <span style="font-size:11px;color:var(--color-text-secondary);letter-spacing:0.08em;text-transform:uppercase;">Neonova</span>
  </div>
</div>

</div>
