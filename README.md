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
            background: #fff;
            color: #000;
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
            color: #000;
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
            background: #fff;
            color: #000;
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
            </ul>
        </nav>
    </header>
    <div class="container">
        <section id="about" class="about">
            <h2>About Me</h2>
            <p>Hi, I'm Amy! I'm the News Photo Editor of Vol. 120 of The Duke Chronicle, and I'm also a freelance photographer in Durham, NC. My 2024-2025 bookings are open.</p>
            <p>If you'd like to get in touch, please email me at <a href="mailto:amy.zhang@duke.edu">amy.zhang@duke.edu</a>.</p>
            <p><a href="https://www.instagram.com/amydotjpeg" target="_blank">To see more of my work, check out my Instagram</a>.</p>
        </section>
        <h2>Gallery</h2>
        <section id="gallery" class="gallery">
            <img src="compressed images/photo1-min.jpg" alt="Photo 1">
            <img src="compressed images/photo2-min.jpg" alt="Photo 2">
            <img src="compressed images/photo3-min.jpg" alt="Photo 3">
            <img src="compressed images/photo4-min.jpg" alt="Photo 4">
            <img src="compressed images/photo5-min.jpg" alt="Photo 5">
            <img src="compressed images/photo6-min.jpg" alt="Photo 6">
            <img src="compressed images/photo7-min.jpg" alt="Photo 7">
            <img src="compressed images/photo8-min.jpg" alt="Photo 8">
            <img src="compressed images/photo9-min.jpg" alt="Photo 9">            
            <img src="compressed images/photo10-min.jpg" alt="Photo 10">
            <img src="compressed images/photo11-min.jpg" alt="Photo 11">
            <img src="compressed images/photo12-min.jpg" alt="Photo 12">            
            <img src="compressed images/photo13-min.jpg" alt="Photo 13">
            <img src="compressed images/photo14-min.jpg" alt="Photo 14">
            <img src="compressed images/photo15-min.jpg" alt="Photo 15">
        </section>
    </div>
    <footer>
        <p>&copy; 2024 Amy Zhang Photography</p>
    </footer>
</body>
</html>
