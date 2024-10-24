<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Beautiful Coastal Homes</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f8ff;
        }
        header {
            background-color: #2c3e50;
            color: white;
            padding: 20px;
            text-align: center;
        }
        nav {
            margin: 20px 0;
        }
        nav a {
            margin: 0 15px;
            color: white;
            text-decoration: none;
            transition: color 0.3s;
        }
        nav a:hover {
            color: #1abc9c;
        }
        .container {
            width: 80%;
            margin: auto;
        }
        .property {
            border: 1px solid #ccc;
            border-radius: 5px;
            margin: 20px 0;
            padding: 10px;
            display: flex;
            flex-direction: column;
            align-items: center;
            transition: box-shadow 0.3s;
        }
        .property:hover {
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
        }
        img {
            max-width: 100%;
            border-radius: 5px;
        }
        footer {
            background-color: #2c3e50;
            color: white;
            text-align: center;
            padding: 10px;
            position: relative;
            bottom: 0;
            width: 100%;
        }
        .contact, .reviews {
            margin: 20px 0;
        }
        .payment {
            margin: 20px 0;
        }
        .review {
            border: 1px solid #ccc;
            border-radius: 5px;
            margin: 10px 0;
            padding: 10px;
            background-color: #ffffff;
        }
        .form-container {
            margin: 20px 0;
        }
        input, textarea {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        button {
            background-color: #1abc9c;
            color: white;
            padding: 10px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        button:hover {
            background-color: #16a085;
        }
    </style>
</head>
<body>

<header>
    <h1>Beautiful Coastal Homes</h1>
    <nav>
        <a href="#properties">العقارات</a>
        <a href="#contact">تواصل معنا</a>
        <a href="#payment">الدفع</a>
        <a href="#reviews">الآراء</a>
    </nav>
</header>

<div class="container">
    <section id="properties">
        <h2>العقارات المتاحة</h2>
        <div class="property">
            <h3>فيلا فاخرة</h3>
            <img src="https://via.placeholder.com/300" alt="فيلا فاخرة">
            <p>موقع: الساحل الشمالي</p>
            <p>سعر: 1,500,000 جنيه</p>
            <button onclick="alert('تم إضافة الفيلا إلى السلة!')">احجز الآن</button>
        </div>
        <div class="property">
            <h3>شاليه مميز</h3>
            <img src="https://via.placeholder.com/300" alt="شاليه مميز">
            <p>موقع: الساحل الشمالي</p>
            <p>سعر: 750,000 جنيه</p>
            <button onclick="alert('تم إضافة الشاليه إلى السلة!')">احجز الآن</button>
        </div>
    </section>

    <section id="contact" class="contact">
        <h2>تواصل معنا</h2>
        <p>لأي استفسارات، اتصل بنا على الرقم: 01004472544</p>
        <div class="form-container">
            <h3>نموذج الاتصال</h3>
            <input type="text" id="name" placeholder="الاسم" required>
            <input type="email" id="email" placeholder="البريد الإلكتروني" required>
            <textarea id="message" placeholder="رسالتك" rows="4" required></textarea>
            <button onclick="sendMessage()">إرسال</button>
        </div>
    </section>

    <section id="payment" class="payment">
        <h2>خيارات الدفع</h2>
        <p>يمكنك الدفع باستخدام فودافون كاش على الرقم: 01004472544</p>
    </section>

    <section id="reviews" class="reviews">
        <h2>الآراء</h2>
        <div class="review">
            <strong>أحمد:</strong>
            <p>خدمة ممتازة، وكل شيء كان رائعًا!</p>
        </div>
        <div class="review">
            <strong>سارة:</strong>
            <p>أنصح الجميع بالتعامل معهم، تجربة رائعة!</p>
        </div>
    </section>
</div>

<footer>
    <p>جميع الحقوق محفوظة © 2024 Beautiful Coastal Homes</p>
</footer>

<script>
    function sendMessage() {
        const name = document.getElementById("name").value;
        const email = document.getElementById("email").value;
        const message = document.getElementById("message").value;

        if (name && email && message) {
            alert(`شكرًا، ${name}! تم إرسال رسالتك بنجاح.`);
            document.getElementById("name").value = '';
            document.getElementById("email").value = '';
            document.getElementById("message").value = '';
        } else {
            alert('يرجى ملء جميع الحقول.');
        }
    }
</script>

</body>
</html>

