<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Amy Zhang Photography Portfolio</title>
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
        .about {
            display: flex;
            flex-direction: column; /* Changed from row to column */
            align-items: center; /* Center items horizontally */
            text-align: center; /* Center text */
        }
        .about img {
            width: 250px; /* Increased size */
            height: 250px; /* Increased size */
            border-radius: 50%;
            margin-top: 20px;
            margin-bottom: 20px;
        }
        .about div {
            margin-bottom: 1em;
        }
        .gallery {
            display: grid;
            grid-template-columns: repeat(3, 1fr); /* 3 columns by default */
            gap: 20px;
            max-width: 900px;
            margin: 0 auto;
        }
        .gallery img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            border-radius: 4px;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            position: relative;
            cursor: pointer;
        }
        .gallery img:hover {
            transform: scale(1.05);
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.3);
        }
        .gallery img::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.3);
            opacity: 0;
            transition: opacity 0.3s ease;
            border-radius: 4px;
        }
        .gallery img:hover::before {
            opacity: 1;
        }
        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.8);
            z-index: 1000;
            align-items: center;
            justify-content: center;
        }
        .modal img {
            max-width: 90%;
            max-height: 80%;
            border-radius: 8px;
        }
        .modal .close {
            position: absolute;
            top: 20px;
            right: 20px;
            font-size: 2em;
            color: #fff;
            cursor: pointer;
        }
        footer {
            background: #fff;
            color: #000;
            text-align: center;
            padding: 1em 0;
        }
        /* Media Queries for Smaller Screens */
        @media (max-width: 768px) {
            .container {
                padding: 1em;
            }
            header h1 {
                font-size: 1.5em;
            }
            .about img {
                width: 200px; /* Slightly smaller size for tablets */
                height: 200px;
            }
            .gallery {
                grid-template-columns: repeat(3, 1fr); /* 3 columns for tablets */
                gap: 15px;
            }
            .modal .close {
                font-size: 1.5em;
                top: 10px;
                right: 10px;
            }
        }

        @media (max-width: 480px) {
            header h1 {
                font-size: 1.2em;
            }
            .about img {
                width: 150px; /* Smaller size for mobile */
                height: 150px;
            }
            .gallery {
                grid-template-columns: repeat(3, 1fr); /* 3 columns for mobile */
                gap: 10px;
            }
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
            <div>
                <h2>About Me</h2>
                <p>Hi, I'm Amy! I'm the News Photo Editor of Vol. 120 of The Duke Chronicle, and I'm also a freelance photographer in Durham, NC. My 2024-2025 bookings are open.</p>
                <p>If you'd like to get in touch, please email me at <a href="mailto:amy.zhang@duke.edu">amy.zhang@duke.edu</a>.</p>
                <p><a href="https://www.instagram.com/amydotjpeg" target="_blank">To see more of my work, check out my Instagram</a>.</p>
            </div>
            <img src="pfp.heic" alt="Amy Zhang">
        </section>
        <h2>Gallery</h2>
        <section id="gallery" class="gallery">
            <img src="compressed images attempt 2/photo1zon.jpg" alt="Photo 1">
            <img src="compressed images attempt 2/photo2zon.jpg" alt="Photo 2">
            <img src="compressed images attempt 2/photo3zon.jpg" alt="Photo 3">
            <img src="compressed images attempt 2/photo4zon.jpg" alt="Photo 4">
            <img src="compressed images attempt 2/photo5zon.jpg" alt="Photo 5">
            <img src="compressed images attempt 2/photo6zon.jpg" alt="Photo 6">
            <img src="compressed images attempt 2/photo7zon.jpg" alt="Photo 7">
            <img src="compressed images attempt 2/photo8zon.jpg" alt="Photo 8">
            <img src="compressed images attempt 2/photo9zon.jpg" alt="Photo 9">            
            <img src="compressed images attempt 2/photo10zon.jpg" alt="Photo 10">
            <img src="compressed images attempt 2/photo11zon.jpg" alt="Photo 11">
            <img src="compressed images attempt 2/photo12zon.jpg" alt="Photo 12">            
            <img src="compressed images attempt 2/photo13zon.jpg" alt="Photo 13">
            <img src="compressed images attempt 2/photo14zon.jpg" alt="Photo 14">
            <img src="compressed images attempt 2/photo15zon.jpg" alt="Photo 15">
        </section>
    </div>
    <footer>
        <p>&copy; 2024 Amy Zhang Photography</p>
    </footer>

    <!-- Modal for Fullscreen Image -->
    <div id="modal" class="modal">
        <span class="close">&times;</span>
        <img id="modal-img" src="" alt="Enlarged Photo">
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', function () {
            const galleryImages = document.querySelectorAll('.gallery img');
            const modal = document.getElementById('modal');
            const modalImg = document.getElementById('modal-img');
            const closeBtn = document.querySelector('.modal .close');

            galleryImages.forEach(img => {
                img.addEventListener('click', function () {
                    modal.style.display = 'flex';
                    modalImg.src = this.src;
                });
            });

            closeBtn.addEventListener('click', function () {
                modal.style.display = 'none';
            });

            window.addEventListener('click', function (event) {
                if (event.target === modal) {
                    modal.style.display = 'none';
                }
            });
        });
    </script>
</body>
</html>

