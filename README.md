<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Photography Portfolio</title>
    <link rel="stylesheet" href="styles.css">
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Roboto', sans-serif;
            margin: 0;
            padding: 0;
            background: #fff;
        }
        header {
            background: #666;
            color: #fff;
            text-align: center;
            padding: 1em 0;
        }
        nav ul {
            list-style: none;
            padding: 0;
        }
        nav ul li {
            display: inline;
            margin: 0 1em;
        }
        nav ul li a {
            color: #fff;
            text-decoration: none;
        }
        .container {
            padding: 2em;
        }

        .gallery {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
            max-width: 900px;
            margin: 0 auto;
        }
        .gallery img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            border-radius: 4px;
        }
        footer {
            background: #666;
            color: #fff;
            text-align: center;
            padding: 1em 0;
        }
    </style>
</head>
<body>
    <header>
        <h1>Amy Zhang Photography</h1>
        <nav>
            <ul>
                <li><a href="#about">About</a></li>
                <li><a href="#gallery">Gallery</a></li>
            </ul>
        </nav>
    </header>
    <div class="container">
        <section id="about" class="about">
            <h2>About Me</h2>
            <p>Hi, I'm Amy! I'm the News Photo Editor of Vol. 120 of The Duke Chronicle, and I'm also a freelance photographer in Durham, NC. My 2024-2025 bookings are open.</p>
            <p>If you'd like to get in touch, please email me at <a href="mailto:amy.zhang@duke.edu">amy.zhang@duke.edu</a>.</p>
        </section>
        <section id="gallery" class="gallery">
            <img src="images/photo1.jpg" alt="Photo 1">
            <img src="images/photo2.jpg" alt="Photo 2">
            <img src="images/photo3.jpg" alt="Photo 3">
            <img src="images/photo4.jpg" alt="Photo 4">
            <img src="images/photo5.jpg" alt="Photo 5">
            <img src="images/photo6.jpg" alt="Photo 6">
            <img src="images/photo7.jpg" alt="Photo 7">
            <img src="images/photo8.jpg" alt="Photo 8">
            <img src="images/photo9.jpg" alt="Photo 9">
        </section>

    </div>
    <footer>
        <p>&copy; 2024 Amy Zhang Photography</p>
    </footer>
</body>
</html>
