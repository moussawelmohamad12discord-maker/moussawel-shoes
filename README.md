# moussawel-shoes
Moussawel Shoes online store

<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>MOUSSAWEL SHOES</title>
<style>
*{box-sizing:border-box}
body{margin:0;background:#101010;color:white;font-family:Arial,sans-serif}
header{background:#080808;padding:22px;text-align:center;border-bottom:2px solid #c69b45}
.logo{font-size:32px;font-weight:bold;color:#d6ad59;letter-spacing:2px}
nav{padding:15px;text-align:center}
nav a{color:#e3bd70;text-decoration:none;margin:12px}
.hero{text-align:center;padding:65px 15px;background:linear-gradient(120deg,#161616,#382912)}
.hero h1{font-size:36px;color:#e3bd70}
.hero p{font-size:18px}
.btn{display:inline-block;background:#d5aa54;color:#111;padding:13px 24px;border-radius:25px;text-decoration:none;font-weight:bold;margin-top:12px}
h2{text-align:center;color:#d6ad59;margin:35px 0 20px}
.products{display:grid;grid-template-columns:repeat(auto-fit,minmax(210px,1fr));gap:18px;padding:18px;max-width:1100px;margin:auto}
.card{background:#202020;border:1px solid #9d793c;border-radius:12px;overflow:hidden;text-align:center;padding-bottom:18px}
.card img{width:100%;height:190px;object-fit:cover}
.card h3{color:#e4c17d}
.price{color:#e5bd67;font-size:21px;font-weight:bold}
footer{text-align:center;background:#080808;padding:28px;margin-top:35px;color:#d6ad59}
</style>
</head>
<body>

<header>
<div class="logo">MOUSSAWEL</div>
<div style="letter-spacing:7px">SHOES</div>
<div style="color:#d6ad59">STEP INTO STYLE</div>
</header>

<nav>
<a href="#home">الرئيسية</a>
<a href="#formal">أحذية رسمية</a>
<a href="#sport">أحذية رياضية</a>
<a href="#contact">اتصل بنا</a>
</nav>

<section class="hero" id="home">
<h1>أناقتك تبدأ من هنا</h1>
<p>اكتشف أحدث الأحذية الرجالية</p>
<p>جودة وأناقة في كل خطوة</p>
<a class="btn" href="#products">اكتشف منتجاتنا</a>
</section>

<h2 id="products">أحذيتنا</h2>

<section class="products">

<div class="card" id="formal">
<img src="https://images.unsplash.com/photo-1614252369475-531eba835eb1?w=600" alt="حذاء رسمي">
<h3>حذاء رجالي رسمي</h3>
<p>أناقة للمناسبات والعمل</p>
<div class="price">اسأل عن السعر</div>
<a class="btn order" href="#">اطلب عبر WhatsApp</a>
</div>

<div class="card" id="sport">
<img src="https://images.unsplash.com/photo-1542291026-7eec264c27ff?w=600" alt="حذاء رياضي">
<h3>حذاء رجالي رياضي</h3>
<p>راحة وأناقة يومية</p>
<div class="price">اسأل عن السعر</div>
<a class="btn order" href="#">اطلب عبر WhatsApp</a>
</div>

</section>

<footer id="contact">
<h2>MOUSSAWEL SHOES</h2>
<p>طرابلس - لبنان</p>
<p>للطلب والاستفسار تواصل معنا</p>
<a class="btn" id="whatsapp" href="#">تواصل عبر WhatsApp</a>
<p>© 2026 MOUSSAWEL SHOES</p>
</footer>

<script>
// ضع رقم WhatsApp الخاص بالمحل هنا
// مثال: 96170123456
const WHATSAPP_NUMBER = "96170069189";

function orderLink(message){
return "https://wa.me/"+WHATSAPP_NUMBER+
"?text="+encodeURIComponent(message);
}

document.querySelectorAll(".order").forEach((button)=>{
button.href=orderLink("مرحباً، أريد الاستفسار عن الأحذية في MOUSSAWEL SHOES");
});

document.getElementById("whatsapp").href=
orderLink("مرحباً، أريد التواصل مع MOUSSAWEL SHOES");
</script>

</body>
</html>
