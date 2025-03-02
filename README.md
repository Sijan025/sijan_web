<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Luxury Timepieces</title>
    <link rel="stylesheet" href="style.css">
    <style>
        body {
            font-family: 'Poppins', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #0a0a0a;
            color: #fff;
        }
        header {
            background: linear-gradient(90deg, #000, #222);
            padding: 20px;
            text-align: center;
            font-size: 30px;
            font-weight: bold;
            letter-spacing: 2px;
            text-transform: uppercase;
            box-shadow: 0 4px 8px rgba(255, 215, 0, 0.3);
        }
        .hero {
            background: url('image5.jpg') no-repeat center/cover;
            height: 80vh;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 50px;
            font-weight: bold;
            text-shadow: 2px 2px 10px rgba(255, 215, 0, 0.8);
            color: gold;
        }
        .section {
            padding: 50px;
            text-align: center;
            font-size: 20px;
            background: url('your-background-image.jpg') no-repeat center/cover; /* Added background image */
            background-size: cover;
            color: #fff; /* Ensures text is visible against the image */
        }
        .gallery {
            display: flex;
            justify-content: center;
            gap: 30px;
            flex-wrap: wrap;
            padding: 30px;
        }
        .gallery .item {
            text-align: center;
            background: #222;
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0 4px 8px rgba(255, 215, 0, 0.5);
            transition: transform 0.3s;
        }
        .gallery .item:hover {
            transform: scale(1.05);
        }
        .gallery img {
            width: 300px;
            border-radius: 10px;
            transition: opacity 0.3s;
        }
        .gallery img:hover {
            opacity: 0.8;
        }
        .price {
            color: gold;
            font-size: 22px;
            margin-top: 10px;
            font-weight: bold;
        }
        .add-to-cart {
            background: gold;
            color: black;
            padding: 10px 20px;
            margin-top: 10px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-weight: bold;
            transition: background 0.3s;
        }
        .add-to-cart:hover {
            background: darkgoldenrod;
        }
        .location {
            text-align: center;
            padding: 40px;
            background: url('your-location-background.jpg') no-repeat center/cover; /* Added background image */
            background-size: cover;
            font-size: 20px;
            box-shadow: 0 -4px 8px rgba(158, 140, 36, 0.3);
            color: #f3ebeb; /* Ensures text is visible against the image */
        }
    </style>
</head>
<body>
    <header>Luxury Timepieces</header>
    <div class="hero">Exclusive Collection</div>
    <div class="section">
        <h2>Discover Our Premium Watches</h2>
        <p>Experience timeless elegance with our handcrafted luxury watches.</p>
    </div>
    <div class="gallery">
        <div class="item">
            <img src="image1.jpg" alt="Premium Watch 1">
            <p class="price">$1,500</p>
            <button class="add-to-cart" onclick="playSound()">Add to Cart</button>
        </div>
        <div class="item">
            <img src="image2.jpg" alt="Premium Watch 2">
            <p class="price">$1,500</p>
            <button class="add-to-cart" onclick="playSound()">Add to Cart</button>
        </div>
        <div class="item">
            <img src="image3.jpg" alt="Premium Watch 3">
            <p class="price">$1,500</p>
            <button class="add-to-cart" onclick="playSound()">Add to Cart</button>
        </div>
        <div class="item">
            <img src="image4.jpg" alt="Premium Watch 4">
            <p class="price">$1,500</p>
            <button class="add-to-cart" onclick="playSound()">Add to Cart</button>
        </div>
        <div class="item">
            <img src="image5.jpg" alt="Premium Watch 5">
            <p class="price">$1,800</p>
            <button class="add-to-cart" onclick="playSound()">Add to Cart</button>
        </div>
    </div>
    <div class="location">
        <h2>1st Time in Nepal - At pokhara-11,Nepal</h2>
        <p>Find our offline store at Pokhara, Nepal.</p>
        <p>Infront of Manipal Teching Hospital</p>
    </div>

    <!-- Audio element for the sound -->
    <audio id="cart-sound" src="click-sound.mp3" preload="auto"></audio>

    <script>
        function playSound() {
            var sound = document.getElementById("cart-sound");
            sound.play(); // Play the sound when the button is clicked
        }
    </script>
</body>
</html>
