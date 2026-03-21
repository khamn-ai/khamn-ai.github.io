<!DOCTYPE html>
<html lang="zh-TW">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>桃園白牌叫車平台 - 專業調度版</title>
    <style>
        :root {
            --bg-deep: #05070a;
            --card-bg: rgba(255, 255, 255, 0.03);
            --card-border: rgba(255, 255, 255, 0.08);
            --neon-blue: #00f2ff;
            --neon-green: #39ff14;
            --neon-red: #ff3131;
            --neon-gold: #ffdf00;
            --text-primary: #ffffff;
            --text-secondary: #94a3b8;
        }

        body {
            margin: 0;
            padding: 0;
            background: var(--bg-deep);
            color: var(--text-primary);
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
            height: 100vh;
            display: flex;
            flex-direction: column;
            overflow: hidden;
        }

        .app-bar {
            padding: 24px 20px 10px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .brand {
            font-size: 1.4rem;
            font-weight: 800;
            background: linear-gradient(135deg, #fff 0%, var(--neon-blue) 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .grid {
            flex: 1;
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            grid-template-rows: repeat(3, 1fr);
            gap: 15px;
            padding: 20px;
            max-width: 500px;
            margin: 0 auto;
            width: 100%;
        }

        .grid-item {
            background: var(--card-bg);
            border: 1px solid var(--card-border);
            border-radius: 28px;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            transition: all 0.2s ease;
            backdrop-filter: blur(10px);
        }

        .grid-item:active { transform: scale(0.92); }

        .icon-box {
            width: 56px;
            height: 56px;
            border-radius: 18px;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 12px;
            font-size: 24px;
        }

        .label { font-size: 1.1rem; font-weight: 600; }
        .sub-label { font-size: 0.75rem; color: var(--text-secondary); }

        .item-1 .icon-box { color: var(--neon-green); border: 1px solid var(--neon-green); }
        .item-2 .icon-box { color: var(--neon-red); border: 1px solid var(--neon-red); }
        .item-3 .icon-box { color: var(--neon-blue); border: 1px solid var(--neon-blue); }
        .item-4 .icon-box { color: var(--neon-gold); border: 1px solid var(--neon-gold); }
        .item-5 .icon-box { color: #a855f7; border: 1px solid #a855f7; }
        .item-6 .icon-box { color: #cbd5e1; border: 1px solid #cbd5e1; }

        .footer-info {
            padding: 20px 30px;
            background: rgba(255,255,255,0.02);
            border-top: 1px solid var(--card-border);
            display: flex;
            justify-content: space-around;
        }

        .stat-value { color: var(--neon-blue); font-weight: 700; }
    </style>
</head>
<body>
    <header class="app-bar">
        <div class="brand">TAOYUAN ELITE</div>
    </header>
    <div class="grid">
        <div class="grid-item item-1">
            <div class="icon-box">⚡</div>
            <div class="label">開工</div>
            <div class="sub-label">接單模式 ON</div>
        </div>
        <div class="grid-item item-2">
            <div class="icon-box">🛑</div>
            <div class="label">下班</div>
            <div class="sub-label">結算數據</div>
        </div>
        <div class="grid-item item-3">
            <div class="icon-box">📅</div>
            <div class="label">排程</div>
            <div class="sub-label">預約單管理</div>
        </div>
        <div class="grid-item item-4">
            <div class="icon-box">💎</div>
            <div class="label">訂閱</div>
            <div class="sub-label">VIP 權限</div>
        </div>
        <div class="grid-item item-5">
            <div class="icon-box">⚠️</div>
            <div class="label">回報</div>
            <div class="sub-label">異常反映</div>
        </div>
        <div class="grid-item item-6">
            <div class="icon-box">🎧</div>
            <div class="label">客服</div>
            <div class="sub-label">專人支援</div>
        </div>
    </div>
    <footer class="footer-info">
        <div><div class="stat-value">12</div><div style="font-size:0.7rem">今日單數</div></div>
        <div><div class="stat-value">$1,850</div><div style="font-size:0.7rem">收入</div></div>
    </footer>
</body>
</html>
