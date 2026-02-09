<!DOCTYPE html>
<html lang="zh-TW">
<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>星空的敘事詩：黃道十二宮</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/reveal.js/4.5.0/reveal.min.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/reveal.js/4.5.0/theme/white.min.css">

    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Noto+Serif+TC:wght@400;700&family=Noto+Sans+TC:wght@300;400;500&family=Playfair+Display:ital,wght@0,400;0,700;1,400&display=swap" rel="stylesheet">

    <style>
        /* --- 核心背景設計：Thesis Gradient Style --- */
        body {
            background: linear-gradient(135deg, #fdfbfb 0%, #ebedee 100%); /* 後備色 */
        }
        
        .reveal {
            /* 模擬圖片中的 蜜桃粉 -> 薰衣草紫 柔和漸層光暈 */
            background: linear-gradient(120deg, #fccb90 0%, #d57eeb 100%);
            /* 如果想要更像圖片的模糊光暈，可以使用這行 (Mesh Gradient 模擬) */
            background: radial-gradient(circle at 10% 20%, rgba(255, 228, 200, 0.9) 0%, rgba(255, 228, 200, 0) 50%),
                        radial-gradient(circle at 90% 80%, rgba(200, 180, 255, 0.9) 0%, rgba(200, 180, 255, 0) 50%),
                        linear-gradient(135deg, #ffd1c2 0%, #e0c3fc 100%);
        }

        /* --- 文字排版系統 --- */
        .reveal h1, .reveal h2, .reveal h3, .reveal h4 {
            font-family: 'Playfair Display', 'Noto Serif TC', serif !important;
            color: #2c3e50;
            text-transform: none !important; /* 取消 Reveal.js 預設的全大寫 */
            letter-spacing: 0.02em;
        }

        .reveal p, .reveal li, .reveal span {
            font-family: 'Noto Sans TC', sans-serif;
            color: #444;
            font-weight: 400;
            line-height: 1.6;
        }

        /* --- 玻璃質感卡片設計 (Glassmorphism) --- */
        .glass-card {
            background: rgba(255, 255, 255, 0.65);
            backdrop-filter: blur(10px); /* 毛玻璃模糊效果 */
            -webkit-backdrop-filter: blur(10px);
            border-radius: 15px;
            border: 1px solid rgba(255, 255, 255, 0.4);
            box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.1);
            padding: 40px !important;
            margin: 20px auto !important;
            max-width: 900px;
        }

        /* --- 裝飾性元素 --- */
        .divider-line {
            height: 2px;
            background: linear-gradient(90deg, transparent, #8e44ad, transparent);
            margin: 30px auto;
            width: 60%;
        }

        /* 重點文字強調 */
        strong {
            color: #8e44ad; /* 深紫色強調 */
            font-weight: 700;
        }
        
        /* 列表樣式 */
        .reveal ul {
            display: block;
            text-align: left;
            margin-left: 10%;
        }
        .reveal li {
            margin-bottom: 15px;
        }

        /* 引用/備註樣式 */
        .quote-box {
            font-family: 'Noto Serif TC', serif;
            font-style: italic;
            color: #666;
            border-left: 4px solid #8e44ad;
            padding-left: 20px;
            margin-top: 20px;
            font-size: 0.8em;
        }
    </style>
</head>
<body>

    <div class="reveal">
        <div class="slides">

            <section>
                <div class="glass-card">
                    <h4 style="font-weight:300; letter-spacing: 2px; font-size: 0.8em; margin-bottom:0;">ASTRONOMY & MYTHOLOGY</h4>
                    <h1 style="font-size: 2.5em; margin: 20px 0;">星空的敘事詩</h1>
                    <div class="divider-line"></div>
                    <h2 style="font-size: 1.2em; font-weight: 400;">黃道十二宮與蛇夫座的奧秘</h2>
                    <p style="font-size: 0.7em; margin-top: 50px; opacity: 0.7;">
                        Created for You<br>
                        Feb 2026
                    </p>
                </div>
            </section>

            <section>
                <div class="glass-card">
                    <h3>Contents</h3>
                    <div class="divider-line" style="width: 20%;"></div>
                    <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 20px; text-align: left; margin-top: 30px;">
                        <div>
                            <p><strong>01.</strong> 天文定義</p>
                            <p style="font-size: 0.7em; margin-left: 25px;">黃道與歲差</p>
                        </div>
                        <div>
                            <p><strong>02.</strong> 四元素</p>
                            <p style="font-size: 0.7em; margin-left: 25px;">火、土、風、水</p>
                        </div>
                        <div>
                            <p><strong>03.</strong> 十二宮神話</p>
                            <p style="font-size: 0.7em; margin-left: 25px;">從牡羊到雙魚</p>
                        </div>
                        <div>
                            <p><strong>04.</strong> 神秘客</p>
                            <p style="font-size: 0.7em; margin-left: 25px;">蛇夫座 Ophiuchus</p>
                        </div>
                    </div>
                </div>
            </section>

            <section>
                <div class="glass-card">
                    <h3>什麼是黃道十二宮？</h3>
                    <p class="fragment fade-up">這是一個結合了<strong>天文學</strong>與<strong>占星學</strong>的座標系統。</p>
                    <div class="fragment fade-up" style="text-align: left; font-size: 0.8em; background: rgba(255,255,255,0.5); padding: 20px; border-radius: 10px; margin-top: 20px;">
                        <p>🌞 <strong>黃道 (Ecliptic)：</strong>從地球看過去，太陽在一年中走過的圓形軌道。</p>
                        <p>📏 <strong>十二宮：</strong>將 360 度的圓環平均切分為 12 個區段。</p>
                        <p>⚠️ <strong>關鍵差異：</strong>因地球「歲差」運動，占星日期與實際天象已相差約一個月。</p>
                    </div>
                </div>
            </section>

            <section>
                <div class="glass-card">
                    <h3>四元素與性格特質</h3>
                    <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 20px; font-size: 0.75em;">
                        <div class="fragment fade-in-then-semi-out">
                            <h4>🔥 火象 (Fire)</h4>
                            <p>行動、熱情、勇氣<br><span style="color:#888">牡羊、獅子、射手</span></p>
                        </div>
                        <div class="fragment fade-in-then-semi-out">
                            <h4>🌍 土象 (Earth)</h4>
                            <p>務實、穩定、感官<br><span style="color:#888">金牛、處女、摩羯</span></p>
                        </div>
                        <div class="fragment fade-in-then-semi-out">
                            <h4>🌬️ 風象 (Air)</h4>
                            <p>思考、溝通、社交<br><span style="color:#888">雙子、天秤、水瓶</span></p>
                        </div>
                        <div class="fragment fade-in-then-semi-out">
                            <h4>💧 水象 (Water)</h4>
                            <p>情感、直覺、療癒<br><span style="color:#888">巨蟹、天蠍、雙魚</span></p>
                        </div>
                    </div>
                </div>
            </section>

            <section>
                <div class="glass-card">
                    <h5 style="color: #e74c3c;">ARIES</h5>
                    <h3>牡羊座：救贖的金羊</h3>
                    <div class="divider-line"></div>
                    <ul style="font-size: 0.7em;">
                        <li class="fragment"><strong>神話核心：</strong>金羊 Chrysomallos 犧牲自己拯救王子 Phrixus。</li>
                        <li class="fragment"><strong>悲劇色彩：</strong>妹妹 Helle 途中墜海，這也是「赫勒海峽」的由來。</li>
                        <li class="fragment"><strong>深度象徵：</strong>星空中的金羊昂首回望，象徵著開拓者在前進時，對犧牲者的溫情與遺憾。</li>
                    </ul>
                </div>
            </section>

            <section>
                <div class="glass-card">
                    <h5 style="color: #27ae60;">TAURUS</h5>
                    <h3>金牛座：文明的遷徙</h3>
                    <div class="divider-line"></div>
                    <ul style="font-size: 0.7em;">
                        <li class="fragment"><strong>神話核心：</strong>Zeus 化身為潔白如雪的公牛，誘拐腓尼基公主 Europa 渡海。</li>
                        <li class="fragment"><strong>形象：</strong>星圖中僅有上半身，下半身沒入海中。</li>
                        <li class="fragment"><strong>深度象徵：</strong>穩穩踏浪的公牛，教會我們將靈感透過耐心與實幹，淬煉成美好實相。</li>
                    </ul>
                </div>
            </section>

            <section>
                <div class="glass-card">
                    <h5 style="color: #f1c40f;">GEMINI</h5>
                    <h3>雙子座：跨越神凡的兄弟情</h3>
                    <div class="divider-line"></div>
                    <div style="font-size: 0.7em; text-align: left;">
                        <p class="fragment"><strong>神話：</strong>Pollux (神子) 與 Castor (凡人) 兄弟情深。弟弟戰死後，哥哥不願獨享永生。</p>
                        <p class="fragment"><strong>結局：</strong>Zeus 允許兩人共享生命，輪流往返天界與冥界。</p>
                        <div class="quote-box fragment">
                            「象徵二元性與溝通。他們是連結生與死、神與人的橋樑。」
                        </div>
                    </div>
                </div>
            </section>

            <section>
                <div class="glass-card">
                    <h5 style="color: #8e44ad;">LIBRA</h5>
                    <h3>天秤座：宇宙的平衡</h3>
                    <div class="divider-line"></div>
                    <ul style="font-size: 0.7em;">
                        <li class="fragment"><strong>獨特地位：</strong>黃道中唯一的「無生物」星座。</li>
                        <li class="fragment"><strong>神話源頭：</strong>正義女神 Astraea 的天平，用來衡量靈魂與真理（羽毛）的重量。</li>
                        <li class="fragment"><strong>天文意義：</strong>標示著「秋分」，晝夜長度相等的時刻。</li>
                    </ul>
                </div>
            </section>

            <section>
                <div class="glass-card">
                    <h5 style="color: #c0392b;">SCORPIO</h5>
                    <h3>天蠍座：致命的轉化</h3>
                    <div class="divider-line"></div>
                    <p style="font-size: 0.8em;" class="fragment">
                        獵人 Orion 狂傲誓言殺盡野獸，卻被大地之母派出的小小毒蠍一擊螫死。
                    </p>
                    <p style="font-size: 0.8em;" class="fragment">
                        <strong>象徵意義：</strong>以小博大的力量。它提醒我們，唯有經歷徹底的「毀滅」與面對黑暗，靈魂才能如鳳凰般重生。
                    </p>
                </div>
            </section>

            <section>
                <div class="glass-card">
                    <h5 style="color: #2c3e50;">THE 13TH SIGN</h5>
                    <h3>蛇夫座：Ophiuchus</h3>
                    <div class="divider-line"></div>
                    <div style="display: flex; align-items: center; justify-content: center;">
                        <div style="text-align: left; font-size: 0.7em;">
                            <p class="fragment">🐍 <strong>原型：</strong>醫神 Asclepius，因悟出起死回生術而被 Zeus 雷擊昇天。</p>
                            <p class="fragment">🔭 <strong>天文事實：</strong>太陽每年 11/30 - 12/17 確實經過此區域。</p>
                            <p class="fragment">❓ <strong>為何不是第13宮？</strong><br>古巴比倫人為了維持數學對稱性（12個月/12宮）與四元素循環，將其排除在占星體系之外。</p>
                        </div>
                    </div>
                </div>
            </section>

            <section>
                <div class="glass-card">
                    <h3>結語</h3>
                    <div class="divider-line"></div>
                    <p>黃道十二宮不僅是性格分類，<br>更是一部人類心靈成長的史詩。</p>
                    <br>
                    <p class="fragment fade-up" style="font-size: 0.8em; color: #666;">
                        從牡羊的「誕生」到雙魚的「消融」，<br>
                        仰望星空，我們看見的是古人對人性的深刻洞察。
                    </p>
                    <br>
                    <h4 style="margin-top: 40px;">Thank You</h4>
                </div>
            </section>

        </div>
    </div>

    <script src="https://cdnjs.cloudflare.com/ajax/libs/reveal.js/4.5.0/reveal.min.js"></script>
    <script>
        // 初始化簡報
        Reveal.initialize({
            controls: true,      // 顯示右下角控制箭頭
            progress: true,      // 顯示進度條
            center: true,        // 內容垂直置中
            hash: true,          // 網址列顯示頁碼
            transition: 'fade',  // 轉場效果：fade (淡入淡出) 最符合 Thesis 風格
            backgroundTransition: 'slide'
        });
    </script>
</body>
</html>
