<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="https://fonts.googleapis.com/css2?family=Trirong" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.2.0/css/all.min.css">
    <title>Our Menu</title>
    <style>
        body {
            font-family: 'Trirong', serif;
            background-color: #f9f9f9;
            margin: 0;
            padding: 0;
        }
        /* Header */
        header {
            background: #000;
        }
        .header img {
            padding-left: 30px;
            height: 30px;
            position: absolute;
            top: 8px;
        }

        .nav-bar {
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 10px 0;
            gap: 20px;
        }

        .nav-bar a {
            color: #fff;
            text-decoration: none;
            font-size: 18px;
            font-weight: 500;
            transition: 0.5s;
        }

        .nav-bar a:hover {
            text-decoration: underline white 2px;
            margin-right: 10px;
        }

        h1 {
            text-align: center;
            color: #333;
        }
        /* Menu */
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        .menu-item {
            display: flex;
            align-items: center;
            margin-bottom: 20px;
        }
        .menu-item img {
            max-width: 100px;
            margin-right: 20px;
            border-radius: 5px;
        }
        .menu-item p {
            font-size: 16px;
            color: #555;
        }
        /* Footer */
        .footer {
            background-color: #222;
            color: #fff;
        }

        .footer-content {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            max-width: 1100px;
            margin: 0 auto;
        }

        .footer-section {
            flex: 1;
            padding: 0 20px;
        }

        .footer-section h2 {
            font-size: 1.5rem;
            margin-bottom: 20px;
        }

        .footer-section p {
            margin-bottom: 20px;
        }

        .footer-section li a {
            color: #b30000;
            text-decoration: none;
        }

        .footer-section li a:hover {
            color: #4245ec;
        }

        .contact span {
            display: block;
            margin-bottom: 10px;
        }

        .contact span a {
            color: #b30000;
            text-decoration: none;
        }

        .contact span a:hover {
            color: #4245ec;
        }

        .socials a {
            color: #fff;
            margin-right: 10px;
        }

        .socials a:hover {
            color: #b30000;
        }

        .footer-bottom {
            background-color: #111;
            padding: 20px 0;
            text-align: center;
            width: 100%;
        }

        .text-input {
            width: 100%;
            padding: 10px;
            margin-bottom: 20px;
            border: 1px solid #fff;
            border-radius: 5px;
            background-color: transparent;
            color: #fff;
            outline: none;
        }

        .btn-primary {
            padding: 10px 20px;
            background-color: #b30000;
            color: #fff;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }

        .btn-primary:hover {
            background-color: #990000;
        }

        .error {
            color: #ff3333;
            margin-bottom: 10px;
            display: none;
        }
    </style>
</head>
<body>
    <header class="header">
        <a href="index.html" class="logo"> <img src="logo.svg" alt="logo" class="img"></a>
        <nav class="nav-bar">
            <a href="index.html#">Menu</a>
        </nav>
    </header>
    <div class="container">
        <h1>Our Menu</h1>
        <div class="menu-item">
            <img src="images/cald.jpg" alt="Dish 1">
            <p>Caldereta</p>
        </div>
        <div class="menu-item">
            <img src="images/jelly.jpg" alt="Dish 2">
            <p>Coffee Jelly</p>
        </div>
        <div class="menu-item">
            <img src="images/vege.jpg" alt="Dish 3">
            <p>Chapseuy</p>
        </div>
        <div class="menu-item">
            <img src="images/MEN.jpg" alt="Dish 4">
            <p>Menudo</p>
        </div>
        <div class="menu-item">
            <img src="images/Leche.jpg" alt="Dish 5">
            <p>Leche Flan</p>
        </div>
        <div class="menu-item">
            <img src="images/lumpia.jpg" alt="Dish 6">
            <p>Pork lumpia</p>
        </div>
    </div>
    <footer class="footer" id="contact">
        <div class="footer-content">
            <div class="footer-section about">
                <h2>About Us</h2>
                <p>LAMSID Catering Company delivers exceptional culinary experiences, from bespoke menus to 
                    attentive event services.</p>
                <div class="contact">
                    <span><i class="fas fa-phone"></i> + (886) 987-654-321</span>
                    <span><i class="fas fa-envelope"></i> <a href="mailto:abc@1234.com"> info@lamsid.com</a></span>
                </div>
                <div class="socials">
                    <a href="#"><i class="fab fa-facebook"></i></a>
                    <a href="#"><i class="fab fa-twitter"></i></a>
                    <a href="#"><i class="fab fa-instagram"></i></a>
                    <a href="#"><i class="fab fa-whatsapp"></i></a>
                </div>
            </div>
            <div class="footer-section links">
                <h2>Quick Links</h2>
                <ul>
                    <li><a href="index.html#">Home</a></li>
                    <li><a href="index.html#about">About</a></li>
                    <li><a href="menu.html">Menu</a></li>
                    <li><a href="index.html#services">Services</a></li>
                    <li><a href="contact_us.html">Contact</a></li>
                </ul>
            </div>
            <div class="footer-section contact-form">
                <h2>Contact Us</h2>
                <form id="contactForm">
                    <input type="email" name="email" id="email" class="text-input contact-input" placeholder="Your email address">
                    <div id="emailError" class="error"></div>
                    <textarea rows="4" name="message" class="text-input contact-input" placeholder="Your message"></textarea>
                    <button type="submit" class="btn-primary">
                        <i class="fas fa-envelope"></i>
                        Send
                    </button>
                </form>
            </div>
        </div>
        <div class="footer-bottom">
            &copy; 2024 LASMID. All rights reserved.
        </div>
    </footer>
    <!-- End Footer -->
    
    <script>
        const emailInput = document.getElementById('email');
        const emailError = document.getElementById('emailError');
    
        function validateEmail(email) {
            // Email validation regex pattern
            const pattern = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
            return pattern.test(email);
        }
    
        function handleFormSubmit(event) {
            event.preventDefault(); // Prevent default form submission
            const email = emailInput.value;
            if (!validateEmail(email)) {
                emailError.textContent = 'Please enter a valid email address.';
                emailError.style.display = 'block';
            } else {
                emailError.textContent = '';
                emailError.style.display = 'none';
                // Proceed with form submission
                console.log('Email submitted:', email);
            }
        }
    
        const contactForm = document.getElementById('contactForm');
        contactForm.addEventListener('submit', handleFormSubmit);
    </script>
</body>
</html>
