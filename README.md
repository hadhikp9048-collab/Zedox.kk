/* Global Styles */
body {
    font-family: 'Arial', sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f9f9f9;
}

header {
    background-color: #333;
    color: white;
    padding: 20px;
    text-align: center;
}

header .logo {
    display: flex;
    align-items: center;
    justify-content: center;
}

header h1 {
    margin-left: 10px;
    font-size: 32px;
}

nav a {
    margin: 0 15px;
    text-decoration: none;
    color: white;
    font-size: 18px;
}

nav a:hover {
    color: #ff6347;
}

main {
    padding: 20px;
}

.product-section h2, .cart-section h2 {
    text-align: center;
    margin-bottom: 20px;
}

.product-container {
    display: flex;
    justify-content: center;
    gap: 20px;
    flex-wrap: wrap;
}

.product {
    background-color: white;
    padding: 20px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    text-align: center;
    width: 250px;
    border-radius: 8px;
}

.product img {
    width: 100%;
    height: auto;
    border-radius: 8px;
}

.product h3 {
    font-size: 20px;
    margin: 10px 0;
}

.product p {
    font-size: 18px;
    color: #333;
}

.add-to-cart {
    background-color: #ff6347;
    color: white;
    padding: 10px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    width: 100%;
}

.add-to-cart:hover {
    background-color: #e5533f;
}

.cart-section {
    background-color: white;
    padding: 20px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    border-radius: 8px;
    margin-top: 40px;
}

.cart-section #cart-items {
    margin-bottom: 20px;
}

.cart-section #cart-total {
    text-align: center;
}

#checkout-btn {
    background-color: #28a745;
    color: white;
    padding: 15px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    font-size: 18px;
}

#checkout-btn:hover {
    background-color: #218838;
}

footer {
    background-color: #333;
    color: white;
    padding: 10px;
    text-align: center;
}

/* Mobile Responsiveness */
@media (max-width: 768px) {
    /* Stack the header elements */
    header {
        text-align: center;
        padding: 15px;
    }

    header .logo {
        flex-direction: column;
        align-items: center;
        justify-content: center;
    }

    header h1 {
        font-size: 26px;
    }

    /* Product section: display in a single column for mobile */
    .product-container {
        flex-direction: column;
        align-items: center;
    }

    .product {
        width: 90%; /* Take full width on small screens */
        margin-bottom: 20px;
    }

    .cart-section {
        padding: 15px;
    }

    /* Adjust font sizes */
    .product h3 {
        font-size: 18px;
    }

    .product p {
        font-size: 16px;
    }

    #checkout-btn {
        font-size: 16px;
        padding: 12px;
    }
}

/* Extra small screens (mobile devices in portrait mode) */
@media (max-width: 480px) {
    .product h3 {
        font-size: 16px;
    }

    .product p {
        font-size: 14px;
    }

    #checkout-btn {
        font-size: 14px;
        padding: 10px;
    }

    /* Cart Section */
    .cart-section {
        padding: 10px;
    }
}
