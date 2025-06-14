<!DOCTYPE html>
<html lang="he" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
    <title>בית</title>
    <meta name="description" content="זמני היום">
    
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Alef:wght@400;700&display=swap" rel="stylesheet">

    <style>
        /* CSS - כל העיצוב של האתר נמצא כאן.
           העיצוב מבוסס על הצבעים והסגנונות מהקוד המקורי שלך.
        */

        /* הגדרת משתני צבע ופונט לאחידות בכל האתר */
        :root {
            --color-background: #F7F4EE; /* רקע בז' בהיר */
            --color-surface: #FFFFFF;    /* רקע לבן לאזורי תוכן */
            --color-primary: #827153;    /* חום-אפרפר ראשי לכותרות וכפתורים */
            --color-accent: #CEA964;     /* הדגשה מוזהבת לקווים וקישורים */
            --color-text: #212121;       /* צבע טקסט כהה וקריא */
            --font-main: 'Alef', sans-serif;
        }

        /* עיצוב בסיס כללי */
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: var(--font-main);
            background-color: var(--color-background);
            color: var(--color-text);
            line-height: 1.7; /* מרווח שורות נוח לקריאה */
            font-size: 17px;
        }
        
        /* קונטיינר - ממקם את התוכן במרכז הדף */
        .container {
            width: 90%;
            max-width: 900px;
            margin: 0 auto;
            padding: 60px 20px;
        }
        
        /* ----- אזור כותרת ראשית (Hero) ----- */
        .hero-section {
            /* תמונת הרקע והשכבה הכהה נלקחו מהעיצוב המקורי */
            background-image: linear-gradient(rgba(0, 0, 0, 0.55), rgba(0, 0, 0, 0.55)), url('https://ssl.gstatic.com/atari/images/aristotle-header-dark.jpg');
            background-size: cover;
            background-position: center;
            color: white;
            text-align: center;
            padding: 100px 20px;
        }

        .hero-section h1 {
            font-size: 3.5rem; /* גודל בהשראת הקוד המקורי */
            font-weight: 700;
            margin-bottom: 15px;
        }

        .hero-section p {
            font-size: 1.3rem;
            color: rgba(255, 255, 255, 0.9);
            max-width: 600px;
            margin: 0 auto;
        }
        
        /* ----- טיפוגרפיה אחידה ----- */
        h1, h2, h3 {
            font-weight: 700;
            line-height: 1.3;
            margin-bottom: 25px;
        }
        
        h2 {
            font-size: 2.5rem;
            color: var(--color-primary);
            text-align: center;
        }
        
        /* קו תחתון דקורטיבי לכותרות, בצבע הדגשה */
        h2::after {
            content: '';
            display: block;
            width: 80px;
            height: 4px;
            background-color: var(--color-accent);
            margin: 20px auto 0;
        }

        p {
            margin-bottom: 1.2rem;
        }
        
        a {
            color: var(--color-accent);
            font-weight: 700;
            text-decoration: none;
            transition: color 0.2s;
        }
        a:hover {
            color: var(--color-primary);
        }
        
        /* ----- אזורי תוכן ----- */
        .content-section {
            background-color: var(--color-surface);
        }

        /* ----- כפתורים ----- */
        .button {
            display: inline-block;
            background-color: var(--color-primary);
            color: white;
            padding: 14px 28px;
            border-radius: 50px; /* כפתור מעוגל מודרני */
            font-weight: 700;
            text-decoration: none;
            transition: transform 0.2s ease, background-color 0.2s ease;
        }
        .button:hover {
            background-color: var(--color-accent);
            transform: translateY(-2px); /* אפקט קפיצה קטן */
        }
        .center-button {
            text-align: center;
            margin-top: 30px;
        }
        
        /* ----- פוטר (חלק תחתון) ----- */
        footer {
            background-color: #2c2c2c;
            color: rgba(255, 255, 255, 0.7);
            text-align: center;
            padding: 40px 20px;
        }
        footer a {
            color: white;
        }

        /* התאמה למסכים קטנים (מובייל) */
        @media (max-width: 768px) {
            body {
                font-size: 16px;
            }
            .hero-section h1 {
                font-size: 2.5rem;
            }
            .hero-section p {
                font-size: 1.1rem;
            }
            h2 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>

    <header class="hero-section">
        <h1>זמני היום</h1>
        <p>מקום מרכזי לכל המידע ההלכתי היומי, מוגש בצורה ברורה ונגישה.</p>
    </header>

    <main>

        <section class="content-section">
            <div class="container">
                <h2>אודות</h2>
                <p>
                    פסקה ראשונה של תוכן. החלף את הטקסט הזה בתוכן המקורי מהאתר שלך. תוכל לכתוב כאן על מטרת האתר, על מי שעומד מאחוריו, או כל מידע רלוונטי אחר שתרצה להציג למבקרים.
                </p>
                <p>
                    זוהי פסקה נוספת. ניתן להוסיף כמה פסקאות שרוצים. השפה העיצובית תשמור על מראה ותחושה אחידים בכל חלקי האתר.
                </p>
                <div class="center-button">
                    <a href="#" class="button">ליצירת קשר</a>
                </div>
            </div>
        </section>

        <section>
            <div class="container">
                <h2>מידע נוסף</h2>
                <p>
                    אזור זה יכול להכיל תוכן מסוג אחר. למשל, עדכונים, מאמרים, או קישורים חשובים. העיצוב המשתנה בין הרקעים (לבן ובז') יוצר עניין ויזואלי ומסייע לחלק את התוכן בצורה הגיונית.
                </p>
                <p>
                    החלף את הטקסט הזה בתוכן הרלוונטי שלך.
                </p>
            </div>
        </section>

    </main>

    <footer>
        <p>&copy; <span id="year"></span> כל הזכויות שמורות.</p>
        <p>נבנה ועוצב מחדש על בסיס הרכיבים שלך.</p>
    </footer>

    <script>
        // סקריפט קטן לעדכון אוטומטי של השנה בפוטר
        document.getElementById('year').textContent = new Date().getFullYear();
    </script>

</body>
</html>
