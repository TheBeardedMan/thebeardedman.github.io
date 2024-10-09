<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Andrew McGaffic - Game Designer | Level Designer</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap');

        body, html {
            margin: 0;
            padding: 0;
            font-family: 'Poppins', sans-serif;
            color: #fff;
            background-color: #000;
            overflow-x: hidden;
        }

        .header {
            height: 100vh;
            width: 100%;
            position: relative;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            overflow: hidden;
        }

        .header video {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            object-fit: cover;
            z-index: -1;
            filter: brightness(50%);
        }

        .header .profile-pic {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            overflow: hidden;
            border: 5px solid #00d1ff;
            margin-bottom: 20px;
            z-index: 2;
            position: relative;
        }

        .header h1 {
            font-size: 60px;
            letter-spacing: 2px;
            margin: 0;
            color: #fff;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
            z-index: 2;
            position: relative;
        }

        .header h2 {
            font-size: 24px;
            margin: 10px 0;
            font-weight: 300;
            color: #a0cfee;
            z-index: 2;
            position: relative;
        }

        .navbar {
            position: fixed;
            top: 10px;
            left: 50%;
            transform: translateX(-50%);
            background-color: rgba(0, 0, 0, 0.7);
            padding: 10px 30px;
            border-radius: 30px;
            z-index: 100;
            display: flex;
            gap: 20px;
            box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.5);
        }

        .navbar a {
            color: #00d1ff;
            text-decoration: none;
            font-weight: 400;
            font-size: 16px;
            transition: color 0.3s ease;
        }

        .navbar a:hover {
            color: #fff;
        }

        .content {
            padding: 50px;
            width: 80%;
            max-width: 1200px;
            margin: 0 auto;
            background: rgba(34, 34, 34, 0.9);
            border-radius: 20px;
            box-shadow: 0 0 20px rgba(0, 0, 0, 0.5);
            margin-top: 50px;
        }

        .content h2 {
            font-size: 40px;
            letter-spacing: 1px;
            margin-bottom: 30px;
            color: #00d1ff;
            text-align: center;
        }

        .portfolio-item, .experience-item, .education-item, .contact-box {
            display: flex;
            justify-content: space-between;
            margin-bottom: 30px;
            background-color: rgba(34, 34, 34, 0.9);
            padding: 20px;
            border-radius: 12px;
            transition: transform 0.3s ease-in-out;
        }

        .portfolio-item:hover, .experience-item:hover, .education-item:hover, .contact-box:hover {
            transform: translateY(-10px);
        }

        .portfolio-item img, .experience-item img {
            width: 50%;
            height: auto;
            border-radius: 8px;
        }

        .portfolio-item div, .experience-item div, .education-item div, .contact-box div {
            width: 45%;
            text-align: left;
        }

        .portfolio-item h3, .experience-item h3, .education-item h3, .contact-box h3 {
            margin: 0 0 10px;
            font-size: 28px;
            color: #00d1ff;
        }

        .portfolio-item p, .experience-item p, .education-item p, .contact-box p {
            font-size: 16px;
            line-height: 1.6;
            color: #ccc;
        }

        .contact-box form {
            display: flex;
            flex-direction: column;
        }

        .contact-box input, .contact-box textarea {
            margin-bottom: 10px;
            padding: 10px;
            border-radius: 8px;
            border: none;
            font-size: 16px;
        }

        .contact-box input[type="submit"] {
            background-color: #00d1ff;
            color: #fff;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }

        .contact-box input[type="submit"]:hover {
            background-color: #00a1cc;
        }

        .scroll-down {
            position: absolute;
            bottom: 20px;
            left: 50%;
            transform: translate(-50%, 0);
            color: #00d1ff;
            font-size: 18px;
            animation: bounce 1.5s infinite;
        }

        @keyframes bounce {
            0%, 20%, 50%, 80%, 100% {
                transform: translateY(0);
            }
            40% {
                transform: translateY(-10px);
            }
            60% {
                transform: translateY(-5px);
            }
        }

    </style>
</head>
<body>

    <div class="navbar">
        <a href="#portfolio">Portfolio</a>
        <a href="#experience">Experience</a>
        <a href="#education">Education</a>
        <a href="#about">About Me</a>
        <a href="#contact">Contact Me</a>
    </div>

    <div class="header">
        <video autoplay muted loop>
            <source src="path-to-your-video.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
        <div class="profile-pic">
            <img src="C:\Users\Brend\OneDrive\Pictures\Screenshots\Screenshot 2024-09-13 094618.png" alt="Andrew McGaffic">
        </div>
        <h1>Andrew McGaffic</h1>
        <h2>Game Designer | Level Designer</h2>
        <div class="scroll-down">Scroll Down</div>
    </div>

    <div id="portfolio" class="content">
        <h2>Portfolio</h2>
        <div class="portfolio-item">
            <a href="https://thebeardedman01.itch.io/litter-ladder" style="color: inherit; text-decoration: none;">
                <img src="path-to-project-image.jpg" alt="Litter Ladder">
                <div>
                    <h3>Litter Ladder</h3>
                    <p>Watch for falling trash! Trash sorting simulator for GMTK 2024.</p>
                </div>
            </a>
        </div>
        <div class="portfolio-item">
            <a href="https://thebeardedman01.itch.io/clean-up" style="color: inherit; text-decoration: none;">
                <img src="path-to-project-image.jpg" alt="Clean Up">
                <div>
                    <h3>Clean Up</h3>
                    <p>A game about cleaning up the ocean.</p>
                </div>
            </a>
        </div>
        <div class="portfolio-item">
            <a href="https://gadig.itch.io/fruit-punch" style="color: inherit; text-decoration: none;">
                <img src="path-to-project-image.jpg" alt="Fruit Punch">
                <div>
                    <h3>Fruit Punch</h3>
                    <p>A game about fruit beating the shit out of each other.</p>
                </div>
            </a>
        </div>
        <div class="portfolio-item">
            <a href="https://gadig.itch.io/princess-starshine-vs-the-demons" style="color: inherit; text-decoration: none;">
                <img src="path-to-project-image.jpg" alt="Princess Starshine vs. the Demons of Hell">
                <div>
                    <h3>Princess Starshine vs. the Demons of Hell</h3>
                    <p>Saving hell one glitter at a time.</p>
                </div>
            </a>
        </div>
    </div>

    <div id="experience" class="content">
        <h2>Experience</h2>
        <div class="experience-item">
            <a href="https://gadig.itch.io/" style="color: inherit; text-decoration: none;">
                <img src="path-to-experience-image.jpg" alt="GADIG Game Studio">
                <div>
                    <h3>GADIG Game Studio</h3>
                    <p>Assistant Design Director with experience leading up to 12 developers with about 7 months of experience.</p>
                </div>
            </a>
        </div>
    </div>

    <div id="education" class="content">
        <h2>Education</h2>
        <div class="education-item">
            <h3>George Mason University</h3>
            <p>Studying Computer Game Design with a specialization in Level Design.</p>
        </div>
    </div>

    <div id="about" class="content">
        <h2>About Me</h2>
        <p>Welcome to my portfolio! I am a passionate game designer with a specialization in level design. My journey in game development started with a love for storytelling and creativity, which I now express through designing immersive game worlds.</p>
    </div>

    <div id="contact" class="content">
        <h2>Contact Me</h2>
        <div class="contact-box">
            <form action="#" method="post">
                <input type="text" name="name" placeholder="Your Name" required>
                <input type="email" name="email" placeholder="Your Email" required>
                <textarea name="message" rows="4" placeholder="Your Message" required></textarea>
                <input type="submit" value="Send Message">
            </form>
        </div>
    </div>

</body>
</html>
