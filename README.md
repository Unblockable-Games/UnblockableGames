<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Download This Site</title>
    <style>
        body {
            margin: 0;
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            background: linear-gradient(135deg, #0a0f1e, #0c1222);
            font-family: 'Segoe UI', system-ui, sans-serif;
        }

        .site-download-btn {
            display: inline-flex;
            align-items: center;
            gap: 14px;
            padding: 1.1rem 2.6rem;
            border-radius: 60px;
            color: #ffffff;
            text-decoration: none;
            font-weight: 800;
            font-size: 1.05rem;
            background: linear-gradient(135deg, #facc15, #f97316, #ec4899, #8b5cf6);
            background-size: 300% 300%;
            animation: gradientShift 6s ease infinite;
            box-shadow: 0 10px 30px -8px rgba(236,72,153,0.55),
                        0 0 40px -10px rgba(250,204,21,0.5);
            transition: transform 0.25s ease, box-shadow 0.25s ease;
        }

        .site-download-btn:hover {
            transform: translateY(-4px) scale(1.03);
            box-shadow: 0 18px 40px -10px rgba(236,72,153,0.75),
                        0 0 60px -10px rgba(250,204,21,0.7);
        }

        .site-download-btn .btn-icon {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 34px;
            height: 34px;
            border-radius: 50%;
            background: rgba(255,255,255,0.18);
            font-size: 1.05rem;
        }

        .site-download-btn .btn-text {
            display: flex;
            flex-direction: column;
            align-items: flex-start;
            line-height: 1.15;
        }

        .site-download-btn .btn-text .main {
            font-size: 1.05rem;
            font-weight: 800;
        }

        .site-download-btn .btn-text .sub {
            font-size: 0.7rem;
            font-weight: 600;
            opacity: 0.85;
            letter-spacing: 0.4px;
            text-transform: uppercase;
        }

        @keyframes gradientShift {
            0%, 100% { background-position: 0% 50%; }
            50%      { background-position: 100% 50%; }
        }
    </style>
</head>
<body>
    <a
        class="site-download-btn"
        href="https://drive.google.com/uc?export=download&id=1kuA9Qtnyuzts_4N7ZMF2TxaVLOlNhuPg"
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
