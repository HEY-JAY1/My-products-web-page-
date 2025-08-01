 <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ADEHUN OLUWA HOME OF VARIETIES</title>
    <style>
        /* CSS for the entire page design */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(180deg, #FFFFFF, #FFC0CB);
            color: #333;
            line-height: 1.6;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
            flex-grow: 1;
            display: flex;
            flex-direction: column;
        }

        header {
            background-color: rgba(255, 255, 255, 0.8);
            text-align: center;
            padding: 20px 0;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
            margin-bottom: 20px;
            border-radius: 10px;
        }

        header h1 {
            color: #E91E63;
            font-size: 2.5em;
            margin: 0;
        }

        nav ul {
            list-style: none;
            padding: 0;
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-top: 10px;
        }

        nav a {
            text-decoration: none;
            color: #555;
            font-weight: bold;
            font-size: 1.1em;
            transition: color 0.3s ease;
        }

        nav a:hover {
            color: #E91E63;
        }
        
        main {
            background-color: rgba(255, 255, 255, 0.8);
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            flex-grow: 1;
            display: flex;
            flex-direction: column;
        }
        
        #home-content {
            text-align: center;
            padding: 50px 20px;
            flex-grow: 1;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
        }
        #home-content h2 {
            color: #E91E63;
            font-size: 2em;
        }
        
        #products-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }

        .product-card {
            background-color: #fff;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            text-align: center;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .product-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15);
        }

        .product-card img {
            width: 100%;
            height: auto;
            border-radius: 8px;
            margin-bottom: 15px;
        }

        .product-card h3 {
            color: #E91E63;
            margin-top: 0;
        }

        .product-card p {
            font-size: 0.9em;
            color: #777;
        }

        .product-card .price {
            font-weight: bold;
            color: #333;
            font-size: 1.2em;
            margin-top: 10px;
            display: block;
        }

        .btn {
            display: inline-block;
            background-color: #E91E63;
            color: white;
            padding: 10px 20px;
            text-decoration: none;
            border-radius: 5px;
            margin-top: 15px;
            font-weight: bold;
            transition: background-color 0.3s ease;
        }

        .btn:hover {
            background-color: #D81B60;
        }

        #contact-content, #about-content {
            text-align: center;
            padding: 50px 20px;
        }
        #contact-content a {
            color: #E91E63;
            text-decoration: none;
            font-weight: bold;
        }
        #contact-content p {
            font-size: 1.2em;
            margin-bottom: 10px;
        }

        footer {
            text-align: center;
            padding: 20px;
            background-color: rgba(255, 255, 255, 0.8);
            margin-top: 20px;
            border-radius: 10px;
            box-shadow: 0 -2px 5px rgba(0, 0, 0, 0.1);
        }

        /* --- NEW CSS for the pop-up message --- */
        #not-available-message {
            display: none; /* Hidden by default */
            position: fixed; /* Fixed position in the viewport */
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.5); /* Semi-transparent black overlay */
            justify-content: center;
            align-items: center;
            z-index: 1000; /* Ensures it's on top of everything */
        }
        
        #message-content {
            background-color: white;
            padding: 40px 60px;
            border-radius: 10px;
            text-align: center;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
            position: relative;
        }
        
        #message-content h2 {
            color: #E91E63;
            font-size: 2em;
            margin: 0;
        }
        
        .close-btn {
            position: absolute;
            top: 10px;
            right: 20px;
            font-size: 2em;
            font-weight: bold;
            color: #aaa;
            cursor: pointer;
        }
        
        .close-btn:hover {
            color: #000;
        }
    </style>
</head>
<body>

    <div class="container">
        
        <header>
            <h1>ADEHUN OLUWA HOME OF VARIETIES</h1>
            <p>Your one-stop shop for quality products</p>
            <nav>
                <ul>
                    <li><a href="javascript:void(0)" onclick="loadPage('home')">Home</a></li>
                    <li><a href="javascript:void(0)" onclick="loadPage('products')">Products</a></li>
                    <li><a href="javascript:void(0)" onclick="loadPage('about')">About Us</a></li>
                    <li><a href="javascript:void(0)" onclick="loadPage('contact')">Contact</a></li>
                </ul>
            </nav>
        </header>

        <main id="main-content">
            </main>

        <footer>
            <p>&copy; 2025 ADEHUN OLUWA HOME OF VARIETIES. All Rights Reserved.</p>
            <p>Designed by <a href="#" style="color: #E91E63;">AJ graphics and web dev</a></p>
        </footer>

    </div>
    
    <div id="not-available-message">
        <div id="message-content">
            <span class="close-btn" onclick="hideMessage()">&times;</span>
            <h2>PRODUCT NOT AVAILABLE RIGHT NOW</h2>
        </div>
    </div>
    
    <script>
        // Define the content for each page
        const pages = {
            home: `
                <div id="home-content">
                    <h2>WELCOME, kindly click on products to order now</h2>
                </div>
            `,
            products: `
                <h2>Featured Products</h2>
                <div id="products-grid">
                    <div class="product-card">
                        <img src="IMG-20250729-WA0002.jpg" alt="Simple luxury handbag">
                        <h3>simple luxury handbag</h3>
                        <p>very simple luxury bag for any occasion,vailable in different colors.</p>
                        <span class="price">₦5,000</span>
                        <a href="javascript:void(0)" class="btn" onclick="showMessage()">View Details</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/300" alt="Product Name 2">
                        <h3>Product Name 2</h3>
                        <p>Another great product you are selling. You can change this text easily.</p>
                        <span class="price">₦8,500</span>
                        <a href="javascript:void(0)" class="btn" onclick="showMessage()">View Details</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/300" alt="Product Name 3">
                        <h3>Product Name 3</h3>
                        <p>Describe your third product here. Highlight what makes it unique.</p>
                        <span class="price">₦12,000</span>
                        <a href="javascript:void(0)" class="btn" onclick="showMessage()">View Details</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/300" alt="Product Name 4">
                        <h3>Product Name 4</h3>
                        <p>A new item in your collection. Use this space for a compelling description.</p>
                        <span class="price">₦15,000</span>
                        <a href="javascript:void(0)" class="btn" onclick="showMessage()">View Details</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/300" alt="Product Name 5">
                        <h3>Product Name 5</h3>
                        <p>Another item you are selling. Describe the features and benefits.</p>
                        <span class="price">₦7,200</span>
                        <a href="javascript:void(0)" class="btn" onclick="showMessage()">View Details</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/300" alt="Product Name 6">
                        <h3>Product Name 6</h3>
                        <p>High-quality product with a unique design. Perfect for your needs.</p>
                        <span class="price">₦22,500</span>
                        <a href="javascript:void(0)" class="btn" onclick="showMessage()">View Details</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/300" alt="Product Name 7">
                        <h3>Product Name 7</h3>
                        <p>A brand new item, just added to our collection. Get it now!</p>
                        <span class="price">₦9,800</span>
                        <a href="javascript:void(0)" class="btn" onclick="showMessage()">View Details</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/300" alt="Product Name 8">
                        <h3>Product Name 8</h3>
                        <p>This product is a customer favorite. Read the reviews!</p>
                        <span class="price">₦18,000</span>
                        <a href="javascript:void(0)" class="btn" onclick="showMessage()">View Details</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/300" alt="Product Name 9">
                        <h3>Product Name 9</h3>
                        <p>A must-have product for your daily life. It's both useful and stylish.</p>
                        <span class="price">₦6,500</span>
                        <a href="javascript:void(0)" class="btn" onclick="showMessage()">View Details</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/300" alt="Product Name 10">
                        <h3>Product Name 10</h3>
                        <p>Limited stock available. Order yours today before it's gone!</p>
                        <span class="price">₦30,000</span>
                        <a href="javascript:void(0)" class="btn" onclick="showMessage()">View Details</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/300" alt="Product Name 11">
                        <h3>Product Name 11</h3>
                        <p>This product offers great value for its price. Check it out!</p>
                        <span class="price">₦4,200</span>
                        <a href="javascript:void(0)" class="btn" onclick="showMessage()">View Details</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/300" alt="Product Name 12">
                        <h3>Product Name 12</h3>
                        <p>A popular choice for many customers. You won't be disappointed.</p>
                        <span class="price">₦11,500</span>
                        <a href="javascript:void(0)" class="btn" onclick="showMessage()">View Details</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/300" alt="Product Name 13">
                        <h3>Product Name 13</h3>
                        <p>Get this product delivered to your doorstep. Fast shipping!</p>
                        <span class="price">₦19,000</span>
                        <a href="javascript:void(0)" class="btn" onclick="showMessage()">View Details</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/300" alt="Product Name 14">
                        <h3>Product Name 14</h3>
                        <p>High-quality materials and craftsmanship. Built to last.</p>
                        <span class="price">₦25,000</span>
                        <a href="javascript:void(0)" class="btn" onclick="showMessage()">View Details</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/300" alt="Product Name 15">
                        <h3>Product Name 15</h3>
                        <p>A versatile product that fits many different needs. Order now.</p>
                        <span class="price">₦8,900</span>
                        <a href="javascript:void(0)" class="btn" onclick="showMessage()">View Details</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/300" alt="Product Name 16">
                        <h3>Product Name 16</h3>
                        <p>A new and improved version of our classic best-seller.</p>
                        <span class="price">₦14,500</span>
                        <a href="javascript:void(0)" class="btn" onclick="showMessage()">View Details</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/300" alt="Product Name 17">
                        <h3>Product Name 17</h3>
                        <p>This is a limited edition product. Don't miss your chance!</p>
                        <span class="price">₦35,000</span>
                        <a href="javascript:void(0)" class="btn" onclick="showMessage()">View Details</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/300" alt="Product Name 18">
                        <h3>Product Name 18</h3>
                        <p>Simple, elegant, and effective. The perfect addition to your life.</p>
                        <span class="price">₦9,000</span>
                        <a href="javascript:void(0)" class="btn" onclick="showMessage()">View Details</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/300" alt="Product Name 19">
                        <h3>Product Name 19</h3>
                        <p>A budget-friendly option without compromising on quality.</p>
                        <span class="price">₦6,000</span>
                        <a href="javascript:void(0)" class="btn" onclick="showMessage()">View Details</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/300" alt="Product Name 20">
                        <h3>Product Name 20</h3>
                        <p>This product is a game-changer. Experience the difference!</p>
                        <span class="price">₦28,000</span>
                        <a href="javascript:void(0)" class="btn" onclick="showMessage()">View Details</a>
                    </div>
                </div>
            `,
            about: `
                <div id="about-content">
                    <h2>About ADEHUN OLUWA HOME OF VARIETIES</h2>
                    <p>As your reliable vendor, I'm happy to tell you about this wonderful business! ADEHUN OLUWA HOME OF VARIETIES is more than just a store; it's a place built on passion and a commitment to quality. The mission is to bring a wide range of unique and useful products directly to you, making your life easier and more enjoyable. From carefully selected items to dedicated customer service, every part of this store is designed with you in mind. We're building something special here, and we're so glad you're a part of it!</p>
                </div>
            `,
            contact: `
                <div id="contact-content">
                    <h2>Contact Us</h2>
                    <p>Feel free to reach out to us with any questions or orders.</p>
                    <p><strong>Phone:</strong> <a href="tel:07077840797">0707 784 0797</a></p>
                    <p><strong>Email:</strong> <a href="mailto:afolabitosinchristiana@gmail.Com">afolabitosinchristiana@gmail.Com</a></p>
                </div>
            `
        };

        // This function loads the correct page content
        function loadPage(pageName) {
            const mainContent = document.getElementById('main-content');
            if (mainContent) {
                mainContent.innerHTML = pages[pageName];
            }
        }

        // JavaScript functions for the pop-up message
        function showMessage() {
            const messageBox = document.getElementById('not-available-message');
            messageBox.style.display = 'flex';
        }
        
        function hideMessage() {
            const messageBox = document.getElementById('not-available-message');
            messageBox.style.display = 'none';
        }

        // Load the home page content when the page first loads
        window.onload = function() {
            loadPage('home');
        };
    </script>
</body>
</html>

