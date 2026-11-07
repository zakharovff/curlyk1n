<html lang="ru" dir="ltr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Curlyk1n - музыкальный коллектив из Москвы, создающий уникальный электронный звук. Слушайте нашу музыку на всех популярных стриминговых платформах.">
    <meta name="keywords" content="Curlyk1n, музыкальная группа, электронная музыка, Ambient, Dubstep, D'n'B, Drum, Bass, Hardcore">
    <meta name="author" content="Curlyk1n">
    <meta property="og:title" content="Curlyk1n - Музыкальный коллектив">
    <meta property="og:description" content="Curlyk1n - музыкальный коллектив из Москвы, создающий уникальный электронный звук">
    <meta property="og:type" content="website">
    
    <title>Curlyk1n - Музыкальный коллектив из Москвы</title>

    <link rel="icon" href="favicon.ico">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.7.2/css/all.min.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;600;700&family=Inter:wght@400;500;600&display=swap" rel="stylesheet">
    
    <style>
        /* Базовые стили и CSS переменные */
        :root {
            --primary-color: #7c3aed;
            --secondary-color: #4f46e5;
            --accent-color: #f472b6;
            --dark-color: #0f0f1a;
            --card-bg: #ffffff;
            --light-color: #f5f4f2;
            --gray-color: #6b7280;
            --text-dark: #1a1a2e;
            --text-light: #f5f4f2;
            --border-color: #e5e7eb;
            --shadow: 0 4px 20px rgba(0, 0, 0, 0.08);
            --shadow-hover: 0 12px 40px rgba(0, 0, 0, 0.14);
            --transition: all 0.25s ease;
            --border-radius: 12px;
            --container-width: 1200px;
        }

        /* Сброс и базовые стили */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: 'Inter', sans-serif;
            line-height: 1.6;
            color: var(--text-dark);
            background-color: var(--light-color);
            overflow-x: hidden;
        }

        h1, h2, h3, h4, h5, h6 {
            font-family: 'Space Grotesk', sans-serif;
            font-weight: 700;
            line-height: 1.3;
            margin-bottom: 1rem;
        }

        h1 {
            font-size: 3rem;
        }

        h2 {
            font-size: 2.4rem;
            text-align: center;
            margin-bottom: 3rem;
            position: relative;
            color: var(--text-dark);
        }

        h2:after {
            content: '';
            position: absolute;
            bottom: -14px;
            left: 50%;
            transform: translateX(-50%);
            width: 48px;
            height: 3px;
            background: var(--primary-color);
            border-radius: 2px;
        }

        p {
            margin-bottom: 1.5rem;
            font-size: 1.05rem;
            color: var(--text-dark);
        }

        a {
            text-decoration: none;
            color: inherit;
            transition: var(--transition);
        }

        ul {
            list-style: none;
        }

        img {
            max-width: 100%;
            height: auto;
            display: block;
        }

        .container {
            width: 100%;
            max-width: var(--container-width);
            margin: 0 auto;
            padding: 0 20px;
        }

        .section {
            padding: 100px 0;
        }

        .btn {
            display: inline-block;
            background: var(--primary-color);
            color: #ffffff;
            padding: 11px 28px;
            border-radius: 8px;
            font-weight: 600;
            font-family: 'Space Grotesk', sans-serif;
            border: none;
            cursor: pointer;
            transition: var(--transition);
            font-size: 0.95rem;
            letter-spacing: 0.01em;
        }

        .btn:hover {
            background: var(--secondary-color);
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(124, 58, 237, 0.35);
            color: #ffffff;
        }

        /* Хедер и навигация */
        header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            background-color: rgba(15, 15, 26, 0.97);
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
            z-index: 1000;
            border-bottom: 1px solid rgba(255, 255, 255, 0.06);
        }

        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
        }

        .logo {
            font-size: 1.6rem;
            font-weight: 700;
            color: white;
            display: flex;
            align-items: center;
            font-family: 'Space Grotesk', sans-serif;
            letter-spacing: -0.02em;
        }

        .logo i {
            color: var(--primary-color);
            margin-right: 10px;
            font-size: 1.4rem;
        }

        .logo span {
            color: #ffffff;
        }

        nav ul {
            display: flex;
            gap: 30px;
        }

        nav a {
            color: rgba(255,255,255,0.75);
            font-weight: 500;
            font-size: 0.95rem;
            position: relative;
            letter-spacing: 0.01em;
        }

        nav a:hover {
            color: #ffffff;
        }

        nav a:after {
            content: '';
            position: absolute;
            bottom: -4px;
            left: 0;
            width: 0;
            height: 2px;
            background: var(--primary-color);
            transition: var(--transition);
            border-radius: 1px;
        }

        nav a:hover:after {
            width: 100%;
        }

        /* Кнопка переключения языка */
        .language-switcher {
            display: flex;
            align-items: center;
            background-color: rgba(255, 255, 255, 0.1);
            border-radius: 50px;
            padding: 5px;
            cursor: pointer;
            margin-left: 20px;
        }

        .language-btn {
            padding: 6px 16px;
            border-radius: 6px;
            font-weight: 600;
            transition: var(--transition);
            background: transparent;
            border: none;
            color: rgba(255,255,255,0.65);
            cursor: pointer;
            font-size: 0.82rem;
            letter-spacing: 0.05em;
            font-family: 'Space Grotesk', sans-serif;
        }

        .language-btn.active {
            background-color: var(--primary-color);
            color: #ffffff;
        }

        .mobile-menu-btn {
            display: none;
            background: none;
            border: none;
            color: white;
            font-size: 1.5rem;
            cursor: pointer;
            margin-left: 20px;
        }

        /* Герой секция - ИСПРАВЛЕНА И ВОССТАНОВЛЕНА */
        .hero {
            position: relative;
            padding: 180px 0 120px;
            background:
                linear-gradient(160deg,
                    rgba(15, 15, 26, 0.82) 0%,
                    rgba(79, 70, 229, 0.75) 50%,
                    rgba(15, 15, 26, 0.88) 100%),
                url('https://images.unsplash.com/photo-1511379938547-c1f69419868d?ixlib=rb-4.0.3&auto=format&fit=crop&w=1470&q=80');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
            color: white;
            text-align: center;
            min-height: 100vh;
            display: flex;
            align-items: center;
            overflow: hidden;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background:
                radial-gradient(ellipse at 20% 50%, rgba(124, 58, 237, 0.18) 0%, transparent 60%),
                radial-gradient(ellipse at 80% 20%, rgba(79, 70, 229, 0.15) 0%, transparent 55%);
            z-index: 1;
        }

        .hero .container {
            position: relative;
            z-index: 2;
            max-width: 800px;
        }

        .hero h1 {
            font-size: 4.8rem;
            margin-bottom: 20px;
            color: #ffffff;
            letter-spacing: -0.03em;
            animation: fadeInUp 0.9s ease-out;
            font-family: 'Space Grotesk', sans-serif;
        }

        .hero p {
            font-size: 1.25rem;
            max-width: 560px;
            margin: 0 auto 44px;
            color: rgba(255, 255, 255, 0.78);
            line-height: 1.7;
            animation: fadeInUp 0.9s ease-out 0.18s both;
        }

        .hero .btn {
            font-size: 1rem;
            padding: 14px 38px;
            animation: fadeInUp 0.9s ease-out 0.35s both;
            position: relative;
            overflow: hidden;
        }

        /* Анимация для героя */
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        /* О группе секция */
        .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 60px;
            align-items: center;
        }

        .about-text {
            font-size: 1.05rem;
        }

        .about-text p {
            color: #374151;
            line-height: 1.75;
        }

        .about-image {
            border-radius: var(--border-radius);
            overflow: hidden;
            box-shadow: var(--shadow);
        }

        .about-image img {
            width: 100%;
            height: 420px;
            object-fit: cover;
            transition: transform 0.4s ease;
        }

        .about-image:hover img {
            transform: scale(1.04);
        }

        /* Музыка секция */
        .music {
            background-color: #f0eef9;
        }

        .platforms-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(270px, 1fr));
            gap: 24px;
        }

        .platform-card {
            background-color: #ffffff;
            border-radius: var(--border-radius);
            overflow: hidden;
            border: 1px solid var(--border-color);
            transition: var(--transition);
            display: flex;
            flex-direction: column;
        }

        .platform-card:hover {
            transform: translateY(-6px);
            box-shadow: var(--shadow-hover);
            border-color: transparent;
        }

        .platform-icon {
            color: white;
            padding: 28px 30px;
            text-align: center;
            font-size: 2.4rem;
            display: flex;
            align-items: center;
            justify-content: center;
            min-height: 100px;
        }

        .platform-content {
            padding: 22px 24px;
            flex: 1;
            display: flex;
            flex-direction: column;
            gap: 14px;
        }

        .platform-content h3 {
            font-size: 1.25rem;
            margin-bottom: 0;
            color: var(--text-dark);
        }

        .platform-content .btn {
            align-self: flex-start;
        }

        /* Контакты секция */
        .contact-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 40px;
            max-width: 600px;
            margin: 0 auto;
        }

        .contact-info {
            background-color: #ffffff;
            padding: 40px;
            border-radius: var(--border-radius);
            border: 1px solid var(--border-color);
        }

        .contact-item {
            display: flex;
            align-items: center;
            margin-bottom: 0;
        }

        .contact-icon {
            background-color: #ede9fe;
            color: var(--primary-color);
            width: 52px;
            height: 52px;
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-right: 18px;
            font-size: 1.3rem;
            flex-shrink: 0;
        }

        .contact-text h4 {
            margin-bottom: 4px;
            font-size: 0.8rem;
            text-transform: uppercase;
            letter-spacing: 0.08em;
            color: var(--gray-color);
            font-weight: 600;
        }

        .contact-text a {
            color: var(--text-dark);
            font-weight: 600;
            font-size: 1rem;
        }

        .contact-text a:hover {
            color: var(--primary-color);
        }

        /* Футер */
        footer {
            background-color: var(--dark-color);
            color: white;
            padding: 60px 0 30px;
            border-top: 1px solid rgba(255,255,255,0.04);
        }

        .footer-content {
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
        }

        .footer-logo {
            font-size: 1.6rem;
            margin-bottom: 16px;
            font-family: 'Space Grotesk', sans-serif;
            font-weight: 700;
            letter-spacing: -0.02em;
            color: #ffffff;
        }

        .footer-logo i {
            color: var(--primary-color);
            margin-right: 8px;
        }

        .footer-content p {
            color: rgba(255,255,255,0.55);
            font-size: 0.95rem;
            margin-bottom: 0;
        }

        .social-links {
            display: flex;
            gap: 20px;
            margin: 30px 0;
        }

        .social-link {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 44px;
            height: 44px;
            border-radius: 10px;
            background-color: rgba(255, 255, 255, 0.08);
            color: rgba(255,255,255,0.75);
            font-size: 1.1rem;
            transition: var(--transition);
            border: 1px solid rgba(255,255,255,0.08);
        }

        .social-link:hover {
            background-color: var(--primary-color);
            color: #ffffff;
            transform: translateY(-3px);
            border-color: transparent;
        }

        .copyright {
            margin-top: 40px;
            padding-top: 20px;
            border-top: 1px solid rgba(255, 255, 255, 0.08);
            width: 100%;
            font-size: 0.85rem;
        }

        .copyright p {
            color: rgba(255, 255, 255, 0.35);
            margin-bottom: 0;
        }

        /* Адаптивность */
        @media (max-width: 992px) {
            h1 {
                font-size: 3rem;
            }
            
            h2 {
                font-size: 2rem;
            }
            
            .hero h1 {
                font-size: 3.2rem;
            }
            
            .about-content {
                grid-template-columns: 1fr;
                gap: 36px;
            }

            .about-image img {
                height: 320px;
            }
            
            .platforms-grid {
                grid-template-columns: repeat(auto-fill, minmax(240px, 1fr));
            }
        }

        @media (max-width: 768px) {
            .header-container {
                flex-wrap: wrap;
            }
            
            .mobile-menu-btn {
                display: block;
                order: 2;
            }
            
            nav {
                width: 100%;
                max-height: 0;
                overflow: hidden;
                transition: max-height 0.5s ease;
                order: 4;
            }
            
            nav.active {
                max-height: 300px;
                margin-top: 20px;
            }
            
            nav ul {
                flex-direction: column;
                gap: 15px;
            }
            
            .language-switcher {
                order: 3;
                margin-left: auto;
            }
            
            .hero {
                padding: 150px 0 80px;
                min-height: 90vh;
                background-attachment: scroll;
            }
            
            .hero h1 {
                font-size: 2.8rem;
            }
            
            .hero p {
                font-size: 1.3rem;
            }
            
            .section {
                padding: 80px 0;
            }
        }

        @media (max-width: 576px) {
            h1 {
                font-size: 2.2rem;
            }
            
            h2 {
                font-size: 1.8rem;
            }
            
            .hero {
                padding: 130px 0 70px;
                background-attachment: scroll;
            }
            
            .hero h1 {
                font-size: 2.6rem;
            }
            
            .hero p {
                font-size: 1rem;
            }
            
            .platforms-grid {
                grid-template-columns: 1fr;
            }
            
            .contact-info {
                padding: 28px 22px;
            }

            .contact-content {
                max-width: 100%;
            }
            
            .header-container {
                justify-content: space-between;
            }
            
            .language-switcher {
                margin-left: 10px;
            }
            
            .language-btn {
                padding: 5px 12px;
                font-size: 0.78rem;
            }
        }
    </style>
</head>
<body>
    <!-- Хедер -->
    <header>
        <div class="container header-container">
            <a href="#" class="logo">
                <i class="fas fa-music"></i>
                <span>Curlyk1n</span>
            </a>
            
            <nav id="mainNav">
                <ul>
                    <li><a href="#about" class="nav-link">О группе</a></li>
                    <li><a href="#music" class="nav-link">Наша музыка</a></li>
                    <li><a href="#contacts" class="nav-link">Контакты</a></li>
                </ul>
            </nav>
            
            <div class="language-switcher" id="languageSwitcher">
                <button class="language-btn active" data-lang="ru">RU</button>
                <button class="language-btn" data-lang="en">EN</button>
            </div>
            
            <button class="mobile-menu-btn" id="mobileMenuBtn">
                <i class="fas fa-bars"></i>
            </button>
        </div>
    </header>

    <!-- Главный контент -->
    <main>
        <!-- Герой секция - ИСПРАВЛЕНА И ВОССТАНОВЛЕНА -->
        <section class="hero">
            <div class="container">
                <h1 id="heroTitle">Curlyk1n</h1>
                <p id="heroSubtitle">Музыкальный коллектив, создающий уникальный электронный звук</p>
                <a href="#music" class="btn" id="listenMusic">Слушать музыку</a>
            </div>
        </section>

        <!-- О группе -->
        <section id="about" class="section">
            <div class="container">
                <h2 id="aboutTitle">О группе</h2>
                <div class="about-content">
                    <div class="about-text">
                        <p id="aboutText1">Curlyk1n — музыкальный коллектив, основанный в 2017 году в Москве. Изначально это была инструментальная группа, основными инструментами являлись баян и фортепиано. Постепенно фокус сместился в сторону электронной музыки.</p>
                        <p id="aboutText2">Группа объединяет в своём творчестве различные оттенки электронной музыки от легкого Ambient до более тяжелых Dubstep и D'n'B, создавая уникальный стиль, который быстро завоевал популярность среди слушателей.</p>
                        <p id="aboutText3">Ранее группа называлась TooToday, затем была переименована в Curlyk1n. За время своего существования Cyrlyk1n выпустили два студийных альбома и несколько успешных синглов. Участники являются призерами различных музыкальных конкурсов и концертов. Наша музыка звучит на крупнейших стриминговых платформах страны и мира.</p>
                    </div>
                    <div class="about-image">
                        <img src="https://images.unsplash.com/photo-1519281682544-5f37c4b14c47?ixlib=rb-4.0.3&auto=format&fit=crop&w=1470&q=80" alt="Группа Curlyk1n в студии" loading="lazy">
                    </div>
                </div>
            </div>
        </section>

        <!-- Наша музыка -->
        <section id="music" class="section music">
            <div class="container">
                <h2 id="musicTitle">Наша музыка</h2>
                <div class="platforms-grid" id="platformsContainer">
                    <!-- Платформы будут загружены через JavaScript -->
                </div>
            </div>
        </section>

        <!-- Контакты -->
        <section id="contacts" class="section">
            <div class="container">
                <h2 id="contactsTitle">Контакты</h2>
                <div class="contact-content">
                    <div class="contact-info">
                        <div class="contact-item">
                            <div class="contact-icon">
                                <i class="fas fa-envelope"></i>
                            </div>
                            <div class="contact-text">
                                <h4 id="emailLabel">Электронная почта</h4>
                                <a href="mailto:tootoday.band@gmail.com">tootoday.band@gmail.com</a>
                            </div>
                        </div>
                   <!--     <div class="contact-item">
                            <div class="contact-icon">
                                <i class="fab fa-telegram"></i>
                            </div>
                            <div class="contact-text">
                                <h4 id="telegramLabel">Telegram канал</h4>
                                <a href="https://t.me/Curlykin" target="_blank" rel="noopener noreferrer">@Curlykin</a>
                            </div> 
                        </div> -->
                    </div>
                </div>
            </div>
        </section>
    </main>

    <!-- Футер -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-logo">
                    <i class="fas fa-music"></i>
                    <span>Curlyk1n</span>
                </div>
                <p id="footerText">Слушайте нашу музыку на всех популярных платформах</p>
                <div class="social-links">
                <!--    <a href="https://t.me/Curlykin" class="social-link" target="_blank" rel="noopener noreferrer" aria-label="Telegram">
                        <i class="fab fa-telegram"></i>
                    </a> -->
                    <a href="https://vk.com/artist/5233716049124375436" class="social-link" target="_blank" rel="noopener noreferrer" aria-label="VKontakte">
                        <i class="fab fa-vk"></i>
                    </a>
                    <a href="https://open.spotify.com/artist/0qLM7oVOVfvIkdBwQnOdO8" class="social-link" target="_blank" rel="noopener noreferrer" aria-label="Spotify">
                        <i class="fab fa-spotify"></i>
                    </a>
                </div>
                <div class="copyright">
                    <p id="copyrightText">© 2023 Curlyk1n. Все права защищены.</p>
                </div>
            </div>
        </div>
    </footer>

    <script>
        // Данные для перевода
        const translations = {
            ru: {
                heroTitle: "Curlyk1n",
                heroSubtitle: "Музыкальный коллектив, создающий уникальный электронный звук",
                listenMusic: "Слушать музыку",
                aboutTitle: "О группе",
                aboutText1: "Curlyk1n — музыкальный коллектив, основанный в 2017 году в Москве. Изначально это была инструментальная группа, основными инструментами являлись баян и фортепиано. Постепенно фокус сместился в сторону электронной музыки.",
                aboutText2: "Группа объединяет в своём творчестве различные оттенки электронной музыки от легкого Ambient до более тяжелых Dubstep и D'n'B, создавая уникальный стиль, который быстро завоевал популярность среди слушателей.",
                aboutText3: "Ранее группа называлась TooToday, затем была переименована в Curlyk1n. За время своего существования Curlyk1n выпустили два студийных альбома и несколько успешных синглов. Участники являются призерами различных музыкальных конкурсов и концертов. Наша музыка звучит на крупнейших стриминговых платформах страны и мира.",
                musicTitle: "Наша музыка",
                contactsTitle: "Контакты",
                emailLabel: "Электронная почта",
                telegramLabel: "Telegram канал",
                footerText: "Слушайте нашу музыку на всех популярных платформах",
                copyrightText: "© 2025 Curlyk1n. Все права защищены.",
                navAbout: "О группе",
                navMusic: "Наша музыка",
                navContacts: "Контакты"
            },
            en: {
                heroTitle: "Curlyk1n",
                heroSubtitle: "Music band creating unique electronic sound",
                listenMusic: "Listen to music",
                aboutTitle: "About Us",
                aboutText1: "Curlyk1n is a music band founded in 2017 in Moscow. Initially, it was an instrumental group with bayan and piano as the main instruments. Gradually, the focus shifted towards electronic music.",
                aboutText2: "The band combines various shades of electronic music from light Ambient to heavier Dubstep and D'n'B, creating a unique style that quickly gained popularity among listeners.",
                aboutText3: "Untill 2026 it was TooToday band and then it was renamed. During its existence, Curlyk1n has released two studio albums and several successful singles. The members are winners of various music competitions and concerts. Our music is available on the largest streaming platforms in the country and worldwide.",
                musicTitle: "Our Music",
                contactsTitle: "Contacts",
                emailLabel: "Email",
                telegramLabel: "Telegram channel",
                footerText: "Listen to our music on all popular platforms",
                copyrightText: "© 2025 Curlyk1n. All rights reserved.",
                navAbout: "About",
                navMusic: "Music",
                navContacts: "Contacts"
            }
        };

        // Данные о стриминговых платформах
        const platforms = [
            {
                name: "Яндекс Музыка",
                nameEn: "Yandex Music",
                icon: "fas fa-music",
                url: "https://music.yandex.com/artist/25201658?utm_medium=copy_link&ref_id=ca7872c1-e376-4cdc-8226-7ad588dd86c2",
                color: "#ffcc00"
            },
            {
                name: "Звук",
                nameEn: "Zvuk",
                icon: "fas fa-headphones",
                url: "https://zvuk.com/artist/214040541",
                color: "#00a2ff"
            },
            {
                name: "ВКонтакте",
                nameEn: "VKontakte",
                icon: "fab fa-vk",
                url: "https://vk.com/artist/5233716049124375436",
                color: "#4c75a3"
            },
            {
                name: "МТС Музыка",
                nameEn: "MTS Music",
                icon: "fas fa-signal",
                url: "https://mts-music-spo.onelink.me/sKFX/vkyuavzp",
                color: "#e30613"
            },
            {
                name: "Одноклассники",
                nameEn: "Odnoklassniki",
                icon: "fab fa-odnoklassniki",
                url: "https://m.ok.ru/music/artist/122909431251668?ysclid=mjhi82rvg6276337956",
                color: "#f7931e"
            },
            {
                name: "Spotify",
                nameEn: "Spotify",
                icon: "fab fa-spotify",
                url: "https://open.spotify.com/artist/0qLM7oVOVfvIkdBwQnOdO8?si=zNlUGOTNTHOY0wKfX6-wcg",
                color: "#1db954"
            },
            {
                name: "Amazon Музыка",
                nameEn: "Amazon Music",
                icon: "fab fa-amazon",
                url: "https://music.amazon.com/artists/B0G9MZ5L1D/tootoday?marketplaceId=ART4WZ8MWBX2Y&musicTerritory=MX&ref=dm_sh_XYOF0r1mrtMbG8e14MlaVzdQn",
                color: "#ff9900"
            },
{
                name: "Apple Музыка",
                nameEn: "Apple Music",
                icon: "fab fa-apple",
                url: "https://music.apple.com/us/artist/tootoday/1866143169",
                color: "#000000"
            },
{
  "name": "Band.Link",
  "nameEn": "Band.Link",
  "icon": "fas fa-link",
  "url": "https://band.link/2WkW9",
  "color": "#3d5afe"
}
        ];

        // Текущий язык
        let currentLanguage = 'ru';

        // DOM элементы
        const languageSwitcher = document.getElementById('languageSwitcher');
        const mobileMenuBtn = document.getElementById('mobileMenuBtn');
        const mainNav = document.getElementById('mainNav');
        const platformsContainer = document.getElementById('platformsContainer');
        const navLinks = document.querySelectorAll('.nav-link');

        // Функция инициализации страницы
        function initPage() {
            // Проверяем сохраненный язык в localStorage
            const savedLanguage = localStorage.getItem('tootoday_language');
            if (savedLanguage && (savedLanguage === 'ru' || savedLanguage === 'en')) {
                currentLanguage = savedLanguage;
                updateLanguageButtons();
            }
            
            // Загружаем платформы
            renderPlatforms();
            
            // Применяем текущий язык
            applyLanguage();
            
            // Настраиваем обработчики событий
            setupEventListeners();
        }

        // Функция отрисовки платформ
        function renderPlatforms() {
            platformsContainer.innerHTML = '';
            
            platforms.forEach(platform => {
                const platformCard = document.createElement('div');
                platformCard.className = 'platform-card';
                
                const platformName = currentLanguage === 'ru' ? platform.name : platform.nameEn;
                const buttonText = currentLanguage === 'ru' ? 'Слушать' : 'Listen';
                
                const bgStyle = platform.color
                    ? `background-color: ${platform.color}`
                    : `background: linear-gradient(to right, var(--primary-color), var(--secondary-color))`;

                platformCard.innerHTML = `
                    <div class="platform-icon" style="${bgStyle}">
                        <i class="${platform.icon}" style="color:#ffffff"></i>
                    </div>
                    <div class="platform-content">
                        <h3>${platformName}</h3>
                        <a href="${platform.url}" target="_blank" rel="noopener noreferrer" class="btn" style="color:#ffffff">
                            ${buttonText}
                        </a>
                    </div>
                `;
                
                platformsContainer.appendChild(platformCard);
            });
        }

        // Функция обновления кнопок языка
        function updateLanguageButtons() {
            const buttons = document.querySelectorAll('.language-btn');
            buttons.forEach(button => {
                button.classList.remove('active');
                if (button.getAttribute('data-lang') === currentLanguage) {
                    button.classList.add('active');
                }
            });
        }

        // Функция применения языка
        function applyLanguage() {
            // Обновляем тексты на странице (безопасно — пропускаем отсутствующие элементы)
            const setText = (id, text) => {
                const el = document.getElementById(id);
                if (el) el.textContent = text;
            };
            setText('heroTitle', translations[currentLanguage].heroTitle);
            setText('heroSubtitle', translations[currentLanguage].heroSubtitle);
            setText('listenMusic', translations[currentLanguage].listenMusic);
            setText('aboutTitle', translations[currentLanguage].aboutTitle);
            setText('aboutText1', translations[currentLanguage].aboutText1);
            setText('aboutText2', translations[currentLanguage].aboutText2);
            setText('aboutText3', translations[currentLanguage].aboutText3);
            setText('musicTitle', translations[currentLanguage].musicTitle);
            setText('contactsTitle', translations[currentLanguage].contactsTitle);
            setText('emailLabel', translations[currentLanguage].emailLabel);
            setText('telegramLabel', translations[currentLanguage].telegramLabel);
            setText('footerText', translations[currentLanguage].footerText);
            setText('copyrightText', translations[currentLanguage].copyrightText);
            
            // Обновляем навигацию
            if (navLinks.length >= 3) {
                navLinks[0].textContent = translations[currentLanguage].navAbout;
                navLinks[1].textContent = translations[currentLanguage].navMusic;
                navLinks[2].textContent = translations[currentLanguage].navContacts;
            }
            
            // Обновляем язык HTML элемента
            document.documentElement.lang = currentLanguage;
            
            // Обновляем кнопки языка
            updateLanguageButtons();
            
            // Перерисовываем платформы
            renderPlatforms();
        }

        // Функция переключения языка
        function switchLanguage(lang) {
            if (lang === currentLanguage) return;
            
            currentLanguage = lang;
            localStorage.setItem('tootoday_language', lang);
            applyLanguage();
        }

        // Настройка обработчиков событий
        function setupEventListeners() {
            // Переключатель языка
            document.querySelectorAll('.language-btn').forEach(button => {
                button.addEventListener('click', function() {
                    const lang = this.getAttribute('data-lang');
                    switchLanguage(lang);
                });
            });
            
            // Мобильное меню
            mobileMenuBtn.addEventListener('click', function() {
                mainNav.classList.toggle('active');
                this.innerHTML = mainNav.classList.contains('active') 
                    ? '<i class="fas fa-times"></i>' 
                    : '<i class="fas fa-bars"></i>';
            });
            
            // Закрытие меню при клике на ссылку
            document.querySelectorAll('.nav-link').forEach(link => {
                link.addEventListener('click', function() {
                    mainNav.classList.remove('active');
                    mobileMenuBtn.innerHTML = '<i class="fas fa-bars"></i>';
                });
            });
            
            // Плавная прокрутка для ссылок
            document.querySelectorAll('a[href^="#"]').forEach(anchor => {
                anchor.addEventListener('click', function(e) {
                    e.preventDefault();
                    
                    const targetId = this.getAttribute('href');
                    if (targetId === '#') return;
                    
                    const targetElement = document.querySelector(targetId);
                    if (targetElement) {
                        window.scrollTo({
                            top: targetElement.offsetTop - 80,
                            behavior: 'smooth'
                        });
                    }
                });
            });
        }

        // Инициализация при загрузке страницы
        document.addEventListener('DOMContentLoaded', initPage);
    </script>


<!-- Yandex.Metrika counter -->
<script type="text/javascript">
    (function(m,e,t,r,i,k,a){
        m[i]=m[i]||function(){(m[i].a=m[i].a||[]).push(arguments)};
        m[i].l=1*new Date();
        for (var j = 0; j < document.scripts.length; j++) {if (document.scripts[j].src === r) { return; }}
        k=e.createElement(t),a=e.getElementsByTagName(t)[0],k.async=1,k.src=r,a.parentNode.insertBefore(k,a)
    })(window, document,'script','https://mc.yandex.ru/metrika/tag.js?id=106071419', 'ym');

    ym(106071419, 'init', {ssr:true, webvisor:true, clickmap:true, ecommerce:"dataLayer", accurateTrackBounce:true, trackLinks:true});
</script>
<noscript><div><img src="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAAAAACH5BAEAAAAALAAAAAABAAEAAAICRAEAOw==" style="position:absolute; left:-9999px;" alt="" /></div></noscript>
<!-- /Yandex.Metrika counter -->


    <!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-C4JTXR5M3S"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'G-C4JTXR5M3S');
</script>

</body>
</html>
