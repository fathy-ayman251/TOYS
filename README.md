<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>TOYS</title>
  <style>
    body {
      background-color: #f8f9fa;
      font-family: 'Cairo', sans-serif;
      margin: 0;
      padding: 0;
    }
    header {
      background-color: #007bff;
      color: white;
      padding: 20px;
      text-align: center;
    }
    .lang-switch {
      position: absolute;
      top: 20px;
      left: 20px;
    }
    .lang-switch select {
      padding: 5px;
    }
    .product-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
      padding: 20px;
    }
    .product {
      background-color: white;
      border-radius: 10px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
      padding: 15px;
      text-align: center;
    }
    .product img {
      max-width: 100%;
      border-radius: 8px;
    }
    .product h3 {
      margin: 10px 0;
    }
    .price {
      color: #28a745;
      font-weight: bold;
    }
    footer {
      text-align: center;
      padding: 20px;
    }
    .social-buttons a {
      margin: 0 10px;
      text-decoration: none;
      font-size: 18px;
      color: white;
      background-color: #25D366;
      padding: 10px 15px;
      border-radius: 8px;
    }
    .social-buttons a.facebook { background-color: #4267B2; }
    .social-buttons a.instagram { background-color: #C13584; }
  </style>
</head>
<body>
  <header>
    <h1>TOYS ♻</h1>
    <div class="lang-switch">
      <select onchange="changeLang(this.value)">
        <option value="ar">العربية</option>
        <option value="en">English</option>
      </select>
    </div>
  </header>

  <main class="product-grid" id="product-grid">
    <!-- يمكنك تكرار هذا البلوك لحد 50 منتج -->
    <div class="product">
      <img src="product1.jpg" alt="منتج 1">
      <h3>اسم المنتج</h3>
      <p>وصف قصير للمنتج.</p>
      <p class="price">150 جنيه</p>
    </div>
    <!-- أضف مزيد من المنتجات هنا -->
  </main>

  <footer>
    <div class="social-buttons">
      <a href="https://wa.me/201000000000" target="_blank">واتساب</a>
      <a href="https://www.facebook.com/messages/t/YOUR_PAGE_ID" class="facebook" target="_blank">فيسبوك</a>
      <a href="https://www.instagram.com/YOUR_PROFILE" class="instagram" target="_blank">إنستجرام</a>
    </div>
  </footer>

  <script>
    function changeLang(lang) {
      // تقدر تطور ده لتبديل النصوص بالكامل حسب اللغة
      alert("تبديل اللغة إلى: " + lang);
    }
  </script>
</body>
</html>
