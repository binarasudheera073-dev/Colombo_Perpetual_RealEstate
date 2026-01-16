<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Colombo Perpetual Real Estate (Pvt) Ltd</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">

<style>
:root{
    --gold:#057818;
    --green:#ca9804;
    --dark:#0b1411;
    --card:#13211c;
}

*{margin:0;padding:0;box-sizing:border-box;font-family:'Poppins',sans-serif;}
body{background:var(--dark);color:#fff;scroll-behavior:smooth;}

/* HEADER */
header{
    position:fixed;top:0;width:100%;
    padding:12px 26px;
    display:flex;justify-content:space-between;align-items:center;
    background:rgba(0,0,0,.6);
    backdrop-filter:blur(6px);
    z-index:100;
}
.brand{display:flex;align-items:center;gap:10px;}
.logo-box{width:42px;height:42px;}
.logo-box img{width:100%;height:100%;object-fit:contain;}
nav a{margin-left:14px;color:#fff;text-decoration:none;font-size:14px;}
nav a:hover{color:var(--gold);}

/* HERO */
.hero{height:100vh;margin-top:70px;position:relative;}
.slide{position:absolute;width:100%;height:100%;background-size:cover;background-position:center;opacity:0;animation:heroSlide 15s infinite;}
.slide:nth-child(1){animation-delay:0s;}
.slide:nth-child(2){animation-delay:5s;}
.slide:nth-child(3){animation-delay:10s;}
@keyframes heroSlide{0%{opacity:0}10%{opacity:1}30%{opacity:1}40%{opacity:0}}
.overlay{position:absolute;width:100%;height:100%;background:linear-gradient(to bottom,rgba(0,0,0,.35),var(--dark));}

.hero-content{
    position:relative;z-index:2;height:100%;
    display:flex;flex-direction:column;justify-content:center;
    padding:0 32px;max-width:650px;
}
.hero-content h2{font-size:13px;letter-spacing:2px;color:var(--green);}
.hero-content h1{font-size:44px;color:var(--gold);margin:6px 0;}
.hero-content p{opacity:.85;margin-bottom:14px;}
.hero-content button{
    width:200px;padding:12px;background:var(--green);
    border:none;font-weight:600;cursor:pointer;
}
.hero-content button:hover{background:var(--gold);}

/* SECTIONS */
section{padding:40px 30px;}
.section-title{font-size:28px;color:var(--gold);margin-bottom:16px;}

/* CONTENT */
.content-box{
    background:var(--card);
    padding:24px;
    border-radius:12px;
    line-height:1.65;
    opacity:.95;
}

/* ANIMATIONS */
.left{animation:slideLeft .8s ease;}
.right{animation:slideRight .8s ease;}
.center{animation:fadeIn .8s ease;}
@keyframes slideLeft{from{transform:translateX(-40px);opacity:0}to{opacity:1}}
@keyframes slideRight{from{transform:translateX(40px);opacity:0}to{opacity:1}}
@keyframes fadeIn{from{opacity:0}to{opacity:1}}

/* SERVICES */
.services{display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:14px;}
.service{
    background:var(--card);padding:18px;border-radius:10px;text-align:center;
    position:relative;
}
.service i{font-size:26px;color:var(--green);margin-bottom:8px;}

/* SLIDESHOW for Lands/Houses */
.slideshow-container {position:relative; width:100%; height:200px; overflow:hidden; border-radius:10px;}
.slideshow-container img {width:100%; height:200px; object-fit:cover; display:none;}
.slideshow-container img.active {display:block;}
.slide-desc {margin-top:6px; font-weight:600; font-size:14px; color:var(--green);}
.slide-price {font-size:12px; color:var(--gold); margin-bottom:6px;}

/* REVIEWS */
.review{background:var(--card);padding:14px;border-radius:10px;margin-bottom:10px;}
.review h4{color:var(--green);}
.review small{font-size:12px;opacity:.7;}

.review-form{
    margin-top:12px;background:var(--card);
    padding:16px;border-radius:10px;max-width:420px;
}
.review-form input,.review-form textarea{
    width:100%;padding:9px;margin-bottom:8px;
    background:#0b1411;border:1px solid #2b3a34;color:#fff;border-radius:6px;
}
.review-form button{
    padding:10px 18px;background:var(--green);
    border:none;font-weight:600;cursor:pointer;
}

/* CONTACT */
.contact-box{background:var(--card);padding:22px;border-radius:12px;text-align:center;}
.contact-box a{
    display:inline-block;margin:6px;padding:10px 18px;
    text-decoration:none;font-weight:600;border-radius:6px;
}
.whatsapp{background:#25D366;color:#000;}
.email{background:var(--green);color:#000;}

/* FOOTER */
footer{background:#000;padding:18px 26px;}
.footer-grid{
    display:grid;
    grid-template-columns:1.2fr 1fr 1fr;
    gap:10px;
}
.footer-grid h3{color:var(--gold);font-size:14px;margin-bottom:3px;}
.footer-grid p,.footer-links a{
    font-size:12px;color:#ccc;text-decoration:none;
}
.social a{font-size:16px;margin-right:8px;color:var(--gold);}
.footer-bottom{text-align:center;font-size:11px;opacity:.6;margin-top:10px;}

@media(max-width:768px){
    header{flex-direction:column;gap:8px;}
    nav{display:flex;flex-wrap:wrap;justify-content:center;}
    .hero-content h1{font-size:34px;}
    section{padding:34px 20px;}
    .footer-grid{grid-template-columns:1fr;}
}
</style>
</head>

<body>

<header>
    <div class="brand">
        <div class="logo-box">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-1/598387204_122111847453133084_5929818682765477844_n.jpg?stp=dst-jpg_s200x200_tt6&_nc_cat=102&ccb=1-7&_nc_sid=2d3e12&_nc_eui2=AeEGsC9b6z5KJUSyeYVV1qYF4DhcvJADBa7gOFy8kAMFrmz0l1BsVPhxE8SfjxdwMfos4BmFusdWspIufRKs9llY&_nc_ohc=K-gb7RY1-EAQ7kNvwFcMGC0&_nc_oc=AdkRiD2V_vV_vc-T6ZgDx8rf4BYE_jyOgyahysh6Z0XCbRuqsJ8diksLFP4uAb3MAVw&_nc_zt=24&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=_UkJCrXd4zWtT-X5afhojw&oh=00_Afrm-3MNAcp5WxfX2z0KGxWTHhmZ0npBlgVbNeqKODgIwA&oe=696ECE42" alt="Logo">
        </div>
        <strong>Colombo Perpetual Real Estate (Pvt) Ltd</strong>
    </div>
    <nav>
        <a href="#about">About</a>
        <a href="#lands">Lands</a>
        <a href="#houses">Houses</a>
        <a href="#reviews">Reviews</a>
        <a href="#contact">Contact</a>
    </nav>
</header>

<div class="hero">
    <div class="slide" style="background-image:url('https://images.unsplash.com/photo-1600585154340-be6161a56a0c');"></div>
    <div class="slide" style="background-image:url('https://images.unsplash.com/photo-1600047509807-ba8f99d2cdde');"></div>
    <div class="slide" style="background-image:url('https://images.unsplash.com/photo-1580587771525-78b9dba3b914');"></div>
    <div class="overlay"></div>

    <div class="hero-content">
        <h2>TRUSTED PROPERTY PARTNER</h2>
        <h1>Find Your Space, Build Your Future</h1>
        <p>Approved lands and quality homes with legal assurance.</p>
        <button onclick="document.getElementById('about').scrollIntoView()">Explore Properties</button>
    </div>
</div>

<section id="about">
    <h2 class="section-title">Our History</h2>
    <div class="content-box left">
        Colombo Perpetual Real Estate (Pvt) Ltd was established in 2025 with the objective of creating
        a transparent, reliable, and client-focused real estate platform in Sri Lanka. From the
        beginning, our company has been committed to offering legally approved lands and quality
        properties while maintaining ethical standards, clear documentation, and long-term client trust.
    </div>
</section>

<section>
    <h2 class="section-title">Our Vision</h2>
    <div class="content-box right">
        Our vision is to become one of Sri Lanka’s most trusted and recognized real estate companies
        by delivering secure property investments, professional guidance, and consistent value to
        our clients locally and internationally.
    </div>
</section>

<section>
    <h2 class="section-title">Our Mission</h2>
    <div class="content-box center">
        Our mission is to provide approved lands, residential, and commercial properties through
        transparent transactions, professional service, and customer-focused solutions, while
        ensuring integrity, reliability, and long-term value in every real estate deal.
    </div>
</section>

<section>
    <h2 class="section-title">Our Services</h2>
    <div class="services">
        <div class="service"><i class="fas fa-map-marked-alt"></i><p>Land Sales</p></div>
        <div class="service"><i class="fas fa-home"></i><p>Residential Properties</p></div>
        <div class="service"><i class="fas fa-building"></i><p>Commercial Properties</p></div>
        <div class="service"><i class="fas fa-file-contract"></i><p>Legal Documentation Support</p></div>
    </div>
</section>

<!-- LANDS SECTION WITH 5 LANDS -->
<section id="lands">
<h2 class="section-title">Available Lands</h2>
<div class="services">
    <div class="service">
        <div class="slideshow-container">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/606830374_122113965237133084_3732859690240534090_n.jpg?_nc_cat=101&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeG58rVkv4EbtFjpQkqaBHymRdnMdo6ZQt9F2cx2jplC32E2UpMoPGN8YvKkJSCYbbCfMjFgCrm093tiHHwsTpnr&_nc_ohc=a6L7GMFydd4Q7kNvwEJYNT0&_nc_oc=AdmoZ1-wu_IdoMr979foCE9Y2H9GBGAQB22FuyMiTryGzbYPKWpqa5fjhdQfosi03Ic&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=pyXL-AUr_UGk32dPmVK7tg&oh=00_Afoze4nDF_dZeZH79qIh9CuOlhBbMnIITYoJh-Eing_eOA&oe=696EB3CC" class="active">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/605552766_122113965069133084_6810628358493565170_n.jpg?_nc_cat=107&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeEW8qWoDGBH6Snrk6EDlWIhQC2RszFEzdFALZGzMUTN0c6-Jb0YATz2Zf4AV7uekXCQeQLElynOIi653oGaEnf3&_nc_ohc=E_MxsikKRh0Q7kNvwH-IB_5&_nc_oc=Adn27yl3TqKWhjVuYKlsd9_BauYuY7XVJCrqdCy2NrK8cgXbwcYUDaJKcQZVHOa1SqY&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=Jz45ukv2fjkODVQBFRWO_Q&oh=00_AfoTvsHESCDtqemw0bFoyHBeLEZy3PZMJT-cFAPuWtsgzw&oe=696EB8DE">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/605932215_122113965033133084_3471864914291549056_n.jpg?_nc_cat=102&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeFQqIG-RrdRZzTysU8mczYF418ly4bYyy3jXyXLhtjLLSIWEhKEXHeNeqFX_8N-ya1Jf2ON_P2QI-L0X8a-kH-m&_nc_ohc=bJU4pU4_tXkQ7kNvwF-5y0m&_nc_oc=AdmjlF2Pba379IjMIsN6PHj2qWvwNUKMEO6aG8osKOc4He4ti86a_56Zr6WRYqxTwGA&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=rzIr_jy7_PNy5QjJWja26w&oh=00_AfpNP2NktYvmj3mHOeaznV1W21Wm1QvToD8d9th2t6g5lg&oe=696ED503">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/606054403_122113965063133084_8205583403032058304_n.jpg?_nc_cat=107&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeFI_KzCvlZ8jAHrUdqRYi1mEXUdbNXMNSYRdR1s1cw1JrBl69jvwBYKVDuFn10Z-Tqh1t7_SyO6l9pKWLNK2MJx&_nc_ohc=J3OHkY7U_PUQ7kNvwHyXPnt&_nc_oc=AdlOLgTLaIkuXmcWmqJLCwOSPk5n756z-LAxp6qxFulO_nx7ncdUx6uwFgiD2ktl4t8&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=6Fimdyv_eveEpl9_fjLJMg&oh=00_Afq90gRx__dWQSZV2Yarc3AT9HuDOHXY3f78R_PVbOkEvQ&oe=696ED726">
        </div>
        <div class="slide-desc">Dickwella – Land</div>
        <div class="slide-price">Price: LKR 2,500,000</div>
    </div>

    <div class="service">
        <div class="slideshow-container">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/606872761_122114156409133084_4364106421123919489_n.jpg?_nc_cat=105&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeElZBiOfl9ZUmRzT8C1TmuFtE_mPqPjM6G0T-Y-o-MzoVKX-5EKJFRkt4jjvciBREnuHkVTZsojfezg0_cfKGrN&_nc_ohc=Jnfb-9pXGZkQ7kNvwEBUZfL&_nc_oc=Adn7eTg3-DPKkRRl0sMg4C2B9JUHFfG0MHe77DF614pCgf3bIH7Ci6fj8BR7DBhi2xA&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=pSZk9YVlUdkcVeeYBiRORA&oh=00_AfoN4bQ9Db-a9p3JQ9RKhCKZoVJ2CVlzzldXTEoGbYikEA&oe=696ED6DE" class="active">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/606865534_122114156235133084_7675868041739777223_n.jpg?_nc_cat=106&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeFZ7c6FpCycVMHtSf9KDhGVPfdGs7PAFXk990azs8AVee6XeYsQiVK0XavQb2_zysd1z4xTOhYUyr26CP9fzCvY&_nc_ohc=52xx6wfEc50Q7kNvwFmfG8J&_nc_oc=AdlEuDoDmiCh1hEXWenreieB9bDzRMpzw-UxbBYo9garv8oWNQfG4-BYm7Ac4rI-3nE&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=oYK8_jR0MAeaJLsYDXUjvg&oh=00_Afr65OpPPffXPKwDkYfQe3zsk6XeFSXj8_jsssGzUJBrEA&oe=696ECB28">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/605700987_122114156337133084_4086358173298020830_n.jpg?_nc_cat=101&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeG39LaQ-MIulXN6Z7SQ2qw1SDMkZotuV5VIMyRmi25XlVrczf1LzQGhHP0M9G9-dnSNECS1MDe8DIeEK-ib9i1q&_nc_ohc=RsLg1q6zRzoQ7kNvwGA7lWX&_nc_oc=AdmupsVWNL2wOyWiHGJVpCK66jgonhxxCBlzPy7mwHRYkssev4S8Ew_vymTzzweL9so&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=PvGTlpwZM99rurglzXE6LQ&oh=00_AfqxKyncLWKjJpHr01bNoAPCV3DZgKMCsAerrbrJYQhCzg&oe=696ED68F">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/606029577_122114156289133084_2283842719166874719_n.jpg?_nc_cat=110&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeGhTKAgoFgSlZ8L6BN3giTO3dIjUoaXbdDd0iNShpdt0LHnVWS9Kx9IbcL1UuPha4T7Kj_ikF5ta_2afres1Uhp&_nc_ohc=jKfNKyzyaMUQ7kNvwExUgp1&_nc_oc=AdlxOrx7uLVAB_zdJEbR_OvBN3zZbOonuyPgn8TapXbUFRtc4W3xzAWaHR0cdsjbgj8&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=M2TxTcsCh0nDa_HCf5S4zQ&oh=00_Afo_cfRK4m4alHM587x4Bp8R4xnHsUUbPbJhrZr6mNfv7w&oe=696ED136">
        </div>
        <div class="slide-desc">Madiwela – Land</div>
        <div class="slide-price">Price: LKR 2,500,000</div>
    </div>

    <div class="service">
        <div class="slideshow-container">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/607451767_122114722131133084_1040448840987592544_n.jpg?_nc_cat=110&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeGkivycvla7E31_FDpwxvEvb9NLcRITkDpv00txEhOQOnbtTXbP8GL9WI0kBo2aF1PiY2eSOufeeHTt7z12lsX2&_nc_ohc=7EvirxNxS3MQ7kNvwEn0PE9&_nc_oc=Adm4QtOPqTO1XNwLah0LnfV4hjOrfvsOR6DiIjGM1vc9QgTLcYvLybfyW4CmtDAzt64&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=MT-TPM5HZ0Tb0FWERAtzwA&oh=00_AfoeSdNEsZCaRxbGygL3oa_ZLCyvWzmOmrHDBvJ6Ztu3bw&oe=696EBF69" class="active">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/609041783_122114722167133084_9055609117367409812_n.jpg?_nc_cat=110&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeFZLxSuyNRUhB1jue_nXwBEqsnbVD78psKqydtUPvymwj7Efm1YaKx2F8UmBGr4llM3k6SwGPYteRXQUyAhDL8D&_nc_ohc=iBNX8WrD9z0Q7kNvwGKWxCD&_nc_oc=AdmXxx1qIoVaPbzYdqloaf96ht4DK6dVYW3pgwGG33uy7McyWZT1303Y_vXKOYEpt1g&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=-ZBqKLDn3ee4LOR0xl37wQ&oh=00_Afp-CoCJL2yJ-0adi560qVUrHfW5Dk4ANfidylI5cE4Vtg&oe=696EDDE8">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/607947721_122114722233133084_3834837283399406583_n.jpg?_nc_cat=106&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeEXSiB2QSc23KhfhJSZWtqSU0_RcUEWMI9TT9FxQRYwj7S2lp5n19FE5b4L1gSttNNgMnGpK8_wZFJzdzGGl6Vl&_nc_ohc=w2m4fAZEzSoQ7kNvwGOft7b&_nc_oc=Adk0rVDTCCamGr2LqABOc-NaIM24c2YZOmG5xiO6y860o_ApEoIvXuPyXI9E9DAfZms&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=aIxAcHIDWYUkwyXCu2v6ag&oh=00_AfrIucibevlyHsM7X0EsPscZ5E5upua1nwk7SjIJ1MiH2g&oe=696EB501">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/611227577_122114722239133084_91094060167356222_n.jpg?_nc_cat=102&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeGvEyYyyoQiIf4C_6na_9uryej-HGLauI7J6P4cYtq4jmranKXeC3N4IDckFri1pR-F-mnzIBaLFHboJWrN4Ljr&_nc_ohc=b0X8REcSMksQ7kNvwFcSWGZ&_nc_oc=Adm4-xumiPkKejJpwkBnDoi0jqM4pTGWwlWsUlaN-YtSDuPvENcW1RK_IxRYJAobp7M&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=Cx9I7_R6uQfSJo6gVR2dKQ&oh=00_AfrPCD0OxBKqMMH7BLkPbS9QWtXEUZg5aaWtTtPM4sXQMg&oe=696EB5DA">
        </div>
        <div class="slide-desc">Galle – Land</div>
        <div class="slide-price">Price: LKR 2,800,000</div>
    </div>

    <div class="service">
        <div class="slideshow-container">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/608199398_122114735139133084_3526678143294561125_n.jpg?_nc_cat=100&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeGAI_qRKu_ooXC6zrQj-2XpEGlSVPDH5L4QaVJU8MfkvuRoN2c45d9zAzWi6VmYQX3HCMuW29NddX_wHjw3neeM&_nc_ohc=g6mrrMIebEkQ7kNvwF7dUzo&_nc_oc=AdlIs-Yf5R5ZjLZvlwP9WyLg58Lc7DEP-NFlCK9wIqI2TNC7g3sySUt16uCfHCC56es&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=ow2HJfYkTPIVoaYAI2AQkA&oh=00_AfrkvtWcngH5rZuShUP2l5zFK1HIywNP4leiq89x3DjW4A&oe=696EE28D" class="active">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/609199255_122114735217133084_3026431063942289062_n.jpg?_nc_cat=101&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeF7pWzb80elxS9MxpWxhwhKrExvyX_kgRasTG_Jf-SBFt0YUcQXtS04-fCsskhBEuM9LW3HNRKqSSn9iTp6PVi6&_nc_ohc=2Dgl54Sz8cUQ7kNvwGrN-5l&_nc_oc=AdlFLIM90JZHlsWB0b23-Qe9uCFwABXV5-JqdLp82CiDK0zuTn1fM5WjzG0ZzotQEcs&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=ERn4_hT2ro7c1XvCcc1eTQ&oh=00_AfryU6yXbM9bPG7IJ3Q7JcgzHa6wHvnFCybB75IP51g2lg&oe=696ECAB6">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/608903571_122114735175133084_1052336132751576714_n.jpg?_nc_cat=103&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeEpoFGZYyiCMeV1ShWj6PoFqzkbJ0h1w26rORsnSHXDbmvQpwPkMihuoffmtRnjY9WyrveyjP8g6_buTZMhtBnp&_nc_ohc=YyW-O8H8jS8Q7kNvwGrSM6a&_nc_oc=Adle0qtee18kDU21S-T3uphu7hVH6VBltZw2mAnXFYMKE_w0XxNr6RdFdhn2v-M1PVU&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=kLRhO5cWpi2EoTffvgdn5A&oh=00_AfpWT1PK_LsO6_44TW9TY5hp5_yNE0N7AFtKm9buREEZIA&oe=696ED205">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/608107314_122114735163133084_5934592554088092485_n.jpg?_nc_cat=103&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeHOw1vRdI5Yps_FniLYE8fraVtFUQULA0dpW0VRBQsDR-6ob8OcgSJ9BfUhmEC817_SZ_PUvnLBXTvAgKke7xY7&_nc_ohc=01VUp5VpDlMQ7kNvwHCR-Es&_nc_oc=AdmB0HwjYj5t1qPcKqK58I-IPUbzF6q8iKFYCq6gLCg__7WAyaWEl9bBA9P2Ld6UXeU&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=uaWGIvX4IYBqhPSanb1Hgw&oh=00_Afod_s1CPt56Op8uh30nukEqdH6z4Nyli1AdBPwN402ohw&oe=696EAD35">
        </div>
        <div class="slide-desc">Mahamodara – Land</div>
        <div class="slide-price">Price: LKR 47,500,000</div>
    </div>

    <div class="service">
        <div class="slideshow-container">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/611219485_122114727249133084_7695048067140864477_n.jpg?_nc_cat=100&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeHhqaMx7gPyYAPKIU__j1RhTmW5rS0PP7hOZbmtLQ8_uCNLqx6GMgh8PR5396AzKWOSzW02vAgyjZqXeGlSqMPf&_nc_ohc=HDpg1LQ3UU8Q7kNvwHmYE39&_nc_oc=AdnuFZ_L1aGBOIkfr1IDtZN-a-hd8bFzeM1mwzo_dIt5ZdRUJ-1ke7Y4ouhi9jgrpYI&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=chTkdVJZGCA-J9nibqrTbw&oh=00_AfrLUDSyS39s_lq2r2XTyUk3SYvz4fI5taKUDSzLsAbsAQ&oe=696EE134" class="active">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/608196358_122114727195133084_3693431672289950503_n.jpg?_nc_cat=109&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeG_MAIaoAbvW41maechJE_OPK6QJtxnTAI8rpAm3GdMAjZznzuTuZwsZyZ5EauFt3AATBIQh6ECvNolqJwNgbrP&_nc_ohc=Stj6UtWGpG4Q7kNvwHqTZ-8&_nc_oc=AdnJNN16CHxqV65a6DMBKw53RjPjFl5jTtqGgs8weY5UFhnhQWJA5JoTSKGIgl3qDCA&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=8x93_1dCcDityGW9gf5W9w&oh=00_AfrPc9W2ygTd82nxRyJDBuK8YES_v2lr-_IqGryr-A5nyA&oe=696EAE2D">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/611844652_122114727201133084_6489077608433578778_n.jpg?_nc_cat=101&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeFw8yAU0Wsh_N0iEsMnTiIYEjXhHb1hy3USNeEdvWHLdZpz-EjxAtZ936k9mtMhShqkf1Q_6HPUbfgkTqslUqFv&_nc_ohc=GFFNrxR3HtYQ7kNvwHeRX0D&_nc_oc=Adli-iOdgrOI2ca7Rq4BNjrNpGNqhBjk8SD16CsBtkf8G_78n7JSx2PiEARXy6RvhMs&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=tL-x76BzHA50AYDQTdyi-A&oh=00_Afp6FwrWMbjdSMKJWNTbFcKafVpVsOhZHnd75ltwXUPoVQ&oe=696EC0CA">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/610906847_122114727189133084_7606011961661763647_n.jpg?_nc_cat=101&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeEKgXTn1zrRUpxmU21tbRvUqVUSQFieeSypVRJAWJ55LLsv2j_zL6YifAudjDj2qhVO5vSZBKyG614JmjlQdpsr&_nc_ohc=Y_LDK13BKu8Q7kNvwHxobvY&_nc_oc=AdkzHQ_YOamEZKmIaGm0gamYtEXXnMdJeVSnhXHrjZX9JgckzgdJ4MvxfnuI8BsMLq4&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=mV-Btq4_5gze3i_nYRYueg&oh=00_AfqoFMDpU2McH8GDDVqs_mC-Z-Z_6-I_9j04hBjN0kERHg&oe=696ECF1E">
        </div>
        <div class="slide-desc">Negombo – Land</div>
        <div class="slide-price">Price: LKR 10,750,000</div>
    </div>
</div>
</section>

<!-- HOUSES SECTION WITH 5 HOUSES -->
<section id="houses">
<h2 class="section-title">Available Houses</h2>
<div class="services">
    <div class="service">
        <div class="slideshow-container">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/608844011_122114535027133084_2259504376130611911_n.jpg?_nc_cat=110&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeH5NpLY70_HXWPRRmJDg17MnPF_WrkBHx6c8X9auQEfHjcNI1rzJcDUJIPEvYL5YZ8QDL3tHep_U7tWTChfU6ou&_nc_ohc=fnhl8ej-4IcQ7kNvwF82Eu0&_nc_oc=AdmBsi6ohPDN0iYWhP8hHhq5j6W740C226wdKyg954D30qInGVkcdLAGUz1bEwqJTtE&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=ijyVsqA6lBlQHKPSOMmBmg&oh=00_Afqa06Nr2lJ8_hBERAwgE8x4xQD0X-IZbe0q4Is5GX_Ktg&oe=696EAE0A" class="active">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/607696928_122114534673133084_3795597021224559364_n.jpg?_nc_cat=108&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeEoSgmn6vUjj67nZ0IBMOIYgmyNn0MdcXSCbI2fQx1xdJ-iMd3RMxCAVS_a6LuI4F2FjVbMr7i8fyRYjsg00K_I&_nc_ohc=oJAlsvwvGkYQ7kNvwGxGvuq&_nc_oc=Adm9b2Be0OrjgUuBjXxSJeFB782pI5Mzdp__e0hFjx-yQXJuXynLKuH7YTTXOZe1lR4&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=lfSNekVV8Da_HS8dCR5bTw&oh=00_AfrEb6Mjzv4mqdWwIhCgUYv74Hh-caOidhgl4uGxTGhiPg&oe=696ED050">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/606762167_122114534733133084_7372009909108222049_n.jpg?_nc_cat=103&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeECm6ivQNxa6KUujebUoWWo9x7PzDS79IX3Hs_MNLv0hb0SSeERwgY5Er5yM_6hbQN3sexKrbJKdPlkUFReM2XD&_nc_ohc=5VCcsj4zsiUQ7kNvwEjgWKB&_nc_oc=AdmQZ8Q_qtZO-tAcwO_vYDPZZFFekzLRUbsuEDN_mO-Q9g5kSwrF5RqvsNID2uJuvIQ&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=ftWnOvwMbtVDWpLqGhOVpw&oh=00_AfrAu2niTWA9_IxxgfZkKHvsI4mEZ28JpyG8nTCyaBfyrA&oe=696ED176">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/607974641_122114534781133084_3867053238207501553_n.jpg?_nc_cat=100&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeEsprzAG9RCaLcMQhZElQhBUUp6ipVhiQhRSnqKlWGJCOUHz3_BLTIn6GU2uMM3xsT3uL2uHJ2hc0nAOtJLYTcU&_nc_ohc=VhHIXMMLbQsQ7kNvwGihWDQ&_nc_oc=Adkg1z5T6OCYwvdv2cYk3ZAxE244LTPLiFN2k-FKIxvqSiQIc3e64pe5DqfIw83SzUM&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=04ZZZ6-3VffUR4rHG00XvQ&oh=00_AfqT70mY07opPUEGrNQCJ9jC47LvfrMvTxlOPEnaWQAlmw&oe=696EC71B">
             <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/608551966_122114534529133084_5707438681854555785_n.jpg?_nc_cat=108&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeHC_SEV_Zpk3dgjfw0-8eirKdqLUDpD7EQp2otQOkPsRJTsSx8Nxdhew6PQtwNBIOJ3L-ORHb8nKruEDbII4csm&_nc_ohc=5_tiOtnG6oAQ7kNvwFVsfmn&_nc_oc=Adnuabo5dvSu4kTOpG0XNuVXATq1uOt-NQxygZDfK_YCeqM6kDCO5DHpAGKT2FNw1_s&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=PdOApptwVRqfPybS49IN9A&oh=00_Afo4rfwRBJAFubVSNI5iH4Y6KEj893Kx6QmqYzgJpBSDsg&oe=696ECB5A">
                <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/611151868_122114534619133084_9167457835633199969_n.jpg?_nc_cat=111&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeEQgreE6LMBKiiM1Si56OAQicErkYhqZWuJwSuRiGplayeHQz9DAO3Flmnnr1Q3wehZrkv8Oaj2hKgDfe0uDuDL&_nc_ohc=CFNFf8Oc0HAQ7kNvwHSzOOP&_nc_oc=Adny_qCS5ZS1zaDWwqlqKNEJ1N8NyLcKEJCm717bhp8_mjRZ5DQuXpNjtaXOBHPDTu0&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=gSHlISytYTOdyEqhvpFFew&oh=00_AfoROzYAS4eYA01A61JeH81U0sS-xqAU7UduDPpDcOqbYA&oe=696EC750">
        </div>
        <div class="slide-desc">Dickwella House</div>
        <div class="slide-price">Price: LKR 47,500,000</div>
    </div>

    <div class="service">
        <div class="slideshow-container">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/608005510_122114526183133084_2283769059349277277_n.jpg?_nc_cat=110&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeERgtE9NgbS-EZM1hGPnke8XL8OSabnwSxcvw5JpufBLNQbQLZbWceyfNzX0xrIFXm16lyk8FSES_s_j527C2ib&_nc_ohc=xFTLmqTZMhgQ7kNvwHXsjcO&_nc_oc=AdnOlvoahJcKWMiGbl48F_J_xAMQHuS3I_EphlNeHAzi3MJ3d9KRqDHKrYpuzKFrSS0&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=cvWANM12wLFbwLbMtoVckw&oh=00_Afp4PBZX2IKklph4FUaahl202suzav4SDVzJSll4nd6adA&oe=696EC0CD" class="active">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/609062380_122114526279133084_3008972623967693391_n.jpg?_nc_cat=110&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeHrGrCXwMTU0rRo_HCsLjn3nuIVStN5R1-e4hVK03lHX-VEgM6i7SIMDVqowpBFsF1lJyiIpSJZ6SO8qd-ptGoP&_nc_ohc=cpFdEoO4sKoQ7kNvwGEnVOu&_nc_oc=Adma2iGGTYyMAO4YXYvKwQC1xeFUfMO2bEWimHn0hhA21j9Wev6enHUVG0DLiZ5uZQo&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=6HQuLpx8zXA9z11min7aQQ&oh=00_AfqbwQqc6ERlqUALs80nnvVpLuWqVC1Y_drxQHK6gvHTzQ&oe=696ED091">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/607648440_122114526273133084_497081800863216881_n.jpg?_nc_cat=103&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeGjEHeuQqVM0bUnIDy6T_sZGL63mTyTJecYvreZPJMl5zFjBDbtuQsC8wXUlrPc7m4usSVdtwaQMU3Ta_28mq1c&_nc_ohc=Q_wuVmD_Jm4Q7kNvwEBj6Ag&_nc_oc=Adl7WeCt3D7MCowYgw6II2_udqubX1Q0kyxusS4w2X-P80oJHhvHM4Y90lweMI9z3IQ&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=5E4Ke7Lxi3PSFYqdEbI4Rw&oh=00_AfryV8-qiGTottVBHsS1zeCA9g5p1u91z57cUvm6KcI4ag&oe=696ED92E">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/607112666_122114526327133084_8012758147163345438_n.jpg?_nc_cat=105&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeFV1mPgAobEuLwn4YvMCje61LiN_pBt4JrUuI3-kG3gmvGq1VVazmmDpqTA6VxF1bxkRLa0oOLRAYZNwikSkCTA&_nc_ohc=JZ_dBzM6hOQQ7kNvwFsARVA&_nc_oc=AdmGNMMvW3Pitt6zQ9EHnCNuLC0I6PPx_vvE4OwHsJf_W57_QhArarbl3F04RRQwb9M&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=sX5Zvu-TsI4_QY_fT5tVtw&oh=00_Afrtm675Qmx_A261FP9nExZ3H8m6sN9uPSkdwX_5_ZANMw&oe=696ED2F5">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/607963096_122114526291133084_4884292859598824550_n.jpg?_nc_cat=101&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeE9Ti6VHXduUs0OYkdB3cLmLT5zYDPzmhMtPnNgM_OaE0u6c92ZD8cgzVkiof4H_2whzeczkoVtnyhybAnUXtdm&_nc_ohc=bCdj1S0aBtEQ7kNvwHCQbAP&_nc_oc=AdlwS3suw5oDU6gJFU3ydYUQr6j1RMN_eerfH6E7pB6-hHPEFT6Ie4ZsAULAT0gZfB0&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=1dZPAnWoJ_TzXYb8OXAcFw&oh=00_AfqY-pfhp-lNqBc1XeaSQeVQ7mQrE1D0kPTR_cqf2VtDTw&oe=696EC468">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/607640025_122114526285133084_2640653418046308870_n.jpg?_nc_cat=101&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeEqQuoCcs0FZ1ZyjuyOFQnsOQmVCZu7LsI5CZUJm7suwvAPsgC6sjA94Vmk-8aJW6nuQ5rqss1TDbj93pRAFhfF&_nc_ohc=jeaNhtOCyvIQ7kNvwHlnhli&_nc_oc=AdnewbpkroPJPYjF7bXQaqZMiZxbLTgo_Qcivt5Lp6h4_1EU9xHLiWg11huCWtMDVag&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=0CNROIqwm4_dU12WEUSx_Q&oh=00_Afogn3VPCW6AEQS7NNaW0PFdakzyBmue_qewXAA8j1w22A&oe=696EBBB8">
               <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/610896005_122114526411133084_5196580518196283562_n.jpg?_nc_cat=103&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeFPNmmuGDZqZBtUXruT3Hqkpp3hXQH52NGmneFdAfnY0fP1hcV2dbDzpcKd3h61O4AWIEAfcdMbbMRsI4UaVbGH&_nc_ohc=kAyTDwhiobcQ7kNvwEgIbml&_nc_oc=Adlj5bKOQsIZJ_nN3PbpPiwqm5yAvIelAk44voTDdePYKB9JwA6vomH4Skv6X1BbZOo&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=lnYlOBZ_eMy-VhNdBjcrCA&oh=00_Afq6-a6wYfdV9sadw29naBy79ncIrL5UoF7qkTC9qT_xOA&oe=696EE335">
        </div>
        <div class="slide-desc">Rajagiriya House</div>
        <div class="slide-price">Price: LKR 70,000,000</div>
    </div>

    <div class="service">
        <div class="slideshow-container">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/608179276_122114346537133084_2470207380070520909_n.jpg?_nc_cat=102&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeFcQVRWVI75LB1gMVQOivOx-i1nBwEqB936LWcHASoH3Y-lqYX9PHBz4SUttyADyJIKTaX0wW0FGSbRGvXoUeh8&_nc_ohc=lFYzcp9dKNUQ7kNvwGzWatk&_nc_oc=AdmwRMVEkK7gYiX_8W0N9HIx4JjhbBKT2vVkEARtQHmE9R0szy-3uWrVYNmUxquqrYI&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=jN3XfviZSEe60RiaAMchRg&oh=00_AfqkuzmlXTvOWr2tvDHqMjmUNPYW9k4nW4n4d9g9meoUJQ&oe=696EB2C8" class="active">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/605970034_122114346675133084_1705210023563558311_n.jpg?_nc_cat=111&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeFC5TqJcJXHHquvH_gUmQkxK2u6ZJTt9Mora7pklO30yrV8T8_c3dLDLZ8AfUkO_aUb1GSikAEVS06NPA0lBsoi&_nc_ohc=2qsKyPPo0osQ7kNvwEV0Vwl&_nc_oc=AdmW175g7mV23ud0vQ4gQTn9_3pwu3QKOXLG9Shrqhvz7s0G_nKSQ9YxGfSAaq2JJFw&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=op1EoyV6sSuUCo0HqNIvfw&oh=00_Afo0bX6zNIbBrgnVkLnoX4eQ-WBN0szMYDpltORR7p-BGA&oe=696EB85C">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/607343220_122114346597133084_7908057145303163148_n.jpg?_nc_cat=104&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeEJz73nlC8lra2NfB4Ym5bAdYc6vZYNP751hzq9lg0_vhQw5QfUVL6_kGpuVbTOteyFGaWIsY6_DK_NkmKXwDlc&_nc_ohc=3xNSP89t65IQ7kNvwEyd-Dv&_nc_oc=AdnozHHFZYuWXeX0UupC6KMNU32VmL9p2cUeNj6o3c-2lS_GvW4MM1_Ks-vDF66EH3w&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=sF6vCM74qkerAbmmMRhcvg&oh=00_AfqFlSs9mBXtj7ugcJ76LGOUBIM_geQlFcWDMAN1ddC6iA&oe=696ED262">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/605785697_122114346465133084_6529914608484494048_n.jpg?_nc_cat=111&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeFkJCXhmW39iWxU0-qE-VdcweJapQc6wEbB4lqlBzrARqXK6T-4ePR4yCIHSwnitRWyCNunWVXHcThwvesHcpXH&_nc_ohc=xZiSsVGjWgkQ7kNvwGbwgOv&_nc_oc=AdluS_IA10D0EBdKV4TWRjLsEtAtN5chVmhi8tuFtYJF_WWnblz3b6Ftq_ULfULshyQ&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=wZczubXdFbCed_CPCd9QXg&oh=00_AfpqIsApHeCjsc7g9yqhaGVvMAw7l0YJ9KvPnptu4eWY5g&oe=696ED231">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/610761183_122114346501133084_1188665559381101521_n.jpg?_nc_cat=107&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeF-8IRf8iqQnziP4r3aA_q10pflSqG_hOPSl-VKob-E46-7EBJBhbuOH1wZCTTBVeRyonCnXQVQxXnlhf4jYHjx&_nc_ohc=piFcMu3H_cEQ7kNvwG_E4Vp&_nc_oc=AdmuydOqNKG0NIlb5_J6UG8cnm84Ezw3TpitZMWzME5yDEDlgVN926zz0MB-o1W20EQ&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=HOmXw3M5FD2kkYzmSBXeFw&oh=00_Afohm9CPQmSbUDIjZbAPS2EdjCIjzSh18aVoola7U_EzUA&oe=696EB2C2">
        </div>
        <div class="slide-desc">Awissawella House</div>
        <div class="slide-price">Price: LKR 55,000,000</div>
    </div>

    <div class="service">
        <div class="slideshow-container">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/615637912_122116938039133084_2265013406324927627_n.jpg?_nc_cat=110&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeHeE02jeVxr9g4WOqR5V5lntyYH3A2qsvK3JgfcDaqy8lOx-hGQKkYbKbu2wf194EIl1taIFWEUX5DSE_nesBWc&_nc_ohc=aU6EAxHWa2oQ7kNvwE7TxfU&_nc_oc=Adk-aRi8jAr5MnINK3soOp3inOJlWZ7rXtjGuH0Y-Mz7VmKhmVuShDNhLA1NcNRsLcA&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=a7RboHnMDi4W8SQDOkJhyA&oh=00_AfpX0Aj2LrUrxbZ5rRfwgkHNLRgaFGTBkdLQ72SYxwZF9g&oe=696FB756" class="active">
</div>
        <div class="slide-desc">Await</div>
        <div class="slide-price"></div>
    </div>

    <div class="service">
        <div class="slideshow-container">
            <img src="https://scontent.fcmb2-2.fna.fbcdn.net/v/t39.30808-6/615637912_122116938039133084_2265013406324927627_n.jpg?_nc_cat=110&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeHeE02jeVxr9g4WOqR5V5lntyYH3A2qsvK3JgfcDaqy8lOx-hGQKkYbKbu2wf194EIl1taIFWEUX5DSE_nesBWc&_nc_ohc=aU6EAxHWa2oQ7kNvwE7TxfU&_nc_oc=Adk-aRi8jAr5MnINK3soOp3inOJlWZ7rXtjGuH0Y-Mz7VmKhmVuShDNhLA1NcNRsLcA&_nc_zt=23&_nc_ht=scontent.fcmb2-2.fna&_nc_gid=a7RboHnMDi4W8SQDOkJhyA&oh=00_AfpX0Aj2LrUrxbZ5rRfwgkHNLRgaFGTBkdLQ72SYxwZF9g&oe=696FB756" class="active">
            
        </div>
        <div class="slide-desc">Await</div>
        <div class="slide-price"></div>
    </div>
</div>
</section>

<section id="reviews">
    <h2 class="section-title">Customer Reviews</h2>
    <div id="reviewList"></div>
    <div class="review-form">
        <input id="rName" placeholder="Your Name">
        <textarea id="rText" placeholder="Your Review"></textarea>
        <button onclick="addReview()">Submit Review</button>
    </div>
</section>

<section id="contact">
    <h2 class="section-title">Contact Us</h2>
    <div class="contact-box">
        <a class="whatsapp" href="https://wa.me/94776173004"><i class="fab fa-whatsapp"></i> WhatsApp</a>
        <a class="email" href="mailto:infocprealestate@gmail.com"><i class="fas fa-envelope"></i> Email</a>
    </div>
</section>

<footer>
    <div class="footer-grid">
        <div>
            <h3>Address</h3>
            <p>46, Edirigoda Road<br>Nugegoda, Sri Lanka</p>
        </div>
        <div>
            <h3>Quick Links</h3>
            <div class="footer-links">
                <a href="#lands">Lands</a><br>
                <a href="#houses">Houses</a><br>
                <a href="#contact">Contact</a><br>
            </div>
        </div>
        <div>
            <h3>Follow Us</h3>
            <div class="social">
                <a href="https://www.facebook.com/profile.php?id=61583992522925"><i class="fab fa-facebook"></i></a>
                <a href="https://www.instagram.com/cph_property_sales/"><i class="fab fa-instagram"></i></a>
                <a href="https://www.tiktok.com/@colombo.perpetual"><i class="fab fa-tiktok"></i></a>
            </div>
        </div>
    </div>

    <div class="footer-bottom">
        © 2026 Colombo Perpetual Real Estate (Pvt) Ltd. All Rights Reserved.
    </div>
</footer>

<script>
function addReview(){
    const name=document.getElementById('rName').value;
    const text=document.getElementById('rText').value;
    if(!name||!text) return;
    const div=document.createElement('div');
    div.className='review';
    div.innerHTML=`<h4>★★★★★</h4><p>${text}</p><small>- ${name}</small>`;
    document.getElementById('reviewList').prepend(div);
    document.getElementById('rName').value='';
    document.getElementById('rText').value='';
}

// LAND/HOUSE SLIDESHOWS
document.querySelectorAll('.slideshow-container').forEach(container=>{
    let index=0;
    const slides=container.querySelectorAll('img');
    setInterval(()=>{
        slides.forEach(s=>s.classList.remove('active'));
        index=(index+1)%slides.length;
        slides[index].classList.add('active');
    },3000);
});
</script>

</body>
</html>
