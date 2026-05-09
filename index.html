<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <title>中医药翻翻乐 · AI配图+双语朗读</title>
    <style>
        * {
            box-sizing: border-box;
            user-select: none;
        }
        body {
            background: linear-gradient(145deg, #1e4a2f 0%, #0f2f1d 100%);
            font-family: 'Segoe UI', 'PingFang SC', Roboto, system-ui, sans-serif;
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 20px;
            margin: 0;
        }
        .game-container {
            max-width: 800px;
            width: 100%;
            background: rgba(255, 252, 240, 0.97);
            border-radius: 48px;
            padding: 20px 24px 35px;
            box-shadow: 0 25px 40px rgba(0,0,0,0.35);
            text-align: center;
        }
        h1 {
            font-size: 1.9rem;
            margin: 0 0 5px;
            color: #1f5436;
        }
        h1 small {
            font-size: 0.8rem;
            background: #b87a42;
            padding: 4px 12px;
            border-radius: 30px;
            color: white;
            font-weight: normal;
        }
        .lang-bar {
            display: flex;
            justify-content: flex-end;
            gap: 12px;
            margin-bottom: 15px;
        }
        .lang-btn {
            background: #e7dbbd;
            border: none;
            padding: 5px 18px;
            border-radius: 40px;
            font-weight: bold;
            cursor: pointer;
            font-size: 0.85rem;
        }
        .lang-btn.active {
            background: #8b5a2b;
            color: white;
        }
        .category-badge {
            display: inline-block;
            padding: 4px 12px;
            border-radius: 30px;
            font-size: 0.7rem;
            font-weight: bold;
            margin-top: 6px;
        }
        .flip-card-container {
            perspective: 1600px;
            margin: 15px auto;
            width: 100%;
            max-width: 560px;
            cursor: pointer;
        }
        .flip-card {
            background: transparent;
            width: 100%;
            aspect-ratio: 3 / 4;
            position: relative;
            transition: transform 0.5s cubic-bezier(0.2, 0.9, 0.4, 1.1);
            transform-style: preserve-3d;
            border-radius: 32px;
            box-shadow: 0 20px 28px -8px rgba(0,0,0,0.3);
        }
        .flipped {
            transform: rotateY(180deg);
        }
        .front, .back {
            position: absolute;
            width: 100%;
            height: 100%;
            backface-visibility: hidden;
            border-radius: 32px;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            padding: 18px;
            text-align: center;
            box-sizing: border-box;
            border: 1px solid rgba(200, 160, 80, 0.6);
            overflow-y: auto;
        }
        .front {
            transform: rotateY(0deg);
            background: #fffef5;
        }
        .back {
            background: #fef7e0;
            transform: rotateY(180deg);
            justify-content: flex-start;
            align-items: flex-start;
            text-align: left;
            font-size: 0.85rem;
            line-height: 1.45;
        }
        .term-zh {
            font-size: 1.9rem;
            font-weight: 800;
            margin-bottom: 8px;
            color: #2c4d2a;
        }
        .front-img {
            width: 55%;
            max-width: 160px;
            margin: 10px auto;
            border-radius: 20px;
            background: #f4efdf;
            padding: 5px;
            object-fit: cover;
        }
        .img-refresh {
            background: none;
            border: none;
            font-size: 0.7rem;
            cursor: pointer;
            margin-top: 4px;
            color: #a56b2f;
            text-decoration: underline;
        }
        .back-item {
            margin-bottom: 10px;
            width: 100%;
            border-bottom: 1px dashed #dbc28c;
            padding-bottom: 6px;
        }
        .back-label {
            font-weight: bold;
            color: #a56b2f;
            font-size: 0.75rem;
        }
        .back-content {
            font-size: 0.85rem;
            color: #2d3e2a;
        }
        .english-term {
            font-size: 1rem;
            font-weight: bold;
            color: #3b6e47;
            background: #eef3e8;
            padding: 4px 10px;
            border-radius: 40px;
            display: inline-block;
        }
        .audio-btn {
            background: #f2e8d2;
            border: none;
            font-size: 0.9rem;
            cursor: pointer;
            padding: 4px 10px;
            margin-left: 8px;
            border-radius: 30px;
        }
        .nav-buttons {
            display: flex;
            justify-content: center;
            gap: 18px;
            margin: 20px 0 12px;
            flex-wrap: wrap;
        }
        button.nav {
            background: #d9ae6c;
            border: none;
            font-size: 1rem;
            padding: 8px 20px;
            border-radius: 60px;
            font-weight: bold;
            cursor: pointer;
        }
        .random-btn {
            background: #b87c3a;
            color: white;
        }
        .counter {
            background: #e1cfaa;
            display: inline-block;
            padding: 5px 16px;
            border-radius: 30px;
            font-size: 0.85rem;
        }
        .footnote {
            margin-top: 18px;
            font-size: 0.7rem;
            background: #e9e0cc;
            padding: 5px 12px;
            border-radius: 25px;
            display: inline-block;
        }
    </style>
</head>
<body>
<div class="game-container">
    <h1>中药药方 · 翻翻乐 <small>AI配图+语音</small></h1>
    <div class="lang-bar">
        <button class="lang-btn" data-lang="zh">中文界面</button>
        <button class="lang-btn" data-lang="en">English UI</button>
    </div>

    <div class="flip-card-container">
        <div class="flip-card" id="flipCard">
            <div class="front" id="frontFace">
                <div class="term-zh" id="frontZh"></div>
                <div id="categoryBadge" class="category-badge"></div>
                <img id="frontImage" class="front-img" alt="AI生成图" style="display: block;">
                <button class="img-refresh" id="refreshImgBtn">换一张图</button>
            </div>
            <div class="back" id="backFace">
                <div style="display: flex; align-items: center; justify-content: space-between; width: 100%; flex-wrap: wrap;">
                    <span class="english-term" id="backEnTerm"></span>
                    <div>
                        <button class="audio-btn" id="speakZhBtn">中文朗读</button>
                        <button class="audio-btn" id="speakEnBtn">English</button>
                    </div>
                </div>
                <div class="back-item"><div class="back-label">介绍</div><div class="back-content" id="backIntro"></div></div>
                <div class="back-item"><div class="back-label">中文例句</div><div class="back-content" id="backExampleZh"></div></div>
                <div class="back-item"><div class="back-label">英文例句</div><div class="back-content" id="backExampleEn"></div></div>
                <div class="back-item"><div class="back-label">出处</div><div class="back-content" id="backSource"></div></div>
            </div>
        </div>
    </div>

    <div class="nav-buttons">
        <button class="nav" id="prevBtn">上一张</button>
        <button class="nav random-btn" id="randomBtn">随机翻阅</button>
        <button class="nav" id="nextBtn">下一张</button>
    </div>
    <div class="counter" id="counter"></div>
    <div class="footnote">点击卡片翻转 · 图片由AI生成 · 可点“换一张图”重试</div>
</div>

<script>
    // 术语库（已去除白芷，包含药材/炮制/方剂）
    const termsData = [
        { category: "中药药材", zh: "阿胶", en: "E Jiao (Donkey-hide Glue)", intro: "中药名，具有补血滋阴、润燥、止血的功效", example_zh: "阿胶甘平，滋阴补血，为补血要药", example_en: "E Jiao nourishes yin and replenishes blood.", source: "中医养生保健-宁夏" },
        { category: "中药药材", zh: "八角", en: "star anise", intro: "药食同源调味食材", example_zh: "八角是常用的药食同源调味香料", example_en: "Star anise is a common seasoning", source: "药膳与食疗技术" },
        { category: "中药药材", zh: "白芍", en: "Bai Shao (radix paeoniae alba)", intro: "养血调经、敛阴止汗", example_zh: "白芍甘酸微寒，养血敛阴", example_en: "Bai Shao nourishes blood and astringes yin.", source: "中医养生保健-宁夏" },
        { category: "中药药材", zh: "百合", en: "Bai He (bulbus lilii)", intro: "养阴润肺、清心安神", example_zh: "百合主要补肺虚", example_en: "Bai He tonifies Lung deficiency.", source: "中医养生保健-宁夏" },
        { category: "中药药材", zh: "板蓝根", en: "isatis root", intro: "清热解毒", example_zh: "板蓝根可用于肺热、咽喉肿痛", example_en: "Isatis root clears heat", source: "药膳与食疗技术" },
        { category: "中药药材", zh: "沉香", en: "Chen Xiang", intro: "行气止痛、温中止呕", example_zh: "沉香辛微温，质重沉降", example_en: "Chen Xiang is pungent and sinking.", source: "中医养生保健-宁夏" },
        { category: "中药药材", zh: "陈皮", en: "dried tangerine peel", intro: "理气健脾", example_zh: "陈皮可化解痰湿", example_en: "Tangerine peel regulates qi", source: "药膳与食疗技术" },
        { category: "中药药材", zh: "赤小豆", en: "rice bean", intro: "利水消肿", example_zh: "赤小豆适合水肿", example_en: "Rice bean reduces edema", source: "药膳与食疗技术" },
        { category: "中药药材", zh: "当归", en: "Dang Gui", intro: "补血活血、调经止痛", example_zh: "被誉为血中圣药", example_en: "Supreme herb for blood.", source: "中医养生保健-宁夏" },
        { category: "中药药材", zh: "党参", en: "Dangshen", intro: "健脾益肺、养血生津", example_zh: "党参甘味", example_en: "Dangshen is sweet.", source: "中医养生保健-宁夏" },
        { category: "中药药材", zh: "荷叶", en: "He Ye", intro: "清暑化湿、升发清阳", example_zh: "荷叶减肥茶", example_en: "He Ye tea for weight loss", source: "中医养生保健-宁夏" },
        { category: "中药药材", zh: "黑芝麻", en: "Hei Zhi Ma", intro: "补肝肾、益精血", example_zh: "淮药芝麻煳", example_en: "Black sesame paste", source: "中医养生保健-宁夏" },
        { category: "炮制方法", zh: "煲汤", en: "soup making", intro: "药膳常见烹饪方式", example_zh: "煲汤是温补药膳常用方法", example_en: "Soup making for tonic diets", source: "药膳与食疗技术" },
        { category: "炮制方法", zh: "炒", en: "fry", intro: "中药炮制方法", example_zh: "麸炒山药补脾健胃", example_en: "Bran-fried yam strengthens spleen", source: "中医养生保健-宁夏" },
        { category: "炮制方法", zh: "发酵", en: "fermentation", intro: "药膳食材加工", example_zh: "发酵提升吸收效率", example_en: "Fermentation improves absorption", source: "药膳与食疗技术" },
        { category: "炮制方法", zh: "飞", en: "flying", intro: "中药炮制", example_zh: "朱砂需水飞", example_en: "Cinnabar needs flying method", source: "中医养生保健-宁夏" },
        { category: "炮制方法", zh: "煎煮", en: "decoction", intro: "中药/药膳制作", example_zh: "药膳煎煮需掌握火候", example_en: "Decocting needs fire control", source: "药膳与食疗技术" },
        { category: "炮制方法", zh: "炮制", en: "processing", intro: "中药材加工", example_zh: "药食同源食材需规范炮制", example_en: "Medicine-food need processing", source: "药膳与食疗技术" },
        { category: "经典方剂", zh: "八珍糕", en: "Eight-Treasure Cake", intro: "健脾养胃药膳", example_zh: "适合脾胃虚弱者", example_en: "For weak spleen and stomach", source: "药膳与食疗技术" },
        { category: "经典方剂", zh: "菠菜猪肝汤", en: "Spinach and Pork-Liver Soup", intro: "补血养肝", example_zh: "适用于血虚萎黄", example_en: "For blood deficiency", source: "中医养生保健-宁夏" },
        { category: "经典方剂", zh: "虫草炖老鸭", en: "Caterpillar Fungus Stewed Duck", intro: "补肾益肺", example_zh: "适用于久咳虚喘", example_en: "For chronic cough", source: "中医养生保健-宁夏" },
        { category: "经典方剂", zh: "四君子汤", en: "Four Gentlemen Decoction", intro: "益气健脾经典方", example_zh: "气虚体质基础药膳", example_en: "Basic for qi deficiency", source: "药膳与食疗技术" },
        { category: "经典方剂", zh: "乌鸡白凤汤", en: "Silkie Chicken Soup", intro: "补气养血", example_zh: "适用于气血两虚", example_en: "For qi-blood deficiency", source: "中医养生保健-宁夏" },
        { category: "经典方剂", zh: "养肝明目汤", en: "Liver-nourishing Soup", intro: "养肝明目", example_zh: "适用于目赤肿痛", example_en: "For red sore eyes", source: "中医养生保健-宁夏" }
    ];

    // 分类配色
    const categoryColor = {
        "中药药材": "linear-gradient(135deg, #e9f5e6, #d4eaca)",
        "炮制方法": "linear-gradient(135deg, #fff0dd, #ffe2bc)",
        "经典方剂": "linear-gradient(135deg, #f3e7ff, #ecd9ff)"
    };
    const categoryBadgeStyle = {
        "中药药材": { bg: "#588157", color: "white" },
        "炮制方法": { bg: "#c48b3b", color: "white" },
        "经典方剂": { bg: "#9b6b9e", color: "white" }
    };

    let currentIndex = 0;
    let currentLang = "zh";
    let isFlipped = false;
    let currentTerm = null;

    const flipCard = document.getElementById("flipCard");
    const frontZh = document.getElementById("frontZh");
    const categoryBadgeSpan = document.getElementById("categoryBadge");
    const frontImage = document.getElementById("frontImage");
    const backEnTerm = document.getElementById("backEnTerm");
    const backIntro = document.getElementById("backIntro");
    const backExampleZh = document.getElementById("backExampleZh");
    const backExampleEn = document.getElementById("backExampleEn");
    const backSource = document.getElementById("backSource");
    const counterSpan = document.getElementById("counter");
    const frontDiv = document.getElementById("frontFace");

    // 图片生成 (Pollinations AI，带重试)
    function getImageUrl(term, attempt) {
        let prompt = `${term.category} ${term.zh} ${term.en} traditional chinese medicine illustration, clean background, no text`;
        if (attempt > 0) prompt += ` style variation ${attempt}`;
        return `https://image.pollinations.ai/prompt/${encodeURIComponent(prompt)}?width=400&height=400&seed=${Date.now()+attempt}&nologo=1`;
    }

    function loadImageWithRetry(img, term, maxRetries) {
        let retries = 0;
        const tryLoad = () => {
            const url = getImageUrl(term, retries);
            img.src = url;
            img.onerror = () => {
                if (retries < maxRetries) {
                    retries++;
                    setTimeout(tryLoad, 500);
                } else {
                    img.src = "data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 100'%3E%3Crect width='100' height='100' fill='%23e0d5b6'/%3E%3Ctext x='50' y='55' font-size='12' text-anchor='middle' fill='%238b5a2b'%3ETCM%3C/text%3E%3C/svg%3E";
                }
            };
        };
        tryLoad();
    }

    function refreshImage() {
        if (currentTerm) loadImageWithRetry(frontImage, currentTerm, 3);
    }

    function updateCard() {
        currentTerm = termsData[currentIndex];
        const t = currentTerm;
        frontZh.innerText = t.zh;
        categoryBadgeSpan.innerText = t.category;
        const style = categoryBadgeStyle[t.category];
        categoryBadgeSpan.style.backgroundColor = style.bg;
        categoryBadgeSpan.style.color = style.color;
        frontDiv.style.background = categoryColor[t.category] || "#fffef5";
        loadImageWithRetry(frontImage, t, 3);
        backEnTerm.innerText = t.en;
        backIntro.innerText = t.intro;
        backExampleZh.innerText = t.example_zh;
        backExampleEn.innerText = t.example_en;
        backSource.innerText = t.source;
        counterSpan.innerText = (currentIndex+1) + "/" + termsData.length;
        if (isFlipped) {
            flipCard.classList.remove("flipped");
            isFlipped = false;
        }
    }

    function toggleFlip() {
        flipCard.classList.toggle("flipped");
        isFlipped = !isFlipped;
    }
    function nextTerm() { currentIndex = (currentIndex+1) % termsData.length; updateCard(); }
    function prevTerm() { currentIndex = (currentIndex-1+termsData.length) % termsData.length; updateCard(); }
    function randomTerm() { let newIdx; do { newIdx = Math.floor(Math.random()*termsData.length); } while(termsData.length>1 && newIdx===currentIndex); currentIndex = newIdx; updateCard(); }

    // 语音
    function speakText(text, lang) {
        const synth = window.speechSynthesis;
        if (!synth) return;
        synth.cancel();
        const utter = new SpeechSynthesisUtterance(text);
        utter.lang = lang;
        utter.rate = 0.9;
        synth.speak(utter);
    }

    // UI语言切换
    function updateUILanguage() {
        document.querySelectorAll(".lang-btn").forEach(btn => {
            if (btn.getAttribute("data-lang") === currentLang) btn.classList.add("active");
            else btn.classList.remove("active");
        });
        const prevBtn = document.getElementById("prevBtn");
        const nextBtn = document.getElementById("nextBtn");
        const randomBtn = document.getElementById("randomBtn");
        const footnote = document.querySelector(".footnote");
        if (currentLang === "zh") {
            prevBtn.innerText = "上一张";
            nextBtn.innerText = "下一张";
            randomBtn.innerText = "随机翻阅";
            footnote.innerHTML = "点击卡片翻转 · 图片由AI生成 · 可点换一张图";
        } else {
            prevBtn.innerText = "Previous";
            nextBtn.innerText = "Next";
            randomBtn.innerText = "Random";
            footnote.innerHTML = "Tap to flip · AI images · Refresh if needed";
        }
    }

    // 绑定事件
    document.getElementById("prevBtn").addEventListener("click", prevTerm);
    document.getElementById("nextBtn").addEventListener("click", nextTerm);
    document.getElementById("randomBtn").addEventListener("click", randomTerm);
    flipCard.addEventListener("click", toggleFlip);
    document.getElementById("refreshImgBtn").addEventListener("click", (e) => { e.stopPropagation(); refreshImage(); });
    document.getElementById("speakZhBtn").addEventListener("click", (e) => { e.stopPropagation(); if(currentTerm) speakText(currentTerm.zh + "。" + currentTerm.example_zh, "zh-CN"); });
    document.getElementById("speakEnBtn").addEventListener("click", (e) => { e.stopPropagation(); if(currentTerm) speakText(currentTerm.en + ". " + currentTerm.example_en, "en-US"); });
    document.querySelectorAll(".lang-btn").forEach(btn => {
        btn.addEventListener("click", () => { currentLang = btn.getAttribute("data-lang"); updateUILanguage(); });
    });

    updateCard();
    updateUILanguage();
</script>
</body>
</html>
