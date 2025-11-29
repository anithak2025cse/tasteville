<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>TasteVille Restaurant</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #fff7e6;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #ff8800;
            padding: 20px;
            text-align: center;
            color: white;
            font-size: 28px;
            font-weight: bold;
        }
        .menu-container {
            padding: 20px;
        }
        .menu-item {
            background: #ffffff;
            padding: 15px;
            margin: 10px 0;
            border-radius: 8px;
            box-shadow: 0px 2px 5px #ccc;
        }
        h3 {
            margin: 0;
        }
        form {
            background: #fff;
            margin: 20px;
            padding: 15px;
            border-radius: 8px;
            box-shadow: 0px 2px 5px #ccc;
        }
        textarea {
            width: 100%;
            height: 80px;
            padding: 8px;
            font-size: 14px;
        }
        button {
            background-color: #ff8800;
            color: white;
            padding: 10px 20px;
            border: none;
            margin-top: 10px;
            cursor: pointer;
            border-radius: 5px;
        }
        button:hover {
            background-color: #e67300;
        }
        .thankyou {
            color: green;
            font-size: 18px;
            margin-top: 10px;
        }
    </style>
</head>
<body>

<header>
    TasteVille Restaurant
</header>

<div class="menu-container">
    <h2>🍽 Available Menu Items</h2>

    <div class="menu-item">
        <h3>🍕 Pizza</h3>
        <p>Price: ₹120</p>
    </div>

    <div class="menu-item">
        <h3>🍔 Burger</h3>
        <p>Price: ₹80</p>
    </div>

    <div class="menu-item">
        <h3>🍛 Fried Rice</h3>
        <p>Price: ₹100</p>
    </div>

    <div class="menu-item">
        <h3>🥪 Sandwich</h3>
        <p>Price: ₹70</p>
    </div>

    <div class="menu-item">
        <h3>☕ Coffee</h3>
        <p>Price: ₹40</p>
    </div>
</div>

<form id="feedbackForm">
    <h2>📝 Submit Your Feedback</h2>
    <textarea id="feedbackText" placeholder="Write your feedback here..." required></textarea>
    <button type="submit">Submit Feedback</button>
    <p class="thankyou" id="thankYouMessage" style="display: none;">Thank you for your feedback! ❤️</p>
</form>

<script>
    document.getElementById("feedbackForm").onsubmit = function(event) {
        event.preventDefault();
        document.getElementById("thankYouMessage").style.display = "block";
        document.getElementById("feedbackText").value = "";
    };
</script>

</body>
</html>
