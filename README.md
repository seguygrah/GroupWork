# GroupWork
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>After School Club</title>
    <script src="https://cdn.jsdelivr.net/npm/vue@2.7.14/dist/vue.js"></script>
</head>
<body>
    <div id="app">
        <h1>Cart: {{cart.length}}</h1>
        <h2>Modules: {{product.modules}}</h2>
        <p>Location: {{product.location}}</p>
        <p>Price: {{product.price}}</p>
        <p>Availability: {{product.availability}}</p>

        <button v-if="product.availability > 0" v-on:click="add_to_cart">Add To Cart</button>
        <button v-if="cart.length > 0" v-on:click="remove_from_cart(product.id)">Remove From Cart</button>

    </div>
</body>
</html>