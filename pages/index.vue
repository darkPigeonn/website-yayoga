<template>
    <div>
        <nav class="navbar navbar-expand-lg fixed-top">
            <a class="navbar-brand d-flex justify-content-center align-items-center mx-5" href="#">
                <img src="/assets/img/logoYyg.png" alt="Logo" class="logo">
                <div class="company-name d-inline-block mx-4">
                    <span>Yayasan</span><br>            
                    <span>Yohannes Gabriel</span>            
                </div>
            </a>
            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse justify-content-center" id="navbarNav">
                <ul class="navbar-nav">
                    <li class="nav-item"><a class="nav-link" href="#">Beranda</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">Profil</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">Galeri</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">Berita</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">Artikel</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">Unit</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">PPDB</a></li>
                </ul>
            </div>
        </nav>
        <div class="hero-section">
            <img src="/assets/img/template/1600x900.png" alt="Hero Image" class="hero-image">
           
        </div>

        <div class="about-section">
            <div class="container">
                <div class="d-flex justify-content-between align-items-center">
                    <div class="desc">
                        <h3>Selamat datang di Yayasan Yohannes Gabriel</h3>
                        <p>Kami dengan tulus menyambut Anda di tempat di mana pendidikan dan pengembangan potensial menjadi prioritas utama. Melalui berbagai program dan inisiatif kami, kami bertekad untuk memberikan akses pendidikan berkualitas.</p>
                    </div>
                    <div class="image-about">
                        <img src="/assets/img/8.png" alt="About Image" class="img-fluid" />
                    </div>
                </div>
            </div>
        </div>

        <div class="about-section">
            <div class="container">
                <div class="d-flex justify-content-between align-items-center">
                    <div class="image-about2">
                        <img src="/assets/img/13.png" alt="About Image" class="img-fluid"/>
                    </div>
                    <div class="desc">
                        <h3>1925 - Sekarang</h3>
                        <p>Yayasan Yohannes Gabriel berdiri sejak 1925 dengan tujuan utama meningkatkan akses dan kualitas pendidikan untuk semua. Melalui program-programnya, yayasan telah memberikan kontribusi besar dalam menciptakan lingkungan belajar yang inklusif dan mempersiapkan generasi muda untuk masa depan yang cerah dan berdaya saing.</p>
                    </div>
                </div>
            </div>
        </div>

        <div class="video-company">
            <div class="container mt-5">
                <div class="card rounded-custom">
                    <div class="card-header">
                        <span class="card-title">Company Profile</span>
                    </div>
                    <div class="card-body text-center">
                        <button class="btn btn-primary btn-play">
                            <i class="fa fa-play"></i>
                        </button>
                    </div>
                </div>
            </div>
        </div>

        <div class="agenda-section mt-5">
            <div class="container">
                <div class="d-flex justify-content-between align-items-center">
                    <div class="">
                        <p>Kalender Akademik</p>
                    </div>
                    <div class="">
                        <p>Disini Agenda</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>


<style scoped>
@import 'https://pro.fontawesome.com/releases/v5.10.0/css/all.css';
.navbar {
    background: linear-gradient(to bottom, blue, transparent);
    background-color: rgba(0, 0, 0, 0.1); /* Fallback for older browsers */
}

.logo {
    width: 50px;
    height: 50px;
}

.company-name span {
    font-size: 18px;
    font-weight: bold;
}


/* hero section */
.hero-section {
    position: relative;
    height: 100vh;
    overflow: hidden;
}

.hero-image {
    width: 100%;
    height: 100%;
    object-fit: cover; /* Ensures the image covers the whole section */
    position: absolute;
    top: 0;
    left: 0;
    z-index: -1; /* Ensures the image stays behind the content */
}

.hero-content {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    text-align: center;
    color: white;
}

/*about section */
.about-section {
    padding: 50px 0; /* Add some padding for spacing */
}

.desc {
    max-width: 600px; /* Limit the width of the text */
}

.image-about img {
    max-width: 100%; /* Ensure the image scales correctly */
    height: 100vh; /* Maintain aspect ratio */
}
.image-about2 img {
    max-width: 100%; /* Ensure the image scales correctly */
     /* Maintain aspect ratio */
}


/* company profile */
.card {
    border: 1px solid #ddd; /* Optional: border for the card */
    border-radius: 15px; /* Radius for the card */
    overflow: hidden; /* Ensure content does not overflow card */
    position: relative; /* Position relative for absolute positioning inside */
    height: 50vh;
}

.card-header {
    background-color: #f8f9fa; /* Background color for header */
    border-bottom: 1px solid #ddd; /* Border for the header */
    padding: 10px 15px; /* Padding inside header */
    position: absolute; /* Absolute positioning */
    top: 0; /* Position at the top */
    left: 0; /* Position at the left */
    border-radius: 15px 15px 0 0; /* Radius on top corners */
}

.card-title {
    font-weight: bold; /* Bold text */
}

.card-body {
    display: flex; /* Flexbox for centering content */
    align-items: center; /* Center vertically */
    justify-content: center; /* Center horizontally */
    height: 200px; /* Set a fixed height for the card body */
}

.btn-play {
    font-size: 3rem; /* Size of the play button */
    background-color: #007bff; /* Button color */
    color: white; /* Text color */
    border: none; /* Remove border */
    border-radius: 50%; /* Circular button */
    width: 80px; /* Width of the button */
    height: 80px; /* Height of the button */
    display: flex; /* Flexbox for centering icon */
    align-items: center; /* Center icon vertically */
    justify-content: center; /* Center icon horizontally */
}

.btn-play i {
    font-size: 2rem; /* Size of the play icon */
}

</style>