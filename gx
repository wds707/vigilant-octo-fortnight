<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>明觉城·每日共修打卡</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        :root {
            --primary-color: #e6c48c; /* 佛经黄 */
            --secondary-color: #8b4513; /* 檀木棕 */
            --accent-color: #d4a76a; /* 金箔色 */
            --light-bg: #f9f5e9; /* 经卷米白 */
            --dark-bg: #5d4037; /* 深褐 */
            --text-color: #4e342e; /* 深棕 */
            --light-text: #f5f5f5; /* 浅色文字 */
            --success-color: #8bc34a; /* 莲花绿 */
            --border-radius: 12px;
            --shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
        }
        
        body {
            font-family: "Microsoft YaHei", "SimHei", sans-serif;
            background-color: var(--light-bg);
            color: var(--text-color);
            line-height: 1.6;
            background-image: url("data:image/svg+xml,%3Csvg width='100' height='100' viewBox='0 0 100 100' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M11 18c3.866 0 7-3.134 7-7s-3.134-7-7-7-7 3.134-7 7 3.134 7 7 7zm48 25c3.866 0 7-3.134 7-7s-3.134-7-7-7-7 3.134-7 7 3.134 7 7 7zm-43-7c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zm63 31c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zM34 90c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zm56-76c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zM12 86c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm28-65c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm23-11c2.76 0 5-2.24 5-5s-2.24-5-5-5-5 2.24-5 5 2.24 5 5 5zm-6 60c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm29 22c2.76 0 5-2.24 5-5s-2.24-5-5-5-5 2.24-5 5 2.24 5 5 5zM32 63c2.76 0 5-2.24 5-5s-2.24-5-5-5-5 2.24-5 5 2.24 5 5 5zm57-13c2.76 0 5-2.24 5-5s-2.24-5-5-5-5 2.24-5 5 2.24 5 5 5zm-9-21c1.105 0 2-.895 2-2s-.895-2-2-2-2 .895-2 2 .895 2 2 2zM60 91c1.105 0 2-.895 2-2s-.895-2-2-2-2 .895-2 2 .895 2 2 2zM35 41c1.105 0 2-.895 2-2s-.895-2-2-2-2 .895-2 2 .895 2 2 2zM12 60c1.105 0 2-.895 2-2s-.895-2-2-2-2 .895-2 2 .895 2 2 2z' fill='%23e6c48c' fill-opacity='0.05' fill-rule='evenodd'/%3E%3C/svg%3E");
            padding: 10px;
            min-height: 100vh;
        }
        
        .container {
            max-width: 500px;
            margin: 0 auto;
        }
        
        /* 顶部区域 */
        .header {
            text-align: center;
            padding: 20px 15px;
            background: linear-gradient(135deg, var(--secondary-color) 0%, var(--dark-bg) 100%);
            color: var(--light-text);
            border-radius: var(--border-radius);
            margin-bottom: 20px;
            box-shadow: var(--shadow);
            position: relative;
            overflow: hidden;
        }
        
        .header::before {
            content: "卍";
            position: absolute;
            font-size: 120px;
            opacity: 0.1;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
        }
        
        .header h1 {
            font-size: 1.8rem;
            margin-bottom: 8px;
            position: relative;
            letter-spacing: 2px;
        }
        
        .header p {
            font-size: 1rem;
            opacity: 0.9;
            position: relative;
        }
        
        .date-display {
            font-size: 1.1rem;
            margin-top: 10px;
            position: relative;
            color: var(--accent-color);
        }
        
        @keyframes gentlePulse {
            0%, 100% { opacity: 0.9; }
            50% { opacity: 1; }
        }
        
        /* 打卡主区域 */
        .checkin-card {
            background-color: white;
            border-radius: var(--border-radius);
            padding: 25px;
            margin-bottom: 20px;
            box-shadow: var(--shadow);
            border: 1px solid rgba(139, 69, 19, 0.1);
        }
        
        .checkin-title {
            display: flex;
            align-items: center;
            margin-bottom: 20px;
            padding-bottom: 15px;
            border-bottom: 1px dashed var(--accent-color);
        }
        
        .lotus-icon {
            color: var(--primary-color);
            font-size: 1.8rem;
            margin-right: 12px;
        }
        
        .checkin-title h2 {
            font-size: 1.5rem;
            color: var(--secondary-color);
        }
        
        .practices-list {
            margin-bottom: 25px;
        }
        
        .practice-item {
            display: flex;
            align-items: center;
            padding: 12px 0;
            border-bottom: 1px solid rgba(0, 0, 0, 0.05);
        }
        
        .practice-item:last-child {
            border-bottom: none;
        }
        
        .practice-name {
            flex: 2.5;
            padding: 10px 12px;
            border: 1px solid #ddd;
            border-radius: 8px;
            font-size: 1rem;
            background-color: #fafafa;
            min-width: 0;
        }
        
        .practice-unit-group {
            display: flex;
            align-items: center;
            flex: 1.5;
            margin: 0 8px;
        }
        
        .practice-amount {
            width: 50px;
            padding: 10px 8px;
            border: 1px solid #ddd;
            border-radius: 8px 0 0 8px;
            font-size: 1rem;
            background-color: #fafafa;
            text-align: center;
        }
        
        .practice-amount:invalid {
            border-color: #ff6b6b;
        }
        
        .unit-text {
            padding: 10px 8px;
            border: 1px solid #ddd;
            border-left: none;
            border-radius: 0 8px 8px 0;
            font-size: 0.9rem;
            background-color: #f9f9f9;
            min-width: 40px;
            text-align: center;
        }
        
        .practice-toggle {
            position: relative;
            width: 50px;
            height: 28px;
            flex-shrink: 0;
        }
        
        .practice-toggle input {
            opacity: 0;
            width: 0;
            height: 0;
        }
        
        .toggle-slider {
            position: absolute;
            cursor: pointer;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background-color: #ccc;
            transition: .4s;
            border-radius: 34px;
        }
        
        .toggle-slider:before {
            position: absolute;
            content: "";
            height: 20px;
            width: 20px;
            left: 4px;
            bottom: 4px;
            background-color: white;
            transition: .4s;
            border-radius: 50%;
        }
        
        input:checked + .toggle-slider {
            background-color: var(--success-color);
        }
        
        input:checked + .toggle-slider:before {
            transform: translateX(22px);
        }
        
        .checkin-button {
            display: block;
            width: 100%;
            padding: 18px;
            background: linear-gradient(to right, var(--primary-color), var(--accent-color));
            color: var(--text-color);
            border: none;
            border-radius: var(--border-radius);
            font-size: 1.3rem;
            font-weight: bold;
            cursor: pointer;
            transition: all 0.3s;
            margin-top: 10px;
            letter-spacing: 3px;
            box-shadow: 0 4px 8px rgba(139, 69, 19, 0.2);
        }
        
        .checkin-button:hover, .checkin-button:active {
            transform: translateY(-2px);
            box-shadow: 0 6px 12px rgba(139, 69, 19, 0.3);
        }
        
        .checkin-button.checked {
            background: linear-gradient(to right, var(--success-color), #7cb342);
            color: white;
        }
        
        .checkin-button:disabled {
            background: #ccc;
            cursor: not-allowed;
            transform: none;
            box-shadow: none;
        }
        
        /* 进度统计 */
        .stats-card {
            background-color: white;
            border-radius: var(--border-radius);
            padding: 20px;
            margin-bottom: 20px;
            box-shadow: var(--shadow);
        }
        
        .stats-title {
            display: flex;
            align-items: center;
            margin-bottom: 20px;
            color: var(--secondary-color);
        }
        
        .stats-icon {
            color: var(--primary-color);
            font-size: 1.5rem;
            margin-right: 10px;
        }
        
        .stats-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 15px;
        }
        
        .stat-item {
            text-align: center;
            padding: 15px 10px;
            background-color: var(--light-bg);
            border-radius: 10px;
        }
        
        .stat-value {
            font-size: 2rem;
            font-weight: bold;
            color: var(--secondary-color);
            margin-bottom: 5px;
        }
        
        .stat-label {
            font-size: 0.9rem;
            color: #777;
        }
        
        /* 今日法语 */
        .dharma-card {
            background-color: white;
            border-radius: var(--border-radius);
            padding: 20px;
            margin-bottom: 20px;
            box-shadow: var(--shadow);
            position: relative;
            border-left: 5px solid var(--accent-color);
        }
        
        .dharma-title {
            color: var(--secondary-color);
            margin-bottom: 15px;
            display: flex;
            align-items: center;
        }
        
        .dharma-icon {
            color: var(--primary-color);
            margin-right: 10px;
        }
        
        .dharma-text {
            font-size: 1.1rem;
            line-height: 1.8;
            color: var(--text-color);
            font-style: italic;
            text-align: justify;
        }
        
        .dharma-source {
            text-align: right;
            margin-top: 10px;
            color: #888;
            font-size: 0.9rem;
        }
        
        /* 鼓励语提示 */
        .encouragement-toast {
            position: fixed;
            bottom: 20px;
            left: 50%;
            transform: translateX(-50%) translateY(100px);
            background-color: var(--success-color);
            color: white;
            padding: 12px 24px;
            border-radius: 30px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
            z-index: 1000;
            opacity: 0;
            transition: all 0.3s ease;
        }
        
        .encouragement-toast.show {
            opacity: 1;
            transform: translateX(-50%) translateY(0);
        }
        
        /* 底部 */
        .footer {
            text-align: center;
            padding: 20px;
            color: #888;
            font-size: 0.9rem;
        }
        
        .sutra-link {
            color: var(--secondary-color);
            text-decoration: none;
            border-bottom: 1px dotted var(--secondary-color);
        }
        
        /* 响应式调整 */
        @media (max-width: 480px) {
            .header h1 {
                font-size: 1.5rem;
            }
            
            .checkin-card, .stats-card, .dharma-card {
                padding: 20px 15px;
            }
            
            .practice-item {
                flex-wrap: wrap;
            }
            
            .practice-name {
                flex: 2.5;
                font-size: 0.9rem;
                padding: 8px 10px;
                min-width: 120px;
            }
            
            .practice-unit-group {
                flex: 1.8;
                margin: 0 5px;
            }
            
            .practice-amount {
                width: 40px;
                padding: 8px 6px;
                font-size: 0.9rem;
            }
            
            .unit-text {
                padding: 8px 6px;
                font-size: 0.8rem;
                min-width: 35px;
            }
            
            .practice-toggle {
                width: 45px;
                height: 26px;
            }
            
            input:checked + .toggle-slider:before {
                transform: translateX(19px);
            }
        }
        
        /* 动画效果 */
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .fade-in {
            animation: fadeIn 0.5s ease-out;
        }
        
        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.05); }
            100% { transform: scale(1); }
        }
        
        .pulse {
            animation: pulse 0.5s ease-in-out;
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- 顶部区域 -->
        <header class="header">
            <h1>明觉城·每日共修打卡</h1>
            <p>精进修行 日积月累 功不唐捐</p>
            <div class="date-display" id="currentDate">2026年2月8日 星期日</div>
        </header>
        
        <!-- 打卡主区域 -->
        <main class="checkin-card fade-in">
            <div class="checkin-title">
                <i class="fas fa-spa lotus-icon"></i>
                <h2>今日功课完成情况</h2>
            </div>
            
            <div class="practices-list" id="practicesList">
                <!-- 10个可自定义的功课行将由JavaScript动态生成 -->
            </div>
            
            <button class="checkin-button" id="checkinBtn">
                <i class="fas fa-check-circle"></i> 完成今日共修
            </button>
        </main>
        
        <!-- 进度统计 -->
        <section class="stats-card fade-in">
            <div class="stats-title">
                <i class="fas fa-chart-line stats-icon"></i>
                <h2>修行进度</h2>
            </div>
            
            <div class="stats-grid">
                <div class="stat-item">
                    <div class="stat-value" id="currentStreak">0</div>
                    <div class="stat-label">连续打卡</div>
                </div>
                
                <div class="stat-item">
                    <div class="stat-value" id="totalDays">0</div>
                    <div class="stat-label">累计天数</div>
                </div>
                
                <div class="stat-item">
                    <div class="stat-value" id="todayParticipants">0</div>
                    <div class="stat-label">今日共修</div>
                </div>
                
                <div class="stat-item">
                    <div class="stat-value" id="completionRate">0%</div>
                    <div class="stat-label">完成率</div>
                </div>
            </div>
        </section>
        
        <!-- 今日法语 -->
        <section class="dharma-card fade-in">
            <div class="dharma-title">
                <i class="fas fa-quote-left dharma-icon"></i>
                <h2>今日法语</h2>
            </div>
            <p class="dharma-text" id="dharmaText">一切有为法，如梦幻泡影，如露亦如电，应作如是观。</p>
            <div class="dharma-source" id="dharmaSource">——《金刚经》</div>
        </section>
        
        <!-- 底部 -->
        <footer class="footer">
            <p>愿以此功德 庄严佛净土 上报四重恩 下济三途苦</p>
            <p>若有见闻者 悉发菩提心 尽此一报身 同生极乐国</p>
            <p>明觉城共修打卡系统 · <a href="#" class="sutra-link">《回向文》</a></p>
        </footer>
        
        <!-- 鼓励语提示 -->
        <div class="encouragement-toast" id="encouragementToast">
            <span id="encouragementText">随喜赞叹！功德无量！</span>
        </div>
    </div>

    <script>
        // 获取DOM元素
        const currentDateEl = document.getElementById('currentDate');
        const checkinBtn = document.getElementById('checkinBtn');
        const practicesListEl = document.getElementById('practicesList');
        const encouragementToast = document.getElementById('encouragementToast');
        const encouragementText = document.getElementById('encouragementText');
        
        // 统计元素
        const currentStreakEl = document.getElementById('currentStreak');
        const totalDaysEl = document.getElementById('totalDays');
        const todayParticipantsEl = document.getElementById('todayParticipants');
        const completionRateEl = document.getElementById('completionRate');
        
        // 法语元素
        const dharmaTextEl = document.getElementById('dharmaText');
        const dharmaSourceEl = document.getElementById('dharmaSource');
        
        // 初始化数据
        let isCheckedIn = false;
        let currentStreak = 0;
        let totalDays = 0;
        let todayParticipants = 0;
        
        // 默认功课数据（10行）- 数量已清零
        const defaultPractices = [
            { name: "金刚经", amount: "", unit: "部", checked: false },
            { name: "地藏经", amount: "", unit: "部", checked: false },
            { name: "准提神咒", amount: "", unit: "遍", checked: false },
            { name: "念佛", amount: "", unit: "声", checked: false },
            { name: "静坐", amount: "", unit: "分钟", checked: false },
            { name: "行善", amount: "", unit: "次", checked: false },
            { name: "大礼拜", amount: "", unit: "拜", checked: false },
            { name: "诵咒", amount: "", unit: "遍", checked: false },
            { name: "阅经", amount: "", unit: "卷", checked: false },
            { name: "放生", amount: "", unit: "次", checked: false }
        ];
        
        // 鼓励语库
        const encouragementQuotes = [
            "功德无量！随喜赞叹！",
            "精进不懈，道业早成！",
            "善哉善哉！福慧双增！",
            "日日精进，早证菩提！",
            "修行路上，感恩有您同行！",
            "持之以恒，必得法益！",
            "勇猛精进，功德圆满！",
            "一念虔诚，一份功德！",
            "修行无倦，福报无边！",
            "精进修行，自利利他！"
        ];
        
        // 今日法语库
        const dharmaQuotes = [
            {
                text: "一切有为法，如梦幻泡影，如露亦如电，应作如是观。",
                source: "——《金刚经》"
            },
            {
                text: "色不异空，空不异色，色即是空，空即是色。",
                source: "——《心经》"
            },
            {
                text: "若人散乱心，入于塔庙中，一称南无佛，皆共成佛道。",
                source: "——《法华经》"
            },
            {
                text: "念佛一声，福增无量；礼佛一拜，罪灭河沙。",
                source: "——净土宗语录"
            },
            {
                text: "诸恶莫作，众善奉行，自净其意，是诸佛教。",
                source: "——《法句经》"
            },
            {
                text: "人生在世如身处荆棘之中，心不动，人不妄动，不动则不伤。",
                source: "——禅宗语录"
            },
            {
                text: "过去心不可得，现在心不可得，未来心不可得。",
                source: "——《金刚经》"
            },
            {
                text: "凡所有相，皆是虚妄。若见诸相非相，即见如来。",
                source: "——《金刚经》"
            },
            {
                text: "是日已过，命亦随减，如少水鱼，斯有何乐？",
                source: "——《法句经》"
            },
            {
                text: "愿我来世，得菩提时，身如琉璃，内外明澈，净无瑕秽。",
                source: "——《药师琉璃光如来本愿功德经》"
            }
        ];
        
        // 初始化日期显示
        function initDate() {
            const now = new Date();
            const options = { year: 'numeric', month: 'long', day: 'numeric', weekday: 'long' };
            const dateStr = now.toLocaleDateString('zh-CN', options);
            
            currentDateEl.textContent = dateStr;
        }
        
        // 初始化今日法语
        function initDharmaQuote() {
            // 根据日期选择不同的法语，确保每天变化
            const today = new Date();
            const dayOfYear = Math.floor((today - new Date(today.getFullYear(), 0, 0)) / 1000 / 60 / 60 / 24);
            const randomIndex = dayOfYear % dharmaQuotes.length;
            
            dharmaTextEl.textContent = dharmaQuotes[randomIndex].text;
            dharmaSourceEl.textContent = dharmaQuotes[randomIndex].source;
        }
        
        // 初始化功课列表
        function initPracticesList() {
            practicesListEl.innerHTML = '';
            
            // 从localStorage加载数据或使用默认数据
            let practices = loadPracticesData();
            
            // 生成10个功课行
            for (let i = 0; i < 10; i++) {
                const practice = practices[i] || { name: "", amount: "", unit: "", checked: false };
                
                const practiceItem = document.createElement('div');
                practiceItem.className = 'practice-item fade-in';
                practiceItem.style.animationDelay = `${i * 0.05}s`;
                
                practiceItem.innerHTML = `
                    <input type="text" class="practice-name" placeholder="功课名称" value="${practice.name}" data-index="${i}">
                    <div class="practice-unit-group">
                        <input type="number" class="practice-amount" placeholder="数" value="${practice.amount}" data-index="${i}" min="1" step="1">
                        <div class="unit-text" data-index="${i}">${practice.unit}</div>
                    </div>
                    <label class="practice-toggle">
                        <input type="checkbox" class="practice-checkbox" ${practice.checked ? 'checked' : ''} data-index="${i}">
                        <span class="toggle-slider"></span>
                    </label>
                `;
                
                practicesListEl.appendChild(practiceItem);
            }
            
            // 添加输入框事件监听
            const nameInputs = document.querySelectorAll('.practice-name');
            const amountInputs = document.querySelectorAll('.practice-amount');
            const checkboxes = document.querySelectorAll('.practice-checkbox');
            
            nameInputs.forEach(input => {
                input.addEventListener('input', function() {
                    savePracticesData();
                    updateStatsDisplay();
                    validateCheckinButton();
                });
            });
            
            amountInputs.forEach(input => {
                input.addEventListener('input', function() {
                    savePracticesData();
                    updateStatsDisplay();
                    validateCheckinButton();
                    
                    // 检查对应的打卡开关是否需要禁用
                    const index = this.getAttribute('data-index');
                    const checkbox = document.querySelector(`.practice-checkbox[data-index="${index}"]`);
                    if (checkbox.checked && (!this.value || parseInt(this.value) < 1)) {
                        checkbox.checked = false;
                        savePracticesData();
                        updateStatsDisplay();
                        validateCheckinButton();
                    }
                });
            });
            
            checkboxes.forEach(checkbox => {
                checkbox.addEventListener('change', function() {
                    const index = this.getAttribute('data-index');
                    const amountInput = document.querySelector(`.practice-amount[data-index="${index}"]`);
                    
                    // 检查数量框是否有有效数字
                    if (this.checked) {
                        if (!amountInput.value || parseInt(amountInput.value) < 1) {
                            this.checked = false;
                            alert("请先填写完成数量，然后才能点亮打卡图标");
                            return;
                        }
                    }
                    
                    savePracticesData();
                    updateStatsDisplay();
                    validateCheckinButton();
                    
                    // 如果是从未选中变为选中，显示鼓励语
                    if (this.checked) {
                        showEncouragement();
                    }
                });
            });
        }
        
        // 验证打卡按钮状态
        function validateCheckinButton() {
            const practices = loadPracticesData();
            const completedCount = practices.filter(p => p.checked).length;
            
            // 检查是否有勾选的项目
            if (completedCount === 0) {
                checkinBtn.disabled = true;
                return;
            }
            
            // 检查勾选的项目是否有数量填写
            const hasInvalidAmount = practices.some(p => {
                if (p.checked) {
                    // 如果勾选了但数量为空，则不允许打卡
                    if (p.amount === "" || p.amount === null || p.amount === undefined) {
                        return true;
                    }
                    // 如果数量不是有效数字
                    if (isNaN(parseInt(p.amount)) || parseInt(p.amount) < 1) {
                        return true;
                    }
                }
                return false;
            });
            
            checkinBtn.disabled = hasInvalidAmount;
        }
        
        // 从localStorage加载功课数据
        function loadPracticesData() {
            const savedData = localStorage.getItem('buddhistPracticesData');
            if (savedData) {
                return JSON.parse(savedData);
            }
            return defaultPractices;
        }
        
        // 保存功课数据到localStorage
        function savePracticesData() {
            const practices = [];
            const nameInputs = document.querySelectorAll('.practice-name');
            const amountInputs = document.querySelectorAll('.practice-amount');
            const unitTexts = document.querySelectorAll('.unit-text');
            const checkboxes = document.querySelectorAll('.practice-checkbox');
            
            for (let i = 0; i < 10; i++) {
                practices.push({
                    name: nameInputs[i]?.value || "",
                    amount: amountInputs[i]?.value || "",
                    unit: unitTexts[i]?.textContent || "",
                    checked: checkboxes[i]?.checked || false
                });
            }
            
            localStorage.setItem('buddhistPracticesData', JSON.stringify(practices));
        }
        
        // 从localStorage加载统计数据
        function loadStatsData() {
            const savedData = localStorage.getItem('buddhistStatsData');
            if (savedData) {
                const data = JSON.parse(savedData);
                
                // 检查是否是同一天
                const today = new Date().toDateString();
                const lastCheckinDate = data.lastCheckinDate;
                
                if (lastCheckinDate === today) {
                    // 如果是同一天，恢复打卡状态
                    isCheckedIn = data.isCheckedIn;
                    currentStreak = data.currentStreak || 0;
                    totalDays = data.totalDays || 0;
                    todayParticipants = data.todayParticipants || Math.floor(Math.random() * 20) + 15;
                    
                    // 恢复复选框状态
                    if (data.practices) {
                        const checkboxes = document.querySelectorAll('.practice-checkbox');
                        for (let i = 0; i < Math.min(10, data.practices.length); i++) {
                            if (checkboxes[i]) {
                                checkboxes[i].checked = data.practices[i].checked || false;
                            }
                        }
                    }
                } else {
                    // 新的一天，重置打卡状态
                    isCheckedIn = false;
                    
                    // 检查是否是连续的一天
                    const lastDate = new Date(lastCheckinDate);
                    const currentDate = new Date();
                    const timeDiff = currentDate.getTime() - lastDate.getTime();
                    const dayDiff = Math.floor(timeDiff / (1000 * 3600 * 24));
                    
                    if (dayDiff === 1 && data.isCheckedIn) {
                        // 如果昨天打卡了，连续打卡加1
                        currentStreak = (data.currentStreak || 0) + 1;
                    } else if (dayDiff > 1) {
                        // 如果间隔超过一天，连续打卡清零
                        currentStreak = 0;
                    } else {
                        // 其他情况保持原连续打卡
                        currentStreak = data.currentStreak || 0;
                    }
                    
                    totalDays = data.totalDays || 0;
                    todayParticipants = Math.floor(Math.random() * 20) + 15;
                    
                    // 保存新数据
                    saveData();
                }
                
                // 更新显示
                updateStatsDisplay();
                updateCheckinButton();
                validateCheckinButton();
            } else {
                // 初始数据
                currentStreak = 0;
                totalDays = 0;
                todayParticipants = Math.floor(Math.random() * 20) + 15;
                updateStatsDisplay();
                validateCheckinButton();
            }
        }
        
        // 保存数据到localStorage
        function saveData() {
            const today = new Date().toDateString();
            const practices = loadPracticesData();
            
            const data = {
                lastCheckinDate: today,
                isCheckedIn: isCheckedIn,
                currentStreak: currentStreak,
                totalDays: totalDays,
                todayParticipants: todayParticipants,
                practices: practices
            };
            
            localStorage.setItem('buddhistStatsData', JSON.stringify(data));
        }
        
        // 更新统计显示
        function updateStatsDisplay() {
            const practices = loadPracticesData();
            const completedCount = practices.filter(p => p.checked).length;
            const totalCount = practices.filter(p => p.name.trim() !== "").length;
            
            currentStreakEl.textContent = currentStreak;
            totalDaysEl.textContent = totalDays;
            todayParticipantsEl.textContent = todayParticipants;
            
            // 计算完成率
            const completionRate = totalCount > 0 ? Math.round((completedCount / totalCount) * 100) : 0;
            completionRateEl.textContent = `${completionRate}%`;
        }
        
        // 更新打卡按钮状态
        function updateCheckinButton() {
            if (isCheckedIn) {
                checkinBtn.innerHTML = '<i class="fas fa-check-circle"></i> 今日已完成打卡';
                checkinBtn.classList.add('checked');
                checkinBtn.disabled = true;
            } else {
                checkinBtn.innerHTML = '<i class="fas fa-check-circle"></i> 完成今日共修';
                checkinBtn.classList.remove('checked');
            }
        }
        
        // 显示鼓励语
        function showEncouragement() {
            const randomIndex = Math.floor(Math.random() * encouragementQuotes.length);
            encouragementText.textContent = encouragementQuotes[randomIndex];
            
            encouragementToast.classList.add('show');
            
            setTimeout(() => {
                encouragementToast.classList.remove('show');
            }, 3000);
        }
        
        // 处理打卡
        function handleCheckin() {
            if (isCheckedIn) return;
            
            // 检查至少完成一项功课
            const practices = loadPracticesData();
            const completedCount = practices.filter(p => p.checked).length;
            
            if (completedCount === 0) {
                alert("请至少完成一项功课再打卡");
                return;
            }
            
            // 检查勾选的功课是否都有有效数量
            const invalidPractices = practices.filter(p => {
                if (p.checked) {
                    return p.amount === "" || p.amount === null || p.amount === undefined || 
                           isNaN(parseInt(p.amount)) || parseInt(p.amount) <= 0;
                }
                return false;
            });
            
            if (invalidPractices.length > 0) {
                alert("请为已完成的功课填写有效数量");
                return;
            }
            
            // 更新状态
            isCheckedIn = true;
            
            // 检查是否是今天第一次打卡
            const today = new Date().toDateString();
            const savedData = localStorage.getItem('buddhistStatsData');
            let lastCheckinDate = "";
            
            if (savedData) {
                const data = JSON.parse(savedData);
                lastCheckinDate = data.lastCheckinDate;
            }
            
            // 如果是新的一天，更新连续打卡和累计天数
            if (lastCheckinDate !== today) {
                // 检查昨天是否打卡
                const lastDate = new Date(lastCheckinDate);
                const currentDate = new Date();
                const timeDiff = currentDate.getTime() - lastDate.getTime();
                const dayDiff = Math.floor(timeDiff / (1000 * 3600 * 24));
                
                if (dayDiff === 1) {
                    // 昨天打卡了，连续打卡加1
                    currentStreak++;
                } else if (dayDiff > 1) {
                    // 间隔超过一天，连续打卡重置为1
                    currentStreak = 1;
                } else {
                    // 同一天或无效日期，连续打卡加0（不应该发生）
                }
                
                // 累计天数加1
                totalDays++;
            }
            
            todayParticipants++;
            
            // 更新显示
            updateStatsDisplay();
            updateCheckinButton();
            
            // 保存数据
            saveData();
            
            // 添加动画效果
            checkinBtn.classList.add('pulse');
            setTimeout(() => {
                checkinBtn.classList.remove('pulse');
            }, 500);
            
            // 显示打卡成功消息
            const messages = [
                "今日共修完成！功德无量！",
                "精进不懈，道业早成！随喜赞叹！",
                "共修圆满！愿您福慧双增！",
                "修行路上，感恩有您同行！"
            ];
            const randomMessage = messages[Math.floor(Math.random() * messages.length)];
            alert(`打卡成功！${randomMessage}`);
        }
        
        // 初始化
        document.addEventListener('DOMContentLoaded', function() {
            initDate();
            initDharmaQuote();
            loadStatsData();
            initPracticesList();
            
            // 添加事件监听
            checkinBtn.addEventListener('click', handleCheckin);
            
            // 添加一些初始动画
            const elements = document.querySelectorAll('.fade-in');
            elements.forEach((el, index) => {
                el.style.animationDelay = `${index * 0.1}s`;
            });
        });
    </script>
</body>
</html>
