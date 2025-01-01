<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chindhukuria Digital Coaching</title>
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background: linear-gradient(to right, #e3f2fd, #ffffff);
        }
        header {
            background-color: #4caf50;
            color: white;
            padding: 30px;
            text-align: center;
            font-size: 36px;
            font-weight: bold;
            text-transform: uppercase;
            letter-spacing: 2px;
            background: linear-gradient(45deg, #ff5722, #2196f3); /* রঙিন গ্রেডিয়েন্ট */
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3); /* হালকা ছায়া */
        }
        .menu-icon {
            position: absolute;
            top: 50px; /* বাটনটিকে নিচে সরানো হলো */
            right: 20px; /* ডান পাশে */
            cursor: pointer;
            display: flex;
            flex-direction: column;
            gap: 5px;
        }
        .menu-icon div {
            width: 30px;
            height: 5px;
            background: linear-gradient(90deg, red, blue); /* লাল ও নীল মিশ্রণ */
            border-radius: 3px;
        }
        nav {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.9);
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            transform: translateX(-100%);
            transition: transform 0.4s ease-in-out;
            z-index: 10;
        }
        nav.active {
            transform: translateX(0);
        }
        nav a {
            color: white;
            text-decoration: none;
            font-size: 20px;
            margin: 15px 0;
            padding: 10px 20px;
            border-radius: 5px;
            transition: background 0.3s;
        }
        nav a:hover {
            background-color: #575757;
        }
        .btn-enroll {
            background-color: red;
            font-weight: bold;
            padding: 10px 20px;
            border-radius: 5px;
        }
        .btn-enroll:hover {
            background-color: darkred;
        }
        section {
            padding: 20px;
            text-align: center;
        }
        footer {
            background-color: #4caf50;
            color: white;
            text-align: center;
            padding: 10px 0;
            position: relative;
            bottom: 0;
            width: 100%;
        }
        .enroll-btn-container {
            text-align: center;
            margin: 20px 0;
        }
    </style>
</head>
<body>
    <header>
        <span>Chindhukuria Digital Coaching</span>
        <div class="menu-icon" onclick="toggleMenu()">
            <div></div>
            <div></div>
            <div></div>
        </div>
    </header>
    <nav id="menu">
        <a href="#about-us" onclick="closeMenu()">আমাদের সম্পর্কে</a>
        <a href="https://shakil228547.github.io/Shakil/" target="_blank" onclick="closeMenu()">নোটিস</a> <!-- Updated link here -->
        <a href="#exam" onclick="closeMenu()">পরীক্ষা</a>
        <a href="#contact" onclick="closeMenu()">যোগাযোগ</a>
        <a href="https://forms.gle/nV6H4RXy8b2xZJGcA" target="_blank" class="btn-enroll" onclick="closeMenu()">ভর্তি হও</a>
    </nav>
    <section id="about-us">
        <h2>আমাদের সম্পর্কে</h2>
        <p>আমরা বিজ্ঞান, গণিত, এবং অন্যান্য বিষয়ের সেরা মানের শিক্ষা দিই। স্মার্ট নোট এবং সাপ্তাহিক পরীক্ষার মাধ্যমে শিক্ষার্থীদের সাফল্য নিশ্চিত করি।</p>
    </section>
    
    <!-- ভর্তি হও বাটন সেকশন -->
    <div class="enroll-btn-container">
        <a href="https://forms.gle/nV6H4RXy8b2xZJGcA" target="_blank" class="btn-enroll">ভর্তি হও</a>
    </div>
    
    <section id="notice">
        <h2>নোটিস</h2>
        <p>১ জানুয়ারি থেকে ক্লাস শুরু হবে।</p>
        <p><a href="https://shakil228547.github.io/Shakil/" target="_blank" style="color: #4caf50; text-decoration: underline;">Visit Shakil's Website</a></p>
    </section>
    
    <!-- পরীক্ষা অপশন এবং লিংক -->
    <section id="exam">
        <h2>পরীক্ষা</h2>
        <p><a href="https://docs.google.com/forms/d/e/1FAIpQLSfP01xGd0UJWS1nBORMJLuDosoSodGRHCXvzpPuxK4BrDa0Rw/viewform" target="_blank" style="color: #4caf50; text-decoration: underline;">পরীক্ষার পেজে যান</a></p>
    </section>
    
    <section id="contact">
        <h2>যোগাযোগ</h2>
        <p>ফোন: 01785228547</p>
        <p>ইমেইল: shakilahmedvir@gmail.com</p>
    </section>
    <footer>
        &copy; 2025 Chindhukuria Digital Coaching. All Rights Reserved.
    </footer>

    <script>
        function toggleMenu() {
            const menu = document.getElementById("menu");
            menu.classList.toggle("active");
        }

        function closeMenu() {
            const menu = document.getElementById("menu");
            menu..remove("active");
        }
    </script>
</body>
</html
