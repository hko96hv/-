# -<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>صفحة الكوميكس الشخصية</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f8ff;
            color: #333;
            margin: 0;
            padding: 0;
        }
        .container {
            width: 80%;
            margin: 0 auto;
            padding: 20px;
        }
        header {
            text-align: center;
            background: #4a90e2;
            color: white;
            padding: 20px 0;
        }
        .decorative-images {
            text-align: center;
            margin-bottom: 20px;
        }
        .decorative-images img {
            max-width: 100%;
            height: auto;
            border-radius: 10px;
            margin: 10px 0;
        }
        .section {
            margin-bottom: 30px;
        }
        .section h2 {
            border-bottom: 2px solid #4a90e2;
            padding-bottom: 10px;
            font-size: 1.5em;
        }
        .section ul {
            list-style-type: none;
            padding: 0;
        }
        .section ul li {
            margin: 10px 0;
        }
        .btn {
            display: inline-block;
            padding: 10px 20px;
            margin: 10px 0;
            background-color: #4a90e2;
            color: white;
            text-decoration: none;
            border-radius: 5px;
        }
        .btn:hover {
            background-color: #357abd;
        }
        footer {
            text-align: center;
            padding: 10px 0;
            background: #4a90e2;
            color: white;
        }
        .stats {
            margin-bottom: 30px;
        }
        .stats p {
            font-size: 1.2em;
        }
        .grid-view ul {
            display: flex;
            flex-wrap: wrap;
            padding: 0;
        }
        .grid-view ul li {
            width: calc(25% - 20px);
            margin: 10px;
            list-style-type: none;
            border: 1px solid #ddd;
            padding: 10px;
            box-shadow: 2px 2px 5px rgba(0,0,0,0.1);
            box-sizing: border-box;
        }
    </style>
</head>
<body>
    <header>
        <h1>صفحة الكوميكس الشخصية</h1>
    </header>

    <div class="container">
        <div class="decorative-images">
            <img src="image1.jpg" alt="Decorative Image 1">
            <img src="image2.jpg" alt="Decorative Image 2">
        </div>

        <!-- قسم اختيار طريقة القراءة -->
        <div class="section">
            <h2>اختيار طريقة القراءة</h2>
            <form id="reading-method-form">
                <label>
                    <input type="radio" name="view" value="list" checked> عرض كقائمة
                </label>
                <label>
                    <input type="radio" name="view" value="grid"> عرض كشبكة
                </label>
                <button type="submit" class="btn">تطبيق</button>
            </form>
        </div>

        <!-- قسم الإحصائيات -->
        <div class="stats">
            <h2>إحصائيات القصص</h2>
            <p>عدد القصص التي قرأتها: <span id="read-count">0</span></p>
            <p>عدد القصص التي أكملتها: <span id="completed-count">0</span></p>
            <p>عدد القصص التي لم أكملها: <span id="not-completed-count">0</span></p>
            <p>عدد القصص المفضلة: <span id="favorite-count">0</span></p>
        </div>

        <!-- قسم الشخصيات -->
        <div class="section" id="characters">
            <h2>الشخصيات</h2>
            <ul>
                <li>
                    <strong>شخصية 1</strong> - [تفاصيل حول الشخصية] 
                    <br>
                    <span>اقتباسات: [أفلام/مسلسلات/روايات/لا تملك اقتباس في نوع أدبي آخر]</span>
                </li>
                <li>
                    <strong>شخصية 2</strong> - [تفاصيل حول الشخصية] 
                    <br>
                    <span>اقتباسات: [أفلام/مسلسلات/روايات/لا تملك اقتباس في نوع أدبي آخر]</span>
                </li>
                <!-- أضف المزيد من الشخصيات حسب الحاجة -->
            </ul>
        </div>

        <!-- قسم الأعمال المكتملة -->
        <div class="section" id="completed-works">
            <h2>الأعمال المكتملة</h2>
            <ul>
                <li>قصة 1 - تاريخ الصدور: [تاريخ]، تاريخ الانتهاء: [تاريخ]، التصنيف العمري: [التصنيف العمري]</li>
                <li>قصة 2 - تاريخ الصدور: [تاريخ]، تاريخ الانتهاء: [تاريخ]، التصنيف العمري: [التصنيف العمري]</li>
                <!-- أضف المزيد من القصص المكتملة حسب الحاجة -->
            </ul>
        </div>

        <!-- قسم الأعمال المستمرة -->
        <div class="section" id="ongoing-works">
            <h2>الأعمال المستمرة</h2>
            <ul>
                <li>قصة 1 - تاريخ الصدور: [تاريخ]، مستمر، التصنيف العمري: [التصنيف العمري]</li>
                <li>قصة 2 - تاريخ الصدور: [تاريخ]، مستمر، التصنيف العمري: [التصنيف العمري]</li>
                <!-- أضف المزيد من القصص المستمرة حسب الحاجة -->
            </ul>
        </div>

        <!-- قسم تاريخ الشركات والكتاب -->
        <div class="section" id="companies-writers">
            <h2>تاريخ الشركات والكتاب</h2>
            <p>[تفاصيل حول تاريخ كل شركة وكل كاتب]</p>
            <p>[تفاصيل حول تطور صناعة الكوميكس، كيف بدأت بعض الشخصيات، ظهور شخصيات أخرى، والشخصيات والكتاب الأكثر تأثيرًا]</p>
        </div>

        <!-- قسم التحميل -->
        <div class="section" id="downloads">
            <h2>تحميل</h2>
            <a href="رابط_التحميل_من_ميديا_فاير" class="btn">تحميل الآن</a>
        </div>

        <!-- قسم القصص الحالية والمكتملة -->
        <div class="section" id="current-reading">
            <h2>القصص التي أقرأها حالياً</h2>
            <ul id="current-reading-list">
                <!-- أضف القصص هنا -->
            </ul>
        </div>

        <div class="section" id="completed-stories">
            <h2>القصص التي أكملتها</h2>
            <ul id="completed-stories-list">
                <!-- أضف القصص هنا -->
            </ul>
        </div>

        <!-- قسم الأعمال المتشابهة -->
        <div class="section" id="similar-works">
            <h2>الأعمال المتشابهة</h2>
            <form id="similar-works-form">
                <label for="work-name">اختر عملًا:</label>
                <select id="work-name">
                    <option value="sandman">ساندمان</option>
                    <!-- أضف المزيد من الخيارات هنا -->
                </select>
                <button type="button" id="find-similar-btn">ابحث عن أعمال متشابهة</button>
            </form>
        </div>
    </div>

    <footer>
        <p>&copy; 2024 صفحة الكوميكس الشخصية. جميع الحقوق محفوظة.</p>
    </footer>
</body>
</html>
