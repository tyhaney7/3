# 3
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>WagerWire Prototype</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f9;
        }
        header {
            background-color: #333;
            color: white;
            padding: 10px 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        header h1 {
            margin: 0;
        }
        nav {
            display: flex;
            gap: 15px;
        }
        nav a {
            color: white;
            text-decoration: none;
        }
        main {
            padding: 20px;
        }
        .section {
            background-color: white;
            padding: 15px;
            margin-bottom: 20px;
            border-radius: 5px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }
        .section h2 {
            margin-top: 0;
        }
        .button {
            padding: 10px 15px;
            background-color: #007bff;
            color: white;
            text-decoration: none;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .button:hover {
            background-color: #0056b3;
        }
        .bet-card {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            margin-bottom: 10px;
        }
        .bet-card h3 {
            margin: 0;
        }
    </style>
</head>
<body>
    <header>
        <h1>WagerWire</h1>
        <nav>
            <a href="#marketplace">Marketplace</a>
            <a href="#my-bets">My Bets</a>
            <a href="#create-bet">Create Bet</a>
        </nav>
    </header>

    <main>
        <section id="marketplace" class="section">
            <h2>Marketplace</h2>
            <div class="bet-card">
                <div>
                    <h3>Chiefs to Win Super Bowl</h3>
                    <p>Odds: +500</p>
                    <p>Price: $25</p>
                </div>
                <button class="button">Buy Now</button>
            </div>
            <div class="bet-card">
                <div>
                    <h3>Bills to Win Super Bowl</h3>
                    <p>Odds: +400</p>
                    <p>Price: $30</p>
                </div>
                <button class="button">Buy Now</button>
            </div>
        </section>

        <section id="my-bets" class="section">
            <h2>My Bets</h2>
            <div class="bet-card">
                <div>
                    <h3>Packers to Win Super Bowl</h3>
                    <p>Odds: +1000</p>
                    <p>Shares Held: 10</p>
                </div>
                <button class="button">List for Sale</button>
            </div>
        </section>

        <section id="create-bet" class="section">
            <h2>Create Bet</h2>
            <form>
                <label for="bet-title">Bet Title:</label><br>
                <input type="text" id="bet-title" name="bet-title" style="width: 100%; padding: 10px; margin: 10px 0;" required><br>
                
                <label for="odds">Odds:</label><br>
                <input type="text" id="odds" name="odds" style="width: 100%; padding: 10px; margin: 10px 0;" required><br>
                
                <label for="price">Price:</label><br>
                <input type="number" id="price" name="price" style="width: 100%; padding: 10px; margin: 10px 0;" required><br>

                <button type="submit" class="button">Create Bet</button>
            </form>
        </section>
    </main>
</body>
</html>
