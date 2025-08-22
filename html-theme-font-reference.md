<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="./assets/css/index.css">
    <script src="./assets/js/index.js" defer></script>
    <title>DJ Dino Bravo</title>
</head>
<body>
    <div id="hero">
        <img src="./assets/images/logo.svg" alt="Logo">
        <p>Yo Momma's Fav DJ</p>
        <nav>
            <ul>
                <li>
                    <a href="#about">About</a>
                </li>
                <li>
                    <a href="#music">Music</a>
                </li>
                <li>
                    <a href="#school">School</a>
                </li>
                <li>
                    <a href="#contact">Bookings</a>
                </li>
            </ul>
        </nav>
        <div class="social__links">
            <a href="https://www.facebook.com/djdinobravo/">
                <img src="./assets/images/hero_fb.svg" alt="Facebook">
            </a>
            <a href="https://www.youtube.com/@djdinobravo">
                <img src="./assets/images/hero_tube.svg" alt="YouTube">
            </a>
            <a href="https://open.spotify.com/artist/6ph0EJhjqYJzgjKZk6dgCG">
                <img src="./assets/images/hero_spot.svg" alt="Spotify">
            </a>
            <a href="https://soundcloud.com/djdinobravo">
                <img src="./assets/images/hero_sc.svg" alt="SoundCLoud">
            </a>
            <a href="https://www.instagram.com/djdinobravo/?hl=en">
                <img src="./assets/images/hero_insta.svg" alt="Instagram">
            </a>
            <a href="">
                <img src="./assets/images/hero_whats.svg" alt="WhatsApp">
            </a>
        </div>
    </div>
    <div id="about">
        <div class="title">
            <h1>
                About Me 
            </h1>
        </div>
        <img src="./assets/images/banner.png" alt="Banner image">
        <p>
            Music has forever been ingrained in my soul and my entry into the music world goes back to the days of my youth where I enjoyed break-dancing 
            and rapping.
        </p>
        <p>
            I remain ever faithful to my indigenous sounds but have continued to reinvent myself over the years. The result of this is the great-sounding 
            rhythms that have, and continue to, set many a dance floor alight! My ongoing evolution proves that I am able to constantly adapt to the latest 
            music trends, sounds and techniques.
        </p>
    </div>
    <div id="music">
        <div class="title">
            <h1>
                Music
            </h1>
            <p>
                fresh from the studio
            </p>
        </div>
        <iframe style="border-radius:12px" src="https://open.spotify.com/embed/album/0qwaNAzbJ2cjQ8JEcxGacg?utm_source=generator" width="100%" height="352" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>

    </div>
    <div id="school">
        <h1>
            School
        </h1>
        <div class="desc">
            <img src="./assets/images/school.jpg" alt="School Logo">
            <p>
                Almost 10 years ago I embarked on a journey to start sharing my talents with the next generation of open minded DJs that want to take their 
                journey to the next level. I started the DJ school to help others and guide them to achieve their full potential in this DJ game.
            </p>
        </div>
        <div class="carousel">
            <div class="slides">
              <img src="./assets/images/gallery_1.jpg" alt="Slide 1">
              <img src="./assets/images/gallery_2.jpg" alt="Slide 2">
              <img src="./assets/images/gallery_3.jpg" alt="Slide 3">
              <img src="./assets/images/gallery_4.jpg" alt="Slide 4">
            </div>
            <button class="prev">&#10094;</button>
            <button class="next">&#10095;</button>
            <div class="dots"></div>
          </div>
    </div>
    <div id="contact">
        <h1>Bookings / Contact</h1>
        <p>Feel free to book me for a gig or inquire about my school.</p>
        <form action="" class="stylish-form">
            <div class="input-group">
              <label for="name">Name:</label>
              <input type="text" id="name" name="name" required>
            </div>
          
            <div class="input-group">
              <label for="email">Email:</label>
              <input type="email" id="email" name="email" required>
            </div>
          
            <div class="input-group">
              <label for="type">Type:</label>
              <select id="type" name="type" required>
                <option value="">Select one...</option>
                <option value="gig">Gig</option>
                <option value="school">School</option>
              </select>
            </div>
          
            <div class="input-group">
              <label for="message">Message:</label>
              <textarea id="message" name="message" rows="5" required></textarea>
            </div>
          
            <button type="submit">Submit</button>
          </form>          
    </div>
    <footer>
        <div class="container">
            <div class="logo__portion">
                <img src="./assets/images/logo.svg" alt="logo">
            </div>
            <p>© DJ Dino Bravo — All rights mixed & mastered.</p>
        </div>
    </footer>
</body>
</html>