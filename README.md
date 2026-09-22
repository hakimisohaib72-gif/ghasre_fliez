<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>قصر فلز | آهن‌های طرح‌دار</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Shabnam:wght@400;700&display=swap" rel="stylesheet">

<style>

/* =========================================================
   QASR FELEZ — ULTRA PROFESSIONAL CSS
   فقط CSS تغییر داده شده
========================================================= */

:root{
    --black:#020202;
    --black2:#070707;
    --black3:#101010;
    --black4:#171717;

    --gold:#c89432;
    --gold2:#f6d77e;
    --gold3:#8b601d;
    --gold4:#fff0b0;

    --white:#ffffff;
    --gray:#bdbdbd;
    --gray2:#777;

    --green:#20c96b;

    --glass:rgba(255,255,255,.055);
    --glass2:rgba(255,255,255,.025);

    --border:rgba(255,255,255,.09);
    --gold-border:rgba(214,168,79,.28);

    --radius:28px;

    --shadow:
        0 25px 70px rgba(0,0,0,.55);

    --gold-shadow:
        0 0 40px rgba(214,168,79,.14);
}


/* =========================================================
   RESET
========================================================= */

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

html{
    scroll-behavior:smooth;
    scroll-padding-top:110px;
}

body{
    min-height:100vh;

    font-family:
        "Shabnam",
        "B Nazanin",
        "Traditional Arabic",
        serif;

    color:var(--white);

    line-height:1.9;

    overflow-x:hidden;

    background:
        radial-gradient(
            circle at 10% 5%,
            rgba(214,168,79,.10),
            transparent 27%
        ),
        radial-gradient(
            circle at 90% 45%,
            rgba(214,168,79,.055),
            transparent 25%
        ),
        radial-gradient(
            circle at 50% 100%,
            rgba(214,168,79,.06),
            transparent 30%
        ),
        linear-gradient(
            135deg,
            #010101,
            #090909 45%,
            #030303
        );
}


/* =========================================================
   PREMIUM METAL TEXTURE
========================================================= */

body::before{
    content:"";

    position:fixed;

    inset:0;

    pointer-events:none;

    z-index:99999;

    opacity:.035;

    background:
        repeating-linear-gradient(
            0deg,
            rgba(255,255,255,.8) 0px,
            rgba(255,255,255,.8) 1px,
            transparent 1px,
            transparent 5px
        );

    mix-blend-mode:overlay;
}

body::after{
    content:"";

    position:fixed;

    inset:0;

    pointer-events:none;

    z-index:99998;

    background:
        radial-gradient(
            circle at center,
            transparent 35%,
            rgba(0,0,0,.30) 100%
        );
}


/* =========================================================
   SELECTION
========================================================= */

::selection{
    color:#111;

    background:
        linear-gradient(
            90deg,
            var(--gold),
            var(--gold2)
        );
}


/* =========================================================
   SCROLLBAR
========================================================= */

::-webkit-scrollbar{
    width:11px;
}

::-webkit-scrollbar-track{
    background:#020202;
}

::-webkit-scrollbar-thumb{
    border-radius:50px;

    border:3px solid #020202;

    background:
        linear-gradient(
            180deg,
            var(--gold4),
            var(--gold),
            var(--gold3)
        );

    box-shadow:
        0 0 15px
        rgba(214,168,79,.3);
}

::-webkit-scrollbar-thumb:hover{
    background:
        linear-gradient(
            180deg,
            #fff3bd,
            var(--gold2),
            var(--gold)
        );
}


/* =========================================================
   HEADER
========================================================= */

header{
    position:sticky;

    top:0;

    z-index:5000;

    display:flex;

    align-items:center;

    justify-content:space-between;

    gap:25px;

    padding:14px 6%;

    background:
        linear-gradient(
            135deg,
            rgba(2,2,2,.93),
            rgba(18,18,18,.80)
        );

    backdrop-filter:blur(25px);

    -webkit-backdrop-filter:blur(25px);

    border-bottom:
        1px solid
        rgba(214,168,79,.20);

    box-shadow:
        0 15px 50px
        rgba(0,0,0,.55);
}

header::before{
    content:"";

    position:absolute;

    right:0;

    bottom:-1px;

    width:38%;

    height:2px;

    background:
        linear-gradient(
            90deg,
            transparent,
            var(--gold),
            var(--gold2),
            transparent
        );

    filter:
        drop-shadow(
            0 0 10px
            rgba(214,168,79,.7)
        );

    animation:
        headerLine 5s ease-in-out infinite;
}


/* =========================================================
   LOGO
========================================================= */

.logo{
    position:relative;

    z-index:2;

    font-size:36px;

    font-weight:bold;

    letter-spacing:1px;

    color:transparent;

    background:
        linear-gradient(
            115deg,
            #fff,
            var(--gold4),
            var(--gold),
            #fff3bd,
            var(--gold3),
            #fff
        );

    background-size:300% 300%;

    -webkit-background-clip:text;
    background-clip:text;

    filter:
        drop-shadow(
            0 0 18px
            rgba(214,168,79,.22)
        );

    animation:
        logoGold 8s ease infinite;

    transition:.45s;
}

.logo::before{
    content:"✦";

    position:absolute;

    right:-25px;

    top:-12px;

    font-size:13px;

    color:var(--gold2);

    animation:
        sparkle 2.5s ease-in-out infinite;
}

.logo:hover{
    transform:
        translateY(-2px)
        scale(1.06);

    filter:
        drop-shadow(
            0 0 30px
            rgba(214,168,79,.55)
        );
}


/* =========================================================
   NAVIGATION
========================================================= */

nav{
    display:flex;

    align-items:center;

    justify-content:center;

    gap:5px;

    flex-wrap:wrap;
}

nav a{
    position:relative;

    isolation:isolate;

    overflow:hidden;

    color:#ddd;

    text-decoration:none;

    padding:9px 16px;

    border-radius:14px;

    transition:
        color .35s,
        transform .35s,
        background .35s;
}

nav a::before{
    content:"";

    position:absolute;

    inset:0;

    z-index:-1;

    border-radius:14px;

    background:
        linear-gradient(
            135deg,
            rgba(214,168,79,.18),
            rgba(214,168,79,.025)
        );

    opacity:0;

    transform:
        scale(.75);

    transition:.4s;
}

nav a::after{
    content:"";

    position:absolute;

    right:15px;
    left:15px;

    bottom:4px;

    height:2px;

    border-radius:50px;

    background:
        linear-gradient(
            90deg,
            transparent,
            var(--gold2),
            transparent
        );

    transform:
        scaleX(0);

    transition:.4s;

    box-shadow:
        0 0 12px
        rgba(214,168,79,.5);
}

nav a:hover{
    color:var(--gold2);

    transform:
        translateY(-3px);
}

nav a:hover::before{
    opacity:1;

    transform:scale(1);
}

nav a:hover::after{
    transform:scaleX(1);
}


/* =========================================================
   HERO
========================================================= */

.hero{
    position:relative;

    min-height:92vh;

    display:flex;

    align-items:center;

    justify-content:center;

    text-align:center;

    overflow:hidden;

    background:
        linear-gradient(
            90deg,
            rgba(0,0,0,.92),
            rgba(0,0,0,.48),
            rgba(0,0,0,.90)
        ),
        url("https://images.unsplash.com/photo-1504917595217-d4dc5ebe6122?auto=format&fit=crop&w=2000&q=90")
        center/cover no-repeat;

    background-attachment:fixed;
}

.hero::before{
    content:"";

    position:absolute;

    inset:0;

    background:
        radial-gradient(
            circle at center,
            transparent 5%,
            rgba(0,0,0,.20) 45%,
            rgba(0,0,0,.82) 100%
        );
}

.hero::after{
    content:"";

    position:absolute;

    width:750px;
    height:750px;

    border-radius:50%;

    background:
        radial-gradient(
            circle,
            rgba(214,168,79,.16),
            rgba(214,168,79,.035) 35%,
            transparent 70%
        );

    animation:
        heroGlow 8s ease-in-out infinite;

    pointer-events:none;
}


/* =========================================================
   HERO DECORATIVE RINGS
========================================================= */

.hero-content::before{
    content:"";

    position:absolute;

    width:600px;
    height:600px;

    right:-420px;
    top:-280px;

    border:
        1px solid
        rgba(214,168,79,.14);

    border-radius:50%;

    box-shadow:
        0 0 0 70px
        rgba(214,168,79,.025),
        0 0 0 140px
        rgba(214,168,79,.015);

    animation:
        ringRotate 20s linear infinite;
}

.hero-content::after{
    content:"";

    position:absolute;

    width:420px;
    height:420px;

    left:-330px;
    bottom:-250px;

    border:
        1px solid
        rgba(214,168,79,.12);

    border-radius:50%;

    box-shadow:
        0 0 0 55px
        rgba(214,168,79,.02),
        0 0 0 110px
        rgba(214,168,79,.012);

    animation:
        ringRotate 25s linear infinite reverse;
}


/* =========================================================
   HERO CONTENT
========================================================= */

.hero-content{
    position:relative;

    z-index:5;

    max-width:1000px;

    padding:50px 20px;

    animation:
        heroEnter 1.2s
        cubic-bezier(.2,.8,.2,1);
}

.hero-badge{
    display:inline-flex;

    align-items:center;

    justify-content:center;

    gap:10px;

    padding:9px 25px;

    margin-bottom:30px;

    color:var(--gold2);

    border:
        1px solid
        rgba(214,168,79,.35);

    border-radius:50px;

    background:
        linear-gradient(
            135deg,
            rgba(214,168,79,.13),
            rgba(255,255,255,.025)
        );

    backdrop-filter:blur(15px);

    box-shadow:
        inset 0 1px
        rgba(255,255,255,.08),
        0 15px 45px
        rgba(0,0,0,.35);

    animation:
        badgeFloat 4s ease-in-out infinite;
}

.hero h1{
    font-size:
        clamp(70px,12vw,150px);

    line-height:.9;

    margin-bottom:28px;

    color:transparent;

    background:
        linear-gradient(
            110deg,
            #fff,
            #fff4c8,
            var(--gold),
            #fff0ae,
            var(--gold3),
            #fff
        );

    background-size:350% 350%;

    -webkit-background-clip:text;
    background-clip:text;

    animation:
        goldText 8s ease infinite;

    filter:
        drop-shadow(
            0 25px 35px
            rgba(0,0,0,.8)
        );
}

.hero p{
    max-width:750px;

    margin:
        0 auto 40px;

    color:#dedede;

    font-size:
        clamp(18px,3vw,27px);

    text-shadow:
        0 4px 20px #000;
}


/* =========================================================
   PREMIUM BUTTON
========================================================= */

.btn{
    position:relative;

    isolation:isolate;

    display:inline-flex;

    align-items:center;

    justify-content:center;

    min-width:190px;

    padding:14px 30px;

    overflow:hidden;

    border:none;

    border-radius:16px;

    color:#171109;

    text-decoration:none;

    font-family:inherit;

    font-size:18px;

    font-weight:bold;

    cursor:pointer;

    background:
        linear-gradient(
            120deg,
            #8d641d,
            #f9db82,
            #c18d2b,
            #fff0ae,
            #91681e
        );

    background-size:350% 350%;

    box-shadow:
        0 15px 35px
        rgba(214,168,79,.20),

        inset 0 1px
        rgba(255,255,255,.9);

    animation:
        buttonGold 7s ease infinite;

    transition:
        transform .35s,
        box-shadow .35s;
}

.btn::before{
    content:"";

    position:absolute;

    z-index:-1;

    top:0;

    left:-130%;

    width:75%;

    height:100%;

    transform:
        skewX(-25deg);

    background:
        linear-gradient(
            90deg,
            transparent,
            rgba(255,255,255,.8),
            transparent
        );

    transition:
        left .8s;
}

.btn:hover{
    transform:
        translateY(-6px)
        scale(1.04);

    box-shadow:
        0 25px 55px
        rgba(214,168,79,.30),

        0 0 35px
        rgba(214,168,79,.13);
}

.btn:hover::before{
    left:150%;
}

.btn:active{
    transform:
        translateY(-2px)
        scale(.98);
}


/* =========================================================
   GENERAL SECTIONS
========================================================= */

section{
    position:relative;

    padding:120px 7%;

    isolation:isolate;
}

.section-title{
    text-align:center;

    margin-bottom:70px;
}

.section-title h2{
    position:relative;

    display:inline-block;

    font-size:
        clamp(35px,5vw,55px);

    color:transparent;

    background:
        linear-gradient(
            135deg,
            #fff,
            var(--gold2),
            var(--gold)
        );

    -webkit-background-clip:text;
    background-clip:text;

    filter:
        drop-shadow(
            0 8px 20px
            rgba(0,0,0,.5)
        );
}

.section-title h2::before{
    content:"✦";

    position:absolute;

    right:-37px;

    top:-8px;

    color:var(--gold2);

    font-size:15px;

    animation:
        sparkle 2.5s infinite;
}

.section-title h2::after{
    content:"";

    position:absolute;

    right:50%;

    bottom:-17px;

    width:140px;

    height:3px;

    transform:
        translateX(50%);

    border-radius:50px;

    background:
        linear-gradient(
            90deg,
            transparent,
            var(--gold2),
            var(--gold),
            transparent
        );

    box-shadow:
        0 0 20px
        rgba(214,168,79,.35);
}


/* =========================================================
   CATEGORIES
========================================================= */

.categories{
    display:grid;

    grid-template-columns:
        repeat(3,1fr);

    gap:30px;
}

.category-card{
    position:relative;

    min-height:260px;

    padding:45px 30px;

    overflow:hidden;

    text-align:center;

    border:
        1px solid
        var(--border);

    border-radius:
        var(--radius);

    background:
        linear-gradient(
            145deg,
            rgba(255,255,255,.075),
            rgba(255,255,255,.018)
        );

    backdrop-filter:blur(20px);

    box-shadow:
        var(--shadow);

    transform:
        translateZ(0);

    transition:
        transform .5s
        cubic-bezier(.2,.8,.2,1),
        border .5s,
        box-shadow .5s;
}

.category-card::before{
    content:"";

    position:absolute;

    width:240px;
    height:240px;

    top:-150px;
    right:-110px;

    border-radius:50%;

    background:
        radial-gradient(
            circle,
            rgba(214,168,79,.18),
            transparent 70%
        );

    transition:.6s;
}

.category-card::after{
    content:"";

    position:absolute;

    top:-130%;

    left:-90%;

    width:50%;

    height:320%;

    transform:
        rotate(25deg);

    background:
        linear-gradient(
            90deg,
            transparent,
            rgba(255,255,255,.10),
            transparent
        );

    transition:
        left 1s;
}

.category-card:hover{
    transform:
        translateY(-16px)
        scale(1.015);

    border-color:
        rgba(214,168,79,.48);

    box-shadow:
        0 40px 90px
        rgba(0,0,0,.72),

        0 0 45px
        rgba(214,168,79,.08);
}

.category-card:hover::before{
    transform:
        scale(1.5);
}

.category-card:hover::after{
    left:150%;
}

.category-icon{
    position:relative;

    z-index:2;

    font-size:67px;

    margin-bottom:15px;

    filter:
        drop-shadow(
            0 0 22px
            rgba(214,168,79,.35)
        );

    transition:.5s;
}

.category-card:hover
.category-icon{
    transform:
        translateY(-9px)
        scale(1.14)
        rotate(-3deg);
}

.category-card h3{
    position:relative;

    z-index:2;

    color:var(--gold2);

    font-size:28px;

    margin-bottom:9px;
}

.category-card p{
    position:relative;

    z-index:2;

    color:#aaa;

    font-size:17px;
}


/* =========================================================
   PRODUCTS
========================================================= */

.products{
    display:grid;

    grid-template-columns:
        repeat(auto-fit,minmax(260px,1fr));

    gap:30px;
}

.product-card{
    position:relative;

    overflow:hidden;

    border:
        1px solid
        rgba(255,255,255,.08);

    border-radius:
        var(--radius);

    background:
        linear-gradient(
            145deg,
            #181818,
            #070707
        );

    box-shadow:
        0 20px 60px
        rgba(0,0,0,.45);

    transition:
        transform .5s
        cubic-bezier(.2,.8,.2,1),
        border .5s,
        box-shadow .5s;
}

.product-card:hover{
    transform:
        translateY(-15px);

    border-color:
        rgba(214,168,79,.48);

    box-shadow:
        0 40px 90px
        rgba(0,0,0,.72),

        0 0 35px
        rgba(214,168,79,.09);
}


/* =========================================================
   PRODUCT IMAGE
========================================================= */

.product-image{
    position:relative;

    height:240px;

    overflow:hidden;

    background:#111;
}

.product-image::before{
    content:"";

    position:absolute;

    inset:0;

    z-index:2;

    background:
        linear-gradient(
            to top,
            rgba(0,0,0,.85),
            transparent 60%
        );

    pointer-events:none;
}

.product-image::after{
    content:"";

    position:absolute;

    z-index:3;

    top:0;

    left:-130%;

    width:65%;

    height:100%;

    transform:
        skewX(-23deg);

    background:
        linear-gradient(
            90deg,
            transparent,
            rgba(255,255,255,.22),
            transparent
        );

    transition:
        left .9s;
}

.product-card:hover
.product-image::after{
    left:150%;
}

.product-image img{
    width:100%;
    height:100%;

    object-fit:cover;

    transition:
        transform .9s
        cubic-bezier(.2,.8,.2,1),
        filter .5s;
}

.product-card:hover
.product-image img{
    transform:
        scale(1.13);

    filter:
        brightness(1.10)
        contrast(1.08)
        saturate(1.08);
}


/* =========================================================
   PRODUCT CONTENT
========================================================= */

.product-content{
    padding:25px;
}

.product-content h3{
    color:var(--gold2);

    font-size:25px;

    margin-bottom:8px;

    transition:.3s;
}

.product-card:hover
.product-content h3{
    color:#fff0b0;
}

.product-content p{
    min-height:58px;

    color:#aaa;

    margin-bottom:20px;

    font-size:16px;
}


/* =========================================================
   ABOUT
========================================================= */

.about{
    overflow:hidden;

    background:
        radial-gradient(
            circle at 15% 50%,
            rgba(214,168,79,.10),
            transparent 34%
        ),
        radial-gradient(
            circle at 90% 30%,
            rgba(214,168,79,.05),
            transparent 28%
        ),
        linear-gradient(
            135deg,
            #151515,
            #050505
        );

    border-top:
        1px solid
        rgba(214,168,79,.16);

    border-bottom:
        1px solid
        rgba(214,168,79,.16);
}

.about::before{
    content:"";

    position:absolute;

    width:650px;
    height:650px;

    left:-380px;
    top:-240px;

    border:
        1px solid
        rgba(214,168,79,.08);

    border-radius:50%;

    box-shadow:
        0 0 0 80px
        rgba(214,168,79,.02),
        0 0 0 160px
        rgba(214,168,79,.012);

    animation:
        ringRotate 30s linear infinite;
}

.about-box{
    position:relative;

    z-index:2;

    max-width:1000px;

    margin:auto;

    padding:60px 55px;

    text-align:center;

    border:
        1px solid
        rgba(214,168,79,.22);

    border-radius:34px;

    background:
        linear-gradient(
            135deg,
            rgba(255,255,255,.065),
            rgba(255,255,255,.012)
        );

    backdrop-filter:blur(22px);

    box-shadow:
        0 35px 90px
        rgba(0,0,0,.62),

        inset 0 1px
        rgba(255,255,255,.07);

    transition:
        transform .5s,
        border .5s;
}

.about-box:hover{
    transform:
        translateY(-7px);

    border-color:
        rgba(214,168,79,.4);
}

.about-box h3{
    color:var(--gold2);

    font-size:33px;

    margin-bottom:22px;
}

.about-box p{
    color:#d5d5d5;

    font-size:21px;

    line-height:2.4;
}

.about-box strong{
    color:var(--gold2);

    font-weight:bold;
}


/* =========================================================
   CONTACT
========================================================= */

.contact-section{
    position:relative;

    overflow:hidden;

    background:
        radial-gradient(
            circle at 50% 0%,
            rgba(214,168,79,.09),
            transparent 35%
        );
}

.contact-section::before{
    content:"";

    position:absolute;

    width:500px;
    height:500px;

    right:-250px;
    bottom:-250px;

    border-radius:50%;

    border:
        1px solid
        rgba(214,168,79,.07);

    box-shadow:
        0 0 0 80px
        rgba(214,168,79,.015);
}

.contact-grid{
    max-width:1200px;

    margin:auto;

    display:grid;

    grid-template-columns:
        repeat(2,1fr);

    gap:30px;
}

.contact-card{
    position:relative;

    overflow:hidden;

    padding:35px;

    border:
        1px solid
        rgba(255,255,255,.08);

    border-radius:
        var(--radius);

    background:
        linear-gradient(
            145deg,
            rgba(255,255,255,.065),
            rgba(255,255,255,.015)
        );

    backdrop-filter:blur(20px);

    box-shadow:
        0 25px 60px
        rgba(0,0,0,.42);

    transition:
        transform .45s,
        border .45s,
        box-shadow .45s;
}

.contact-card::before{
    content:"";

    position:absolute;

    width:190px;
    height:190px;

    top:-110px;
    right:-90px;

    border-radius:50%;

    background:
        radial-gradient(
            circle,
            rgba(214,168,79,.16),
            transparent 70%
        );

    transition:.5s;
}

.contact-card:hover{
    transform:
        translateY(-10px);

    border-color:
        rgba(214,168,79,.42);

    box-shadow:
        0 35px 80px
        rgba(0,0,0,.62),

        0 0 35px
        rgba(214,168,79,.06);
}

.contact-card:hover::before{
    transform:
        scale(1.35);
}

.contact-card h3{
    position:relative;

    z-index:2;

    color:var(--gold2);

    font-size:29px;

    margin-bottom:15px;
}

.contact-card p{
    position:relative;

    z-index:2;

    color:#d0d0d0;

    font-size:19px;
}

.contact-card a{
    color:#eee;

    text-decoration:none;

    transition:.3s;
}

.contact-card a:hover{
    color:var(--gold2);
}


/* =========================================================
   WHATSAPP BUTTON
========================================================= */

.whatsapp{
    position:relative;

    overflow:hidden;

    display:block;

    margin-top:13px;

    padding:13px 20px;

    text-align:center;

    color:#fff !important;

    border-radius:15px;

    background:
        linear-gradient(
            135deg,
            #25d96f,
            #08794e
        );

    box-shadow:
        0 12px 30px
        rgba(32,201,107,.15);

    transition:
        transform .35s,
        box-shadow .35s;
}

.whatsapp::before{
    content:"";

    position:absolute;

    top:0;

    left:-120%;

    width:60%;

    height:100%;

    transform:
        skewX(-25deg);

    background:
        linear-gradient(
            90deg,
            transparent,
            rgba(255,255,255,.28),
            transparent
        );

    transition:
        left .7s;
}

.whatsapp:hover{
    transform:
        translateY(-5px);

    box-shadow:
        0 20px 45px
        rgba(32,201,107,.30);
}

.whatsapp:hover::before{
    left:150%;
}


/* =========================================================
   FORM
========================================================= */

form{
    display:flex;

    flex-direction:column;

    gap:15px;
}

input,
textarea{
    width:100%;

    padding:16px 18px;

    border:
        1px solid
        rgba(255,255,255,.10);

    border-radius:15px;

    outline:none;

    color:white;

    background:
        linear-gradient(
            145deg,
            rgba(0,0,0,.65),
            rgba(255,255,255,.025)
        );

    font-family:inherit;

    font-size:16px;

    transition:
        border .35s,
        box-shadow .35s,
        transform .35s,
        background .35s;
}

input::placeholder,
textarea::placeholder{
    color:#777;
}

input:focus,
textarea:focus{
    transform:
        translateY(-2px);

    border-color:
        rgba(214,168,79,.75);

    background:
        rgba(214,168,79,.035);

    box-shadow:
        0 0 0 3px
        rgba(214,168,79,.055),

        0 0 30px
        rgba(214,168,79,.07);
}

textarea{
    min-height:145px;

    resize:vertical;
}


/* =========================================================
   FLOATING WHATSAPP
========================================================= */

.whatsapp-float{
    position:fixed;

    left:24px;
    bottom:24px;

    z-index:6000;

    width:66px;
    height:66px;

    display:flex;

    align-items:center;
    justify-content:center;

    border-radius:50%;

    color:#fff;

    text-decoration:none;

    font-size:28px;

    background:
        linear-gradient(
            135deg,
            #29df74,
            #08794e
        );

    border:
        3px solid
        rgba(255,255,255,.12);

    box-shadow:
        0 15px 40px
        rgba(32,201,107,.35);

    animation:
        whatsappPulse 2.5s ease-in-out infinite;

    transition:.35s;
}

.whatsapp-float:hover{
    transform:
        translateY(-7px)
        scale(1.12);

    box-shadow:
        0 20px 55px
        rgba(32,201,107,.55);
}


/* =========================================================
   FOOTER
========================================================= */

footer{
    position:relative;

    padding:45px 7%;

    text-align:center;

    color:#777;

    background:#020202;

    border-top:
        1px solid
        rgba(214,168,79,.17);

    overflow:hidden;
}

footer::before{
    content:"";

    position:absolute;

    top:0;

    right:50%;

    width:260px;

    height:1px;

    transform:
        translateX(50%);

    background:
        linear-gradient(
            90deg,
            transparent,
            var(--gold),
            transparent
        );
}

footer strong{
    color:var(--gold2);

    text-shadow:
        0 0 18px
        rgba(214,168,79,.25);
}


/* =========================================================
   ANIMATIONS
========================================================= */

@keyframes heroEnter{
    from{
        opacity:0;

        transform:
            translateY(55px)
            scale(.95);
    }

    to{
        opacity:1;

        transform:
            translateY(0)
            scale(1);
    }
}

@keyframes heroGlow{
    0%,100%{
        transform:
            scale(.75);

        opacity:.35;
    }

    50%{
        transform:
            scale(1.18);

        opacity:1;
    }
}

@keyframes goldText{
    0%,100%{
        background-position:
            0% 50%;
    }

    50%{
        background-position:
            100% 50%;
    }
}

@keyframes buttonGold{
    0%,100%{
        background-position:
            0% 50%;
    }

    50%{
        background-position:
            100% 50%;
    }
}

@keyframes logoGold{
    0%,100%{
        background-position:
            0% 50%;
    }

    50%{
        background-position:
            100% 50%;
    }
}

@keyframes sparkle{
    0%,100%{
        opacity:.35;

        transform:
            scale(.8)
            rotate(0deg);
    }

    50%{
        opacity:1;

        transform:
            scale(1.35)
            rotate(180deg);
    }
}

@keyframes headerLine{
    0%,100%{
        opacity:.3;

        transform:
            scaleX(.55);
    }

    50%{
        opacity:1;

        transform:
            scaleX(1);
    }
}

@keyframes badgeFloat{
    0%,100%{
        transform:
            translateY(0);
    }

    50%{
        transform:
            translateY(-5px);
    }
}

@keyframes ringRotate{
    from{
        transform:
            rotate(0deg);
    }

    to{
        transform:
            rotate(360deg);
    }
}

@keyframes whatsappPulse{
    0%,100%{
        box-shadow:
            0 15px 40px
            rgba(32,201,107,.28);
    }

    50%{
        box-shadow:
            0 15px 65px
            rgba(32,201,107,.58);
    }
}


/* =========================================================
   TABLET
========================================================= */

@media(max-width:900px){

    header{
        padding:13px 4%;

        flex-direction:column;

        gap:9px;
    }

    .logo{
        font-size:30px;
    }

    nav{
        justify-content:center;
    }

    nav a{
        padding:7px 10px;

        font-size:14px;
    }

    .hero{
        min-height:84vh;

        background-attachment:
            scroll;
    }

    .hero h1{
        font-size:
            clamp(65px,16vw,105px);
    }

    section{
        padding:90px 5%;
    }

    .categories{
        grid-template-columns:1fr;
    }

    .contact-grid{
        grid-template-columns:1fr;
    }

    .about-box{
        padding:45px 30px;
    }

    .products{
        grid-template-columns:
            repeat(
                auto-fit,
                minmax(240px,1fr)
            );
    }
}


/* =========================================================
   MOBILE
========================================================= */

@media(max-width:520px){

    header{
        padding:11px 3%;
    }

    .logo{
        font-size:27px;
    }

    nav{
        gap:2px;
    }

    nav a{
        padding:5px 7px;

        font-size:13px;
    }

    .hero{
        min-height:82vh;
    }

    .hero-content{
        padding:35px 15px;
    }

    .hero h1{
        font-size:60px;
    }

    .hero p{
        font-size:17px;

        margin-bottom:30px;
    }

    .hero-badge{
        font-size:13px;

        padding:7px 15px;
    }

    .btn{
        width:100%;

        min-width:0;

        padding:13px 20px;
    }

    section{
        padding:70px 5%;
    }

    .section-title{
        margin-bottom:50px;
    }

    .section-title h2{
        font-size:32px;
    }

    .section-title h2::before{
        right:-25px;
    }

    .category-card{
        min-height:225px;

        padding:35px 20px;
    }

    .category-icon{
        font-size:55px;
    }

    .product-image{
        height:215px;
    }

    .product-content{
        padding:20px;
    }

    .product-content h3{
        font-size:22px;
    }

    .product-content p{
        min-height:auto;

        margin-bottom:18px;
    }

    .about-box{
        padding:32px 20px;

        border-radius:25px;
    }

    .about-box h3{
        font-size:27px;
    }

    .about-box p{
        font-size:18px;

        line-height:2.2;
    }

    .contact-card{
        padding:25px 20px;

        border-radius:22px;
    }

    .contact-card h3{
        font-size:25px;
    }

    .whatsapp-float{
        width:57px;
        height:57px;

        left:15px;
        bottom:15px;

        font-size:24px;
    }
}


/* =========================================================
   REDUCED MOTION
========================================================= */

@media(prefers-reduced-motion:reduce){

    *,
    *::before,
    *::after{
        animation-duration:.01ms !important;
        animation-iteration-count:1 !important;
        scroll-behavior:auto !important;
        transition-duration:.01ms !important;
    }
}

</style>
</head>

<body>

<header>

    <div class="logo">
        قصر فلز
    </div>

    <nav>
        <a href="#home">خانه</a>
        <a href="#categories">دسته‌بندی</a>
        <a href="#products">محصولات</a>
        <a href="#about">درباره ما</a>
        <a href="#contact">تماس با ما</a>
    </nav>

</header>

<section class="hero" id="home">

    <div class="hero-content">

        <div class="hero-badge">
            ✦ آهن‌های طرح‌دار و محصولات فلزی ✦
        </div>

        <h1>قصر فلز</h1>

        <p>
            زیبایی، استحکام و طراحی خاص برای پروژه‌های شما
        </p>

        <a href="#products" class="btn">
            مشاهده محصولات
        </a>

    </div>

</section>

<section id="categories">

    <div class="section-title">
        <h2>دسته‌بندی محصولات</h2>
    </div>

    <div class="categories">

        <div class="category-card">
            <div class="category-icon">⚒️</div>
            <h3>آهن‌های طرح‌دار</h3>
            <p>
                انواع آهن با طرح‌های زیبا و متنوع
            </p>
        </div>

        <div class="category-card">
            <div class="category-icon">🔩</div>
            <h3>محصولات فلزی</h3>
            <p>
                محصولات فلزی مقاوم و باکیفیت
            </p>
        </div>

        <div class="category-card">
            <div class="category-icon">✦</div>
            <h3>طرح‌های دکوراتیو</h3>
            <p>
                طرح‌های زیبا برای پروژه‌ها و دکوراسیون
            </p>
        </div>

    </div>

</section>

<section id="products">

    <div class="section-title">
        <h2>محصولات قصر فلز</h2>
    </div>

    <div class="products">

        <script>
        const products = [
            ["1504307651254-35680f356dfd","مدل فلزی شماره ۱","آهن طرح‌دار با طراحی زیبا."],
            ["1530124566582-a618bc2615dc","مدل فلزی شماره ۲","مناسب برای استفاده‌های دکوراتیو."],
            ["1504917595217-d4dc5ebe6122","مدل فلزی شماره ۳","ساخته‌شده با فلز مقاوم."],
            ["1565793298595-6a879b1d9492","مدل فلزی شماره ۴","طرح خاص برای دکوراسیون."],
            ["1518709268805-4e9042af9f23","مدل فلزی شماره ۵","طراحی مدرن و مقاوم."],
            ["1503387762-592deb58ef4e","مدل فلزی شماره ۶","مناسب برای پروژه‌های مختلف."],
            ["1486406146926-c627a92ad1ab","مدل فلزی شماره ۷","ظاهر شیک و طراحی متفاوت."],
            ["1541888946425-d81bb19240f5","مدل فلزی شماره ۸","کیفیت مناسب و ظاهر زیبا."],
            ["1531835551805-16d864c8d311","مدل فلزی شماره ۹","طرح دکوراتیو فلزی."],
            ["1590479773265-7464e5d48118","مدل فلزی شماره ۱۰","طرح خاص و مقاوم."],
            ["1505577058444-a3dab90d4253","مدل فلزی شماره ۱۱","مناسب برای طراحی داخلی."],
            ["1497366754035-f200968a6e72","مدل فلزی شماره ۱۲","طراحی زیبا و کاربردی."],
            ["1504328345606-18bbc8c9d7d1","مدل فلزی شماره ۱۳","یکی از مدل‌های خاص قصر فلز."]
        ];

        document.write(
            products.map(p => `
                <div class="product-card">

                    <div class="product-image">
                        <img
                            src="https://images.unsplash.com/photo-${p[0]}?auto=format&fit=crop&w=800&q=80"
                            alt="${p[1]}"
                        >
                    </div>

                    <div class="product-content">

                        <h3>${p[1]}</h3>

                        <p>${p[2]}</p>

                        <a href="#contact" class="btn">
                            تماس برای قیمت
                        </a>

                    </div>

                </div>
            `).join("")
        );
        </script>

    </div>

</section>

<section class="about" id="about">

    <div class="section-title">
        <h2>درباره ما</h2>
    </div>

    <div class="about-box">

        <h3>
            درباره قصر فلز
        </h3>

        <p>
            قصر فلز یک فروشگاه تخصصی در زمینه
            <strong>آهن‌های طرح‌دار و محصولات فلزی</strong>
            است.
        </p>

        <p>
            ما تلاش می‌کنیم محصولات فلزی با
            طراحی زیبا، کیفیت مناسب و ظاهر خاص
            برای پروژه‌های مختلف در اختیار مشتریان
            قرار دهیم.
        </p>

        <p>
            📍 آدرس:
            هرات، جاده انصاری، دوکان قصر فلز
        </p>

    </div>

</section>

<section class="contact-section" id="contact">

    <div class="section-title">
        <h2>تماس با ما</h2>
    </div>

    <div class="contact-grid">

        <div class="contact-card">

            <h3>📍 آدرس ما</h3>

            <p>
                هرات، جاده انصاری،
                دوکان قصر فلز
            </p>

        </div>

        <div class="contact-card">

            <h3>📞 شماره تماس</h3>

            <p>
                <a href="tel:0795346316">
                    0795346316
                </a>
            </p>

            <p>
                <a href="tel:0790790571">
                    0790790571
                </a>
            </p>

        </div>

        <div class="contact-card">

            <h3>💬 واتساپ</h3>

            <a
                class="whatsapp"
                href="https://wa.me/93795346316"
                target="_blank">
                واتساپ شماره اول
            </a>

            <a
                class="whatsapp"
                href="https://wa.me/93790790571"
                target="_blank">
                واتساپ شماره دوم
            </a>

        </div>

        <div class="contact-card">

            <h3>✉️ ارسال پیام</h3>

            <form
                action="https://formsubmit.co/hakimisohaib72@gmail.com"
                method="POST">

                <input
                    type="hidden"
                    name="_subject"
                    value="پیام جدید از وب‌سایت قصر فلز">

                <input
                    type="hidden"
                    name="_captcha"
                    value="false">

                <input
                    type="text"
                    name="name"
                    placeholder="نام شما"
                    required>

                <input
                    type="email"
                    name="email"
                    placeholder="ایمیل شما"
                    required>

                <textarea
                    name="message"
                    placeholder="پیام خود را بنویسید..."
                    required></textarea>

                <button
                    type="submit"
                    class="btn">
                    ارسال پیام
                </button>

            </form>

        </div>

    </div>

</section>

<a
    href="https://wa.me/93795346316"
    target="_blank"
    class="whatsapp-float"
    title="واتساپ قصر فلز">
    ☎
</a>

<footer>

    <p>
        © 2026
        <strong>قصر فلز</strong>
        — تمام حقوق محفوظ است.
    </p>

</footer>

</body>
</html>
```
