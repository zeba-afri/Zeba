<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Blooming Flower</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #fce4ec;
            flex-direction: column;
            text-align: center;
        }
        #flower {
            width: 150px;
            cursor: pointer;
            transition: opacity 1s ease-in-out;
        }
        #message {
            font-size: 20px;
            font-weight: bold;
            color: #d81b60;
            margin-top: 20px;
            display: none;
        }
    </style>
</head>
<body>

    <img id="flower" src="https://via.placeholder.com/150/ff0000/ffffff?text=Bud" alt="Closed Flower" onclick="bloomFlower()">
    <p id="message">A flower to my favorite person, AFRIDI</p>

    <script>
        function bloomFlower() {
            let flower = document.getElementById("flower");
            let message = document.getElementById("message");

            flower.src = "https://via.placeholder.com/150/00ff00/ffffff?text=Bloom"; // Change this to an actual flower image URL
            setTimeout(() => {
                message.style.display = "block";
            }, 1000);
        }
    </script>

</body>
</html>
