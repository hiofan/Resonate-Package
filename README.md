<!DOCTYPE html>
<html lang="zh-TW">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>R⁴esonate达人主播品类专属拍摄方案</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Noto+Sans+TC:wght@400;500;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Noto Sans TC', 'Segoe UI', sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #f8f9fa, #e9ecef);
            color: #343a40;
            padding: 20px;
            min-height: 100vh;
        }
        
        .container {
            max-width: 1400px;
            margin: 0 auto;
        }
        
        header {
            text-align: center;
            padding: 30px 20px;
            background: linear-gradient(120deg, #2c3e50, #1a1a2e);
            color: white;
            border-radius: 12px;
            margin-bottom: 30px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.15);
            position: relative;
            overflow: hidden;
        }
        
        .logo {
            font-size: 2.8rem;
            font-weight: 800;
            margin-bottom: 10px;
            letter-spacing: 2px;
            color: #fff;
            text-shadow: 0 2px 4px rgba(0,0,0,0.3);
        }
        
        .logo span {
            color: #4ecdc4;
        }
        
        .tagline {
            font-size: 1.2rem;
            max-width: 800px;
            margin: 0 auto 20px;
            opacity: 0.9;
        }
        
        h1 {
            font-size: 2.2rem;
            margin-bottom: 15px;
        }
        
        .subtitle {
            font-size: 1.1rem;
            max-width: 800px;
            margin: 0 auto;
            line-height: 1.6;
        }
        
        .tabs-container {
            background: white;
            border-radius: 12px;
            padding: 20px;
            margin-bottom: 30px;
            box-shadow: 0 8px 25px rgba(0,0,0,0.08);
        }
        
        .tabs {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-bottom: 20px;
        }
        
        .tab-btn {
            padding: 12px 25px;
            background: #e9ecef;
            border: none;
            border-radius: 50px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            display: flex;
            align-items: center;
            gap: 8px;
        }
        
        .tab-btn i {
            font-size: 1.2rem;
        }
        
        .tab-btn.active, .tab-btn:hover {
            background: #2c3e50;
            color: white;
        }
        
        .tab-content {
            display: none;
            padding: 20px;
            background: #f8f9fa;
            border-radius: 10px;
        }
        
        .tab-content.active {
            display: block;
            animation: fadeIn 0.5s ease;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .formula-section {
            background: white;
            border-radius: 12px;
            padding: 30px;
            margin-bottom: 30px;
            box-shadow: 0 8px 25px rgba(0,0,0,0.08);
        }
        
        .formula-section h2 {
            text-align: center;
            color: #2c3e50;
            margin-bottom: 25px;
            font-size: 1.8rem;
            padding-bottom: 15px;
            border-bottom: 2px solid #4ecdc4;
        }
        
        .formula-steps {
            display: flex;
            justify-content: space-between;
            flex-wrap: wrap;
            gap: 20px;
        }
        
        .step {
            flex: 1;
            min-width: 250px;
            background: #f8f9fa;
            border-radius: 10px;
            padding: 25px;
            text-align: center;
            position: relative;
            overflow: hidden;
        }
        
        .step::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 5px;
            background: #4ecdc4;
        }
        
        .step-number {
            font-size: 2.5rem;
            font-weight: 800;
            color: #e9ecef;
            position: absolute;
            top: 10px;
            right: 20px;
            z-index: 1;
        }
        
        .step h3 {
            color: #2c3e50;
            margin: 15px 0 10px;
            font-size: 1.4rem;
            position: relative;
            z-index: 2;
        }
        
        .step p {
            color: #495057;
            line-height: 1.6;
            position: relative;
            z-index: 2;
        }
        
        .script-section {
            background: white;
            border-radius: 12px;
            padding: 30px;
            margin-bottom: 30px;
            box-shadow: 0 8px 25px rgba(0,0,0,0.08);
        }
        
        .script-section h2 {
            color: #2c3e50;
            margin-bottom: 25px;
            font-size: 1.8rem;
            text-align: center;
            padding-bottom: 15px;
            border-bottom: 2px solid #4ecdc4;
        }
        
        .script-container {
            display: flex;
            gap: 30px;
            flex-wrap: wrap;
        }
        
        .script-preview {
            flex: 1;
            min-width: 300px;
            background: #f8f9fa;
            border-radius: 10px;
            padding: 25px;
            position: relative;
        }
        
        .script-preview h3 {
            color: #2c3e50;
            margin-bottom: 20px;
            font-size: 1.5rem;
            text-align: center;
        }
        
        .script-content {
            background: white;
            border-radius: 8px;
            padding: 20px;
            height: 400px;
            overflow-y: auto;
            box-shadow: inset 0 0 10px rgba(0,0,0,0.05);
        }
        
        .script-item {
            margin-bottom: 20px;
            padding-bottom: 20px;
            border-bottom: 1px dashed #e9ecef;
        }
        
        .script-time {
            font-weight: 700;
            color: #4ecdc4;
            margin-bottom: 5px;
        }
        
        .script-desc {
            color: #495057;
            line-height: 1.6;
        }
        
        .script-desc strong {
            color: #2c3e50;
        }
        
        .script-desc.highlight {
            background: #fff9db;
            padding: 5px;
            border-radius: 4px;
            display: inline-block;
        }
        
        .tips-section {
            background: white;
            border-radius: 12px;
            padding: 30px;
            margin-bottom: 40px;
            box-shadow: 0 8px 25px rgba(0,0,0,0.08);
        }
        
        .tips-section h2 {
            color: #2c3e50;
            margin-bottom: 25px;
            font-size: 1.8rem;
            text-align: center;
            padding-bottom: 15px;
            border-bottom: 2px solid #4ecdc4;
        }
        
        .tips-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 25px;
        }
        
        .tip-card {
            background: #f8f9fa;
            border-radius: 10px;
            padding: 25px;
            border-left: 4px solid #4ecdc4;
        }
        
        .tip-card h3 {
            color: #2c3e50;
            margin-bottom: 15px;
            font-size: 1.3rem;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .tip-card h3 i {
            color: #4ecdc4;
        }
        
        .tip-card ul {
            padding-left: 20px;
        }
        
        .tip-card li {
            margin-bottom: 10px;
            line-height: 1.6;
        }
        
        .cta-section {
            text-align: center;
            background: linear-gradient(120deg, #2c3e50, #1a1a2e);
            color: white;
            padding: 50px 30px;
            border-radius: 12px;
            margin-bottom: 40px;
        }
        
        .cta-section h2 {
            font-size: 2.2rem;
            margin-bottom: 20px;
        }
        
        .cta-section p {
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto 30px;
            line-height: 1.6;
        }
        
        .cta-button {
            display: inline-block;
            background: #4ecdc4;
            color: white;
            padding: 15px 40px;
            border-radius: 50px;
            font-size: 1.2rem;
            font-weight: 600;
            text-decoration: none;
            transition: all 0.3s ease;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }
        
        .cta-button:hover {
            background: #3dbab1;
            transform: translateY(-3px);
            box-shadow: 0 8px 20px rgba(0,0,0,0.25);
        }
        
        footer {
            text-align: center;
            padding: 25px;
            color: #6c757d;
            font-size: 0.9rem;
        }
        
        .product-highlight {
            background: #e3f2fd;
            padding: 20px;
            border-radius: 8px;
            margin-bottom: 25px;
        }
        
        .product-highlight h3 {
            color: #2c3e50;
            margin-bottom: 15px;
            font-size: 1.4rem;
            text-align: center;
        }
        
        .specs-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 15px;
            margin-bottom: 20px;
        }
        
        .spec-card {
            background: white;
            border-radius: 8px;
            padding: 15px;
            text-align: center;
            box-shadow: 0 3px 10px rgba(0,0,0,0.05);
        }
        
        .spec-card h4 {
            color: #4ecdc4;
            margin-bottom: 8px;
            font-size: 1rem;
        }
        
        .spec-card p {
            color: #495057;
            font-size: 0.95rem;
        }
        
        .feature-list {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            justify-content: center;
        }
        
        .feature-tag {
            background: #4ecdc4;
            color: white;
            padding: 6px 15px;
            border-radius: 20px;
            font-size: 0.9rem;
        }
        
        @media (max-width: 768px) {
            header {
                padding: 20px 15px;
            }
            
            .logo {
                font-size: 2.2rem;
            }
            
            h1 {
                font-size: 1.8rem;
            }
            
            .subtitle {
                font-size: 1rem;
            }
            
            .step {
                min-width: 100%;
            }
            
            .script-container {
                flex-direction: column;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <div class="logo">R⁴<span>esonate</span></div>
            <p class="tagline">天然稻殻纖維 · 抗菌99.9% · 0塑0重金屬0雙酚A</p>
            <h1>达人主播品类专属拍摄方案</h1>
            <p class="subtitle">根据不同产品特性定制高流量拍摄脚本，结合市场验证的流量公式，轻松创作爆款内容</p>
        </header>
        
        <div class="tabs-container">
            <div class="tabs">
                <button class="tab-btn active" data-tab="chopping-board">
                    <i class="fas fa-utensils"></i> 小方菜板
                </button>
                <button class="tab-btn" data-tab="tableware">
                    <i class="fas fa-mug-hot"></i> 稻壳餐具
                </button>
                <button class="tab-btn" data-tab="kids">
                    <i class="fas fa-cookie-bite"></i> 儿童餐具
                </button>
                <button class="tab-btn" data-tab="storage">
                    <i class="fas fa-box-open"></i> 收纳系列
                </button>
                <button class="tab-btn" data-tab="camping">
                    <i class="fas fa-campground"></i> 露营套装
                </button>
            </div>
            
            <div class="tab-content active" id="chopping-board">
                <div class="product-highlight">
                    <h3>小方菜板 - 22cm × 22cm</h3>
                    <div class="specs-grid">
                        <div class="spec-card">
                            <h4>材质</h4>
                            <p>天然稻壳纤维</p>
                        </div>
                        <div class="spec-card">
                            <h4>尺寸</h4>
                            <p>22cm × 22cm</p>
                        </div>
                        <div class="spec-card">
                            <h4>特性</h4>
                            <p>双面两用设计</p>
                        </div>
                        <div class="spec-card">
                            <h4>适用场景</h4>
                            <p>宿舍/宝宝辅食/户外</p>
                        </div>
                    </div>
                    <div class="feature-list">
                        <div class="feature-tag">不发霉</div>
                        <div class="feature-tag">无异味</div>
                        <div class="feature-tag">防滑表面</div>
                        <div class="feature-tag">微波炉适用</div>
                        <div class="feature-tag">洗碗机适用</div>
                        <div class="feature-tag">日式简约</div>
                    </div>
                </div>
                
                <h3>核心卖点与痛点解决方案</h3>
                <ul>
                    <li><strong>空间痛点：</strong> 小尺寸设计解决宿舍/小厨房空间不足问题</li>
                    <li><strong>卫生痛点：</strong> 稻壳材质抗菌99.9%，不发霉无异味</li>
                    <li><strong>功能痛点：</strong> 双面设计（生熟分开）+ 防溢水槽</li>
                    <li><strong>安全痛点：</strong> 0塑0重金属，适合宝宝辅食制作</li>
                    <li><strong>便捷痛点：</strong> 可直接微波加热，洗碗机清洗</li>
                </ul>
            </div>
            
            <div class="tab-content" id="tableware">
                <!-- 其他品类内容 -->
            </div>
        </div>
        
        <div class="formula-section">
            <h2>高流量视频公式（市场验证）</h2>
            <div class="formula-steps">
                <div class="step">
                    <div class="step-number">1</div>
                    <h3>前3秒：强吸引力开场</h3>
                    <p>使用视觉冲击画面或提出痛点问题，瞬间抓住观众注意力</p>
                </div>
                <div class="step">
                    <div class="step-number">2</div>
                    <h3>5-15秒：痛点放大</h3>
                    <p>深入展示用户痛点，引发共鸣和焦虑感</p>
                </div>
                <div class="step">
                    <div class="step-number">3</div>
                    <h3>15-25秒：解决方案</h3>
                    <p>自然引入产品，展示核心功能和优势</p>
                </div>
                <div class="step">
                    <div class="step-number">4</div>
                    <h3>25-40秒：价值证明</h3>
                    <p>通过实验对比、场景演示证明产品效果</p>
                </div>
                <div class="step">
                    <div class="step-number">5</div>
                    <h3>最后5秒：行动号召</h3>
                    <p>限时优惠或紧迫感促使立即行动</p>
                </div>
            </div>
        </div>
        
        <div class="script-section">
            <h2>小方菜板专属拍摄脚本模板</h2>
            <div class="script-container">
                <div class="script-preview">
                    <h3>方案一：痛点解决型</h3>
                    <div class="script-content">
                        <div class="script-item">
                            <div class="script-time">0-3秒</div>
                            <div class="script-desc"><strong>视觉冲击：</strong> 发霉木砧板特写 + 问题字幕"还在用发霉菜板做辅食？"</div>
                        </div>
                        <div class="script-item">
                            <div class="script-time">3-8秒</div>
                            <div class="script-desc"><strong>痛点放大：</strong> "普通菜板用久发霉滋生细菌，危害宝宝健康！"</div>
                        </div>
                        <div class="script-item">
                            <div class="script-time">8-15秒</div>
                            <div class="script-desc"><strong>引入方案：</strong> 展示R⁴esonate小方菜板 + "稻壳材质，天然抗菌99.9%！"</div>
                        </div>
                        <div class="script-item">
                            <div class="script-time">15-25秒</div>
                            <div class="script-desc"><strong>功能演示：</strong> 双面使用展示（一面切水果，一面切肉）+ 防溢水槽演示</div>
                        </div>
                        <div class="script-item">
                            <div class="script-time">25-35秒</div>
                            <div class="script-desc"><strong>场景应用：</strong> 宿舍切水果、制作宝宝辅食、露营使用场景</div>
                        </div>
                        <div class="script-item">
                            <div class="script-time">35-45秒</div>
                            <div class="script-desc"><strong>价值证明：</strong> 实验室报告展示 + 与普通菜板对比实验</div>
                        </div>
                        <div class="script-item">
                            <div class="script-time">最后5秒</div>
                            <div class="script-desc highlight"><strong>行动号召：</strong> "前100名下单送辅食刀具，点击链接立即升级厨房安全！"</div>
                        </div>
                    </div>
                </div>
                
                <div class="script-preview">
                    <h3>方案二：生活方式型</h3>
                    <div class="script-content">
                        <div class="script-item">
                            <div class="script-time">0-3秒</div>
                            <div class="script-desc"><strong>美好场景：</strong> 精致早餐制作过程 + 日式简约厨房展示</div>
                        </div>
                        <div class="script-item">
                            <div class="script-time">3-10秒</div>
                            <div class="script-desc"><strong>问题引入：</strong> "小厨房如何保持整洁又健康？传统菜板太占空间！"</div>
                        </div>
                        <div class="script-item">
                            <div class="script-time">10-18秒</div>
                            <div class="script-desc"><strong>产品亮相：</strong> 小方菜板旋转展示 + "22cm完美尺寸，小空间救星！"</div>
                        </div>
                        <div class="script-item">
                            <div class="script-time">18-28秒</div>
                            <div class="script-desc"><strong>功能演示：</strong> 双面使用切换 + 防滑测试 + 斜面防溢演示</div>
                        </div>
                        <div class="script-item">
                            <div class="script-time">28-38秒</div>
                            <div class="script-desc"><strong>多场景展示：</strong> 宿舍早餐/宝宝辅食/露营野餐/办公室午餐</div>
                        </div>
                        <div class="script-item">
                            <div class="script-time">38-45秒</div>
                            <div class="script-desc"><strong>便捷优势：</strong> 直接放入微波炉加热 + 洗碗机清洗演示</div>
                        </div>
                        <div class="script-item">
                            <div class="script-time">最后5秒</div>
                            <div class="script-desc highlight"><strong>行动号召：</strong> "简约生活从菜板开始！今日下单享8折，点击购买！"</div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        
        <div class="tips-section">
            <h2>高流量创作技巧</h2>
            <div class="tips-grid">
                <div class="tip-card">
                    <h3><i class="fas fa-eye"></i> 前3秒黄金法则</h3>
                    <ul>
                        <li>使用强对比画面：发霉菜板 vs 全新稻壳菜板</li>
                        <li>提出问题："您知道砧板细菌是马桶的200倍吗？"</li>
                        <li>震撼开场：直接敲碎发霉菜板</li>
                        <li>好奇驱动："这个小菜板如何解决大问题？"</li>
                    </ul>
                </div>
                
                <div class="tip-card">
                    <h3><i class="fas fa-flask"></i> 产品演示技巧</h3>
                    <ul>
                        <li>实验对比：普通菜板 vs R⁴esonate 细菌培养测试</li>
                        <li>功能可视化：倒水展示防溢水槽效果</li>
                        <li>暴力测试：用刀猛砍展示耐用性</li>
                        <li>场景切换：快速展示多个使用场景</li>
                    </ul>
                </div>
                
                <div class="tip-card">
                    <h3><i class="fas fa-bullhorn"></i> 转化提升技巧</h3>
                    <ul>
                        <li>紧迫感："前50名赠辅食刀具"</li>
                        <li>社会认同："10万妈妈的选择"</li>
                        <li)解决方案："一套解决所有砧板问题"</li>
                        <li>价格锚点：展示原价划掉，突出优惠价</li>
                    </ul>
                </div>
            </div>
        </div>
        
        <div class="cta-section">
            <h2>获取完整品类拍摄方案手册</h2>
            <p>包含所有品类详细脚本、分镜模板及高流量案例解析</p>
            <a href="#" class="cta-button">立即下载完整资源包</a>
        </div>
        
        <footer>
            <p>R⁴esonate &copy; 2023 - 天然稻壳纤维健康生活倡导者 | 本内容模板可直接复制到Word文档使用</p>
        </footer>
    </div>

    <script>
        // Tab切换功能
        document.querySelectorAll('.tab-btn').forEach(button => {
            button.addEventListener('click', () => {
                // 移除所有active类
                document.querySelectorAll('.tab-btn').forEach(btn => {
                    btn.classList.remove('active');
                });
                document.querySelectorAll('.tab-content').forEach(content => {
                    content.classList.remove('active');
                });
                
                // 添加active类
                button.classList.add('active');
                const tabId = button.getAttribute('data-tab');
                document.getElementById(tabId).classList.add('active');
            });
        });
        
        // 滚动动画
        document.querySelectorAll('.script-content').forEach(el => {
            el.scrollTop = 0;
        });
    </script>
</body>
</html>
