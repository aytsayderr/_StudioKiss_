<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=yes, viewport-fit=cover">
    <title>StudioKiss | Организация мероприятий</title>
    <!-- Яндекс.Метрика -->
    <script>
        (function(m,e,t,r,i,k,a){
            m[i]=m[i]||function(){(m[i].a=m[i].a||[]).push(arguments)};
            m[i].l=1*new Date();
            k=e.createElement(t),a=e.getElementsByTagName(t)[0],k.async=1,k.src=r,a.parentNode.insertBefore(k,a)
        })(window, document, "script", "https://mc.yandex.ru/metrika/tag.js", "ym");
        ym(98765432, "init", {
            clickmap:true,
            trackLinks:true,
            accurateTrackBounce:true,
            webvisor:true
        });
    </script>
    <!-- SEO -->
    <meta name="description" content="StudioKiss — организация праздников, мероприятий, свадеб, корпоративов. Оформление, кейтеринг, фотозоны. Закажите мероприятие онлайн.">
    <meta name="keywords" content="мероприятие, организация праздников, студия интерьера, галерея работ, заказать мероприятие">
    <meta name="author" content="StudioKiss">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            -webkit-tap-highlight-color: transparent;
        }

        body {
            font-family: system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', sans-serif;
            background: #f5f9fe;
            color: #1a2c3e;
            line-height: 1.45;
            overflow-x: hidden;
        }

        .container {
            width: 100%;
            max-width: 1280px;
            margin: 0 auto;
            padding: 0 16px;
        }

        /* Мобильная оптимизация header */
        header {
            background: #ffffff;
            border-bottom: 2px solid #cbdff2;
            padding: 16px 0;
            position: sticky;
            top: 0;
            z-index: 100;
            backdrop-filter: blur(0px);
        }

        .header-inner {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            align-items: center;
            gap: 12px;
        }

        .logo h1 {
            font-size: 1.5rem;
            font-weight: 700;
            letter-spacing: -0.3px;
            color: #2c5a7a;
        }

        .logo p {
            font-size: 0.7rem;
            color: #567d9e;
        }

        .contact-info {
            text-align: right;
            font-size: 0.8rem;
        }

        .contact-info div:first-child {
            font-weight: 600;
            font-size: 0.9rem;
        }

        .contact-info a {
            color: #2c5a7a;
            text-decoration: none;
            font-weight: 500;
        }

        .social-icons {
            display: flex;
            gap: 8px;
        }

        .social-icons a {
            text-decoration: none;
            font-weight: bold;
            color: #2c5a7a;
            border: 1px solid #cbdff2;
            padding: 6px 12px;
            display: inline-block;
            font-size: 0.75rem;
            border-radius: 6px;
            transition: all 0.2s;
        }

        /* Мобильное меню - гамбургер */
        .main-nav {
            background: #e9f0f8;
            border-bottom: 1px solid #cbdff2;
            position: sticky;
            top: 74px;
            z-index: 99;
        }

        .nav-toggle {
            display: none;
            background: none;
            border: none;
            font-size: 1.8rem;
            cursor: pointer;
            padding: 8px 12px;
            color: #1f4e6e;
        }

        .nav-links {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            list-style: none;
            padding: 12px 0;
            transition: all 0.3s ease;
        }

        .nav-links a {
            text-decoration: none;
            font-weight: 500;
            color: #1f4e6e;
            font-size: 0.95rem;
            cursor: pointer;
            padding: 6px 0;
            display: inline-block;
            white-space: nowrap;
        }

        .nav-links a:active {
            opacity: 0.7;
        }

        section {
            margin: 32px 0;
        }

        .section-title {
            font-size: 1.5rem;
            font-weight: 600;
            border-left: 5px solid #6c9ebf;
            padding-left: 14px;
            margin-bottom: 24px;
            color: #1f4e6e;
        }

        .order-form-card {
            background: white;
            padding: 20px;
            border: 1px solid #cbdff2;
            border-radius: 12px;
        }

        .form-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 14px;
        }

        input, select, button {
            padding: 14px 16px;
            border: 1px solid #cbdff2;
            font-size: 1rem;
            font-family: inherit;
            background: white;
            border-radius: 10px;
            -webkit-appearance: none;
            appearance: none;
        }

        button {
            background: #2c5a7a;
            color: white;
            font-weight: 600;
            border: none;
            cursor: pointer;
            transition: all 0.2s;
            padding: 14px;
        }

        button:active {
            transform: scale(0.98);
            background: #1f415c;
        }

        /* Слайдер с сенсорной поддержкой */
        .gallery-slider {
            position: relative;
            background: #eef3fc;
            border: 1px solid #cbdff2;
            overflow: hidden;
            border-radius: 16px;
            touch-action: pan-y pinch-zoom;
        }

        .slides {
            display: flex;
            transition: transform 0.4s cubic-bezier(0.2, 0.9, 0.4, 1.1);
            cursor: grab;
        }

        .slides:active {
            cursor: grabbing;
        }

        .slide {
            min-width: 100%;
            height: 280px;
            background-size: cover;
            background-position: center;
            display: flex;
            align-items: flex-end;
            justify-content: flex-start;
            padding: 20px;
            color: white;
            text-shadow: 0 1px 3px rgba(0,0,0,0.3);
            font-weight: bold;
            font-size: 1.2rem;
        }

        .slider-buttons {
            position: absolute;
            bottom: 12px;
            right: 12px;
            display: flex;
            gap: 8px;
        }

        .slider-buttons button {
            background: rgba(44,90,122,0.85);
            backdrop-filter: blur(4px);
            border: none;
            color: white;
            font-size: 1rem;
            padding: 8px 16px;
            border-radius: 30px;
            min-width: 44px;
            min-height: 44px;
        }

        /* Сетки для мобильных */
        .services-grid, .interior-grid, .services-catalog {
            display: grid;
            grid-template-columns: 1fr;
            gap: 20px;
        }

        .service-item, .interior-item {
            background: white;
            border: 1px solid #cbdff2;
            padding: 18px;
            border-radius: 16px;
            transition: transform 0.2s ease, box-shadow 0.2s ease;
        }

        .service-item:active, .interior-item:active {
            transform: scale(0.99);
        }

        .service-photo {
            width: 100%;
            height: 180px;
            object-fit: cover;
            border-radius: 12px;
            margin-bottom: 14px;
            background: #eef3fc;
        }

        .price {
            font-weight: 700;
            color: #2c5a7a;
            margin: 8px 0;
            font-size: 1.1rem;
        }

        .btn-more {
            display: inline-block;
            margin-top: 10px;
            background: none;
            border: 1px solid #2c5a7a;
            color: #2c5a7a;
            padding: 8px 20px;
            text-decoration: none;
            font-weight: 500;
            cursor: pointer;
            border-radius: 30px;
            transition: all 0.2s;
            text-align: center;
        }

        .btn-more:active {
            background: #e2edf9;
            transform: scale(0.96);
        }

        footer {
            background: #e0ecf5;
            border-top: 2px solid #cbdff2;
            padding: 28px 0;
            margin-top: 32px;
        }

        .footer-inner {
            display: flex;
            flex-direction: column;
            gap: 24px;
        }

        .footer-menu a {
            display: block;
            margin-bottom: 8px;
            text-decoration: none;
            color: #1f4e6e;
            cursor: pointer;
            padding: 6px 0;
        }

        .footer-social a {
            margin-right: 16px;
            text-decoration: none;
            font-weight: 500;
            display: inline-block;
            padding: 6px 0;
        }

        hr {
            border-color: #cbdff2;
            margin: 16px 0;
        }

        .page-card {
            background: white;
            border: 1px solid #cbdff2;
            padding: 20px;
            margin-bottom: 24px;
            border-radius: 20px;
        }

        .about-flex {
            display: flex;
            flex-direction: column;
            gap: 20px;
            align-items: center;
        }

        .about-img {
            width: 100%;
            background: #cbdff2;
            min-height: 200px;
            background-size: cover;
            background-position: center;
            border-radius: 16px;
        }

        .filters {
            display: flex;
            gap: 10px;
            margin-bottom: 24px;
            flex-wrap: wrap;
            overflow-x: auto;
            padding-bottom: 4px;
            -webkit-overflow-scrolling: touch;
        }

        .filter-btn {
            background: #eef3fc;
            border: 1px solid #cbdff2;
            padding: 10px 18px;
            cursor: pointer;
            border-radius: 40px;
            transition: all 0.2s;
            font-size: 0.9rem;
            white-space: nowrap;
            flex-shrink: 0;
        }

        .filter-btn.active {
            background: #2c5a7a;
            color: white;
            border-color: #2c5a7a;
        }

        .pagination {
            display: flex;
            justify-content: center;
            gap: 10px;
            flex-wrap: wrap;
            margin-top: 20px;
        }

        .pagination button {
            background: white;
            border: 1px solid #cbdff2;
            color: #1f4e6e;
            cursor: pointer;
            padding: 10px 16px;
            border-radius: 40px;
            min-width: 44px;
        }

        .pagination button.active-page {
            background: #2c5a7a;
            color: white;
        }

        /* Баннер-ссылки */
        .quick-links {
            display: flex;
            gap: 12px;
            flex-wrap: wrap;
            justify-content: center;
        }
        .quick-links .btn-more {
            background: #fff;
            flex: 1;
            min-width: 100px;
            text-align: center;
        }

        /* Адаптация для планшетов */
        @media (min-width: 640px) {
            .container {
                padding: 0 24px;
            }
            .services-grid, .interior-grid, .services-catalog {
                grid-template-columns: repeat(2, 1fr);
            }
            .footer-inner {
                flex-direction: row;
                justify-content: space-between;
            }
            .about-flex {
                flex-direction: row;
            }
            .form-grid {
                grid-template-columns: repeat(2, 1fr);
            }
            .slide {
                height: 360px;
            }
        }

        @media (min-width: 1024px) {
            .services-grid, .interior-grid, .services-catalog {
                grid-template-columns: repeat(3, 1fr);
            }
            .form-grid {
                grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
            }
            .nav-toggle {
                display: none;
            }
            .nav-links {
                display: flex !important;
            }
        }

        /* Мобильное меню (по умолчанию показано, для маленьких экранов сворачиваем) */
        @media (max-width: 768px) {
            .main-nav {
                position: relative;
                top: 0;
            }
            .nav-toggle {
                display: block;
                width: 100%;
                text-align: left;
                background: #e9f0f8;
                border: none;
                padding: 12px 16px;
                font-size: 1.3rem;
                font-weight: 600;
                color: #1f4e6e;
                border-bottom: 1px solid #cbdff2;
            }
            .nav-links {
                display: none;
                flex-direction: column;
                gap: 0;
                padding: 0;
            }
            .nav-links.show {
                display: flex;
            }
            .nav-links li {
                border-bottom: 1px solid #cbdff2;
            }
            .nav-links a {
                display: block;
                padding: 14px 16px;
                white-space: normal;
            }
            .header-inner {
                flex-direction: row;
                flex-wrap: nowrap;
                justify-content: space-between;
            }
            .contact-info {
                font-size: 0.7rem;
            }
            .logo h1 {
                font-size: 1.2rem;
            }
            .logo p {
                display: none;
            }
            .social-icons a {
                padding: 4px 8px;
                font-size: 0.7rem;
            }
        }

        /* Улучшение touch-целей */
        button, a, .filter-btn, .btn-more, .pagination button {
            touch-action: manipulation;
        }

        /* Карта адаптив */
        iframe {
            width: 100%;
            height: 200px;
            border-radius: 12px;
        }
        
        @media (min-width: 640px) {
            iframe {
                height: 250px;
            }
        }
    </style>
</head>
<body>
<header>
    <div class="container header-inner">
        <div class="logo">
            <h1>StudioKiss</h1>
            <p>дизайн событий и интерьерные студии</p>
        </div>
        <div class="contact-info">
            <div>+7 (812) 345-67-89</div>
            <div><a href="mailto:hello@studiokiss.ru">hello@studiokiss.ru</a></div>
        </div>
        <div class="social-icons">
            <a href="#">VK</a>
            <a href="#">Max</a>
        </div>
    </div>
</header>

<div class="main-nav">
    <button class="nav-toggle" id="navToggle" aria-label="Меню">☰ Меню</button>
    <div class="container" style="padding: 0;">
        <ul class="nav-links" id="mainNav">
            <li><a data-page="home">Главная</a></li>
            <li><a data-page="about">О нас</a></li>
            <li><a data-page="gallery">Галерея работ</a></li>
            <li><a data-page="servicesPage">Наши услуги</a></li>
            <li><a data-page="interiors">Интерьерные студии</a></li>
            <li><a data-page="contacts">Контакты</a></li>
            <li><a data-page="orderQuick">Заказать мероприятие</a></li>
        </ul>
    </div>
</div>

<main class="container" id="appRoot"></main>

<footer>
    <div class="container footer-inner">
        <div class="footer-menu">
            <strong>Меню</strong>
            <a data-page="home">Главная</a>
            <a data-page="about">О нас</a>
            <a data-page="servicesPage">Услуги</a>
            <a data-page="contacts">Контакты</a>
        </div>
        <div>
            <strong>Реквизиты</strong><br>
            ООО «Студио Кисс»<br>
            ИНН 7842156789, КПП 784201001<br>
            Санкт-Петербург, Российский проспект 10
        </div>
        <div class="footer-social">
            <strong>Соцсети</strong><br>
            <a href="#">VK</a> <a href="#">Max</a>
        </div>
    </div>
    <div class="container" style="text-align:center; font-size:0.7rem; margin-top:20px;">
        © StudioKiss 2026 — Организация мероприятий и дизайн-студия
    </div>
</footer>

<script>
    // Все пути к изображениям с префиксом "image/"
    const galleryImages = [
        "image/vecher.jpg",
        "image/svadiba.jpg",
        "image/korparat.jpg"
    ];
    
    const interiorStudios = [
        { 
            title: "Loft Студия", 
            desc: "Просторный loft с панорамными окнами, высокие потолки, industrial стиль", 
            price: "аренда от 4 000 ₽/час", 
            features: "120 м², до 50 гостей",
            image: "image/loft.jpeg"
        },
        { 
            title: "Белая студия", 
            desc: "Светлая фотостудия с профессиональным оборудованием для мероприятий", 
            price: "от 3 500 ₽/час", 
            features: "80 м², до 30 гостей",
            image: "image/white.jpg"
        },
        { 
            title: "Премиум зал", 
            desc: "Зеркала, гримерки, профессиональный свет, звуковое оборудование", 
            price: "от 8 000 ₽/час", 
            features: "200 м², до 120 гостей",
            image: "image/premium.jpg"
        },
        { 
            title: "Садовый павильон", 
            desc: "Уютное пространство с выходом в зимний сад", 
            price: "от 5 500 ₽/час", 
            features: "95 м², до 60 гостей",
            image: "image/sad.jpeg"
        }
    ];

    const allServices = [
        { id:1, name:"Свадебное оформление", desc:"Полное оформление зала, цветы, арки", price:"от 45 000 ₽", category:"swd", photo:"image/svadiba.jpg" },
        { id:2, name:"Корпоратив", desc:"Ведущий, кейтеринг, фотозона", price:"от 70 000 ₽", category:"corp", photo:"image/korparat.jpg" },
        { id:3, name:"Детский праздник", desc:"Аниматоры, шоу мыльных пузырей", price:"от 25 000 ₽", category:"kids", photo:"image/deti.jpg" },
        { id:4, name:"Фуршет/банкет", desc:"Организация питания и сервировка", price:"от 30 000 ₽", category:"corp", photo:"image/furshet.jpg" },
        { id:5, name:"Тимбилдинг", desc:"Командные игры на природе", price:"от 50 000 ₽", category:"corp", photo:"image/timbilding.jpeg" },
        { id:6, name:"Юбилей", desc:"Шоу программа, декор", price:"от 55 000 ₽", category:"swd", photo:"image/ubiley.webp" }
    ];

    let currentPage = "home";
    let currentServiceFilter = "all";
    let currentServicesPage = 1;
    const perPage = 3;
    const app = document.getElementById('appRoot');
    let touchStartX = 0;
    let touchEndX = 0;

    function render() {
        if (currentPage === "home") renderHome();
        else if (currentPage === "about") renderAbout();
        else if (currentPage === "gallery") renderGalleryFull();
        else if (currentPage === "servicesPage") renderServicesCatalog();
        else if (currentPage === "interiors") renderInteriorsFull();
        else if (currentPage === "contacts") renderContacts();
        else if (currentPage === "orderQuick") renderOrderFormOnly();
        else renderHome();
        
        attachNavEvents();
        attachFormSubmit();
        closeMobileMenuOnLink();
    }

    function renderHome() {
        app.innerHTML = `
            <section>
                <h2 class="section-title">Заказать мероприятие</h2>
                <div class="order-form-card" id="orderFormBlock">
                    <form id="eventOrderForm">
                        <div class="form-grid">
                            <select name="eventType" required>
                                <option value="">Выберите мероприятие</option>
                                <option>Свадьба</option>
                                <option>Корпоратив</option>
                                <option>День рождения</option>
                                <option>Юбилей</option>
                            </select>
                            <input type="text" name="fullname" placeholder="ФИО" required>
                            <input type="tel" name="phone" placeholder="Телефон" required>
                            <input type="email" name="email" placeholder="Электронная почта" required>
                            <input type="date" name="date" required>
                            <button type="submit">Отправить заявку</button>
                        </div>
                    </form>
                </div>
            </section>
            <section>
                <h2 class="section-title">Галерея работ</h2>
                <div class="gallery-slider" id="gallerySlider">
                    <div class="slides" id="gallerySlides">${galleryImages.map(img => `<div class="slide" style="background-image:url('${img}'); background-size:cover;"></div>`).join('')}</div>
                    <div class="slider-buttons"><button id="prevSlide">←</button><button id="nextSlide">→</button></div>
                </div>
            </section>
            <section>
                <div class="quick-links">
                    <a data-page="about" class="btn-more">О нас</a>
                    <a data-page="servicesPage" class="btn-more">Наши услуги</a>
                    <a data-page="contacts" class="btn-more">Контакты</a>
                </div>
            </section>
            <section>
                <h2 class="section-title">Наши услуги</h2>
                <div class="services-grid" id="homeServices">${allServices.slice(0,3).map(s => `
                    <div class="service-item">
                        <img class="service-photo" src="${s.photo}" alt="${s.name}" onerror="this.src='https://placehold.co/400x300?text=Фото+не+найдено'">
                        <h3>${s.name}</h3>
                        <p>${s.desc}</p>
                        <div class="price">${s.price}</div>
                        <a data-page="servicesPage" class="btn-more">Подробнее</a>
                    </div>
                `).join('')}</div>
            </section>
            <section>
                <h2 class="section-title">Интерьерные студии</h2>
                <div class="interior-grid">
                    ${interiorStudios.map(st => `
                        <div class="interior-item">
                            <div style="background-image: url('${st.image}'); background-size: cover; background-position: center; height:160px; margin-bottom:16px; border-radius:12px;">
                            </div>
                            <h3>${st.title}</h3>
                            <p>${st.desc}</p>
                            <div class="price">${st.price}</div>
                            <div style="font-size:0.8rem; color:#567d9e; margin-top:6px;"> ${st.features}</div>
                            <a data-page="orderQuick" class="btn-more">Забронировать</a>
                        </div>
                    `).join('')}
                </div>
            </section>
        `;
        initGallerySlider();
        initTouchSlider();
    }

    function renderAbout() {
        app.innerHTML = `<div class="page-card"><h2 class="section-title">О нас</h2><div class="about-flex"><div class="about-img" style="background-image: url('image/komanda.jpg'); background-size: cover; background-position: center;"></div><div><p><strong>StudioKiss</strong> — команда профессионалов с 10-летним опытом в организации праздников, свадеб, корпоративов и оформлении интерьерных студий. Мы создаем неповторимую атмосферу, учитываем каждую деталь. Наша миссия — вдохновлять и делать события особенными.</p><p>Работаем по всему Санкт-Петербургу. Более 500 довольных клиентов.</p></div></div></div>`;
    }

    function renderGalleryFull() {
        app.innerHTML = `<div class="page-card"><h2 class="section-title">Галерея работ</h2><div class="gallery-slider" id="gallerySliderFull"><div class="slides" id="gallerySlidesFull">${galleryImages.map(img=>`<div class="slide" style="background-image:url('${img}'); height:350px;"></div>`).join('')}</div><div class="slider-buttons"><button id="prevSlideFull">←</button><button id="nextSlideFull">→</button></div></div></div>`;
        let idx=0;
        const slidesDiv = document.getElementById('gallerySlidesFull');
        if(!slidesDiv) return;
        const update = ()=> slidesDiv.style.transform = `translateX(-${idx*100}%)`;
        const prevBtn = document.getElementById('prevSlideFull');
        const nextBtn = document.getElementById('nextSlideFull');
        if(prevBtn) prevBtn.addEventListener('click',()=>{ idx=(idx-1+galleryImages.length)%galleryImages.length; update();});
        if(nextBtn) nextBtn.addEventListener('click',()=>{ idx=(idx+1)%galleryImages.length; update();});
        addTouchToSlider(slidesDiv, (newIdx)=>{ idx=newIdx; update(); });
    }

    function renderServicesCatalog() {
        let filtered = currentServiceFilter === "all" ? allServices : allServices.filter(s=>s.category===currentServiceFilter);
        const totalPages = Math.ceil(filtered.length / perPage);
        const start = (currentServicesPage-1)*perPage;
        const paged = filtered.slice(start, start+perPage);
        app.innerHTML = `<div class="page-card"><h2 class="section-title">Наши услуги</h2><div class="filters"><button data-filter="all" class="filter-btn ${currentServiceFilter==='all'?'active':''}">Все</button><button data-filter="swd" class="filter-btn ${currentServiceFilter==='swd'?'active':''}">Свадьбы/Юбилеи</button><button data-filter="corp" class="filter-btn ${currentServiceFilter==='corp'?'active':''}">Корпоративы</button><button data-filter="kids" class="filter-btn ${currentServiceFilter==='kids'?'active':''}">Детские</button></div><div class="services-catalog" id="catalogList">${paged.map(s=>`
                        <div class="service-item">
                            <img class="service-photo" src="${s.photo}" alt="${s.name}" onerror="this.src='https://placehold.co/400x300?text=Фото+не+найдено'">
                            <h3>${s.name}</h3>
                            <p>${s.desc}</p>
                            <div class="price">${s.price}</div>
                        </div>
                    `).join('')}</div><div class="pagination" id="paginationBlock"></div></div>`;
        const pagDiv = document.getElementById('paginationBlock');
        if(pagDiv && totalPages>1) {
            pagDiv.innerHTML = '';
            for(let i=1;i<=totalPages;i++) pagDiv.innerHTML += `<button class="page-btn ${i===currentServicesPage?'active-page':''}" data-page="${i}">${i}</button>`;
            document.querySelectorAll('.page-btn').forEach(btn=>btn.addEventListener('click',(e)=>{
                currentServicesPage = parseInt(btn.dataset.page);
                renderServicesCatalog();
            }));
        }
        document.querySelectorAll('.filter-btn').forEach(btn=>btn.addEventListener('click',(e)=>{
            currentServiceFilter = btn.dataset.filter;
            currentServicesPage = 1;
            renderServicesCatalog();
        }));
    }

    function renderInteriorsFull() {
        app.innerHTML = `
            <div class="page-card">
                <h2 class="section-title">Интерьерные студии</h2>
                <p style="margin-bottom:20px;">Аренда стильных пространств для ваших мероприятий, съёмок и встреч</p>
                <div class="interior-grid">
                    ${interiorStudios.map(st => `
                        <div class="interior-item">
                            <div style="background-image: url('${st.image}'); background-size: cover; background-position: center; height:180px; margin-bottom:14px; border-radius:12px;">
                            </div>
                            <h3>${st.title}</h3>
                            <p>${st.desc}</p>
                            <div class="price">${st.price}</div>
                            <div style="font-size:0.8rem; color:#567d9e;">📐 ${st.features}</div>
                            <a data-page="orderQuick" class="btn-more" style="margin-top:14px;">Забронировать студию</a>
                        </div>
                    `).join('')}
                </div>
            </div>
        `;
    }

    function renderContacts() {
        app.innerHTML = `<div class="page-card"><h2 class="section-title">Контакты</h2><p>📍 Адрес: Санкт-Петербург, Российский проспект 10, офис 405</p><p>📞 Телефон: +7 (812) 513-67-67, +7 (921) 513-67-67</p><p>✉️ E-mail: hello@studiokiss.ru, booking@studiokiss.ru</p><p>🕒 Режим работы: ежедневно 9:00 – 20:00</p><hr><iframe width="100%" height="220" style="border:1px solid #cbdff2; background:#f0f0f0; border-radius:12px;" title="Карта проезда" src="https://maps.google.com/maps?q=Санкт-Петербург%20Российский%20проспект%2010&t=&z=15&ie=UTF8&iwloc=&output=embed"></iframe></div>`;
    }

    function renderOrderFormOnly() {
        app.innerHTML = `<div class="page-card"><h2 class="section-title">Оставить заявку на мероприятие</h2><div class="order-form-card"><form id="eventOrderFormQuick"><div class="form-grid"><select name="eventType"><option>Свадьба</option><option>Корпоратив</option><option>День рождения</option><option>Юбилей</option></select><input name="fullname" placeholder="ФИО"><input name="phone" placeholder="Телефон"><input name="email" placeholder="Email"><input type="date" name="date"><button type="submit">Отправить</button></div></form></div></div>`;
        attachFormSubmit();
    }
    
    function attachFormSubmit() {
        const forms = document.querySelectorAll('#eventOrderForm, #eventOrderFormQuick');
        forms.forEach(form=>{
            form.removeEventListener('submit', handleSubmit);
            form.addEventListener('submit', handleSubmit);
        });
    }
    
    function handleSubmit(e) {
        e.preventDefault();
        alert('Заявка отправлена! Мы свяжемся с вами в ближайшее время.');
        e.target.reset();
    }

    function attachNavEvents() {
        document.querySelectorAll('[data-page]').forEach(link=>{
            link.removeEventListener('click', navClickHandler);
            link.addEventListener('click', navClickHandler);
        });
    }
    
    function navClickHandler(e) {
        e.preventDefault();
        const page = this.getAttribute('data-page');
        if(page) { 
            currentPage = page; 
            currentServicesPage = 1; 
            currentServiceFilter = 'all'; 
            render(); 
            closeMobileMenu();
        }
    }

    function closeMobileMenuOnLink() {
        const links = document.querySelectorAll('.nav-links a');
        links.forEach(link => {
            link.removeEventListener('click', closeMobileMenu);
            link.addEventListener('click', closeMobileMenu);
        });
    }
    
    function closeMobileMenu() {
        const nav = document.querySelector('.nav-links');
        if(nav && window.innerWidth <= 768) {
            nav.classList.remove('show');
        }
    }

    // Сенсорные жесты для слайдера
    function initTouchSlider() {
        const slider = document.getElementById('gallerySlider');
        if(!slider) return;
        const slidesDiv = document.getElementById('gallerySlides');
        if(!slidesDiv) return;
        addTouchToSlider(slidesDiv, (idx) => {
            slidesDiv.style.transform = `translateX(-${idx * 100}%)`;
        });
    }

    function addTouchToSlider(slidesElement, onSlideChange) {
        let currentIdx = 0;
        let startX = 0;
        let isDragging = false;
        slidesElement.addEventListener('touchstart', (e) => {
            startX = e.touches[0].clientX;
            isDragging = true;
        });
        slidesElement.addEventListener('touchmove', (e) => {
            if(!isDragging) return;
            const diff = e.touches[0].clientX - startX;
            if(Math.abs(diff) > 50) {
                if(diff > 0) currentIdx = (currentIdx - 1 + galleryImages.length) % galleryImages.length;
                else currentIdx = (currentIdx + 1) % galleryImages.length;
                onSlideChange(currentIdx);
                isDragging = false;
                startX = e.touches[0].clientX;
            }
        });
        slidesElement.addEventListener('touchend', () => { isDragging = false; });
    }

    let sliderIndex = 0;
    function initGallerySlider() {
        sliderIndex = 0;
        const slidesDiv = document.getElementById('gallerySlides');
        if(!slidesDiv) return;
        const update=()=> slidesDiv.style.transform=`translateX(-${sliderIndex*100}%)`;
        const prevBtn = document.getElementById('prevSlide');
        const nextBtn = document.getElementById('nextSlide');
        if(prevBtn) prevBtn.addEventListener('click',()=>{ sliderIndex=(sliderIndex-1+galleryImages.length)%galleryImages.length; update();});
        if(nextBtn) nextBtn.addEventListener('click',()=>{ sliderIndex=(sliderIndex+1)%galleryImages.length; update();});
        addTouchToSlider(slidesDiv, (newIdx)=>{ sliderIndex=newIdx; update(); });
    }

    // Мобильное меню
    const toggleBtn = document.getElementById('navToggle');
    if(toggleBtn) {
        toggleBtn.addEventListener('click', () => {
            const nav = document.querySelector('.nav-links');
            nav.classList.toggle('show');
        });
    }

    render();
</script>
</body>
</html>
