<!DOCTYPE html>
<html lang="zh-TW">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>蘆小姐保險保障深度分析報告</title>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <style>
        body {
            font-family: 'Microsoft JhengHei', Arial, sans-serif;
            line-height: 1.6;
            color: #333;
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
            background-color: #f9f9f9;
        }
        .header {
            background: linear-gradient(135deg, #0056b3 0%, #003366 100%);
            color: white;
            padding: 30px;
            text-align: center;
            border-radius: 10px;
            margin-bottom: 30px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
        }
        .section {
            background-color: white;
            padding: 25px;
            margin-bottom: 30px;
            border-radius: 10px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        h1, h2, h3 {
            color: #0056b3;
        }
        h1 {
            margin: 0;
            font-size: 28px;
        }
        h2 {
            border-bottom: 2px solid #0056b3;
            padding-bottom: 10px;
            margin-top: 30px;
        }
        h3 {
            color: #333;
            margin-top: 20px;
        }
        .chart-container {
            margin: 30px 0;
            text-align: center;
            background-color: #f5f5f5;
            padding: 20px;
            border-radius: 5px;
            position: relative;
            height: 400px;
        }
        .chart-title {
            font-weight: bold;
            margin-bottom: 10px;
            color: #0056b3;
        }
        .gap-analysis {
            background-color: #fff8e1;
            padding: 20px;
            border-left: 5px solid #ffc107;
            margin: 20px 0;
        }
        .recommendation {
            background-color: #e8f5e9;
            padding: 20px;
            border-left: 5px solid #4caf50;
            margin: 20px 0;
        }
        .warning {
            background-color: #ffebee;
            padding: 20px;
            border-left: 5px solid #f44336;
            margin: 20px 0;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
        }
        th, td {
            border: 1px solid #ddd;
            padding: 12px;
            text-align: left;
        }
        th {
            background-color: #0056b3;
            color: white;
        }
        tr:nth-child(even) {
            background-color: #f2f2f2;
        }
        .highlight {
            background-color: #fffde7;
            padding: 15px;
            border-radius: 5px;
            margin: 20px 0;
        }
        .footer {
            text-align: center;
            margin-top: 50px;
            padding: 20px;
            color: #666;
            font-size: 14px;
        }
        .cta-button {
            display: inline-block;
            background-color: #e53935;
            color: white;
            padding: 15px 30px;
            text-decoration: none;
            border-radius: 5px;
            font-weight: bold;
            margin: 20px 0;
            transition: background-color 0.3s;
        }
        .cta-button:hover {
            background-color: #c62828;
        }
        .two-column {
            display: flex;
            justify-content: space-between;
            flex-wrap: wrap;
        }
        .column {
            width: 48%;
            min-width: 300px;
        }
        .exclusion-list {
            list-style-type: none;
            padding-left: 0;
        }
        .exclusion-list li {
            padding: 10px;
            border-bottom: 1px solid #eee;
            position: relative;
            padding-left: 30px;
        }
        .exclusion-list li:before {
            content: "✖";
            color: #f44336;
            position: absolute;
            left: 0;
            font-weight: bold;
        }
        @media (max-width: 768px) {
            .column {
                width: 100%;
            }
        }
        .medical-process {
            background-color: #f5f5f5;
            padding: 20px;
            border-radius: 5px;
            margin: 20px 0;
        }
        .process-step {
            display: flex;
            margin-bottom: 15px;
            align-items: center;
        }
        .process-icon {
            width: 40px;
            height: 40px;
            background-color: #0056b3;
            color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-right: 15px;
            flex-shrink: 0;
        }
        .process-content {
            flex-grow: 1;
        }
        .process-cost {
            background-color: #ffebee;
            padding: 5px 10px;
            border-radius: 3px;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <div class="header">
        <h1>蘆小姐保險保障深度分析報告</h1>
        <p>專業風險評估 · 理賠限制解析 · 全方位保障建議</p>
    </div>

    <div class="section">
        <h2>現有保單保障與理賠限制分析</h2>
        
        <div class="two-column">
            <div class="column">
                <h3>現有保障摘要</h3>
                <ul>
                    <li>意外身故：105.48萬</li>
                    <li>住院日額：1,000元/日</li>
                    <li>手術保障：3,000-8萬元</li>
                    <li>傷害醫療限額：5萬元</li>
                </ul>
            </div>
            <div class="column">
                <h3>主要保障缺口</h3>
                <ul>
                    <li>無實支實付醫療險</li>
                    <li>重大疾病保障不足</li>
                    <li>癌症保障嚴重不足</li>
                    <li>無長期照顧保障</li>
                </ul>
            </div>
        </div>
        
        <div class="warning">
            <h3>舊保單的「不賠」條款與漏洞</h3>
            <ul class="exclusion-list">
                <li><strong>自費醫材不賠：</strong>達文西手術、特殊醫材、新型治療等自費項目不予理賠</li>
                <li><strong>門診治療限制：</strong>多數門診治療（如癌症標靶治療）不在保障範圍內</li>
                <li><strong>術前檢查不賠：</strong>MRI、CT等術前必要檢查費用不予給付</li>
                <li><strong>術後復健排除：</strong>物理治療、職能治療等術後復健費用不在保障內</li>
                <li><strong>雜費限額過低：</strong>5萬傷害醫療限額無法支應重大手術雜費</li>
                <li><strong>住院天數限制：</strong>部分條款對加護病房天數有嚴格限制</li>
            </ul>
        </div>
    </div>

    <div class="section">
        <h2>醫療自費支出趨勢分析</h2>
        
        <div class="chart-container">
            <div class="chart-title">圖1：台灣醫療自費比例趨勢（2015-2023）</div>
            <canvas id="trendChart"></canvas>
            <p>根據健保署統計，醫療自費比例從2015年的18%上升至2023年的32%，其中手術相關自費項目增長最為明顯。</p>
        </div>
        
        <div class="two-column">
            <div class="column">
                <div class="chart-container">
                    <div class="chart-title">圖2：住院自費項目比例分布</div>
                    <canvas id="pieChart"></canvas>
                    <p>手術材料費佔自費項目42%，為最大支出項目，現有保單對此類費用保障嚴重不足。</p>
                </div>
            </div>
            <div class="column">
                <div class="chart-container">
                    <div class="chart-title">圖3：各類手術自費金額比較</div>
                    <canvas id="barChart"></canvas>
                    <p>心臟手術平均自費25萬元，骨科手術18萬元，均遠超現有保單5萬元的傷害醫療限額。</p>
                </div>
            </div>
        </div>
    </div>

    <div class="section">
        <h2>手術全過程費用分析 vs 現有保障</h2>
        
        <div class="medical-process">
            <div class="process-step">
                <div class="process-icon">1</div>
                <div class="process-content">
                    <strong>術前檢查階段</strong>
                    <p>MRI、CT、心電圖等必要檢查</p>
                    <div class="process-cost">平均自費：8,000-15,000元</div>
                </div>
            </div>
            <div class="process-step">
                <div class="process-icon">2</div>
                <div class="process-content">
                    <strong>手術進行階段</strong>
                    <p>特殊醫材、達文西機械手臂、麻醉</p>
                    <div class="process-cost">平均自費：50,000-200,000元</div>
                </div>
            </div>
            <div class="process-step">
                <div class="process-icon">3</div>
                <div class="process-content">
                    <strong>住院恢復階段</strong>
                    <p>單人病房差額、自費藥物、營養品</p>
                    <div class="process-cost">平均自費：3,000-10,000元/日</div>
                </div>
            </div>
            <div class="process-step">
                <div class="process-icon">4</div>
                <div class="process-content">
                    <strong>術後復健階段</strong>
                    <p>物理治療、職能治療、輔具</p>
                    <div class="process-cost">平均自費：2,000-5,000元/次</div>
                </div>
            </div>
        </div>
        
        <div class="chart-container">
            <div class="chart-title">圖4：手術全過程費用 vs 現有保障對比圖</div>
            <canvas id="comparisonChart"></canvas>
            <p>現有保障僅能覆蓋約15-20%的實際醫療支出，且多數高額自費項目不在保障範圍內。</p>
        </div>
    </div>

    <div class="section">
        <h2>重大疾病風險分析</h2>
        
        <div class="two-column">
            <div class="column">
                <h3>台灣十大癌症治療費用</h3>
                <table>
                    <tr>
                        <th>癌症類型</th>
                        <th>平均治療費用</th>
                    </tr>
                    <tr>
                        <td>肺癌</td>
                        <td>80-150萬</td>
                    </tr>
                    <tr>
                        <td>大腸癌</td>
                        <td>60-120萬</td>
                    </tr>
                    <tr>
                        <td>乳癌</td>
                        <td>50-100萬</td>
                    </tr>
                    <tr>
                        <td>肝癌</td>
                        <td>70-130萬</td>
                    </tr>
                </table>
                <p>現有癌症身故僅5.48萬，無法支應治療費用。</p>
            </div>
            <div class="column">
                <h3>女性重大疾病發生率</h3>
                <ul>
                    <li>30歲女性罹癌機率：約10%</li>
                    <li>40歲女性罹癌機率：約18%</li>
                    <li>女性一生中需重大手術機率：約70%</li>
                    <li>住院超過2週機率：約45%</li>
                </ul>
                <p>數據來源：衛福部國民健康署</p>
            </div>
        </div>
    </div>

    <div class="recommendation">
        <h2>保障升級緊急建議</h2>
        
        <div class="two-column">
            <div class="column">
                <h3>女性必備保障項目</h3>
                <ol>
                    <li><strong>實支實付醫療險</strong> - 建議額度30萬/次</li>
                    <li><strong>重大疾病險</strong> - 一次性給付100萬</li>
                    <li><strong>女性癌症險</strong> - 特別加強乳癌、子宮頸癌保障</li>
                    <li><strong>手術全過程保障</strong> - 涵蓋術前術後費用</li>
                </ol>
            </div>
            <div class="column">
                <h3>為什麼現在就該行動？</h3>
                <ul>
                    <li>女性30歲後保費逐年增加5-10%</li>
                    <li>婦科健康變化可能導致拒保</li>
                    <li>女性癌症發生率逐年上升</li>
                    <li>現有保障缺口等於財務漏洞</li>
                </ul>
            </div>
        </div>
        
        <div style="text-align: center; margin-top: 30px;">
            <a href="#" class="cta-button">立即預約女性專屬保障規劃</a>
            <p>限時提供女性保單健檢優惠，名額有限</p>
        </div>
    </div>

    <div class="footer">
        <p>本報告依據公開數據及專業分析製作，實際保障內容以保單條款為準</p>
        <p>國泰人壽保險股份有限公司 © 2023 版權所有</p>
    </div>

    <script>
        // 圖1：台灣醫療自費比例趨勢折線圖
        const trendCtx = document.getElementById('trendChart').getContext('2d');
        const trendChart = new Chart(trendCtx, {
            type: 'line',
            data: {
                labels: ['2015', '2016', '2017', '2018', '2019', '2020', '2021', '2022', '2023'],
                datasets: [{
                    label: '醫療自費比例 (%)',
                    data: [18, 20, 22, 24, 26, 27, 29, 30, 32],
                    borderColor: '#0056b3',
                    backgroundColor: 'rgba(0, 86, 179, 0.1)',
                    borderWidth: 3,
                    fill: true,
                    tension: 0.3
                }]
            },
            options: {
                responsive: true,
                maintainAspectRatio: false,
                scales: {
                    y: {
                        beginAtZero: true,
                        title: {
                            display: true,
                            text: '自費比例 (%)'
                        }
                    }
                }
            }
        });

        // 圖2：住院自費項目比例分布圓餅圖
        const pieCtx = document.getElementById('pieChart').getContext('2d');
        const pieChart = new Chart(pieCtx, {
            type: 'pie',
            data: {
                labels: ['手術材料費', '特殊檢查費', '自費藥物', '病房差額', '其他'],
                datasets: [{
                    data: [42, 25, 18, 10, 5],
                    backgroundColor: [
                        '#0056b3',
                        '#4caf50',
                        '#ff9800',
                        '#9c27b0',
                        '#f44336'
                    ],
                    borderWidth: 1
                }]
            },
            options: {
                responsive: true,
                maintainAspectRatio: false,
                plugins: {
                    legend: {
                        position: 'right'
                    }
                }
            }
        });

        // 圖3：各類手術自費金額比較柱狀圖
        const barCtx = document.getElementById('barChart').getContext('2d');
        const barChart = new Chart(barCtx, {
            type: 'bar',
            data: {
                labels: ['心臟手術', '骨科手術', '婦科手術', '腸胃手術', '神經外科'],
                datasets: [{
                    label: '平均自費金額 (萬元)',
                    data: [25, 18, 15, 12, 22],
                    backgroundColor: [
                        'rgba(0, 86, 179, 0.7)',
                        'rgba(0, 86, 179, 0.7)',
                        'rgba(0, 86, 179, 0.7)',
                        'rgba(0, 86, 179, 0.7)',
                        'rgba(0, 86, 179, 0.7)'
                    ],
                    borderColor: [
                        '#0056b3',
                        '#0056b3',
                        '#0056b3',
                        '#0056b3',
                        '#0056b3'
                    ],
                    borderWidth: 1
                }]
            },
            options: {
                responsive: true,
                maintainAspectRatio: false,
                scales: {
                    y: {
                        beginAtZero: true,
                        title: {
                            display: true,
                            text: '自費金額 (萬元)'
                        }
                    }
                }
            }
        });

        // 圖4：手術全過程費用 vs 現有保障對比圖
        const comparisonCtx = document.getElementById('comparisonChart').getContext('2d');
        const comparisonChart = new Chart(comparisonCtx, {
            type: 'bar',
            data: {
                labels: ['術前檢查', '手術進行', '住院恢復', '術後復健'],
                datasets: [
                    {
                        label: '實際自費支出 (元)',
                        data: [12000, 150000, 50000, 20000],
                        backgroundColor: 'rgba(244, 67, 54, 0.7)',
                        borderColor: '#f44336',
                        borderWidth: 1
                    },
                    {
                        label: '現有保障給付 (元)',
                        data: [0, 30000, 10000, 0],
                        backgroundColor: 'rgba(0, 86, 179, 0.7)',
                        borderColor: '#0056b3',
                        borderWidth: 1
                    }
                ]
            },
            options: {
                responsive: true,
                maintainAspectRatio: false,
                scales: {
                    y: {
                        beginAtZero: true,
                        title: {
                            display: true,
                            text: '金額 (元)'
                        }
                    }
                }
            }
        });
    </script>
</body>
</html>
