<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Photography Portfolio</title>
    <link rel="stylesheet" href="styles.css">
    <style>
        body {
            font-family: 'Times New Roman', Times, serif;
            margin: 0;
            padding: 0;
            background: #fff;
        }
        header {
            background: #000;
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
        .about, .contact {
            margin-bottom: 2em;
        }
        .gallery {
            display: flex;
            flex-wrap: wrap;
            gap: 1em;
        }
        .gallery img {
            max-width: calc(33.333% - 1em);
            width: 100%;
            height: auto;
        }
        footer {
            background: #000;
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
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>
    <div class="container">
        <section id="about" class="about">
            <h2>About Me</h2>
            <p>Hi, I'm Amy! I'm the News Photo Editor of Vol. 120 of The Duke Chronicle, and I'm also a freelance photographer in Durham, NC. My 2024-2025 bookings are open.</p>
        </section>
        <section id="gallery" class="gallery">
            <h2>Gallery</h2>
            <img src="images/photo1.jpg" alt="Photo 1">
            <img src="images/photo2.jpg" alt="Photo 2">
            <img src="images/photo3.jpg" alt="Photo 3">
            <!-- Add more images as needed -->
        </section>
        <section id="contact" class="contact">
            <h2>Contact</h2>
            <p>If you'd like to get in touch, please email me at <a href="mailto:amy.zhang@duke.edu">amy.zhang@duke.edu</a>.</p>
        </section>
    </div>
    <footer>
        <p>&copy; 2024 Amy Zhang Photography</p>
    </footer>
</body>
</html>
