<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>تطبيق إصال</title>

<style>
* {
    box-sizing: border-box;
}

body {
    margin: 0;
    padding: 22px 16px 30px;
    font-family: Arial, sans-serif;
    background: #ffffff;
    color: #493426;
}

.container {
    width: 100%;
    max-width: 500px;
    margin: auto;
}

/* رأس التطبيق */
.header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 12px;
    margin-bottom: 26px;
    animation: fadeIn 0.8s ease both;
}

.brand {
    display: flex;
    flex-direction: column;
    gap: 5px;
}

.brand-name {
    color: #c95b16;
    font-size: 34px;
    font-weight: 900;
    margin: 0;
}

.tagline {
    font-size: 13px;
    color: #493426;
    margin: 0;
}

.logo-icon {
    width: 58px;
    height: 58px;
    min-width: 58px;
    border-radius: 50%;
    background: #f5ead9;
    border: 1px solid #f0e5d9;
    display: flex;
    align-items: center;
    justify-content: center;
}

.logo-icon svg {
    width: 30px;
    height: 30px;
}

/* بطاقة اكتشف ما يناسبك */
.intro {
    background: #f5ead9;
    border: 1px solid #eee0cf;
    border-radius: 23px;
    padding: 23px 18px;
    margin-bottom: 24px;
    animation: fadeIn 0.9s ease both;
}

.intro h2 {
    font-size: 22px;
    margin: 0 0 10px;
    color: #493426;
}

.intro p {
    font-size: 14px;
    line-height: 1.8;
    margin: 0;
    color: #746050;
}

/* بطاقات الاختيار */
.choice {
    display: flex;
    flex-direction: column;
    position: relative;
    width: 100%;
    margin-bottom: 19px;
    overflow: hidden;
    border-radius: 24px;
    background: transparent;
    border: none;
    text-decoration: none;
    color: #493426;
    box-shadow: none;
    opacity: 0;
    transform: translateY(35px) scale(0.94);
    animation: arrive 0.8s cubic-bezier(.2,.8,.2,1) forwards;
}

.choice:nth-of-type(1) {
    animation-delay: 0.25s;
}

.choice.second {
    animation-delay: 0.75s;
}

/* الصورة في الأعلى */
.choice img {
    width: 100%;
    height: 190px;
    object-fit: cover;
    display: block;
    border-radius: 24px;
    transition: transform 0.5s ease;
}

.choice:active img {
    transform: scale(1.02);
}

/* العنوان والوصف والسهم تحت الصورة بدون إطار */
.choice-content {
    position: static;
    z-index: 2;
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 12px;
    padding: 16px 4px;
    background: transparent;
    border: none;
    box-shadow: none;
    border-radius: 0;
}

.choice-text {
    flex: 1;
    min-width: 0;
}

.choice-text h3 {
    font-size: 20px;
    margin: 0 0 8px;
    font-weight: 800;
    color: #493426;
}

.choice-text p {
    font-size: 13px;
    line-height: 1.7;
    margin: 0;
    color: #746050;
}

/* السهم البرتقالي */
.arrow {
    width: 43px;
    height: 43px;
    min-width: 43px;
    border-radius: 50%;
    background: #c95b16;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 25px;
    color: #ffffff;
}

/* الحركات */
@keyframes fadeIn {
    from {
        opacity: 0;
        transform: translateY(12px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

@keyframes arrive {
    0% {
        opacity: 0;
        transform: translateY(35px) scale(0.94);
    }
    70% {
        opacity: 1;
        transform: translateY(-4px) scale(1.01);
    }
    100% {
        opacity: 1;
        transform: translateY(0) scale(1);
    }
}

/* الهواتف الصغيرة */
@media (max-width: 360px) {
    body {
        padding: 18px 12px 25px;
    }

    .choice img {
        height: 165px;
    }

    .choice-text h3 {
        font-size: 18px;
    }

    .intro h2 {
        font-size: 20px;
    }
}

/* احترام إعدادات تقليل الحركة */
@media (prefers-reduced-motion: reduce) {
    *, *::before, *::after {
        animation-duration: 0.01ms !important;
        animation-iteration-count: 1 !important;
        transition-duration: 0.01ms !important;
    }

    .choice {
        opacity: 1;
        transform: none;
    }
}
</style>
</head>

<body>

<div class="container">

    <!-- رأس التطبيق -->
    <header class="header">
        <div class="brand">
            <h1 class="brand-name">إصال</h1>
            <p class="tagline">اختيارات أكثر لحياتك اليومية</p>
        </div>

        <div class="logo-icon">
            <svg viewBox="0 0 24 24" fill="none"
                 stroke="#c95b16" stroke-width="2"
                 stroke-linecap="round" stroke-linejoin="round"
                 aria-hidden="true">
                <path d="M12 2.5l1.8 6.2L20 11l-6.2 1.8L12 19l-1.8-6.2L4 11l6.2-2.3L12 2.5z"></path>
                <path d="M19 15l1 2.5 2.5 1-2.5 1-1 2.5-1-2.5-2.5-1 2.5-1 1-2.5z"></path>
            </svg>
        </div>
    </header>

    <!-- بطاقة اكتشف ما يناسبك -->
    <section class="intro">
        <h2>اكتشف ما يناسبك</h2>
        <p>تجربة سهلة لاكتشاف العروض والتخفيضات</p>
    </section>

    <!-- الخيار الأول -->
    <a class="choice"
       href="https://isal.trinavo.com/">

        <img
            src="https://i.postimg.cc/kGjg4wQG/image-c7761245.jpg"
            alt="العروض والتخفيضات"
            loading="eager">

        <div class="choice-content">
            <div class="choice-text">
                <h3>العروض والتخفيضات</h3>
                <p>اكتشف أحدث العروض</p>
            </div>

            <div class="arrow">←</div>
        </div>
    </a>

    <!-- الخيار الثاني -->
    <a class="choice second"
       href="https://isal-357.trinavo.com/">

        <img
            src="https://i.postimg.cc/zfmt6rsW/Picsart-26-10-14-00-20-24-628.png"
            alt="اختار منتجاتك"
            loading="eager">

        <div class="choice-content">
            <div class="choice-text">
                <h3>اختار منتجاتك</h3>
                <p>تصفّح المنتجات واختر ما تحتاجه</p>
            </div>

            <div class="arrow">←</div>
        </div>
    </a>

</div>

</body>
</html>
