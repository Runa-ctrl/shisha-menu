```html
<!DOCTYPE html>
<html lang="bg">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Shisha Point Bar - Меню</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Caveat:wght@400;500;600;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Caveat', cursive;
            background: linear-gradient(135deg, #1a1a2e 0%, #16213e 100%);
            color: #fff;
            padding: 20px;
            line-height: 1.6;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            background: rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 40px;
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.3);
        }

        h1 {
            text-align: center;
            font-size: 3.5em;
            margin-bottom: 10px;
            background: linear-gradient(45deg, #f093fb, #f5576c);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            font-weight: 700;
        }

        .subtitle {
            text-align: center;
            font-size: 1.4em;
            color: #aaa;
            margin-bottom: 40px;
            font-weight: 500;
        }

        .menu-section {
            margin-bottom: 50px;
        }

        .section-title {
            font-size: 2.5em;
            margin-bottom: 20px;
            padding-bottom: 10px;
            border-bottom: 3px solid #f5576c;
            display: flex;
            align-items: center;
            gap: 10px;
            font-weight: 700;
        }

        .menu-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 15px;
        }

        .menu-item {
            background: rgba(255, 255, 255, 0.08);
            padding: 15px 20px;
            border-radius: 10px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            transition: all 0.3s ease;
            border-left: 4px solid transparent;
        }

        .menu-item:hover {
            background: rgba(255, 255, 255, 0.12);
            border-left-color: #f5576c;
            transform: translateX(5px);
        }

        .item-name {
            font-size: 1.4em;
            font-weight: 600;
        }

        .item-details {
            font-size: 1.1em;
            color: #bbb;
            margin-top: 3px;
            font-weight: 400;
        }

        .item-price {
            font-size: 1.6em;
            font-weight: 700;
            color: #f093fb;
            white-space: nowrap;
            margin-left: 15px;
        }

        .hookah-section .menu-item {
            border-left-color: #9d4edd;
        }

        .hookah-section .menu-item:hover {
            border-left-color: #c77dff;
        }

        hr {
            border: none;
            height: 2px;
            background: linear-gradient(90deg, transparent, #f5576c, transparent);
            margin: 50px 0;
        }

        @media (max-width: 768px) {
            .container {
                padding: 20px;
            }

            h1 {
                font-size: 2.5em;
            }

            .section-title {
                font-size: 2em;
            }

            .menu-grid {
                grid-template-columns: 1fr;
            }
        }

        .coming-soon {
            text-align: center;
            color: #888;
            font-style: italic;
            padding: 20px;
            font-size: 1.3em;
        }

        .no-price {
            color: #ff6b6b;
            font-size: 1.1em;
            font-style: italic;
        }

        footer {
            text-align: center;
            margin-top: 60px;
            padding-top: 30px;
            border-top: 2px solid rgba(255, 255, 255, 0.1);
            color: #888;
            font-size: 1.2em;
        }

        footer a {
            color: #f093fb;
            text-decoration: none;
        }

        footer a:hover {
            color: #f5576c;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>☕ SHISHA POINT BAR</h1>
        <p class="subtitle">бул. Македония 16, София | 📞 0887 800 808</p>

        <!-- НАРГИЛЕТА -->
        <div class="menu-section hookah-section">
            <h2 class="section-title">💨 НАРГИЛЕТА / HOOKAH</h2>
            <div class="menu-grid">
                <div class="menu-item">
                    <span class="item-name">TANGIERS</span>
                    <span class="item-price">19.40€</span>
                </div>
                <div class="menu-item">
                    <span class="item-name">DARK SIDE</span>
                    <span class="item-price">18.40€</span>
                </div>
                <div class="menu-item">
                    <span class="item-name">BLACK BURN</span>
                    <span class="item-price">18.40€</span>
                </div>
                <div class="menu-item">
                    <span class="item-name">MUST HAVE</span>
                    <span class="item-price">18.40€</span>
                </div>
                <div class="menu-item">
                    <span class="item-name">O'S</span>
                    <span class="item-price">18.40€</span>
                </div>
                <div class="menu-item">
                    <span class="item-name">SPECTRUM</span>
                    <span class="item-price">18.40€</span>
                </div>
                <div class="menu-item">
                    <span class="item-name">ELEMENT</span>
                    <span class="item-price">18.40€</span>
                </div>
                <div class="menu-item">
                    <span class="item-name">DOZAJ</span>
                    <span class="item-price">18.40€</span>
                </div>
                <div class="menu-item">
                    <span class="item-name">DOZAJ BLACK</span>
                    <span class="item-price">18.40€</span>
                </div>
                <div class="menu-item">
                    <span class="item-name">BRUSKO</span>
                    <span class="item-price">18.40€</span>
                </div>
            </div>
        </div>

        <hr>

        <!-- ЧАЙ -->
        <div class="menu-section">
            <h2 class="section-title">🍵 ЧАЙ / TEA</h2>
            <div class="menu-grid">
                <div class="menu-item">
                    <div>
                        <div class="item-name">Чаша чай</div>
                        <div class="item-details">250ml</div>
                    </div>
                    <span class="item-price">2.50€</span>
                </div>
                <div class="menu-item">
                    <div>
                        <div class="item-name">Чайник</div>
                        <div class="item-details">500ml</div>
                    </div>
                    <span class="item-price">4.80€</span>
                </div>
                <div class="menu-item">
                    <div>
                        <div class="item-name">Турски чай</div>
                        <div class="item-details">130ml</div>
                    </div>
                    <span class="item-price">1.40€</span>
                </div>
            </div>
        </div>

        <hr>

        <!-- БЕЗАЛКОХОЛНИ -->
        <div class="menu-section">
            <h2 class="section-title">🥤 БЕЗАЛКОХОЛНИ / SOFT DRINKS</h2>
            <div class="menu-grid">
                <div class="menu-item">
                    <div>
                        <div class="item-name">Вода</div>
                        <div class="item-details">350ml</div>
                    </div>
                    <span class="item-price">1.50€</span>
                </div>
                <div class="menu-item">
                    <div>
                        <div class="item-name">Вода</div>
                        <div class="item-details">750ml</div>
                    </div>
                    <span class="item-price">2.50€</span>
                </div>
                <div class="menu-item">
                    <div>
                        <div class="item-name">Rilana минерална вода</div>
                        <div class="item-details">330ml</div>
                    </div>
                    <span class="item-price">1.75€</span>
                </div>
                <div class="menu-item">
                    <div>
                        <div class="item-name">Perrier вода</div>
                        <div class="item-details">330ml</div>
                    </div>
                    <span class="item-price">3.30€</span>
                </div>
                <div class="menu-item">
                    <div>
                        <div class="item-name">Сода</div>
                        <div class="item-details">350ml</div>
                    </div>
                    <span class="item-price">1.60€</span>
                </div>
                <div class="menu-item">
                    <div>
                        <div class="item-name">Сода</div>
                        <div class="item-details">750ml</div>
                    </div>
                    <span class="item-price">2.90€</span>
                </div>
                <div class="menu-item">
                    <div>
                        <div class="item-name">Pepsi Twist</div>
                        <div class="item-details">250ml</div>
                    </div>
                    <span class="item-price">2.10€</span>
                </div>
                <div class="menu-item">
                    <div>
                        <div class="item-name">Pepsi</div>
                        <div class="item-details">250ml</div>
                    </div>
                    <span class="item-price">2.10€</span>
                </div>
                <div class="menu-item">
                    <div>
                        <div class="item-name">Pepsi Max</div>
                        <div class="item-details">250ml</div>
                    </div>
                    <span class="item-price">2.10€</span>
                </div>
                <div class="menu-item">
                    <div>
                        <div class="item-name">7UP</div>
                        <div class="item-details">250ml</div>
                    </div>
                    <span class="item-price">2.10€</span>
                </div>
                <div class="menu-item">
                    <div>
                        <div class="item-name">Prisun ябълка</div>
                        <div class="item-details">250ml</div>
                    </div>
                    <span class="item-price">2.20€</span>
                </div>
                <div class="menu-item">
                    <div>
                        <div class="item-name">Prisun праскова</div>
                        <div class="item-details">250ml</div>
                    </div>
                    <span class="item-price">2.20€</span>
                </div>
                <div class="menu-item">
                    <div>
                        <div class="item-name">Prisun вишна</div>
                        <div class="item-details">250ml</div>
                    </div>
                    <span class="item-price">2.20€</span>
                </div>
                <div class="menu-item">
                    <div>
                        <div class="item-name">Prisun портокал</div>
                        <div class="item-details">250ml</div>
                    </div>
                    <span class="item-price">2.20€</span>
                </div>
                <div class="menu-item">
                    <div>
                        <div class="item-name">Prisun ягода и банан</div>
                        <div class="item-details">250ml</div>
                    </div>
                    <span class="item-price">2.20€</span>
                </div>
                <div class="menu-item">
                    <div>
                        <div class="item-name">Lipton лимон</div>
                        <div class="item-details">250ml</div>
                    </div>
                    <span class="item-price">2.50€</span>
                </div>
                <div class="menu-item">
                    <div>
                        <div class="item-name">Lipton праскова</div>
                        <div class="item-details">250ml</div>
                    </div>
                    <span class="item-price">2.50€</span>
                </div>
                <div class="menu-item">
                    <div>
                        <div class="item-name">Vidas студен чай без захар</div>
                        <div class="item-details">250ml</div>
                    </div>
                    <span class="item-price">2.50€</span>
                </div>
                <div class="menu-item">
                    <div>
                        <div class="item-name">Fresh</div>
                        <div class="item-details">250ml</div>
                    </div>
                    <span class="item-price">3.50€</span>
                </div>
                <div class="menu-item">
                    <div>
                        <div class="item-name">Тоник</div>
                        <div class="item-
