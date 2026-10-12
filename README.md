<!DOCTYPE html>
<html lang="en" dir="ltr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vento Cafe & Restaurant</title>
    <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@600;700&family=Playfair+Display:wght@600;700&family=Tajawal:wght@400;500;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --bg-dark: #0f0f11;
            --card-bg: #18181c;
            --accent-gold: #d4af37;
            --accent-gold-light: #f3e5ab;
            --text-main: #f5f5f7;
            --text-muted: #a1a1aa;
            --border-gold: rgba(212, 175, 55, 0.3);
        }

        * { box-sizing: border-box; margin: 0; padding: 0; }
        
        body {
            background-color: var(--bg-dark);
            color: var(--text-main);
            font-family: 'Tajawal', sans-serif;
            padding-bottom: 40px;
        }

        header {
            background: linear-gradient(180deg, #1c1c22 0%, var(--bg-dark) 100%);
            border-bottom: 1px solid var(--border-gold);
            padding: 20px 15px;
            text-align: center;
            position: sticky;
            top: 0;
            z-index: 100;
        }

        .top-bar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            max-width: 800px;
            margin: 0 auto 10px;
        }

        .logo {
            font-family: 'Cinzel', serif;
            font-size: 26px;
            font-weight: 700;
            color: var(--accent-gold);
            letter-spacing: 2px;
        }

        .lang-btn {
            background: transparent;
            border: 1px solid var(--accent-gold);
            color: var(--accent-gold);
            padding: 6px 14px;
            border-radius: 20px;
            cursor: pointer;
            font-weight: bold;
        }

        .wifi-card {
            background: rgba(212, 175, 55, 0.08);
            border: 1px dashed var(--accent-gold);
            border-radius: 10px;
            padding: 10px;
            max-width: 400px;
            margin: 10px auto;
            font-size: 14px;
            color: var(--accent-gold-light);
        }

        .categories {
            display: flex;
            overflow-x: auto;
            gap: 10px;
            padding: 15px;
            max-width: 800px;
            margin: 0 auto;
            scrollbar-width: none;
        }

        .categories::-webkit-scrollbar { display: none; }

        .cat-btn {
            background: var(--card-bg);
            border: 1px solid rgba(255, 255, 255, 0.1);
            color: var(--text-main);
            padding: 8px 18px;
            border-radius: 20px;
            white-space: nowrap;
            cursor: pointer;
        }

        .cat-btn.active {
            background: var(--accent-gold);
            color: #000;
            font-weight: bold;
            border-color: var(--accent-gold);
        }

        .menu-container {
            max-width: 800px;
            margin: 0 auto;
            padding: 0 15px;
        }

        .menu-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(320px, 1fr));
            gap: 15px;
        }

        .item-card {
            background: var(--card-bg);
            border: 1px solid rgba(255, 255, 255, 0.05);
            border-radius: 12px;
            padding: 15px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
