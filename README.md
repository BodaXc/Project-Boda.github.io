<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>منهج أسس التغذية - Xs.boda</title>
    
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Amiri:ital,wght@0,400;0,700;1,400&family=Cairo:wght@300;600;900&family=Great+Vibes&display=swap" rel="stylesheet">

    <style>
        :root {
            --primary-color: #2c5f78;
            --secondary-color: #d9e8ef;
            --accent-color: #fbbf24; /* لون ذهبي من الهيدر الثاني */
            --text-color: #333;
            --bg-color: #f4f7f6;
            --dark-blue: #1e293b;
        }

        body {
            font-family: 'Cairo', sans-serif;
            background-color: var(--bg-color);
            color: var(--text-color);
            line-height: 1.6;
            margin: 0;
            padding: 0;
        }

        /* تنسيق الهيدر الفخم */
        .main-header {
            background: linear-gradient(135deg, #1e293b 0%, #0f172a 100%);
            color: white;
            padding: 60px 20px;
            text-align: center;
            border-bottom: 5px solid var(--accent-color);
        }

        .brand-name {
            font-family: 'Great Vibes', cursive;
            font-size: 4rem;
            color: var(--accent-color);
            margin: 0 0 10px 0;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
        }

        .course-name {
            font-weight: 300;
            font-size: 1.5rem;
            letter-spacing: 1px;
            opacity: 0.9;
            margin: 10px 0;
        }

        .separator {
            width: 80px;
            border: 1px solid var(--accent-color);
            margin: 20px auto;
        }

        .students-section h3 {
            font-weight: 900;
            font-size: 1.8rem;
            margin-bottom: 20px;
            color: #f8fafc;
        }

        .students-list {
            list-style: none;
            padding: 0;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
            gap: 15px;
            max-width: 1000px;
            margin: 0 auto;
        }

        .students-list li {
            font-family: 'Amiri', serif;
            font-size: 1.1rem;
            background: rgba(255, 255, 255, 0.05);
            padding: 10px;
            border-radius: 8px;
            transition: transform 0.3s ease;
        }

        .students-list li:hover {
            transform: translateY(-5px);
            background: rgba(251, 191, 36, 0.1);
            color: var(--accent-color);
        }

        /* تنسيق المحتوى الرئيسي */
        .container {
            max-width: 1000px;
            margin: 40px auto;
            background: white;
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.1);
        }

        .section-header {
            text-align: center;
            background-color: var(--primary-color);
            color: white;
            padding: 20px;
            border-radius: 10px;
            margin-bottom: 30px;
        }

        .sub-section {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            margin-bottom: 40px;
            padding: 20px;
            border-bottom: 2px solid var(--secondary-color);
            align-items: center;
        }

        .sub-section:last-of-type { border-bottom: none; }

        .content-box {
            flex: 1;
            min-width: 300px;
        }

        .image-placeholder {
            flex: 0 0 250px;
            height: 200px;
            background-color: var(--secondary-color);
            border: 2px dashed var(--primary-color);
            display: flex;
            align-items: center;
            justify-content: center;
            border-radius: 10px;
            color: var(--primary-color);
            font-weight: bold;
            text-align: center;
        }

        h2 { color: var(--primary-color); border-right: 5px solid var(--accent-color); padding-right: 10px; }
        
        .formula {
            background: #eee;
            padding: 10px;
            border-radius: 5px;
            font-family: 'Courier New', Courier, monospace;
            direction: ltr;
            text-align: center;
            margin: 10px 0;
        }

        .tag {
            display: inline-block;
            background: #e67e22;
            color: white;
            padding: 2px 10px;
            border-radius: 5px;
            font-size: 0.9em;
            margin-bottom: 10px;
        }

        /* تنسيق الأكورديون (Details) */
        .section-title {
            background-color: #27ae60;
            color: white;
            padding: 15px;
            border-radius: 5px;
            margin-top: 40px;
            text-align: center;
        }

        details {
            background: #fff;
            margin-bottom: 15px;
            padding: 15px;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            border: 1px solid #eee;
        }

        summary {
            font-weight: bold;
            cursor: pointer;
            outline: none;
            list-style: none;
            color: #2e86de;
            font-size: 1.1rem;
        }

        summary::before { content: "➕ "; }
        details[open] summary::before { content: "➖ "; }
        details[open] { border-right: 5px solid #27ae60; }

        .highlight { color: #d35400; font-weight: bold; }

        /* موبايل ريسبونسيف */
        @media (max-width: 600px) {
            .brand-name { font-size: 2.5rem; }
            .students-list { grid-template-columns: 1fr 1fr; }
            .sub-section { flex-direction: column; }
            .image-placeholder { width: 100%; flex: none; }
        }
    </style>
</head>
<body>

<header class="main-header">
    <div class="overlay">
        <h1 class="brand-name">Xs.boda</h1>
        <h2 class="course-name">أسس التغذية / الاقتصاد المنزلي</h2>
        <hr class="separator">
        <div class="students-section">
            <h3>إعداد الطلاب</h3>
            <ul class="students-list">
                <li>عبدالرحمن مصطفى عويس</li>
                <li>عمر محسن عبد العزيز</li>
                <li>علي عباس علي</li>
                <li>صبري حاتم صبري محمد</li>
                <li>هنا محمود مصطفي محمد</li>
                <li>منه رجب عبد التواب</li>
                <li>هدير احمد مصطفي</li>
                <li>ياسمين ابراهيم احمد</li>
                <li>فاطمه فايز منصور</li>
                <li>منه الله وليد فاروق</li>
            </ul>
        </div>
    </div>
</header>

<div class="container">
    
    <div class="section-header">
        <h1>دليل المذاكرة الشامل: الخميرة والبيتزا</h1>
        <p>خطة تعليمية تفصيلية لمكونات وعمليات العجين</p>
    </div>

    <div class="sub-section">
        <div class="content-box">
            <span class="tag">القسم الأول</span>
            <h2>أساسيات الخميرة</h2>
            <p><strong>التعريف:</strong> كائنات دقيقة غنية بفيتامين B المركب والبروتينات.</p>
            <p><strong>الأنواع:</strong></p>
            <ul>
                <li><strong>خميرة بيرة طازجة:</strong> سريعة المفعول، رطوبة عالية، تحتاج اختبار فوران.</li>
                <li><strong>خميرة بيرة جافة:</strong> حبيبات، صلاحية أطول، تفعيل مختلف.</li>
            </ul>
        </div>
        <div class="image-placeholder">
            [صورة أنواع الخميرة <br> وشكل الخلايا]
        </div>
    </div>

    <div class="sub-section">
        <div class="image-placeholder">
            [صورة مخطط <br> الدفء/الغذاء/الرطوبة]
        </div>
        <div class="content-box">
            <span class="tag">القسم الثاني</span>
            <h2>الظروف المناسبة والكيمياء</h2>
            <p>تحتاج الخميرة للنمو: <strong>الغذاء، الرطوبة، والدفء.</strong></p>
            <p>المعادلة الكيميائية للتخمير:</p>
            <div class="formula">
                Sucrose -> Glucose -> Fructose -> Alcohol + CO2
            </div>
            <p>ينتج غاز $CO_2$ وهو المسؤول عن رفع العجين.</p>
        </div>
    </div>

    <div class="sub-section">
        <div class="content-box">
            <span class="tag">القسم الثالث</span>
            <h2>صنع البيتزا والطرق</h2>
            <ul>
                <li><strong>الطريقة البطيئة:</strong> تخمير متعدد، أفضل قوام.</li>
                <li><strong>الطريقة المعتدلة:</strong> توقيت متوسط.</li>
                <li><strong>الخلط العنيف:</strong> سريعة، خلط أولي أقل.</li>
            </ul>
            <p><strong>المقادير:</strong> دقيق، ملح، زيت، خميرة، سكر، حليب، بيضة.</p>
        </div>
        <div class="image-placeholder">
            [صورة أيقونات المقادير <br> دقيق/زيت/بيض]
        </div>
    </div>

    <h2 class="section-title">📚 ملخص منهج أسس التغذية - الفرقة الأولى</h2>

    <details>
        <summary>1. مقدمة في علم التغذية</summary>
        <div class="content">
            <p><strong>الغذاء:</strong> المادة التي يتناولها الكائن الحي.</p>
            <p><strong>التغذية:</strong> العمليات التي يحول بها الجسم الغذاء إلى طاقة وأنسجة.</p>
            <p><strong>العناصر الغذائية:</strong> المواد الكيميائية في الطعام (كربوهيدرات، بروتينات، إلخ).</p>
            <p><strong>الحالة الغذائية:</strong> حالة الجسم نتيجة لما يتناوله ومدى استفادته منه.</p>
        </div>
    </details>

    <details>
        <summary>2. العناصر الغذائية الكبرى (Macronutrients)</summary>
        <div class="content">
            <p><strong>الكربوهيدرات:</strong> المصدر الرئيسي للطاقة (سكريات، نشويات، ألياف).</p>
            <p><strong>البروتينات:</strong> أحجار البناء، بناء العضلات وترميم الأنسجة.</p>
            <p><strong>الدهون:</strong> مصدر مركز للطاقة، وامتصاص الفيتامينات وحماية الأعضاء.</p>
        </div>
    </details>

    <details>
        <summary>3. العناصر الغذائية الصغرى (Micronutrients)</summary>
        <div class="content">
            <p><span class="highlight">الفيتامينات:</span></p>
            <ul>
                <li>ذائبة في الدهون: (A, D, E, K).</li>
                <li>ذائبة في الماء: (مجموعة B، وفيتامين C).</li>
            </ul>
            <p><strong>الأملاح المعدنية:</strong> الكالسيوم، الحديد، الفسفور، واليود.</p>
        </div>
    </details>

    <details>
        <summary>4. الماء ووظائفه</summary>
        <div class="content">
            <ul>
                <li>تنظيم درجة حرارة الجسم.</li>
                <li>نقل العناصر الغذائية والتخلص من الفضلات.</li>
                <li>وسط للتفاعلات الكيميائية داخل الخلايا.</li>
            </ul>
        </div>
    </details>

    <details>
        <summary>5. عمليات التمثيل الغذائي (Metabolism)</summary>
        <div class="content">
            <p><strong>الهضم:</strong> تحويل الطعام من صورة معقدة إلى بسيطة.</p>
            <p><strong>الامتصاص:</strong> انتقال الغذاء من الأمعاء إلى الدم.</p>
            <p><strong>التمثيل (الأيض):</strong> استغلال العناصر في الطاقة أو البناء.</p>
        </div>
    </details>

    <details>
        <summary>6. الطاقة والقيمة الحرارية</summary>
        <div class="content">
            <ul>
                <li>1 جرام كربوهيدرات = 4 سعرات.</li>
                <li>1 جرام بروتين = 4 سعرات.</li>
                <li>1 جرام دهون = 9 سعرات.</li>
            </ul>
            <p class="highlight">💡 نصيحة: استخدم هذه القيم لحساب احتياجاتك اليومية.</p>
        </div>
    </details>

</div>

<footer style="text-align: center; padding: 20px; color: #777; font-size: 0.9em;">
    &copy; 2024 جميع الحقوق محفوظة لطلاب الفرقة الأولى - قسم الاقتصاد المنزلي
</footer>

</body>
</html>
