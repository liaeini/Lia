<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Digital Art Store</title>
    <style>
        body {
            font-family: 'Cursive', sans-serif;
            background-color: #ffe6f2;
            color: #333;
            text-align: center;
            margin: 0;
            padding: 0;
        }

        header {
            background-color: #ff99cc;
            padding: 20px;
        }

        header h1 {
            color: white;
            font-size: 24px;
        }

        nav ul {
            list-style-type: none;
            padding: 0;
        }

        nav ul li {
            display: inline;
            margin: 0 15px;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            cursor: pointer;
        }

        .banner {
            background-color: #ffccdd;
            padding: 50px;
            margin: 20px auto;
        }

        .gallery, .shop, .about, .contact {
            display: none;
            padding: 20px;
        }

        .art-container {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
        }

        .art-item {
            background: white;
            padding: 10px;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            width: 250px;
        }

        .art-item img {
            width: 100%;
            border-radius: 8px;
        }

        .buy-btn {
            background-color: #ff66a3;
            color: white;
            border: none;
            padding: 10px;
            cursor: pointer;
            font-size: 16px;
            margin-top: 10px;
            width: 100%;
        }

        .buy-btn:hover {
            background-color: #ff3385;
        }

        footer {
            background-color: #ff99cc;
            color: white;
            padding: 10px;
            margin-top: 20px;
        }
    </style>
</head>
<body>

    <header>
        <h1>Welcome to My Digital Art Store</h1>
        <nav>
            <ul>
                <li><a onclick="showSection('home')">Home</a></li>
                <li><a onclick="showSection('shop')">Shop</a></li>
                <li><a onclick="showSection('about')">About</a></li>
                <li><a onclick="showSection('contact')">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- עמוד ראשי -->
    <section id="home" class="banner">
        <h2>Discover Unique Digital Art</h2>
        <p>High-quality artwork for startups and businesses</p>
    </section>

    <!-- חנות -->
    <section id="shop" class="shop">
        <h2>Shop - Available Artworks</h2>
        <div class="art-container">
            <div class="art-item">
                <img src="art1.jpg" alt="Art 1">
                <p>Abstract Digital Piece</p>
                <button class="buy-btn">Buy with Bit</button>
            </div>
            <div class="art-item">
                <img src="art2.jpg" alt="Art 2">
                <p>Modern Aesthetic</p>
                <button class="buy-btn">Buy with Bit</button>
            </div>
        </div>
    </section>

    <!-- אודות -->
    <section id="about" class="about">
        <h2>About Me</h2>
        <p>Hello! I'm a digital artist creating unique pieces for startups and businesses. My goal is to bring visual identity to brands through art.</p>
    </section>

    <!-- צור קשר -->
    <section id="contact" class="contact">
        <h2>Contact</h2>
        <p>Have a question or custom request? Reach out to me at:</p>
        <p>Email: myemail@example.com</p>
    </section>

    <footer>
        <p>© 2025 My Digital Art Store | All rights reserved.</p>
    </footer>

    <script>
        function showSection(section) {
            document.getElementById("home").style.display = "none";
            document.getElementById("shop").style.display = "none";
            document.getElementById("about").style.display = "none";
            document.getElementById("contact").style.display = "none";
            document.getElementById(section).style.display = "block";
        }

        // מציג את עמוד הבית כברירת מחדל
        showSection('home');
    </script>

</body>
</html>
