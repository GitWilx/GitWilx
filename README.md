<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>Wilx - Online Clothing Store</title>
</head>
<body>
    <header>
        <h1>Wilx</h1>
    </header>

    <main id="products">
        <!-- Product listings go here -->
    </main>

    <footer>
        <p>&copy; 2023 Wilx - Online Clothing Store</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
body {
    font-family: 'Arial', sans-serif;
    margin: 0;
    padding: 0;
}

header {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 1em;
}

main {
    padding: 1em;
}

footer {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 1em;
    position: fixed;
    bottom: 0;
    width: 100%;
}
// Sample product data
const products = [
    { id: 1, name: 'T-Shirt', price: 20.99 },
    { id: 2, name: 'Jeans', price: 49.99 },
    // Add more products as needed
];

document.addEventListener('DOMContentLoaded', () => {
    const productsSection = document.getElementById('products');

    // Display products
    products.forEach(product => {
        const productCard = document.createElement('div');
        productCard.classList.add('product-card');
        productCard.innerHTML = `
            <h2>${product.name}</h2>
            <p>$${product.price.toFixed(2)}</p>
            <button onclick="addToCart(${product.id})">Add to Cart</button>
        `;
        productsSection.appendChild(productCard);
    });
});

// Example function to handle adding a product to the cart
function addToCart(productId) {
    // Implement your cart logic here
    alert(`Product with ID ${productId} added to cart`);
}
