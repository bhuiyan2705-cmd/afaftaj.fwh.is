# afaftaj.fwh.is<!DOCTYPE html>
<html lang="bn">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Afaf | World Command</title>
    <style>
        body { margin: 0; padding: 0; background: #111; color: white; font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; overflow: hidden; }
        
        /* উপরের রিসোর্স বার */
        .top-bar {
            position: fixed; top: 0; width: 100%; height: 50px;
            background: rgba(0, 0, 0, 0.8); display: flex;
            align-items: center; justify-content: space-around;
            border-bottom: 2px solid #555; z-index: 100;
        }
        .stat { display: flex; align-items: center; gap: 5px; font-size: 14px; }
        .stat span { color: #f1c40f; font-weight: bold; }

        /* ম্যাপ কন্টেইনার */
        #map-container {
            width: 100vw; height: 100vh;
            background: url('https://images.unsplash.com/photo-1526778548025-fa2f459cd5c1?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80'); 
            background-size: cover; background-position: center;
            position: relative; cursor: grab;
        }

        /* নিচের নেভিগেশন বার */
        .bottom-nav {
            position: fixed; bottom: 10px; left: 50%; transform: translateX(-50%);
            display: flex; gap: 15px; background: rgba(0,0,0,0.7);
            padding: 10px 25px; border-radius: 50px; border: 1px solid #00ff00;
        }
        .nav-item { width: 40px; height: 40px; background: #333; border-radius: 5px; cursor: pointer; transition: 0.3s; }
        .nav-item:hover { background: #00ff00; transform: scale(1.1); }

        /* VIP ও প্রোফাইল */
        .profile { position: fixed; top: 10px; left: 10px; display: flex; align-items: center; gap: 10px; z-index: 101; }
        .avatar { width: 45px; height: 45px; border-radius: 50%; border: 2px solid #e74c3c; background: #444; }
        .vip-badge { background: #8e44ad; padding: 2px 8px; border-radius: 5px; font-size: 12px; }
    </style>
</head>
<body>

    <div class="profile">
        <div class="avatar"></div>
        <div>
            <div class="vip-badge">VIP - 15</div>
            <div style="font-size: 12px;">CEO: Afaf01</div>
        </div>
    </div>

    <div class="top-bar">
        <div class="stat">🪙 <span>15k</span></div>
        <div class="stat">💎 <span>300</span></div>
        <div class="stat">⚡ <span>434.1M</span></div>
        <div class="stat">🛡️ <span>14.6M</span></div>
    </div>

    <div id="map-container">
        </div>

    <div class="bottom-nav">
        <div class="nav-item" title="ম্যাপ"></div>
        <div class="nav-item" title="সৈন্য"></div>
        <div class="nav-item" title="রিসোর্স"></div>
        <div class="nav-item" title="সেটিংস"></div>
    </div>

</body>
</html>
