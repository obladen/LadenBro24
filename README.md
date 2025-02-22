# LadenB<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Free Fire Top-Up</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f4f4f4;
            padding: 20px;
        }
        .container {
            max-width: 500px;
            margin: auto;
            background: white;
            padding: 20px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            border-radius: 10px;
        }
        input, button {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border-radius: 5px;
            border: 1px solid #ccc;
        }
        button {
            background-color: #28a745;
            color: white;
            font-size: 16px;
            cursor: pointer;
        }
        button:hover {
            background-color: #218838;
        }
    </style>
</head>
<body>
    <div class="container">
        <h2>Free Fire Diamond Top-Up</h2>
        <p>Enter your Player ID and choose a top-up amount.</p>
        <input type="text" id="playerId" placeholder="Enter Player ID" required>
        <input type="number" id="amount" placeholder="Enter Diamond Amount" required>
        <button onclick="topUp()">Submit</button>
        <p id="message"></p>
    </div>

    <script>
        function topUp() {
            let playerId = document.getElementById('playerId').value;
            let amount = document.getElementById('amount').value;
            let message = document.getElementById('message');
            
            if (playerId === '' || amount === '') {
                message.innerHTML = "Please enter all details!";
                message.style.color = "red";
                return;
            }
            
            message.innerHTML = "Your top-up request is being processed!";
            message.style.color = "green";
        }
    </script>
</body>
</html>
ro24
