<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Photography Portfolio</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;600&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Montserrat', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f8f8f8;
            color: #333;
            line-height: 1.6;
        }
        header {
            background-color: #fff;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
            padding: 1em 0;
            position: sticky;
            top: 0;
            z-index: 1000;
        }
        h1 {
            text-align: center;
            font-weight: 300;
            font-size: 2.5em;
            margin: 0;
            padding: 0.5em 0;
        }
        nav ul {
            list-style: none;
            padding: 0;
            text-align: center;
        }
        nav ul li {
            display: inline;
            margin: 0 1em;
        }
        nav ul li a {
            color: #333;
            text-decoration: none;
            font-weight: 400;
            transition: color 0.3s ease;
        }
        nav ul li a:hover {
            color: #666;
        }
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 2em;
        }
        .about {
            background-color: #fff;
            padding: 2em;
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
            margin-bottom: 2em;
        }
        h2 {
            font-weight: 600;
            color: #222;
        }
        .gallery {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
        }
        .gallery img {
            width: 100%;
            height: 300px;
            object-fit: cover;
            border-radius: 8px;
            transition: transform 0.3s ease;
        }
        .gallery img:hover {
            transform: scale(1.05);
        }
        footer {
            background-color: #fff;
            color: #333;
            text-align: center;
            padding: 1em 0;
            margin-top: 2em;
            box-shadow: 0 -2px 4px rgba(0,0,0,0.1);
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
        <h2>Gallery</h2>
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
