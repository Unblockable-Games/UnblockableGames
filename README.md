<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Download This Site</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      background: linear-gradient(135deg, #0a0f1e 0%, #0c1222 100%);
      font-family: 'Segoe UI', 'Poppins', 'Inter', system-ui, -apple-system, sans-serif;
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 2rem;
    }

    .site-download-btn {
      position: relative;
      display: inline-flex;
      align-items: center;
      gap: 16px;
      padding: 1.2rem 2.8rem;
      border-radius: 60px;
      border: none;
      cursor: pointer;
      font-family: inherit;
      font-weight: 800;
      font-size: 1.1rem;
      letter-spacing: 0.3px;
      color: #ffffff;
      text-decoration: none;
      background: linear-gradient(135deg, #facc15 0%, #f97316 35%, #ec4899 70%, #8b5cf6 100%);
      background-size: 300% 300%;
      animation: gradientShift 6s ease infinite;
      box-shadow:
        0 0 0 1px rgba(255, 255, 255, 0.15) inset,
        0 10px 30px -8px rgba(236, 72, 153, 0.55),
        0 0 40px -10px rgba(250, 204, 21, 0.5);
      transition: transform 0.25s ease, box-shadow 0.25s ease;
      overflow: hidden;
      isolation: isolate;
    }

    .site-download-btn::before {
      content: "";
      position: absolute;
      inset: 0;
      border-radius: 60px;
      padding: 2px;
      background: linear-gradient(135deg, #facc15, #ec4899, #8b5cf6, #3b82f6);
      -webkit-mask: linear-gradient(#000 0 0) content-box, linear-gradient(#000 0 0);
      -webkit-mask-composite: xor;
              mask-composite: exclude;
      opacity: 0.9;
      z-index: -1;
    }

    .site-download-btn::after {
      content: "";
      position: absolute;
      top: 0;
      left: -120%;
      width: 60%;
      height: 100%;
      background: linear-gradient(
        100deg,
        transparent 0%,
        rgba(255, 255, 255, 0.5) 50%,
        transparent 100%
      );
      transform: skewX(-20deg);
      animation: shimmerSweep 3.5s ease-in-out infinite;
      z-index: 0;
    }

    .site-download-btn .btn-icon {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      width: 38px;
      height: 38px;
      border-radius: 50%;
      background: rgba(255, 255, 255, 0.18);
      backdrop-filter: blur(4px);
      font-size: 1.2rem;
      animation: iconPulse 2s ease-in-out infinite;
      position: relative;
      z-index: 1;
    }

    .site-download-btn .btn-text {
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      line-height: 1.15;
      position: relative;
      z-index: 1;
    }

    .site-download-btn .btn-text .main {
      font-size: 1.1rem;
      font-weight: 800;
      text-shadow: 0 1px 2px rgba(0, 0, 0, 0.25);
    }

    .site-download-btn .btn-text .sub {
      font-size: 0.72rem;
      font-weight: 600;
      opacity: 0.85;
      letter-spacing: 0.4px;
      text-transform: uppercase;
    }

    .site-download-btn:hover {
      transform: translateY(-4px) scale(1.03);
      box-shadow:
        0 0 0 1px rgba(255, 255, 255, 0.25) inset,
        0 18px 40px -10px rgba(236, 72, 153, 0.75),
        0 0 60px -10px rgba(250, 204, 21, 0.7);
    }

    .site-download-btn:active {
      transform: translateY(-1px) scale(0.99);
    }

    .site-download-btn .arrow {
      display: inline-block;
      position: relative;
      z-index: 1;
      font-size: 1.2rem;
      transition: transform 0.25s ease;
    }

    .site-download-btn:hover .arrow {
      transform: translateX(4px);
    }

    @keyframes gradientShift {
      0%, 100% { background-position: 0% 50%; }
      50%      { background-position: 100% 50%; }
    }

    @keyframes shimmerSweep {
      0%   { left: -120%; }
      60%  { left: 160%; }
      100% { left: 160%; }
    }

    @keyframes iconPulse {
      0%, 100% { transform: scale(1); box-shadow: 0 0 0 0 rgba(255, 255, 255, 0.4); }
      50%      { transform: scale(1.08); box-shadow: 0 0 0 8px rgba(255, 255, 255, 0); }
    }

    @media (max-width: 640px) {
      .site-download-btn {
        padding: 1rem 2rem;
        gap: 12px;
      }
      .site-download-btn .btn-text .main {
        font-size: 1rem;
      }
      .site-download-btn .btn-text .sub {
        font-size: 0.65rem;
      }
      .site-download-btn .btn-icon {
        width: 32px;
        height: 32px;
        font-size: 1rem;
      }
    }
  </style>
</head>
<body>
  <a
    class="site-download-btn"
    href="https://drive.google.com/uc?export=download&id=1CsIpG7n8gmkVnU6_qPC17Q9rupecPKrq"
    download
    target="_blank"
    rel="noopener noreferrer"
  >
    <span class="btn-icon">📥</span>
    <span class="btn-text">
      <span class="main">Download This Site</span>
      <span class="sub">Offline · No setup · Just open</span>
    </span>
    <span class="arrow">→</span>
  </a>
</body>
</html>
