<!-- index.html (Page 1) -->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dian's Web</title>
    <link href="https://fonts.googleapis.com/css2?family=Darumadrop+One&family=Outfit:wght@400;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="styles.css">
    <script src="script.js" defer></script>
</head>
<body>
    <div class="header">Dian's Web</div>
    <img src="cover-image.jpeg" alt="Cover Image" class="cover">
    <div class="section-bar">
        <img src="profile.jpeg" alt="Profile Picture">
        <p>Halo-halo min-na!! 😼<br>
            Namaku <strong>Dian Wulandari</strong>, yang artinya <strong>Pelita yang bersinar seperti bulan penuh</strong>. Yoroshiku ne~! 💖</p>
    </div>
    <div class="content">
        <p><strong>Likes!!</strong><br>
            Ungu dan biru, kucing, mie ayam, main game, menulis, menggambar, membaca, menonton anime dan film, romance, angst
        </p>
        <img src="stiker-wawan-1.png" alt="Icon" id="wawan-icon">
        <p><strong>Dislikes!!</strong><br>
            Ketidakadilan, orang yang berisik dan kasar, extreme gore
        </p>
    </div>
    <div class="skills">
        <h2>My Skills</h2>
        <img src="ibis-paint.png" alt="Skill 1">
        <img src="alight-motion.png" alt="Skill 2">
    </div>
    <div class="navigation">
        <div class="dots">● ● ● ● ●</div>
        <div class="next"><a href="hobbies.html"><strong>Next Page</strong></a></div>
    </div>
    <div class="copyright">
        <p>&copy; 2025 Dian Wulandari. All rights reserved.</p>
    </div>    
</body>
</html>

<!-- hobbies.html (Page 2) -->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Hobbies</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="hobbies-container">
        <div class="hobbies-header"><h2>My hobbies</h2></div>
        <div class="hobbies-section">
            <div>
                <img src="wawan.jpeg" alt="Hobby 1">
                <p>Bermain Genshin Impact adalah hiburan yang seru bagiku. Karakter kesayanganku adalah Wanderer (alias Wawan)! Dia keren dan tamvan!😆✨</p>
            </div>
            <div>
                <img src="86-anime.jpeg" alt="Hobby 2">
                <p>Aku suka banget nonton anime, dan salah satu anime yang menurutku keren adalah 86! Ceritanya dalam, penuh emosi, dan hubungan Shin & Lena bikin baper!🥺</p>
            </div>
            <div>
                <img src="solo-leveling.jpeg" alt="Hobby 3">
                <p>Membaca manhwa adalah salah satu hobiku! Favoritku Solo Leveling, kisah Sung Jin-Woo yang berkembang dari terlemah menjadi terkuat. Sekarang sudah diadaptasi menjadi anime!</p>
            </div>
        </div>
    </div>
    <div class="gallery-container">
        <div class="gallery-header"><h2>Gallery Corner</h2></div>
        <div class="gallery">
            <img src="genshin-2.png" alt="Gallery 1">
            <img src="me-1.jpeg" alt="Gallery 2">
            <img src="friend-1.jpeg" alt="Gallery 3">
            <img src="friend-2.jpeg" alt="Gallery 4">
            <img src="friend.jpeg" alt="Gallery 5">
        </div>
    </div>
    <div class="navigation">
        <div class="dots">● ● ● ● ●</div>
        <div class="prev"><a href="index.html"><strong>Previous Page</strong></a></div>
    </div>
    <div class="copyright">
        <p>&copy; 2025 Dian Wulandari. All rights reserved.</p>
    </div>    
</body>
</html>

<!-- styles.css -->
/* Gabungan CSS dari kedua halaman */
body {
    background-color: #FFF2F2;
    font-family: Arial, sans-serif;
    text-align: center;
    margin: 0;
    padding: 0;
}
.header, .hobbies-container, .gallery-container, .skills, .copyright {
    background-color: #A9B5DF;
    color: #2D336B;
    padding: 10px;
    border-radius: 10px;
    margin: 20px;
}
.navigation {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px;
}
.dots {
    flex-grow: 1;
    text-align: left;
    color: #7886C7;
}
.next, .prev {
    background-color: #7886C7;
    padding: 10px;
    border-radius: 10px;
    transition: transform 0.3s;
}
.next a, .prev a {
    text-decoration: none;
    color: white;
    font-size: 16px;
    font-family: 'Outfit', sans-serif;
}

<!-- script.js -->
document.addEventListener("DOMContentLoaded", function() {
    let iconImg = document.getElementById("wawan-icon");
    if (iconImg) {
        iconImg.addEventListener('mouseenter', function() {
            this.src = 'stiker-wawan-2.png';
        });
        iconImg.addEventListener('mouseleave', function() {
            this.src = 'stiker-wawan-1.png';
        });
    }
});
