<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Basic Website</title>
    <style>
        /* Base Styles */
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            color: #333;
            background-color: #f4f4f9;
        }

        /* Header & Navigation */
        header {
            background-color: #2c3e50;
            color: #fff;
            padding: 1rem 0;
            position: sticky;
            top: 0;
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            max-width: 1100px;
            margin: 0 auto;
            padding: 0 20px;
        }

        nav .logo {
            font-size: 1.5rem;
            font-weight: bold;
        }

        nav ul {
            list-style: none;
            display: flex;
            margin: 0;
            padding: 0;
        }

        nav ul li {
            margin-left: 20px;
        }

        nav ul li a {
            color: #fff;
            text-decoration: none;
            font-weight: 500;
        }

        nav ul li a:hover {
            color: #1abc9c;
        }

        /* Main Content Container */
        .container {
            max-width: 1100px;
            margin: 40px auto;
            padding: 0 20px;
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, #34495e, #2c3e50);
            color: white;
            padding: 60px 20px;
            text-align: center;
            border-radius: 8px;
            margin-bottom: 30px;
        }

        .hero h1 {
            margin-top: 0;
            font-size: 2.5rem;
        }

        /* Interactive Button Section */
        .interactive-section {
            background: white;
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
            text-align: center;
        }

        button {
            background-color: #1abc9c;
            color: white;
            border: none;
            padding: 12px 24px;
            font-size: 1rem;
            border-radius: 5px;
            cursor: pointer;
            transition: background 0.3s;
        }

        button:hover {
            background-color: #16a085;
        }

        #message {
            margin-top: 20px;
            font-weight: bold;
            color: #2c3e50;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 20px;
            background-color: #2c3e50;
            color: white;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
    </style>
</head>
<body>

    <header>
        <nav>
            <div class="logo">MyWebsite</div>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">About</a></li>
                <li><a href="#">Contact</a></li>
            </ul>
        </nav>
    </header>

    <div class="container">
        <section class="hero">
            <h1>Welcome to My Website</h1>
            <p>This is a clean, minimal layout to help you start your web development journey.</p>
        </section>

        <section class="interactive-section">
            <h2>Test JavaScript Feature</h2>
            <p>Click the button below to trigger a live script interaction.</p>
            <button id="actionBtn">Click Me!</button>
            <p id="message"></p>
        </section>
    </div>

    <footer>
        <p>&copy; 2026 My Website. Created from scratch.</p>
    </footer>

    <script>
        // JavaScript for basic interactivity
        const button = document.getElementById('actionBtn');
        const message = document.getElementById('message');

        button.addEventListener('click', () => {
            message.textContent = "🎉 Hello! You successfully triggered the website's code.";
            button.style.backgroundColor = '#34495e';
            button.textContent = 'Clicked!';
        });
    </script>
</body>
</html>
