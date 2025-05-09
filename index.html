<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <title>نظام العدّ للمرشحين</title>
    <style>
        body { 
            font-family: 'Arial', 'Segoe UI', Tahoma, sans-serif;
            padding: 10px; 
            direction: rtl;
            text-align: right;
        }
        .list { 
            margin-bottom: 15px; 
            padding: 10px; 
            border-radius: 5px;
        }
        .list-title {
            font-weight: bold;
            font-size: 1.3em;
            margin-bottom: 10px;
            text-align: center;
            padding: 5px;
        }
        #list1 .list-title { 
            color: red;
            background-color: #ffeeee;
        }
        #list2 .list-title { 
            color: green;
            background-color: #eeffee;
        }
        #list3 .list-title { 
            color: blue;
            background-color: #eeeeff;
        }
        .candidate-row {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            margin-bottom: 8px;
            justify-content: center;
        }
        .candidate-item {
            display: flex;
            align-items: center;
            background: #f5f5f5;
            padding: 5px 10px;
            border-radius: 4px;
            margin: 3px;
            flex-grow: 1;
            max-width: calc(50% - 20px);
            box-shadow: 0 1px 3px rgba(0,0,0,0.1);
        }
        .candidate-name {
            flex-grow: 1;
            margin: 0 8px;
        }
        button { 
            background: #4CAF50; 
            color: white; 
            border: none; 
            padding: 5px 10px; 
            border-radius: 3px; 
            font-size: 0.9em;
            cursor: pointer;
        }
        button:active { 
            background: #45a049; 
        }
        .count {
            min-width: 20px;
            text-align: center;
            font-weight: bold;
        }
        .export { 
            background: #2196F3; 
            margin: 20px auto;
            padding: 10px 20px;
            font-size: 1em;
            display: block;
            border-radius: 5px;
        }
        h1 {
            text-align: center;
            color: #333;
            margin-bottom: 20px;
        }
        @media (max-width: 600px) {
            .candidate-item {
                max-width: 100%;
            }
        }
    </style>
</head>
<body>
    <h1>نظام العدّ للمرشحين</h1>
    
    <!-- القائمة 1 -->
    <div class="list" id="list1">
        <div class="list-title">سوا ضيعتنا اقوى</div>
        <div class="candidate-row" id="list1-candidates"></div>
    </div>
    
    <!-- القائمة 2 -->
    <div class="list" id="list2">
        <div class="list-title">لعيون ضيعتنا</div>
        <div class="candidate-row" id="list2-candidates"></div>
    </div>
    
    <!-- القائمة 3 -->
    <div class="list" id="list3">
        <div class="list-title">القرار والتغيير</div>
        <div class="candidate-row" id="list3-candidates"></div>
    </div>
    
    <button class="export" onclick="exportData()">تصدير البيانات (Excel)</button>
    
    <script>
        // المرشحون
        const candidates = [
            // القائمة 1
            [
                "ماريو حنا عبود",
                "حسن احمد الحاج",
                "كمال نورالدين مقصود",
                "محمد ياسر ضاهر",
                "بلال حكمت الحاج",
                "نبال محمود حامد",
                "غازي ديب الخوري",
                "طلال محمد محمد عبدو",
                "ياسر علي المقصود",
                "خالد احمد علي",
                "مروان مصطفى سعيد",
                "شادي احمد ضاهر",
                "رامي وليد زرزوري",
                "الياس ابراهيم ابراهيم",
                "سامو فيصل عباس"
            ],
            // القائمة 2
            [
                "مصطفى ابراهيم ابراهيم",
                "رامي عادل حداد",
                "حسين مصطفى سعيد",
                "احمد جمال الراعي",
                "محمد احمد عباس",
                "احمد عبد الله يحيا",
                "نزار سميح بيطار",
                "غازي محمد المقصود",
                "مصطفى قاسم ضاهر",
                "خضر علي خضر",
                "علي ابراهيم عثمان",
                "فؤاد سعيد عبدو",
                "سعاد قاسم قاسم",
                "عصام محمد زرزوري"
            ],
            // القائمة 3
            [
                "وليد صبري عباس",
                "شفيق موسى ديب حداد",
                "نريمان اسعد ديب عبود",
                "جمال عامر سعيد",
                "محمد احمد سعيد",
                "احمد خالد طنطاوي",
                "مازن معروف يوسف",
                "حبيب عفيف ابراهيم عبود",
                "ابراهيم احمد يحيى",
                "علاء عطيه عبيد",
                "فهمية محمد العبيدان حيدر",
                "عمر شكري برهان",
                "عبدو محمد عبدو حمود",
                "يسرا احمد الخضر الزرزوري"
            ]
        ];
        
        // العدادات
        let counts = {};
        
        // إنشاء واجهة المرشحين
        function setupLists() {
            candidates.forEach((list, listIndex) => {
                const listDiv = document.getElementById(`list${listIndex+1}-candidates`);
                list.forEach((name, candidateIndex) => {
                    const key = `list${listIndex+1}_${candidateIndex}`;
                    counts[key] = 0;
                    
                    const item = document.createElement("div");
                    item.className = "candidate-item";
                    item.innerHTML = `
                        <button onclick="increment('${key}')">+</button>
                        <span class="count" id="count_${key}">0</span>
                        <span class="candidate-name">${name}</span>
                    `;
                    listDiv.appendChild(item);
                });
            });
        }
        
        // زيادة العداد
        function increment(key) {
            counts[key]++;
            document.getElementById(`count_${key}`).textContent = counts[key];
        }
        
        // تصدير البيانات
        function exportData() {
            let csv = "القائمة,المرشح,عدد الأصوات\n";
            candidates.forEach((list, listIndex) => {
                const listName = document.querySelector(`#list${listIndex+1} .list-title`).textContent;
                list.forEach((name, candidateIndex) => {
                    const key = `list${listIndex+1}_${candidateIndex}`;
                    csv += `"${listName}","${name}",${counts[key]}\n`;
                });
            });
            
            // تنزيل الملف
            const blob = new Blob(["\uFEFF"+csv], { type: 'text/csv;charset=utf-8;' });
            const url = URL.createObjectURL(blob);
            const a = document.createElement('a');
            a.href = url;
            a.download = 'نتائج_العد.csv';
            document.body.appendChild(a);
            a.click();
            document.body.removeChild(a);
        }
        
        // تهيئة الصفحة
        window.onload = setupLists;

        // ===== VIEW-ONLY MODE SCRIPT =====
        // Check if in view-only mode (?view in URL)
        const urlParams = new URLSearchParams(window.location.search);
        if(urlParams.has('view')) {
            // Hide all buttons
            document.querySelectorAll('button').forEach(btn => {
                btn.style.display = 'none';
            });
            // Hide export button
            document.querySelector('.export').style.display = 'none';
            // Add "View Only" to title
            document.title += " (عرض فقط)";
        }
    </script>
</body>
</html>
