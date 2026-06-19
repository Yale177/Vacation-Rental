<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Casa Marea — Guest Guide</title>
<link rel="preconnect" href="https://fonts.googleapis.com" />
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
<link href="https://fonts.googleapis.com/css2?family=Fraunces:opsz,wght@9..144,400;9..144,500;9..144,600&family=Inter:wght@400;500;600&display=swap" rel="stylesheet" />
<style>
  :root {
    --sea: #115E59;
    --sea-deep: #0C4641;
    --paper: #F7F2E9;
    --sand: #EFE7D6;
    --amber: #E08D3C;
    --ink: #20302E;
    --muted: #6B7B78;
    --line: #E2D8C6;
    --white: #FFFFFF;
  }
  * { box-sizing: border-box; margin: 0; padding: 0; }
  body {
    font-family: 'Inter', system-ui, sans-serif;
    color: var(--ink);
    background: radial-gradient(120% 80% at 50% -10%, #1c6f69 0%, var(--sea) 40%, var(--sea-deep) 100%);
    min-height: 100dvh;
    display: flex;
    justify-content: center;
  }
  .page {
    width: 100%;
    max-width: 480px;
    background: var(--paper);
    min-height: 100dvh;
  }
  @media (min-width: 520px) {
    .page { min-height: auto; margin: 24px 0; border-radius: 24px; overflow: hidden; box-shadow: 0 24px 70px rgba(0,0,0,0.3); }
  }

  .header {
    background: var(--sea);
    color: var(--paper);
    padding: 30px 26px 26px;
    position: relative;
  }
  .header::after {
    content: "";
    position: absolute; left: 0; right: 0; bottom: -1px; height: 14px;
    background: var(--paper);
    -webkit-mask: radial-gradient(10px at 14px 14px, transparent 98%, #000) repeat-x;
    mask: radial-gradient(10px at 14px 14px, transparent 98%, #000) repeat-x;
    -webkit-mask-size: 28px 14px; mask-size: 28px 14px;
  }
  .eyebrow {
    font-size: 11px; letter-spacing: 0.2em; text-transform: uppercase;
    color: var(--amber); font-weight: 600; margin-bottom: 8px;
  }
  .home-name {
    font-family: 'Fraunces', Georgia, serif; font-size: 34px; font-weight: 500;
    line-height: 1.05; letter-spacing: -0.01em;
  }
  .home-loc { font-size: 13.5px; color: rgba(247,242,233,0.78); margin-top: 7px; }
  .lead { font-size: 14px; line-height: 1.5; color: rgba(247,242,233,0.92); margin-top: 16px; max-width: 36ch; }

  .qa { padding: 24px 20px 36px; display: flex; flex-direction: column; gap: 14px; }

  .card {
    background: var(--white);
    border: 1px solid var(--line);
    border-radius: 16px;
    padding: 18px 18px 16px;
  }
  .card .q {
    display: flex; align-items: center; gap: 10px;
    font-size: 15px; font-weight: 600; color: var(--sea-deep);
  }
  .ic {
    width: 30px; height: 30px; flex-shrink: 0;
    background: var(--sand); border-radius: 9px;
    display: grid; place-items: center; font-size: 15px;
  }
  .card .a { margin-top: 11px; font-size: 16px; line-height: 1.5; color: var(--ink); padding-left: 40px; }

  .pill {
    display: inline-block;
    font-family: 'DejaVu Sans Mono', ui-monospace, monospace;
    font-size: 17px; font-weight: 600; letter-spacing: 0.03em;
    background: var(--sand); color: var(--sea-deep);
    border: 1px dashed var(--amber);
    padding: 8px 14px; border-radius: 10px;
    user-select: all; -webkit-user-select: all;
  }
  .hint { display: block; font-size: 12px; color: var(--muted); margin-top: 8px; }

  .foot {
    text-align: center; font-size: 12px; color: var(--muted);
    padding: 0 24px 30px;
  }
  .foot .rule { width: 44px; height: 3px; background: var(--amber); margin: 0 auto 14px; border-radius: 2px; }
</style>
</head>
<body>
  <div class="page">
    <div class="header">
      <div class="eyebrow">Guest Guide</div>
      <div class="home-name">Casa Marea</div>
      <div class="home-loc">Everything you need for your stay</div>
      <div class="lead">A few quick answers for your stay. Tap and hold any password to copy it.</div>
    </div>

    <div class="qa">
      <div class="card">
        <div class="q"><span class="ic">📶</span> What's the Wi-Fi password?</div>
        <div class="a">
          <span class="pill">CLaude1221</span>
          <span class="hint">Look for the network in your phone's Wi-Fi settings, then enter this password.</span>
        </div>
      </div>

      <div class="card">
        <div class="q"><span class="ic">🍽️</span> Where should we eat?</div>
        <div class="a">Two solid picks nearby: <strong>Earls</strong> and <strong>The Keg</strong>.</div>
      </div>

      <div class="card">
        <div class="q"><span class="ic">🥐</span> What time is breakfast?</div>
        <div class="a">Breakfast is served at <strong>9:00 AM</strong>.</div>
      </div>
    </div>

    <div class="foot">
      <div class="rule"></div>
      Enjoy your stay. Questions not answered here? Reach out to your host.
    </div>
  </div>
</body>
</html>
