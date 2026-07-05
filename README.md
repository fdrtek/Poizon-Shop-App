[poizon shop app.html](https://github.com/user-attachments/files/29678276/poizon.shop.app.html)
<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Poizon Shop App</title>

<!-- Шрифт -->
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Manrope:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

body{
    font-family:"Manrope",sans-serif;
    min-height:100vh;
    display:flex;
    justify-content:center;
    align-items:center;
    overflow:hidden;
    background:linear-gradient(-45deg,#5dd6da,#000000,#5dd6da,#000000);
    background-size:400% 400%;
    animation:gradient 15s ease infinite;
}

@keyframes gradient{
    0%{background-position:0% 50%;}
    50%{background-position:100% 50%;}
    100%{background-position:0% 50%;}
}

/* Светящиеся круги */
body::before,
body::after{
    content:"";
    position:absolute;
    width:420px;
    height:420px;
    border-radius:50%;
    filter:blur(110px);
    opacity:.35;
    animation:float 10s ease-in-out infinite;
}

body::before{
    background:#60A5FA;
    top:-120px;
    left:-120px;
}

body::after{
    background:#1D4ED8;
    bottom:-120px;
    right:-120px;
    animation-delay:5s;
}

@keyframes float{
    0%,100%{
        transform:translateY(0) translateX(0);
    }
    50%{
        transform:translateY(30px) translateX(20px);
    }
}

/* Карточка */
.card{
    position:relative;
    z-index:2;

    width:380px;
    padding:40px 35px;

    background:rgba(255,255,255,.12);
    border:1px solid rgba(255,255,255,.25);
    border-radius:28px;

    backdrop-filter:blur(22px);
    -webkit-backdrop-filter:blur(22px);

    box-shadow:
        0 20px 45px rgba(0,0,0,.25),
        inset 0 1px 0 rgba(255,255,255,.25);

    text-align:center;

    animation:appear .8s ease;
}

@keyframes appear{
    from{
        opacity:0;
        transform:translateY(30px) scale(.95);
    }
    to{
        opacity:1;
        transform:translateY(0) scale(1);
    }
}

/* Аватар */
.avatar{
    width:100px;
    height:100px;
    margin:0 auto 20px;
    border-radius:50%;

    background:rgba(255,255,255,.18);
    border:2px solid rgba(255,255,255,.25);

    display:flex;
    justify-content:center;
    align-items:center;

    font-size:42px;
    color:#fff;

    box-shadow:0 10px 25px rgba(0,0,0,.15);
}

h1{
    color:#fff;
    font-size:34px;
    font-weight:800;
    letter-spacing:-1px;
}

.subtitle{
    color:rgba(255,255,255,.82);
    margin:10px 0 28px;
    font-size:15px;
    font-weight:500;
}

/* Кнопки */
.link{
    display:flex;
    align-items:center;
    justify-content:center;
    gap:10px;

    width:100%;
    padding:15px;
    margin:14px 0;

    text-decoration:none;
    color:#fff;
    font-size:16px;
    font-weight:600;

    background:rgba(255,255,255,.15);
    border:1px solid rgba(255,255,255,.18);
    border-radius:16px;

    transition:.25s ease;
}

.link:hover{
    transform:translateY(-4px);
    background:rgba(255,255,255,.25);
    box-shadow:0 12px 24px rgba(0,0,0,.2);
}

/* Подвал */
.footer{
    margin-top:28px;
    color:rgba(255,255,255,.65);
    font-size:14px;
}
</style>
</head>

<body>

<div class="card">

    <h1>Poizon Shop</h1>

    <p class="subtitle">
        Добро пожаловать! Здесь собраны все ссылки на приложения.
    </p>

    <a class="link" href="https://play.google.com/store/apps/details?id=com.newword.medved.bbb" target="_blank">
        🇷🇺 / android
    </a>

    <a class="link" href="https://apps.apple.com/ru/app/%D0%B4%D1%8D%D0%B2%D1%83-poizon-%D0%BE%D1%84%D0%B8%D1%86%D0%B8%D0%B0%D0%BB%D1%8C%D0%BD%D0%BE%D0%B5/id6742818619" target="_blank">
        🇷🇺 / apple
    </a>

    <a class="link" href="https://h5coml.vivo.com.cn/h5coml/appdetail_h5/browser_v2/index.html?appId=553351&resource=301&source=7" target="_blank">
        🇨🇳 / android
    </a>

    <a class="link" href="https://dewu.com/" target="_blank">
        🇨🇳 / apple
    </a>

    <div class="footer">
        © 2026 • Сделано с ❤️
    </div>

</div>

</body>
</html>
