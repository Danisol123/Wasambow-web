<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>WASAMBOW | Reggaetón Comercial - Ibagué, Colombia</title>
    <meta name="description" content="WASAMBOW - Juan Pablo Valencia Parra, artista de Reggaetón Comercial de Ibagué, Colombia. Videos MALAFAMA, PSYCHO y más.">
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;600;900&family=Oswald:wght@500;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Montserrat', sans-serif;
            background: #0a0a0a;
            color: #ffffff;
            overflow-x: hidden;
        }

        /* Navegación */
        nav {
            position: fixed;
            top: 0;
            width: 100%;
            padding: 20px 50px;
            background: rgba(10, 10, 10, 0.95);
            backdrop-filter: blur(10px);
            z-index: 1000;
            display: flex;
            justify-content: space-between;
            align-items: center;
            border-bottom: 1px solid rgba(255, 0, 128, 0.3);
        }

        .logo {
            font-family: 'Oswald', sans-serif;
            font-size: 2rem;
            font-weight: 700;
            color: #ff0080;
            text-transform: uppercase;
            letter-spacing: 5px;
            text-shadow: 0 0 20px rgba(255, 0, 128, 0.5);
        }

        .nav-links {
            display: flex;
            gap: 30px;
            list-style: none;
        }

        .nav-links a {
            color: #ffffff;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s;
            text-transform: uppercase;
            font-size: 0.9rem;
            letter-spacing: 1px;
        }

        .nav-links a:hover {
            color: #ff0080;
            text-shadow: 0 0 10px rgba(255, 0, 128, 0.8);
        }

        /* Hero Section */
        .hero {
            height: 100vh;
            background: linear-gradient(135deg, rgba(0,0,0,0.7), rgba(0,0,0,0.7)), url('https://drive.google.com/uc?export=view&id=14BV771acgrAorIUraISqov9yocdBpJZU');
            background-size: cover;
            background-position: center;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: radial-gradient(circle, rgba(255, 0, 128, 0.15) 0%, transparent 70%);
            animation: pulse 4s ease-in-out infinite;
        }

        @keyframes pulse {
            0%, 100% { transform: scale(1); opacity: 0.5; }
            50% { transform: scale(1.1); opacity: 0.8; }
        }

        .hero-content {
            position: relative;
            z-index: 2;
        }

        h1 {
            font-family: 'Oswald', sans-serif;
            font-size: 6rem;
            font-weight: 900;
            text-transform: uppercase;
            letter-spacing: 15px;
            margin-bottom: 20px;
            background: linear-gradient(45deg, #ff0080, #ff4da6, #ff0080);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            animation: shine 3s ease-in-out infinite;
            text-shadow: 0 0 30px rgba(255, 0, 128, 0.3);
        }

        @keyframes shine {
            0%, 100% { filter: brightness(1); }
            50% { filter: brightness(1.3); }
        }

        .subtitle {
            font-size: 1.5rem;
            color: #888;
            margin-bottom: 10px;
            font-weight: 300;
            letter-spacing: 8px;
            text-transform: uppercase;
        }

        .location {
            font-size: 1.2rem;
            color: #ff0080;
            margin-bottom: 40px;
            font-weight: 600;
            letter-spacing: 3px;
        }

        .cta-button {
            display: inline-block;
            padding: 18px 50px;
            background: linear-gradient(45deg, #ff0080, #cc0066);
            color: #ffffff;
            text-decoration: none;
            font-weight: 700;
            text-transform: uppercase;
            letter-spacing: 3px;
            border-radius: 50px;
            transition: all 0.3s;
            box-shadow: 0 4px 20px rgba(255, 0, 128, 0.4);
            border: 2px solid transparent;
        }

        .cta-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 30px rgba(255, 0, 128, 0.6);
            border-color: #ff4da6;
        }

        /* Video Destacado Section */
        .featured-video {
            padding: 80px 50px;
            background: linear-gradient(180deg, #0a0a0a 0%, #1a0a1a 50%, #0a0a0a 100%);
            text-align: center;
        }

        .featured-badge {
            display: inline-block;
            padding: 8px 20px;
            background: #ff0080;
            color: white;
            font-weight: 700;
            font-size: 0.9rem;
            border-radius: 20px;
            margin-bottom: 20px;
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        .featured-video h2 {
            font-family: 'Oswald', sans-serif;
            font-size: 2.5rem;
            color: #ff0080;
            margin-bottom: 30px;
            text-transform: uppercase;
            letter-spacing: 5px;
        }

        .video-container {
            max-width: 900px;
            margin: 0 auto;
            border-radius: 20px;
            overflow: hidden;
            border: 3px solid #ff0080;
            box-shadow: 0 0 50px rgba(255, 0, 128, 0.3);
        }

        .video-container iframe {
            width: 100%;
            height: 500px;
            border: none;
        }

        /* Galería de Videos */
        .videos-gallery {
            padding: 80px 50px;
            background: #0a0a0a;
        }

        .year-section {
            margin-bottom: 60px;
        }

        .year-title {
            font-family: 'Oswald', sans-serif;
            font-size: 2rem;
            color: #ff0080;
            margin-bottom: 30px;
            text-align: center;
            text-transform: uppercase;
            letter-spacing: 3px;
            position: relative;
            padding-bottom: 15px;
        }

        .year-title::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 3px;
            background: linear-gradient(90deg, transparent, #ff0080, transparent);
        }

        .videos-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 30px;
            max-width: 1200px;
            margin: 0 auto;
        }

        .video-card {
            background: linear-gradient(145deg, #1a1a1a, #0a0a0a);
            border-radius: 20px;
            overflow: hidden;
            border: 1px solid rgba(255, 0, 128, 0.2);
            transition: all 0.3s;
        }

        .video-card:hover {
            transform: scale(1.02);
            border-color: #ff0080;
            box-shadow: 0 15px 40px rgba(255, 0, 128, 0.2);
        }

        .video-card iframe {
            width: 100%;
            height: 200px;
            border: none;
        }

        .video-info {
            padding: 20px;
        }

        .video-number {
            display: inline-block;
            width: 30px;
            height: 30px;
            background: #ff0080;
            color: white;
            border-radius: 50%;
            text-align: center;
            line-height: 30px;
            font-weight: 700;
            margin-bottom: 10px;
            font-size: 0.9rem;
        }

        .video-info h3 {
            color: #ff0080;
            font-family: 'Oswald', sans-serif;
            font-size: 1.2rem;
            margin-bottom: 5px;
        }

        .video-type {
            display: inline-block;
            padding: 4px 12px;
            background: rgba(255, 0, 128, 0.2);
            color: #ff0080;
            font-size: 0.75rem;
            border-radius: 10px;
            margin-bottom: 10px;
            text-transform: uppercase;
            font-weight: 600;
        }

        .video-info p {
            color: #888;
            font-size: 0.85rem;
        }

        /* Música Section */
        .music-section {
            padding: 100px 50px;
            background: #111;
        }

        .section-title {
            font-family: 'Oswald', sans-serif;
            font-size: 3rem;
            text-align: center;
            margin-bottom: 50px;
            color: #ff0080;
            text-transform: uppercase;
            letter-spacing: 5px;
        }

        .music-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 30px;
            max-width: 1200px;
            margin: 0 auto;
        }

        .music-card {
            background: linear-gradient(145deg, #1a1a1a, #0a0a0a);
            border-radius: 20px;
            padding: 30px;
            border: 1px solid rgba(255, 0, 128, 0.2);
            transition: all 0.3s;
            position: relative;
            overflow: hidden;
        }

        .music-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 0, 128, 0.1), transparent);
            transition: left 0.5s;
        }

        .music-card:hover::before {
            left: 100%;
        }

        .music-card:hover {
            transform: translateY(-10px);
            border-color: #ff0080;
            box-shadow: 0 15px 40px rgba(255, 0, 128, 0.2);
        }

        .music-card h3 {
            color: #ff0080;
            margin-bottom: 10px;
            font-size: 1.5rem;
            font-family: 'Oswald', sans-serif;
        }

        .music-card p {
            color: #aaa;
            margin-bottom: 20px;
        }

        .embed-container {
            margin-top: 20px;
            border-radius: 12px;
            overflow: hidden;
            border: 1px solid rgba(255, 0, 128, 0.3);
        }

        /* Bio Section */
        .bio-section {
            padding: 100px 50px;
            background: linear-gradient(135deg, #0a0a0a 0%, #1a0a1a 100%);
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 60px;
            flex-wrap: wrap;
        }

        .bio-image-container {
            position: relative;
        }

        .bio-image {
            width: 400px;
            height: 500px;
            border-radius: 20px;
            overflow: hidden;
            border: 3px solid #ff0080;
            box-shadow: 0 0 40px rgba(255, 0, 128, 0.3);
        }

        .bio-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .bio-content {
            max-width: 500px;
        }

        .bio-content h2 {
            font-family: 'Oswald', sans-serif;
            font-size: 2.5rem;
            color: #ff0080;
            margin-bottom: 20px;
            text-transform: uppercase;
            letter-spacing: 3px;
        }

        .bio-content .real-name {
            color: #888;
            font-size: 1.1rem;
            margin-bottom: 20px;
            font-style: italic;
        }

        .bio-content p {
            line-height: 1.8;
            color: #ccc;
            margin-bottom: 20px;
            font-size: 1.1rem;
        }

        .highlight {
            color: #ff0080;
            font-weight: 600;
        }

        .discography {
            margin: 20px 0;
        }

        .discography h4 {
            color: #ff0080;
            margin-bottom: 15px;
            font-family: 'Oswald', sans-serif;
            font-size: 1.2rem;
        }

        .year-block {
            margin-bottom: 15px;
            padding: 15px;
            background: rgba(255, 0, 128, 0.1);
            border-radius: 10px;
            border-left: 3px solid #ff0080;
        }

        .year-block strong {
            color: #ff0080;
            display: block;
            margin-bottom: 8px;
        }

        .year-block ul {
            list-style: none;
            padding-left: 0;
        }

        .year-block li {
            color: #ccc;
            margin: 5px 0;
            font-size: 0.95rem;
        }

        .year-block li::before {
            content: '🎵 ';
        }

        .location-tag {
            display: inline-block;
            padding: 8px 20px;
            background: rgba(255, 0, 128, 0.2);
            border: 1px solid #ff0080;
            border-radius: 20px;
            color: #ff0080;
            font-weight: 600;
            margin-top: 10px;
        }

        /* Galería de Fotos */
        .gallery-section {
            padding: 100px 50px;
            background: #0a0a0a;
        }

        .gallery-tabs {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-bottom: 40px;
            flex-wrap: wrap;
        }

        .gallery-tab {
            padding: 12px 30px;
            background: transparent;
            border: 2px solid #ff0080;
            color: #ff0080;
            border-radius: 30px;
            cursor: pointer;
            font-weight: 600;
            text-transform: uppercase;
            letter-spacing: 2px;
            transition: all 0.3s;
        }

        .gallery-tab.active, .gallery-tab:hover {
            background: #ff0080;
            color: #0a0a0a;
        }

        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            max-width: 1200px;
            margin: 0 auto;
        }

        .gallery-item {
            position: relative;
            border-radius: 15px;
            overflow: hidden;
            border: 2px solid rgba(255, 0, 128, 0.3);
            transition: all 0.3s;
            aspect-ratio: 4/3;
        }

        .gallery-item:hover {
            transform: scale(1.05);
            border-color: #ff0080;
            box-shadow: 0 10px 30px rgba(255, 0, 128, 0.3);
        }

        .gallery-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .gallery-caption {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            background: linear-gradient(transparent, rgba(0,0,0,0.9));
            padding: 20px;
            color: white;
            font-weight: 600;
        }

        /* Contacto Section */
        .contact-section {
            padding: 100px 50px;
            background: linear-gradient(135deg, #111 0%, #0a0a0a 100%);
            text-align: center;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 30px;
            margin-top: 40px;
            flex-wrap: wrap;
        }

        .social-links a {
            width: 70px;
            height: 70px;
            border: 2px solid #ff0080;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #ff0080;
            text-decoration: none;
            font-weight: 700;
            font-size: 1.2rem;
            transition: all 0.3s;
            background: transparent;
        }

        .social-links a:hover {
            background: #ff0080;
            color: #0a0a0a;
            transform: rotate(360deg) scale(1.1);
            box-shadow: 0 0 30px rgba(255, 0, 128, 0.6);
        }

        .booking-info {
            margin-top: 50px;
            padding: 30px;
            background: rgba(255, 0, 128, 0.1);
            border-radius: 15px;
            border: 1px solid rgba(255, 0, 128, 0.3);
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
        }

        .booking-info h3 {
            color: #ff0080;
            margin-bottom: 15px;
            font-family: 'Oswald', sans-serif;
            font-size: 1.5rem;
        }

        .booking-email {
            font-size: 1.3rem;
            color: #fff;
            font-weight: 600;
            word-break: break-all;
        }

        .booking-email a {
            color: #ff0080;
            text-decoration: none;
            transition: all 0.3s;
        }

        .booking-email a:hover {
            text-shadow: 0 0 10px rgba(255, 0, 128, 0.8);
        }

        .booking-info p {
            color: #888;
            margin-top: 10px;
        }

        /* Footer */
        footer {
            padding: 40px 30px;
            background: #000;
            text-align: center;
            color: #666;
            border-top: 1px solid rgba(255, 0, 128, 0.3);
        }

        footer p {
            margin-bottom: 10px;
        }

        .footer-social {
            color: #ff0080;
            font-weight: 600;
        }

        /* Responsive */
        @media (max-width: 768px) {
            h1 { 
                font-size: 3rem; 
                letter-spacing: 8px; 
            }
            .nav-links { 
                display: none; 
            }
            .hero { 
                padding: 0 20px; 
            }
            .subtitle {
                font-size: 1rem;
                letter-spacing: 4px;
            }
            .location {
                font-size: 1rem;
            }
            .music-section, .bio-section, .contact-section, .featured-video, .videos-gallery, .gallery-section { 
                padding: 60px 20px; 
            }
            .bio-image { 
                width: 100%; 
                max-width: 350px;
                height: 400px; 
            }
            .music-grid, .videos-grid, .gallery-grid {
                grid-template-columns: 1fr;
            }
            .section-title, .year-title {
                font-size: 1.8rem;
            }
            .video-container iframe {
                height: 250px;
            }
            .video-card iframe {
                height: 180px;
            }
            .booking-email {
                font-size: 1rem;
            }
            .gallery-tabs {
                gap: 10px;
            }
            .gallery-tab {
                padding: 8px 20px;
                font-size: 0.8rem;
            }
        }

        /* Menú móvil */
        .mobile-menu {
            display: none;
            color: #ff0080;
            font-size: 1.5rem;
            cursor: pointer;
        }

        @media (max-width: 768px) {
            .mobile-menu {
                display: block;
            }
        }
    </style>
</head>
<body>

    <!-- Navegación -->
    <nav>
        <div class="logo">WASAMBOW</div>
        <ul class="nav-links">
            <li><a href="#inicio">Inicio</a></li>
            <li><a href="#video">Video</a></li>
            <li><a href="#videos">Videos</a></li>
            <li><a href="#musica">Música</a></li>
            <li><a href="#bio">Bio</a></li>
            <li><a href="#galeria">Galería</a></li>
            <li><a href="#contacto">Contacto</a></li>
        </ul>
        <div class="mobile-menu">☰</div>
    </nav>

    <!-- Hero Section -->
    <section id="inicio" class="hero">
        <div class="hero-content">
            <h1>WASAMBOW</h1>
            <p class="subtitle">Reggaetón Comercial • Urban Latino</p>
            <p class="location">📍 Ibagué, Tolima - Colombia</p>
            <a href="#video" class="cta-button">Ver MALAFAMA</a>
        </div>
    </section>

    <!-- Video Destacado Principal - MALAFAMA -->
    <section id="video" class="featured-video">
        <div class="featured-badge">🔥 Último Lanzamiento</div>
        <h2>MALAFAMA – Video Oficial</h2>
        <div class="video-container">
            <iframe src="https://www.youtube.com/embed/koupefFvwxs" 
                    title="WASAMBOW - MALAFAMA (Video Oficial)" 
                    frameborder="0" 
                    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" 
                    allowfullscreen>
            </iframe>
        </div>
    </section>

    <!-- Galería de Videos Completa -->
    <section id="videos" class="videos-gallery">
        
        <!-- Lanzamientos Recientes -->
        <div class="year-section">
            <h2 class="year-title">🎬 Lanzamientos Recientes</h2>
            <div class="videos-grid">
                
                <!-- MALAFAMA -->
                <div class="video-card">
                    <iframe src="https://www.youtube.com/embed/koupefFvwxs" 
                            title="MALAFAMA - Video Oficial" 
                            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
                            allowfullscreen>
                    </iframe>
                    <div class="video-info">
                        <span class="video-number">4</span>
                        <span class="video-type">Video Oficial</span>
                        <h3>MALAFAMA</h3>
                        <p>Lanzamiento más reciente</p>
                    </div>
                </div>

                <!-- PSYCHO -->
                <div class="video-card">
                    <iframe src="https://www.youtube.com/embed/Lh8zq8Cl1o4" 
                            title="PSYCHO - Audio" 
                            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
                            allowfullscreen>
                    </iframe>
                    <div class="video-info">
                        <span class="video-number">3</span>
                        <span class="video-type">Audio / Canción</span>
                        <h3>PSYCHO</h3>
                        <p>Audio oficial en YouTube</p>
                    </div>
                </div>

            </div>
        </div>

        <!-- Lanzamientos 2021 -->
        <div class="year-section">
            <h2 class="year-title">🎬 Lanzamientos 2021</h2>
            <div class="videos-grid">
                
                <!-- Video 2021 - 1 -->
                <div class="video-card">
                    <iframe src="https://www.youtube.com/embed/N0LXcnxPefw" 
                            title="WASAMBOW - Lanzamiento 2021 #1" 
                            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
                            allowfullscreen>
                    </iframe>
                    <div class="video-info">
                        <span class="video-number">1</span>
                        <span class="video-type">2021</span>
                        <h3>Lanzamiento 2021 #1</h3>
                        <p>Primeros pasos de WASAMBOW</p>
                    </div>
                </div>

                <!-- Video 2021 - 2 -->
                <div class="video-card">
                    <iframe src="https://www.youtube.com/embed/W7GWFHlWgU8" 
                            title="WASAMBOW - Lanzamiento 2021 #2" 
                            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
                            allowfullscreen>
                    </iframe>
                    <div class="video-info">
                        <span class="video-number">2</span>
                        <span class="video-type">2021</span>
                        <h3>Lanzamiento 2021 #2</h3>
                        <p>Continuando el legado</p>
                    </div>
                </div>

            </div>
        </div>

    </section>

    <!-- Música Section -->
    <section id="musica" class="music-section">
        <h2 class="section-title">🎵 Escucha en Plataformas</h2>
        <div class="music-grid">
            <div class="music-card">
                <h3>Spotify</h3>
                <p>MALAFAMA, PSYCHO y discografía completa</p>
                <div class="embed-container">
                    <iframe style="border-radius:12px" 
                            src="https://open.spotify.com/embed/artist/2n9Bjg0vxm22Jfaa7Bo6h1?utm_source=generator" 
                            width="100%" height="352" 
                            frameBorder="0" 
                            allowfullscreen="" 
                            allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" 
                            loading="lazy">
                    </iframe>
                </div>
            </div>
            <div class="music-card">
                <h3>YouTube Channel</h3>
                <p>4 videos disponibles</p>
                <div class="embed-container">
                    <a href="https://www.youtube.com/results?search_query=wasambow" target="_blank" style="display: block; padding: 50px; background: #ff0000; color: white; text-decoration: none; border-radius: 12px; font-weight: 700; text-align: center; font-size: 1.2rem;">
                        Ver Canal de YouTube →
                    </a>
                </div>
            </div>
            <div class="music-card">
                <h3>Todas las Plataformas</h3>
                <p>Disponible en todas las plataformas digitales</p>
                <div class="embed-container" style="padding: 30px; text-align: center;">
                    <p style="color: #888; margin-bottom: 20px;">Apple Music • Deezer • Tidal • Amazon Music</p>
                    <a href="https://open.spotify.com/artist/2n9Bjg0vxm22Jfaa7Bo6h1" target="_blank" style="display: inline-block; padding: 15px 30px; background: #1DB954; color: white; text-decoration: none; border-radius: 25px; font-weight: 700; margin: 5px;">
                        Abrir Spotify
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- Biografía -->
    <section id="bio" class="bio-section">
        <div class="bio-image-container">
            <div class="bio-image">
                <img src="https://drive.google.com/uc?export=view&id=1X4DjzIuxnR1XgZdce_70X7dH19JgO9dU" alt="WASAMBOW - Juan Pablo Valencia Parra">
            </div>
        </div>
        <div class="bio-content">
            <h2>La Historia de WASAMBOW</h2>
            <p class="real-name">Juan Pablo Valencia Parra | 21 años</p>
            <p><span class="highlight">WASAMBOW</span> representa la nueva ola del reggaetón comercial desde el corazón de Colombia. Originario de <span class="highlight">Ibagué, Tolima</span>, este joven artista de 21 años lleva la esencia del género urbano latino con un sello único.</p>
            
            <div class="discography">
                <h4>📀 Discografía en Videos</h4>
                <div class="year-block">
                    <strong>2024 - Lanzamientos Recientes</strong>
                    <ul>
                        <li>MALAFAMA – Video Oficial</li>
                        <li>PSYCHO – Audio / Canción</li>
                    </ul>
                </div>
                <div class="year-block">
                    <strong>2021 - Inicios</strong>
                    <ul>
                        <li>Lanzamiento #1 – Video 2021</li>
                        <li>Lanzamiento #2 – Video 2021</li>
                    </ul>
                </div>
            </div>
            
            <p>Con 4 videos en su canal de YouTube y su música disponible en todas las plataformas digitales, WASAMBOW ha logrado posicionar su arte en la escena urbana colombiana.</p>
            <div class="location-tag">🇨🇴 Hecho en Ibagué, Colombia</div>
        </div>
    </section>

    <!-- Galería de Fotos -->
    <section id="galeria" class="gallery-section">
        <h2 class="section-title">📸 Galería</h2>
        
        <div class="gallery-tabs">
            <button class="gallery-tab active" onclick="filterGallery('all')">Todas</button>
            <button class="gallery-tab" onclick="filterGallery('conciertos')">Conciertos</button>
            <button class="gallery-tab" onclick="filterGallery('medios')">Medios</button>
            <button class="gallery-tab" onclick="filterGallery('backstage')">Backstage</button>
        </div>

        <div class="gallery-grid" id="galleryGrid">
            <!-- Foto 1: Concierto -->
            <div class="gallery-item" data-category="conciertos">
                <img src="https://drive.google.com/uc?export=view&id=14BV771acgrAorIUraISqov9yocdBpJZU" alt="WASAMBOW en concierto">
                <div class="gallery-caption">En Vivo</div>
            </div>
            
            <!-- Foto 2: Concierto 2 -->
            <div class="gallery-item" data-category="conciertos">
                <img src="https://drive.google.com/uc?export=view&id=1VP-jqyq-a0yQAncWqRQd5v6KwJGtcWOc" alt="WASAMBOW performance">
                <div class="gallery-caption">Performance</div>
            </div>
            
            <!-- Foto 3: Medios/Radio -->
            <div class="gallery-item" data-category="medios">
                <img src="https://drive.google.com/uc?export=view&id=1YiUDG0sdbHqwqywxzX9QIN8PXiOCppZj" alt="WASAMBOW en medios">
                <div class="gallery-caption">Entrevista</div>
            </div>
            
            <!-- Foto 4: Backstage/Estudio -->
            <div class="gallery-item" data-category="backstage">
                <img src="https://drive.google.com/uc?export=view&id=1tir3ZORyHLrNCe-JHLhr8E9vyrIH182q" alt="WASAMBOW backstage">
                <div class="gallery-caption">Backstage</div>
            </div>
            
            <!-- Foto 5: Presentación -->
            <div class="gallery-item" data-category="conciertos">
                <img src="https://drive.google.com/uc?export=view&id=1t-3tw1Axz1NtAhvG_v8SEOjifKrnsYLg" alt="WASAMBOW show">
                <div class="gallery-caption">Show en Vivo</div>
            </div>
            
            <!-- Foto 6: Extra (usamos la primera como extra) -->
            <div class="gallery-item" data-category="backstage">
                <img src="https://drive.google.com/uc?export=view&id=1X4DjzIuxnR1XgZdce_70X7dH19JgO9dU" alt="WASAMBOW portrait">
                <div class="gallery-caption">Sesión de Fotos</div>
            </div>
        </div>
    </section>

    <!-- Contacto -->
    <section id="contacto" class="contact-section">
        <h2 class="section-title">📱 Conecta con WASAMBOW</h2>
        <div class="social-links">
            <a href="https://instagram.com/xwasamboux" target="_blank" title="Instagram">IG</a>
            <a href="https://youtube.com/@wasambow" target="_blank" title="YouTube">YT</a>
            <a href="https://tiktok.com/@wasambow" target="_blank" title="TikTok">TT</a>
            <a href="https://open.spotify.com/artist/2n9Bjg0vxm22Jfaa7Bo6h1" target="_blank" title="Spotify">SP</a>
            <a href="#" target="_blank" title="Twitter/X">X</a>
        </div>
        
        <div class="booking-info">
            <h3>📧 Booking & Contacto</h3>
            <p class="booking-email">
                <a href="mailto:juanpablovalenciaparra7@gmail.com">juanpablovalenciaparra7@gmail.com</a>
            </p>
            <p>Ibagué, Colombia • Booking • Prensa • Colaboraciones • Eventos</p>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2024 WASAMBOW. Todos los derechos reservados.</p>
        <p class="footer-social">Juan Pablo Valencia Parra • @xwasamboux • Ibagué, Colombia</p>
        <p style="color: #444; font-size: 0.9rem; margin-top: 10px;">4 Videos en YouTube • Desde 2021</p>
    </footer>

    <script>
        // Smooth scroll para navegación
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });

        // Animación al scroll
        const observerOptions = {
            threshold: 0.1,
            rootMargin: "0px 0px -50px 0px"
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.opacity = '1';
                    entry.target.style.transform = 'translateY(0)';
                }
            });
        }, observerOptions);

        // Seleccionar elementos para animar
        const animatedElements = document.querySelectorAll('.music-card, .bio-content, .video-container, .booking-info, .video-card, .year-section, .gallery-item');
        
        animatedElements.forEach((el) => {
            el.style.opacity = '0';
            el.style.transform = 'translateY(30px)';
            el.style.transition = 'all 0.6s ease-out';
            observer.observe(el);
        });

        // Efecto de navbar al scroll
        let lastScroll = 0;
        window.addEventListener('scroll', () => {
            const currentScroll = window.pageYOffset;
            const nav = document.querySelector('nav');
            
            if (currentScroll > 100) {
                nav.style.background = 'rgba(10, 10, 10, 0.98)';
            } else {
                nav.style.background = 'rgba(10, 10, 10, 0.95)';
            }
            
            lastScroll = currentScroll;
        });

        // Filtro de galería
        function filterGallery(category) {
            const items = document.querySelectorAll('.gallery-item');
            const tabs = document.querySelectorAll('.gallery-tab');
            
            // Actualizar tabs activos
            tabs.forEach(tab => {
                tab.classList.remove('active');
                if (tab.textContent.toLowerCase().includes(category) || (category === 'all' && tab.textContent === 'Todas')) {
                    tab.classList.add('active');
                }
            });
            
            // Filtrar items
            items.forEach(item => {
                if (category === 'all' || item.dataset.category === category) {
                    item.style.display = 'block';
                    setTimeout(() => {
                        item.style.opacity = '1';
                        item.style.transform = 'scale(1)';
                    }, 10);
                } else {
                    item.style.opacity = '0';
                    item.style.transform = 'scale(0.8)';
                    setTimeout(() => {
                        item.style.display = 'none';
                    }, 300);
                }
            });
        }
    </script>

</body>
</html>
