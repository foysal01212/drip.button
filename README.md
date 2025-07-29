<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta name="description" content="Drip Button - Minimalist premium shirts. Keep dripping with style." />
  <title>Drip Button - Premium Minimalist Shirts</title>
  <link rel="icon" href="images/favicon.png" type="image/png"> <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg: #ffffff;
      --text: #1a1a1a;
      --primary: #000000;
      --accent: #f5f5f5;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Inter', sans-serif;
    }

    body {
      background: var(--bg);
      color: var(--text);
      line-height: 1.6;
      min-height: 100vh;
      display: flex;
      flex-direction: column;
    }

    header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 1rem 2rem;
      background: var(--bg);
      border-bottom: 1px solid #eee;
      position: sticky;
      top: 0;
      z-index: 10;
    }

    nav a {
      margin-left: 1.5rem;
      text-decoration: none;
      color: var(--text);
      font-weight: 500;
      transition: color 0.3s ease; /* Smooth hover effect */
    }

    nav a:hover {
      color: var(--primary);
    }

    .hero {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      padding: 4rem 2rem;
      background-color: var(--accent);
    }

    .hero h1 {
      font-size: 2.8rem; /* Slightly larger heading */
      margin-bottom: 1rem;
    }

    .hero p {
      font-size: 1.2rem;
      max-width: 600px;
      margin-bottom: 2rem; /* Space below paragraph */
    }

    .hero-button {
      background-color: var(--primary);
      color: var(--bg);
      padding: 1rem 2rem;
      border-radius: 5px;
      text-decoration: none;
      font-weight: 600;
      display: inline-block;
      transition: background-color 0.3s ease;
    }

    .hero-button:hover {
      background-color: #333;
    }

    .section {
      padding: 4rem 2rem;
      max-width: 1100px;
      margin: auto;
    }

    .section h2 { /* Centralized h2 styling */
      text-align: center;
      margin-bottom: 2rem;
    }

    .section p.centered-text { /* New class for centered paragraphs */
      max-width: 700px;
      margin: auto;
      text-align: center;
    }

    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); /* Slightly larger min-width */
      gap: 2rem;
    }

    .product-card {
      background: #fafafa;
      padding: 1.5rem; /* More padding */
      border-radius: 8px;
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.08); /* Stronger shadow for depth */
      text-align: center;
      display: flex;
      flex-direction: column;
      justify-content: space-between; /* Pushes button to bottom */
    }

    .product-image {
      max-width: 100%;
      height: 250px; /* Fixed height for consistent look */
      object-fit: cover; /* Ensures image covers area, crops if needed */
      border-radius: 4px;
      margin-bottom: 1rem;
    }

    .product-card h3 {
      margin-bottom: 0.5rem;
      font-size: 1.3rem;
    }

    .product-card p {
      margin-bottom: 1rem;
      font-size: 1.1rem;
      font-weight: 600;
      color: var(--primary);
    }

    .add-to-cart-btn {
      background-color: var(--primary);
      color: var(--bg);
      padding: 0.75rem 1.5rem;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      font-size: 1rem;
      margin-top: auto; /* Pushes button to the bottom */
      transition: background-color 0.3s ease;
    }

    .add-to-cart-btn:hover {
      background-color: #333;
    }

    footer {
      margin-top: auto;
      text-align: center;
      padding: 2rem;
      font-size: 0.9rem;
      background: var(--accent);
      color: #555; /* Slightly muted footer text */
    }

    /* Basic responsiveness */
    @media (max-width: 768px) {
      header {
        flex-direction: column;
        padding: 1rem;
      }

      nav a {
        margin: 0.5rem 1rem;
      }

      .hero h1 {
        font-size: 2rem;
      }

      .hero p {
        font-size: 1rem;
      }

      .section {
        padding: 2rem 1rem;
      }
    }
  </style>
</head>

<body>
  <header>
    <h2>Drip Button</h2>
    <nav>
      <a href="#home">Home</a>
      <a href="#shop">Shop</a>
      <a href="#about">About Us</a>
      <a href="#contact">Contact</a>
      <a href="#cart">Cart <span id="cart-item-count">(0)</span></a> </nav>
  </header>

  <section class="hero" id="home">
    <h1>Keep Dripping with Style</h1>
    <p>Premium quality minimalist shirts designed for everyday comfort and elevated aesthetics.</p>
    <a href="#shop" class="hero-button">Shop Now</a>
  </section>

  <section class="section" id="shop">
    <h2>Shop Our Collection</h2>
    <div class="grid">
      <div class="product-card" data-product-id="1" data-name="Classic Black Tee" data-price="29.99">
        <img src="images/black-tee.jpg" alt="Drip Button Classic Black Tee" class="product-image">
        <h3>Classic Black Tee</h3>
        <p>$29.99</p>
        <button class="add-to-cart-btn">Add to Cart</button>
      </div>
      <div class="product-card" data-product-id="2" data-name="Crisp White Polo" data-price="39.99">
        <img src="images/white-polo.jpg" alt="Drip Button Crisp White Polo" class="product-image">
        <h3>Crisp White Polo</h3>
        <p>$39.99</p>
        <button class="add-to-cart-btn">Add to Cart</button>
      </div>
      <div class="product-card" data-product-id="3" data-name="Navy Crewneck" data-price="34.99">
        <img src="images/navy-crewneck.jpg" alt="Drip Button Navy Crewneck" class="product-image">
        <h3>Navy Crewneck</h3>
        <p>$34.99</p>
        <button class="add-to-cart-btn">Add to Cart</button>
      </div>
      <div class="product-card" data-product-id="4" data-name="Heather Grey Hoodie" data-price="49.99">
        <img src="images/grey-hoodie.jpg" alt="Drip Button Heather Grey Hoodie" class="product-image">
        <h3>Heather Grey Hoodie</h3>
        <p>$49.99</p>
        <button class="add-to-cart-btn">Add to Cart</button>
      </div>
      </div>
  </section>

  <section class="section" id="about">
    <h2>About Us</h2>
    <p class="centered-text">
      At Drip Button, we believe in timeless design and effortless style. Our shirts are crafted for those who value simplicity, quality, and confidence. Whether it's for your everyday look or a bold statement, we’re here to keep your drip consistent and classic.
    </p>
  </section>

  <section class="section" id="contact">
    <h2>Contact Us</h2>
    <p class="centered-text">
      Email: <a href="mailto:mdabidshahriar@gmail.com">mdabidshahriar@gmail.com</a><br>
      Instagram: <a href="https://instagram.com/drip_button" target="_blank" rel="noopener noreferrer">@drip_button</a>
    </p>
    </section>

  <footer>
    &copy; 2025 Drip Button. All rights reserved.
  </footer>

  <script>
    // Basic JavaScript for a simple "add to cart" (client-side only)
    let cart = []; // Your shopping cart array

    document.addEventListener('DOMContentLoaded', () => {
      const cartItemCount = document.getElementById('cart-item-count');
      const addToCartButtons = document.querySelectorAll('.add-to-cart-btn');

      // Load cart from localStorage if it exists
      if (localStorage.getItem('dripButtonCart')) {
        cart = JSON.parse(localStorage.getItem('dripButtonCart'));
        updateCartCount();
      }

      addToCartButtons.forEach(button => {
        button.addEventListener('click', (event) => {
          const productCard = event.target.closest('.product-card');
          const productId = productCard.dataset.productId;
          const productName = productCard.dataset.name;
          const productPrice = parseFloat(productCard.dataset.price);

          const existingItem = cart.find(item => item.id === productId);

          if (existingItem) {
            existingItem.quantity++;
          } else {
            cart.push({ id: productId, name: productName, price: productPrice, quantity: 1 });
          }

          localStorage.setItem('dripButtonCart', JSON.stringify(cart)); // Save to localStorage
          updateCartCount();
          alert(${productName} added to cart!);
          console.log('Current Cart:', cart); // For debugging
        });
      });

      function updateCartCount() {
        const totalItems = cart.reduce((sum, item) => sum + item.quantity, 0);
        cartItemCount.textContent = (${totalItems});
      }

      // Placeholder for a very basic cart page rendering (you'd need a dedicated #cart section)
      // This would go on your actual "cart" page or pop-up
      if (window.location.hash === '#cart') {
          // You'd typically have a dedicated page or modal for the cart
          // For now, let's just log it to console
          console.log("Welcome to your Cart page. Items:", cart);
          // Here you'd loop through 'cart' array and dynamically create HTML elements
          // to display the cart items, quantities, and total.
      }
    });
  </script>
</body>

</html>
