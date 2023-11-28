<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Website</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            text-align: center;
            margin: 20px;
        }

        form {
            display: flex;
            flex-direction: column;
            align-items: center;
            max-width: 300px;
            margin: 0 auto;
        }

        input, button {
            margin: 5px;
            padding: 8px;
        }
    </style>
</head>
<body>
    <h1>Welcome to Your Website</h1>

    <form action="https://www.google.com" method="GET">
        <label for="searchQuery">Search on Google:</label>
        <input type="text" id="searchQuery" name="q" placeholder="Type your query">
        <button type="submit">Search</button>
    </form>
</body>
</html>
