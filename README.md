<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>NovaStark Hub - Wallpapers, Icons, Themes</title>
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@600&display=swap" rel="stylesheet">
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: radial-gradient(circle at center, #000 60%, #111 100%);
      font-family: 'Orbitron', sans-serif;
      color: #0ff;
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      align-items: center;
    }

    header {
      margin-top: 30px;
      text-align: center;
    }

    header h1 {
      font-size: 2.5rem;
    }

    header h1 span {
      color: #f00;
    }

    header p {
      font-size: 1rem;
      color: #ccc;
      margin-top: 8px;
    }

    .reactor {
      position: relative;
      width: 250px;
      height: 250px;
      margin-top: 40px;
      animation: pulse 3s infinite alternate ease-in-out;
    }

    .core {
      position: absolute;
      width: 80px;
      height: 80px;
      background: #0ff;
      border-radius: 50%;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      box-shadow: 0 0 30px #0ff, 0 0 60px #0ff;
      z-index: 2;
    }

    .glow {
      position: absolute;
      width: 160px;
      height: 160px;
      border-radius: 50%;
      background: radial-gradient(circle, rgba(0,255,255,0.4) 30%, transparent 70%);
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      z-index: 1;
    }

    .ring {
      position: absolute;
      border: 3px solid #0ff;
      border-radius: 50%;
      box-shadow: 0 0 20px #0ff;
    }

    .r1 { width: 120px; height: 120px; top: 50%; left: 50%; transform: translate(-50%, -50%); animation: spin 10s linear infinite; }
    .r2 { width: 160px; height: 160px; top: 50%; left: 50%; transform: translate(-50%, -50%); animation: spinReverse 15s linear infinite; }
    .r3 { width: 200px; height: 200px; top: 50%; left: 50%; transform: translate(-50%, -50%); animation: spin 20s linear infinite; }

    @keyframes pulse {
      from { transform: scale(1); opacity: 0.7; }
      to { transform: scale(1.1); opacity: 1; }
    }

    @keyframes spin {
      from { transform: translate(-50%, -50%) rotate(0deg); }
      to { transform: translate(-50%, -50%) rotate(360deg); }
    }

    @keyframes spinReverse {
      from { transform: translate(-50%, -50%) rotate(0deg); }
      to { transform: translate(-50%, -50%) rotate(-360deg); }
    }

    .downloads {
      margin: 50px 0;
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 20px;
    }

    .downloads a {
      padding: 12px 20px;
      background: #0ff;
      color: #000;
      text-decoration: none;
      font-weight: bold;
      border-radius: 8px;
      transition: all 0.3s ease;
    }

    .downloads a:hover {
      background: #0cc;
      transform: scale(1.05);
    }

    footer {
      margin-top: auto;
      padding: 20px;
      text-align: center;
      font-size: 0.9rem;
      color: #888;
    }
  </style>
</head>
<body>
  <header>
    <h1>NOVA<span>STARK</span> HUB</h1>
    <p>Premium Wallpapers, Icons & Themes</p>
  </header>

  <div class="reactor">
    <div class="core"></div>
    <div class="glow"></div>
    <div class="ring r1"></div>
    <div class="ring r2"></div>
    <div class="ring r3"></div>
  </div>

  <section class="downloads">
    <a href="#" download>🔥 Download Wallpaper Pack</a>
    <a href="#" download>🚀 Download Icon Set</a>
    <a href="#" download>💻 Download Theme Template</a>
  </section>

  <footer>
    <p>© 2025 NovaStark Reactor Systems. All rights reserved.</p>
  </footer>

  <script>
    console.log("🔋 NovaStark Arc Reactor: Core online.");

    const core = document.querySelector('.core');
    const glow = document.querySelector('.glow');
    let boosted = false;

    document.body.addEventListener('click', () => {
      boosted = !boosted;
      if (boosted) {
        core.style.boxShadow = "0 0 60px #0ff, 0 0 120px #0ff";
        glow.style.background = "radial-gradient(circle, rgba(0,255,255,0.8) 30%, transparent 70%)";
        console.log("⚡ Power boost engaged!");
      } else {
        core.style.boxShadow = "0 0 30px #0ff, 0 0 60px #0ff";
        glow.style.background = "radial-gradient(circle, rgba(0,255,255,0.4) 30%, transparent 70%)";
        console.log("⚡ Power back to normal.");
      }
    });
  </script>
</body>
</html>
