<h1>Code For Homepage </h1>
____________________________________________________________________________________________________

<!doctype html>
<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <meta http-equiv="X-UA-Compatible" content="ie=edge" />
        <title>ABC Fitness Studio</title>
        <style>
            * {
                margin: 0;
                padding: 0;
                box-sizing: border-box;
            }

            body {
                font-family:
                    Arial Bold,
                    Calibri Normal;
                background-color: #d3d3d3;
            }

            header {
                background-color: #001f3f;
                color: #001f3f;
                padding: 10px 0;
                display: flex;
                justify-content: space-between;
                align-items: center;
            }

            .logo {
                margin-left: 20px;
            }

            nav {
                margin-right: 20px;
            }

            nav ul {
                list-style: none;
                display: flex;
            }

            nav ul li {
                margin-left: 20px;
            }

            nav ul li a {
                color: #fff;
                text-decoration: none;
                font-weight: bold;
            }

            .main-content {
                padding: 20px;
                text-align: center;
            }

            .main-content h1 {
                margin-bottom: 30px;
            }

            .items {
                display: flex;
                justify-content: space-around;
                margin: 30px 0;
            }

            .items img {
                width: 150px;
                height: 150px;
                border: 2px solid #ddd;
                padding: 10px;
                background-color: #fff;
            }

            .shopping-perks {
                background-color: #fff;
                padding: 20px;
                border-radius: 8px;
                margin-top: 20px;
            }

            footer {
                background-color: #001f3f;
                color: #fff;
                padding: 20px;
                text-align: center;
            }

            .social-media,
            .newsletter {
                margin: 10px 0;
            }

            .social-media a,
            .newsletter button {
                background-color: #d3d3d3;
                color: #fff;
                padding: 10px 15px;
                margin: 5px;
                border: none;
                border-radius: 5px;
                text-decoration: none;
            }

            .footer-links {
                margin-top: 20px;
                text-align: center;
            }

            .footer-links a {
                color: #fff;
                text-decoration: none;
                margin: 0 10px;
            }
        </style>
    </head>
    <body>
        <header>
            <div class="logo">
                <img
                    src="Client2_LogoPalette2_D3D3D3.png"
                    alt="ABC Fitness Studio Logo"
                    width="50"
                    height="50"
                />
            </div>
            <nav>
                <ul>
                    <li><a href="index.html">Home</a></li>
                    <li><a href="index (copy) 1.html">About Us</a></li>
                    <li><a href="index (copy).html">Gallary</a></li>
                    <li><a href="index (copy)2.html">Testimonials</a></li>
                </ul>
            </nav>
        </header>

        <div class="main-content">
            <h1>Welcome to ABC Fitness Studio</h1>
            <div class="items">
                <div><img src="Boxing.png" alt="Item 1" /></div>
                <div><img src="Kickboxing.png" alt="Item 2" /></div>
                <div><img src="Yoga.png" alt="Item 3" /></div>
            </div>

            <div class="shopping-perks">
                <h2>Why Shop With Us?</h2>
                <ul>
                    <li>Free shipping on orders over $50</li>
                    <li>30-day money-back guarantee</li>
                    <li>Exclusive fitness products</li>
                </ul>
            </div>
        </div>

        <footer>
            <div class="social-media">
                <a href="#facebook">Facebook</a>
                <a href="#instagram">Instagram</a>
                <a href="#twitter">Twitter</a>
            </div>

            <div class="newsletter">
                <form id="subscribeForm" onsubmit="return thankYouAlert()">
                    <input type="email" id="email" name="email" placeholder="Enter your email" required>
                    <button type="submit">Subscribe</button>
                </form>
            </div>

            <div class="footer-links">
                <a href="index.html">Home</a>
                <a href="index(copy) 1.html">About Us</a>
                <a href="index(copy).html">Gallary</a>
                <a href="index (copy)2.html">Testimonials</a>
            </div>
        </footer>

        <script>
            function thankYouAlert() {
                const email = document.getElementById('email').value;
                if (email) {
                    alert("Thank you for subscribing with the email: " + email);
                } else {
                    alert("Please enter a valid email.");
                }
                return false;  // Prevents form from actually submitting to a server
            }
        </script>
    </body>
</html>
_______________________________________________________________________________________________
<h1>Code for gallery/store</h1>
______________________________________________________________________________________________

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Gallery - ABC Fitness Studio</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial Bold, Calibri Normal;
            background-color: #d3d3d3;
        }

        header {
            background-color: #001f3f;
            color: #fff;
            padding: 10px 0;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            margin-left: 20px;
        }

        nav {
            margin-right: 20px;
        }

        nav ul {
            list-style: none;
            display: flex;
        }

        nav ul li {
            margin-left: 20px;
        }

        nav ul li a {
            color: #fff;
            text-decoration: none;
            font-weight: bold;
        }

        .main-content {
            padding: 20px;
            text-align: center;
        }

        .main-content h1 {
            margin-bottom: 30px;
        }

        .gallery {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
            margin-top: 30px;
        }

        .gallery-item {
            background-color: #fff;
            padding: 20px;
            border: 2px solid #ddd;
            border-radius: 8px;
        }

        .gallery-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }

        .gallery-item h3 {
            margin-top: 15px;
            font-size: 18px;
        }

        .gallery-item p {
            margin: 10px 0;
            font-size: 16px;
        }

        .gallery-item button {
            background-color: #007BFF;
            color: #fff;
            padding: 10px;
            border: none;
            cursor: pointer;
            border-radius: 5px;
        }

        .gallery-item button:hover {
            background-color: #0056b3;
        }

        footer {
            background-color: #001f3f;
            color: #fff;
            padding: 20px;
            text-align: center;
        }

        .social-media, .newsletter {
            margin: 10px 0;
        }

        .social-media a, .newsletter button {
            background-color: #d3d3d3;
            color: #fff;
            padding: 10px 15px;
            margin: 5px;
            border: none;
            border-radius: 5px;
            text-decoration: none;
        }

        .footer-links {
            margin-top: 20px;
            text-align: center;
        }

        .footer-links a {
            color: #fff;
            text-decoration: none;
            margin: 0 10px;
        }

        /* Modal Styling */
        .modal {
            display: none;
            position: fixed;
            z-index: 1;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0,0,0,0.4);
        }

        .modal-content {
            background-color: #fff;
            margin: 15% auto;
            padding: 20px;
            border: 1px solid #888;
            width: 80%;
            max-width: 400px;
            text-align: center;
            border-radius: 10px;
        }

        .close {
            color: #aaa;
            float: right;
            font-size: 28px;
            font-weight: bold;
            cursor: pointer;
        }

        .close:hover,
        .close:focus {
            color: black;
            text-decoration: none;
            cursor: pointer;
        }

        /* Cart summary styling */
        #cartSummary {
            position: fixed;
            bottom: 20px;
            right: 20px;
            background-color: #fff;
            padding: 15px;
            border: 1px solid #888;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        #cartSummary button {
            margin-top: 10px;
            padding: 10px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }

        .clear-cart {
            background-color: #f44336;
            color: #fff;
        }

        .process-order {
            background-color: #4CAF50;
            color: #fff;
        }
    </style>
</head>
<body>
    <header>
        <div class="logo">
            <img src="Client2_LogoPalette2_D3D3D3.png" alt="ABC Fitness Studio Logo" width="50" height="50">
        </div>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="index (copy) 1.html">About Us</a></li>
                <li><a href="index (copy).html">Gallery</a></li> 
                <li><a href="index (copy)2.html">Testimonials</a></li>
            </ul>
        </nav>
    </header>

    <div class="main-content">
        <h1>Gallery - ABC Fitness Studio</h1>

        <div class="gallery">
            <div class="gallery-item">
                <img src="Bottle.png" alt="Fitness Product 1">
                <h3>Product 1</h3>
                <p>$29.99</p>
                <button onclick="addToCart('Product 1', 29.99)">Buy Now</button>
            </div>

            <div class="gallery-item">
                <img src="Shirt.png" alt="Fitness Product 2">
                <h3>Product 2</h3>
                <p>$39.99</p>
                <button onclick="addToCart('Product 2', 39.99)">Buy Now</button>
            </div>

            <div class="gallery-item">
                <img src="Yoga mat.png" alt="Fitness Product 3">
                <h3>Product 3</h3>
                <p>$49.99</p>
                <button onclick="addToCart('Product 3', 49.99)">Buy Now</button>
            </div>
        </div>
    </div>

    <!-- Add to Cart Modal -->
    <div id="cartModal" class="modal">
        <div class="modal-content">
            <span class="close" onclick="closeCartModal()">&times;</span>
            <p id="cartModalMessage">Item added to cart!</p>
        </div>
    </div>

    <!-- Cart Summary Box -->
    <div id="cartSummary">
        <h4>Your Cart</h4>
        <div id="cartItems"></div>
        <p id="cartTotal"></p>
        <button class="clear-cart" onclick="clearCart()">Clear Cart</button>
        <button class="process-order" onclick="processOrder()">Process Order</button>
    </div>

    <footer>
        <div class="social-media">
            <a href="#facebook">Facebook</a>
            <a href="#instagram">Instagram</a>
            <a href="#twitter">Twitter</a>
        </div>

        <div class="newsletter">
            <form id="subscribeForm" onsubmit="return thankYouAlert()">
                <input type="email" id="email" name="email" placeholder="Enter your email" required>
                <button type="submit">Subscribe</button>
            </form>
        </div>

        <div class="footer-links">
            <a href="index.html">Home</a>
            <a href="index (copy) 1.html">About Us</a>
            <a href="index (copy).html">Gallery</a>
            <a href="index (copy)2.html">Testimonials</a>
        </div>
    </footer>

    <script>
        // Cart array to store added items
        let cart = [];

        function addToCart(productName, price) {
            cart.push({ name: productName, price: price });
            openCartModal(productName, price);
            updateCartItems();
        }

        function openCartModal(productName, price) {
            document.getElementById("cartModalMessage").textContent = `"${productName}" added to your cart! (Price: $${price})`;
            document.getElementById("cartModal").style.display = "block";
        }

        function closeCartModal() {
            document.getElementById("cartModal").style.display = "none";
        }

        function updateCartItems() {
            let cartContent = document.getElementById("cartItems"); 
            cartContent.innerHTML = ''; // Clear existing content

            if (cart.length === 0) {
                cartContent.innerHTML = 'Your cart is empty!';
                document.getElementById("cartTotal").innerHTML = 'Total: $0.00';  // Reset total price
            } else {
                let cartTotal = 0;
                cartContent.innerHTML = '<ul>';
                cart.forEach((item, index) => {
                    cartContent.innerHTML += `
                        <li>${item.name} - $${item.price.toFixed(2)}
                            <button onclick="removeFromCart(${index})" class="remove-btn">Remove</button>
                        </li>`;
                    cartTotal += item.price;
                });
                cartContent.innerHTML += '</ul>';
                document.getElementById("cartTotal").innerHTML = `Total: $${cartTotal.toFixed(2)}`;
            }
        }

        function removeFromCart(index) {
            cart.splice(index, 1); // Remove the item from the cart
            updateCartItems(); // Update the cart display
        }

        function clearCart() {
            cart = []; // Clear all items from the cart
            updateCartItems(); // Update the cart display
            document.getElementById("cartTotal").innerHTML = 'Total: $0.00'; // Reset the total price to zero
        }

        function processOrder() {
            if (cart.length === 0) {
                alert("Your cart is empty. Please add items before processing the order.");
            } else {
                alert("Your order has been processed. Thank you for shopping!");
                clearCart(); // Clear cart after processing the order
            }
        }

        // Initialize cart display
        updateCartItems();

        // Close modal if clicked outside of modal content
        window.onclick = function(event) {
            if (event.target == document.getElementById("cartModal")) {
                closeCartModal();
            }
        }

        function thankYouAlert() {
            const email = document.getElementById('email').value;
            if (email) {
                alert("Thank you for subscribing with the email: " + email);
            } else {
                alert("Please enter a valid email.");
            }
            return false;  // Prevent form from actually submitting to a server
        }
    </script>
</body>
</html>
_______________________________________________________________________________________________

<h1>Code for Gallery/ Shop Page</h1>
_______________________________________________________________________________________________

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Gallery - ABC Fitness Studio</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial Bold, Calibri Normal;
            background-color: #d3d3d3;
        }

        header {
            background-color: #001f3f;
            color: #fff;
            padding: 10px 0;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            margin-left: 20px;
        }

        nav {
            margin-right: 20px;
        }

        nav ul {
            list-style: none;
            display: flex;
        }

        nav ul li {
            margin-left: 20px;
        }

        nav ul li a {
            color: #fff;
            text-decoration: none;
            font-weight: bold;
        }

        .main-content {
            padding: 20px;
            text-align: center;
        }

        .main-content h1 {
            margin-bottom: 30px;
        }

        .gallery {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
            margin-top: 30px;
        }

        .gallery-item {
            background-color: #fff;
            padding: 20px;
            border: 2px solid #ddd;
            border-radius: 8px;
        }

        .gallery-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }

        .gallery-item h3 {
            margin-top: 15px;
            font-size: 18px;
        }

        .gallery-item p {
            margin: 10px 0;
            font-size: 16px;
        }

        .gallery-item button {
            background-color: #007BFF;
            color: #fff;
            padding: 10px;
            border: none;
            cursor: pointer;
            border-radius: 5px;
        }

        .gallery-item button:hover {
            background-color: #0056b3;
        }

        footer {
            background-color: #001f3f;
            color: #fff;
            padding: 20px;
            text-align: center;
        }

        .social-media, .newsletter {
            margin: 10px 0;
        }

        .social-media a, .newsletter button {
            background-color: #d3d3d3;
            color: #fff;
            padding: 10px 15px;
            margin: 5px;
            border: none;
            border-radius: 5px;
            text-decoration: none;
        }

        .footer-links {
            margin-top: 20px;
            text-align: center;
        }

        .footer-links a {
            color: #fff;
            text-decoration: none;
            margin: 0 10px;
        }

        /* Modal Styling */
        .modal {
            display: none;
            position: fixed;
            z-index: 1;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0,0,0,0.4);
        }

        .modal-content {
            background-color: #fff;
            margin: 15% auto;
            padding: 20px;
            border: 1px solid #888;
            width: 80%;
            max-width: 400px;
            text-align: center;
            border-radius: 10px;
        }

        .close {
            color: #aaa;
            float: right;
            font-size: 28px;
            font-weight: bold;
            cursor: pointer;
        }

        .close:hover,
        .close:focus {
            color: black;
            text-decoration: none;
            cursor: pointer;
        }

        /* Cart summary styling */
        #cartSummary {
            position: fixed;
            bottom: 20px;
            right: 20px;
            background-color: #fff;
            padding: 15px;
            border: 1px solid #888;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        #cartSummary button {
            margin-top: 10px;
            padding: 10px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }

        .clear-cart {
            background-color: #f44336;
            color: #fff;
        }

        .process-order {
            background-color: #4CAF50;
            color: #fff;
        }
    </style>
</head>
<body>
    <header>
        <div class="logo">
            <img src="Client2_LogoPalette2_D3D3D3.png" alt="ABC Fitness Studio Logo" width="50" height="50">
        </div>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="index (copy) 1.html">About Us</a></li>
                <li><a href="index (copy).html">Gallery</a></li> 
                <li><a href="index (copy)2.html">Testimonials</a></li>
            </ul>
        </nav>
    </header>

    <div class="main-content">
        <h1>Gallery - ABC Fitness Studio</h1>

        <div class="gallery">
            <div class="gallery-item">
                <img src="Bottle.png" alt="Fitness Product 1">
                <h3>Product 1</h3>
                <p>$29.99</p>
                <button onclick="addToCart('Product 1', 29.99)">Buy Now</button>
            </div>

            <div class="gallery-item">
                <img src="Shirt.png" alt="Fitness Product 2">
                <h3>Product 2</h3>
                <p>$39.99</p>
                <button onclick="addToCart('Product 2', 39.99)">Buy Now</button>
            </div>

            <div class="gallery-item">
                <img src="Yoga mat.png" alt="Fitness Product 3">
                <h3>Product 3</h3>
                <p>$49.99</p>
                <button onclick="addToCart('Product 3', 49.99)">Buy Now</button>
            </div>
        </div>
    </div>

    <!-- Add to Cart Modal -->
    <div id="cartModal" class="modal">
        <div class="modal-content">
            <span class="close" onclick="closeCartModal()">&times;</span>
            <p id="cartModalMessage">Item added to cart!</p>
        </div>
    </div>

    <!-- Cart Summary Box -->
    <div id="cartSummary">
        <h4>Your Cart</h4>
        <div id="cartItems"></div>
        <p id="cartTotal"></p>
        <button class="clear-cart" onclick="clearCart()">Clear Cart</button>
        <button class="process-order" onclick="processOrder()">Process Order</button>
    </div>

    <footer>
        <div class="social-media">
            <a href="#facebook">Facebook</a>
            <a href="#instagram">Instagram</a>
            <a href="#twitter">Twitter</a>
        </div>

        <div class="newsletter">
            <form id="subscribeForm" onsubmit="return thankYouAlert()">
                <input type="email" id="email" name="email" placeholder="Enter your email" required>
                <button type="submit">Subscribe</button>
            </form>
        </div>

        <div class="footer-links">
            <a href="index.html">Home</a>
            <a href="index (copy) 1.html">About Us</a>
            <a href="index (copy).html">Gallery</a>
            <a href="index (copy)2.html">Testimonials</a>
        </div>
    </footer>

    <script>
        // Cart array to store added items
        let cart = [];

        function addToCart(productName, price) {
            cart.push({ name: productName, price: price });
            openCartModal(productName, price);
            updateCartItems();
        }

        function openCartModal(productName, price) {
            document.getElementById("cartModalMessage").textContent = `"${productName}" added to your cart! (Price: $${price})`;
            document.getElementById("cartModal").style.display = "block";
        }

        function closeCartModal() {
            document.getElementById("cartModal").style.display = "none";
        }

        function updateCartItems() {
            let cartContent = document.getElementById("cartItems"); 
            cartContent.innerHTML = ''; // Clear existing content

            if (cart.length === 0) {
                cartContent.innerHTML = 'Your cart is empty!';
                document.getElementById("cartTotal").innerHTML = 'Total: $0.00';  // Reset total price
            } else {
                let cartTotal = 0;
                cartContent.innerHTML = '<ul>';
                cart.forEach((item, index) => {
                    cartContent.innerHTML += `
                        <li>${item.name} - $${item.price.toFixed(2)}
                            <button onclick="removeFromCart(${index})" class="remove-btn">Remove</button>
                        </li>`;
                    cartTotal += item.price;
                });
                cartContent.innerHTML += '</ul>';
                document.getElementById("cartTotal").innerHTML = `Total: $${cartTotal.toFixed(2)}`;
            }
        }

        function removeFromCart(index) {
            cart.splice(index, 1); // Remove the item from the cart
            updateCartItems(); // Update the cart display
        }

        function clearCart() {
            cart = []; // Clear all items from the cart
            updateCartItems(); // Update the cart display
            document.getElementById("cartTotal").innerHTML = 'Total: $0.00'; // Reset the total price to zero
        }

        function processOrder() {
            if (cart.length === 0) {
                alert("Your cart is empty. Please add items before processing the order.");
            } else {
                alert("Your order has been processed. Thank you for shopping!");
                clearCart(); // Clear cart after processing the order
            }
        }

        // Initialize cart display
        updateCartItems();

        // Close modal if clicked outside of modal content
        window.onclick = function(event) {
            if (event.target == document.getElementById("cartModal")) {
                closeCartModal();
            }
        }

        function thankYouAlert() {
            const email = document.getElementById('email').value;
            if (email) {
                alert("Thank you for subscribing with the email: " + email);
            } else {
                alert("Please enter a valid email.");
            }
            return false;  // Prevent form from actually submitting to a server
        }
    </script>
</body>
</html>
_______________________________________________________________________________________________
<h1>Code For About Us/ Contact Fourm Page</h1>
_______________________________________________________________________________________________

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>About Us - ABC Fitness Studio</title>
    <style>
        /* Styling remains unchanged */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial Bold, Calibri Normal;
            background-color: #d3d3d3;
        }

        header {
            background-color: #001f3f;
            color: #fff;
            padding: 10px 0;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            margin-left: 20px;
        }

        nav {
            margin-right: 20px;
        }

        nav ul {
            list-style: none;
            display: flex;
        }

        nav ul li {
            margin-left: 20px;
        }

        nav ul li a {
            color: #fff;
            text-decoration: none;
            font-weight: bold;
        }

        .main-content {
            padding: 20px;
        }

        .main-content h1 {
            text-align: center;
            margin-bottom: 30px;
        }

        .business-hours {
            text-align: center;
            margin-bottom: 40px;
        }

        .contact-form {
            max-width: 600px;
            margin: 0 auto;
            background-color: #fff;
            padding: 20px;
            border-radius: 8px;
            border: 2px solid #ddd;
        }

        .contact-form label {
            display: block;
            margin-bottom: 10px;
            font-size: 16px;
        }

        .contact-form input, .contact-form textarea {
            width: 100%;
            padding: 10px;
            margin-bottom: 20px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }

        .contact-form input[type="checkbox"] {
            width: auto;
        }

        .form-buttons {
            display: flex;
            justify-content: space-between;
        }

        .form-buttons button {
            padding: 10px 20px;
            border: none;
            background-color: #d3d3d3;
            color: #fff;
            cursor: pointer;
            border-radius: 5px;
        }

        footer {
            background-color: #001f3f;
            color: #fff;
            padding: 20px;
            text-align: center;
        }

        .social-media, .newsletter {
            margin: 10px 0;
        }

        .social-media a, .newsletter button {
            background-color: #d3d3d3;
            color: #fff;
            padding: 10px 15px;
            margin: 5px;
            border: none;
            border-radius: 5px;
            text-decoration: none;
        }

        .footer-links {
            margin-top: 20px;
        }

        .footer-links a {
            color: #fff;
            text-decoration: none;
            margin: 0 10px;
        }
    </style>
</head>
<body>
    <header>
        <div class="logo">
            <img src="Client2_LogoPalette2_D3D3D3.png" alt="ABC Fitness Studio Logo" width="50" height="50">
        </div>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="index (copy) 1.html">About</a></li>
                <li><a href="index (copy).html">Gallery</a></li>
                <li><a href="index (copy)2.html">Testimonial</a></li>
            </ul>
        </nav>
    </header>

    <div class="main-content">
        <h1>About Us - ABC Fitness Studio</h1>

        <!-- Business Hours Section -->
        <div class="business-hours">
            <h2>Business Hours</h2>
            <p>Monday - Friday: 9 AM - 8 PM</p>
            <p>Saturday: 10 AM - 6 PM</p>
            <p>Sunday: Closed</p>
        </div>

        <!-- Contact Form Section -->
        <div class="contact-form">
            <h2>Contact Us</h2>

            <form id="contactForm" onsubmit="return handleFormSubmit()">
                <label for="name">Full Name:</label>
                <input type="text" id="name" name="name" placeholder="Enter your full name" required>

                <label for="email">Email Address:</label>
                <input type="email" id="email" name="email" placeholder="Enter your email address" required>

                <label for="phone">Phone Number:</label>
                <input type="tel" id="phone" name="phone" placeholder="Enter your phone number" required>

                <label for="feedback">Feedback/Order Information:</label>
                <textarea id="feedback" name="feedback" rows="4" placeholder="Write your message" required></textarea>

                <label for="custom-order">
                    <input type="checkbox" id="custom-order" name="custom-order">
                    Custom Order
                </label>

                <!-- Form Buttons -->
                <div class="form-buttons">
                    <button type="submit">Submit</button>
                    <button type="button" onclick="clearForm()">Clear</button>
                </div>
            </form>
        </div>
    </div>

    <!-- Footer Section -->
    <footer>
        <div class="social-media">
            <a href="#facebook">Facebook</a>
            <a href="#instagram">Instagram</a>
            <a href="#twitter">Twitter</a>
        </div>

        <div class="newsletter">
            <form id="subscribeForm" onsubmit="return thankYouAlert()">
                <input type="email" id="newsletter-email" name="email" placeholder="Enter your email" required>
                <button type="submit">Subscribe</button>
            </form>
        </div>

        <div class="footer-links">
            <a href="index.html">Home</a>
            <a href="index (copy) 1.html">About Us</a>
            <a href="index (copy).html">Gallery</a>
            <a href="index (copy)2.html">Testimonials</a>
        </div>
    </footer>

    <script>
        // Handles form submission and displays a thank you message
        function handleFormSubmit() {
            alert("Thank you for submitting your details!");
            return false;  // Prevent actual form submission
        }

        // Clears all form fields in the Contact Us form
        function clearForm() {
            document.getElementById('contactForm').reset();  // Resets all form fields
        }

        // For the newsletter subscription form
        function thankYouAlert() {
            const email = document.getElementById('newsletter-email').value;
            if (email) {
                alert("Thank you for subscribing with the email: " + email);
            } else {
                alert("Please enter a valid email.");
            }
            return false;  // Prevent form from actually submitting to a server
        }
    </script>
</body>
</html>
______________________________________________________________________________________________
<h1>Code For Testimonial Page</h1>
______________________________________________________________________________________________

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Testimonials - ABC Fitness Studio</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            background-color: #d3d3d3;
        }

        header {
            background-color: #001f3f;
            color: #fff;
            padding: 10px 0;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            margin-left: 20px;
        }

        nav {
            margin-right: 20px;
        }

        nav ul {
            list-style: none;
            display: flex;
        }

        nav ul li {
            margin-left: 20px;
        }

        nav ul li a {
            color: #fff;
            text-decoration: none;
            font-weight: bold;
        }

        .main-content {
            padding: 20px;
            text-align: center;
        }

        .main-content h1 {
            margin-bottom: 30px;
        }

        .testimonials {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 20px;
        }

        .testimonial-item {
            background-color: #fff;
            padding: 20px;
            border: 2px solid #ddd;
            border-radius: 8px;
        }

        .testimonial-item h3 {
            margin-bottom: 10px;
            font-size: 18px;
        }

        .testimonial-item p {
            font-size: 16px;
            line-height: 1.6;
        }

        footer {
            background-color: #001f3f;
            color: #fff;
            padding: 20px;
            text-align: center;
        }

        .social-media, .newsletter {
            margin: 10px 0;
        }

        .social-media a, .newsletter button {
            background-color: #d3d3d3;
            color: #fff;
            padding: 10px 15px;
            margin: 5px;
            border: none;
            border-radius: 5px;
            text-decoration: none;
        }

        .footer-links {
            margin-top: 20px;
        }

        .footer-links a {
            color: #fff;
            text-decoration: none;
            margin: 0 10px;
        }

        @media (max-width: 768px) {
            .testimonials {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="logo">
            <img src="Client2_LogoPalette2_D3D3D3.png" alt="ABC Fitness Studio Logo" width="50" height="50">
        </div>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="index (copy) 1.html">About Us</a></li>
                <li><a href="index (copy).html">Gallery</a></li>
                <li><a href="index (copy)2.html">Testimonials</a></li>
            </ul>
        </nav>
    </header>

    <div class="main-content">
        <h1>Testimonials - ABC Fitness Studio</h1>

        <!-- Testimonials Section -->
        <div class="testimonials">
            <!-- Testimonial 1 -->
            <div class="testimonial-item">
                <h3>John Doe</h3>
                <p>
                    "ABC Fitness Studio completely transformed my fitness journey! The trainers are highly skilled and the environment is welcoming. I’ve seen amazing results and can’t recommend it enough!"
                </p>
            </div>

            <!-- Testimonial 2 -->
            <div class="testimonial-item">
                <h3>Jane Smith</h3>
                <p>
                    "I’ve tried many gyms, but nothing compares to the personalized attention and support I’ve received at ABC Fitness Studio. Their programs are top-notch, and I’m in the best shape of my life!"
                </p>
            </div>

            <!-- Testimonial 3 -->
            <div class="testimonial-item">
                <h3>Michael Johnson</h3>
                <p>
                    "The atmosphere at ABC Fitness Studio is just incredible. It’s the perfect place for anyone looking to get serious about fitness. I’ve been a member for over a year and have never looked back!"
                </p>
            </div>

            <!-- Testimonial 4 -->
            <div class="testimonial-item">
                <h3>Sarah Williams</h3>
                <p>
                    "ABC Fitness Studio’s team really cares about your goals and progress. I’ve lost weight, gained strength, and most importantly, I’ve gained confidence. This gym is fantastic!"
                </p>
            </div>
        </div>
    </div>

    <!-- Footer Section -->

        <footer>
            <div class="social-media">
                <a href="#facebook">Facebook</a>
                <a href="#instagram">Instagram</a>
                <a href="#twitter">Twitter</a>
            </div>

            <div class="newsletter">
                <form id="subscribeForm" onsubmit="return thankYouAlert()">
                    <input type="email" id="email" name="email" placeholder="Enter your email" required>
                    <button type="submit">Subscribe</button>
                </form>
            </div>

            <div class="footer-links">
                <a href="index.html">Home</a>
                <a href="index (copy) 1.html">About Us</a>
                <a href="index (copy).html">Gallary</a>
                <a href="index (copy)2.html">Testimonials</a>
            </div>
        </footer>

        <script>
            function thankYouAlert() {
                const email = document.getElementById('email').value;
                if (email) {
                    alert("Thank you for subscribing with the email: " + email);
                } else {
                    alert("Please enter a valid email.");
                }
                return false;  // Prevents form from actually submitting to a server
            }
        </script>
    </body>
</html>
