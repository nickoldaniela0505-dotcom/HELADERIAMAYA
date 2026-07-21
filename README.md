<!DOCTYPE html>
<html lang="es">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Heladería y Frutería Arcoíris</title>
    <meta name="description"
        content="Sabor, color y frescura en cada bocado. Disfruta de los mejores helados y frutas en Tocaima.">
    <!-- Google Fonts -->
    <link
        href="https://fonts.googleapis.com/css2?family=Fredoka:wght@400;600;700&family=Nunito:wght@400;600;700&display=swap"
        rel="stylesheet">
    <!-- FontAwesome for icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Custom CSS -->
    <link rel="stylesheet" href="styles.css">
</head>

<body>

    <!-- Cart Widget -->
    <div id="cart-widget" class="cart-widget minimized">
        <div class="cart-header" id="cart-header">
            <h3><i class="fa-solid fa-cart-shopping"></i> Mi Pedido</h3>
            <span id="cart-count" class="cart-count">0</span>
            <button id="toggle-cart" class="toggle-cart-btn"><i class="fa-solid fa-chevron-up"></i></button>
        </div>
        <div class="cart-body" id="cart-body">
            <ul id="carrito" class="cart-list">
                <li class="empty-cart">El carrito está vacío</li>
            </ul>
            <div class="cart-total">
                <span>Total:</span>
                <span>$<span id="total">0</span></span>
            </div>
            <a href="https://wa.me/573134292831" target="_blank" class="btn btn-primary cart-checkout-btn"
                id="checkout-btn">
                <i class="fa-brands fa-whatsapp"></i> Pedir por WhatsApp
            </a>
        </div>
    </div>
    <!-- Header -->
    <header class="header">
        <div class="header-container">
            <div class="logo">
                <i class="fa-solid fa-rainbow logo-icon"></i>
                <div class="logo-text">
                    <h1>Arcoíris</h1>
                    <span>Heladería y Frutería</span>
                </div>
            </div>
            <button class="mobile-menu-btn" aria-label="Abrir menú">
                <i class="fa-solid fa-bars"></i>
            </button>
            <nav class="nav-menu">
                <ul>
                    <li><a href="#inicio" class="active">Inicio</a></li>
                    <li><a href="#productos">Productos</a></li>
                    <li><a href="#nosotros">Nosotros</a></li>
                    <li><a href="#contacto">
                            <class="nav-link">Contacto</a></li>
                    <li><a href="#equipo de trabajo">
                            <class="nav-link">equipo de trabajo</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <main>
        <!-- Inicio Section -->
        <section id="inicio" class="hero">
            <div class="hero-content">
                <h2 class="slogan">Sabor, color y frescura en cada bocado con la heladeria maya</h2>
                <p class="welcome-text">Descubre la magia de lo natural con nuestros deliciosos helados y frutas frescas
                    de la mejor calidad. ¡Te esperamos en Tocaima para endulzar tu día!</p>
                <div class="hero-buttons">
                    <a href="#productos" class="btn btn-primary"><i class="fa-solid fa-ice-cream"></i> Ver Menú</a>
                    <a href="#contacto" class="btn btn-secondary"><i class="fa-solid fa-location-dot"></i> Visítanos</a>
                </div>
            </div>
            <div class="hero-image-container">
                <div class="blob-shape"></div>
                <img id="foto" src="https://images.unsplash.com/photo-1501443762994-82bd5dace89a?auto=format&fit=crop&w=600&q=80" width="200" class="circulo">

                <script>


                    let imagenes = [
                        "https://images.unsplash.com/photo-1501443762994-82bd5dace89a?auto=format&fit=crop&w=600&q=80",
                        "https://images.unsplash.com/photo-1563805042-7684c019e1cb?auto=format&fit=crop&w=600&q=80",
                        "https://images.unsplash.com/photo-1579954115545-a95591f28bfc?auto=format&fit=crop&w=600&q=80"
                    ];
                    let i = 0;

                    setInterval(() => {
                        i = (i + 1) % imagenes.length;
                        document.getElementById("foto").src = imagenes[i];
                    }, 2000); // cambia cada 2 segundos

                </script>

            </div>
            <style>
                .contenedor {
                    position: relative;
                    width: 100%;
                    max-width: 300px;
                    height: 200px;
                    margin: 0 auto;
                }

                .circulo {
                    width: 100%;
                    height: 100%;
                    background: orange;
                    border-radius: 100px;
                    display: flex;
                    justify-content: center;
                    align-items: center;
                }

                .foto {
                    width: 180px;
                    border-radius: 10px;
                }
            </style>



        </section>

        <!-- Productos Section -->
        <section id="productos" class="products-section">
            <div class="section-header">
                <h2>Nuestros Productos</h2>
                <div class="rainbow-divider"></div>
            </div>

            <h3 class="category-title">Ensaladas</h3>
            <div class="products-grid">
                <div class="product-card" data-category="ensaladas">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1540420773420-3366772f4999?auto=format&fit=crop&w=500&q=80"
                            alt="ensalada mini">
                        <span class="category-helado-badge">ensaladas</span>
                    </div>
                    <div class="card-content">
                        <h3>ensalada mini</h3>
                        <div class="price-row">
                            <span class="price">$8.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>

                <div class="product-card" data-category="ensaladas">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1511690656952-34342bb7c2f2?auto=format&fit=crop&w=500&q=80"
                            alt="ensalada sencilla">
                        <span class="category-badge helados-badge">ensaladas</span>
                    </div>
                    <div class="card-content">
                        <h3>ensalada sencilla</h3>
                        <div class="price-row">
                            <span class="price">$10.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>

                <div class="product-card" data-category="ensaladas">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1498837167922-ddd27525d352?auto=format&fit=crop&w=500&q=80"
                            alt="ensalada especial">
                        <span class="category-badge helados-badge">ensaladas</span>
                    </div>
                    <div class="card-content">
                        <h3>ensalada especial</h3>
                        <div class="price-row">
                            <span class="price">$13.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>

                <!-- Ensaladas de frutas -->
                <div class="product-card" data-category="frutas">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1505576399279-565b52d4ac71?auto=format&fit=crop&w=500&q=80"
                            alt="Ensalada super maya">
                        <span class="category-badge frutas-badge">Ensaladas</span>
                    </div>
                    <div class="card-content">
                        <h3>Ensalada super mayal</h3>
                        <div class="price-row">
                            <span class="price">$15.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>

                <div class="product-card" data-category="frutas">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1519996521430-02b798c1d881?auto=format&fit=crop&w=500&q=80"
                            alt="ensalada maya suprema">
                        <span class="category-badge frutas-badge">Ensaladas</span>
                    </div>
                    <div class="card-content">
                        <h3>ensalada maya super</h3>
                        <div class="price-row">
                            <span class="price">$20.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>

                <!-- Jugos -->
                <div class="product-card" data-category="frutas">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1516685018646-549198525c1b?auto=format&fit=crop&w=500&q=80"
                            alt="ensalada full fruta">
                        <span class="category-badge jugos-badge">ensaladas</span>
                    </div>
                    <div class="card-content">
                        <h3>ensalada full fruta</h3>
                        <div class="price-row">
                            <span class="price">$10.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>
            </div>

            <h3 class="category-title">Preparaciones con Helado</h3>
            <div class="products-grid">
                <div class="product-card" data-category="preparaciones con helado">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1579954115545-a95591f28bfc?auto=format&fit=crop&w=500&q=80"
                            alt="banana split">
                        <span class="category-badge jugos-badge">preparaciones con helado</span>
                    </div>
                    <div class="card-content">
                        <h3>banana split</h3>
                        <div class="price-row">
                            <span class="price">$14.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>

                <div class="product-card" data-category="preparaciones con helado">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1501443762994-82bd5dace89a?auto=format&fit=crop&w=500&q=80"
                            alt="Jugo Natural en Leche">
                        <span class="category-badge jugos-badge">preparaciones con helado</span>
                    </div>
                    <div class="card-content">
                        <h3>banana split super</h3>
                        <div class="price-row">
                            <span class="price">$17.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>

                <div class="product-card" data-category="preparaciones con helado">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1606313564200-e75d5e30476c?auto=format&fit=crop&w=500&q=80"
                            alt="Jugo Natural en Leche">
                        <span class="category-badge jugos-badge">preparaciones con helado</span>
                    </div>
                    <div class="card-content">
                        <h3>brownie con helado</h3>
                        <div class="price-row">
                            <span class="price">$13.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>

                <div class="product-card" data-category="preparaciones con helado">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1488477181946-6428a0291777?auto=format&fit=crop&w=500&q=80"
                            alt="Jugo Natural en Leche">
                        <span class="category-badge jugos-badge">preparaciones con helado</span>
                    </div>
                    <div class="card-content">
                        <h3>copa de helado con fruta</h3>
                        <div class="price-row">
                            <span class="price">$15.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>

                <div class="product-card" data-category="preparaciones con helado">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1563805042-7684c019e1cb?auto=format&fit=crop&w=500&q=80"
                            alt="Jugo Natural en Leche">
                        <span class="category-badge jugos-badge">preparaciones con helado</span>
                    </div>
                    <div class="card-content">
                        <h3>copa de helado de durazno</h3>
                        <div class="price-row">
                            <span class="price">$15.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>

                <div class="product-card" data-category="preparaciones con helado">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1590080875515-8a3a8dc5735e?auto=format&fit=crop&w=500&q=80"
                            alt="Jugo Natural en Leche">
                        <span class="category-badge jugos-badge">preparaciones con helado</span>
                    </div>
                    <div class="card-content">
                        <h3>fresas con crema clasicas</h3>
                        <div class="price-row">
                            <span class="price">$10.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>

                <div class="product-card" data-category="preparaciones con helado">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1469533748051-9be432b7377c?auto=format&fit=crop&w=500&q=80"
                            alt="Jugo Natural en Leche">
                        <span class="category-badge jugos-badge">preparaciones con helado</span>
                    </div>
                    <div class="card-content">
                        <h3>fresas con crema y helado</h3>
                        <div class="price-row">
                            <span class="price">$13.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>

                <div class="product-card" data-category="preparaciones con helado">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1587314168485-3236d6710814?auto=format&fit=crop&w=500&q=80"
                            alt="Jugo Natural en Leche">
                        <span class="category-badge jugos-badge">preparaciones con helado</span>
                    </div>
                    <div class="card-content">
                        <h3>fresas con crema especiales</h3>
                        <div class="price-row">
                            <span class="price">$16.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>

                <div class="product-card" data-category="conos">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1567206563066-ec152f031a3a?auto=format&fit=crop&w=500&q=80"
                            alt="Jugo Natural en Leche">
                        <span class="category-badge jugos-badge">conos</span>
                    </div>
                    <div class="card-content">
                        <h3>cono doble</h3>
                        <div class="price-row">
                            <span class="price">$8.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>
            </div>



            <h3 class="category-title">Comida Rápida</h3>
            <div class="products-grid">
                <div class="product-card" data-category="comida rapida">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1568901346375-23c9450c58cd?auto=format&fit=crop&w=500&q=80"
                            alt="hamburguesa especial">
                        <span class="category-badge jugos-badge">comida rapida</span>
                    </div>
                    <div class="card-content">
                        <h3>hamburguesa especial</h3>
                        <div class="price-row">
                            <span class="price">$15.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>

                <div class="product-card" data-category="comida rapida">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1550547660-d9450f859349?auto=format&fit=crop&w=500&q=80"
                            alt="Jugo Natural en Leche">
                        <span class="category-badge jugos-badge">comida rapida</span>
                    </div>
                    <div class="card-content">
                        <h3>hamburguesa sencilla</h3>
                        <div class="price-row">
                            <span class="price">$10.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>
            </div>

            <h3 class="category-title">Bebidas</h3>
            <div class="products-grid">
                <div class="product-card" data-category="bebidas">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1497534446932-c925b458314e?auto=format&fit=crop&w=500&q=80"
                            alt="Jugo Natural en Leche">
                        <span class="category-badge jugos-badge">bebidas</span>
                    </div>
                    <div class="card-content">
                        <h3>granizado</h3>
                        <div class="price-row">
                            <span class="price">$8.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>

                <div class="product-card" data-category="bebidas">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1595981267035-7b04ca84a82d?auto=format&fit=crop&w=500&q=80"
                            alt="Jugo Natural en Leche">
                        <span class="category-badge jugos-badge">bebidas</span>
                    </div>
                    <div class="card-content">
                        <h3>michelada</h3>
                        <div class="price-row">
                            <span class="price">$10.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>

                <div class="product-card" data-category="jugos">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1572490122747-3968b75cc699?auto=format&fit=crop&w=500&q=80"
                            alt="Jugo Natural en Leche">
                        <span class="category-badge jugos-badge">Jugos</span>
                    </div>
                    <div class="card-content">
                        <h3>Jugo Natural en Leche</h3>
                        <div class="price-row">
                            <span class="price">$7.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>

                <div class="product-card" data-category="jugos">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1512621776951-a57141f2eefd?auto=format&fit=crop&w=500&q=80"
                            alt="Jugo Natural en Leche">
                        <span class="category-badge jugos-badge">Jugos</span>
                    </div>
                    <div class="card-content">
                        <h3>limonada de coco</h3>
                        <div class="price-row">
                            <span class="price">$8.500</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Nosotros Section -->
        <section id="nosotros" class="about-section">
            <div class="about-container">
                <div class="about-image">
                    <img src="https://images.unsplash.com/photo-1505935428862-770b6f24f629?auto=format&fit=crop&w=800&q=80"
                        alt="Interior de la heladería">
                </div>
                <div class="about-content">
                    <h2>Sobre Nosotros</h2>
                    <div class="rainbow-divider-left"></div>
                    <p class="history">Nacimos en el corazón de Tocaima con un sueño dulce: llevar alegría y frescura a
                        cada familia. Desde nuestros inicios, nos hemos dedicado a crear los mejores helados y ensaladas
                        de frutas utilizando ingredientes 100% naturales y de la más alta calidad.</p>

                    <div class="mission-vision">
                        <div class="mv-card">
                            <div class="mv-icon"><i class="fa-solid fa-bullseye"></i></div>
                            <h3>Misión</h3>
                            <p>Brindar anuestros clientes productos frescos, saludables y de excelente
                                calidad, ofreciendo una variedad de helados y frutas que satisfagan sus
                                gustos, en un ambiente agradable, con atencion amable y precios justos que
                                generen bienestar y confianza en la comunidad
                            </p>
                        </div>
                        <div class="mv-card">
                            <div class="mv-icon"><i class="fa-solid fa-eye"></i></div>
                            <h3>Visión</h3>
                            <p>ser reconocidos como la heladeria y fruteria lider en nuestra region, destacandonos
                                por la calidad de nuestros productos, la innovacion en sabores y la preferencia de
                                nuestros clientes, contribuyendo a una alimentacion mas saludable y el crecimiento
                                de nuestro negocio.
                            </p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Contacto Section -->
        <section id="contacto" class="contact-section">
            <div class="section-header">
                <h2>Encuéntranos</h2>
                <div class="rainbow-divider"></div>
                <p>¡Ven a disfrutar de nuestros sabores o haz tu pedido a domicilio!</p>
            </div>

            <div class="contact-container">
                <div class="contact-info">
                    <div class="info-item">
                        <div class="info-icon"><i class="fa-solid fa-location-dot"></i></div>
                        <div>
                            <h4>Dirección</h4>
                            <p>calle 4 #6-55, tocaima, colombia</p>
                        </div>
                    </div>
                    <div class="info-item">
                        <div class="info-icon"><i class="fa-solid fa-phone"></i></div>
                        <div>
                            <h4>Teléfono</h4>
                            <p>313 4292831</p>
                        </div>
                    </div>
                    <div class="info-item">
                        <div class="info-icon"><i class="fa-solid fa-clock"></i></div>
                        <div>
                            <h4>Horario</h4>
                            <p>Lunes a Domingo: 11:00 AM - 11:00 PM</p>
                        </div>
                    </div>
                    <div class="info-item">
                        <div class="info-icon" style="color: #1877F2;"><i class="fa-brands fa-facebook"></i></div>
                        <div>
                            <h4>Facebook</h4>
                            <p><a href="https://www.facebook.com/share/1Etc48D2zr/" target="_blank"
                                    style="color: var(--color-blue); font-weight: 600;">Heladería Arcoíris Tocaima</a>
                            </p>
                        </div>
                    </div>
                    <div class="info-item">
                        <div class="info-icon" style="color: #E4405F;"><i class="fa-brands fa-instagram"></i></div>
                        <div>
                            <h4>Instagram</h4>
                            <p><a href="https://www.instagram.com/fruteria_maya?igsh=MXVuamFrbHdyYm02dg%3D%3D"
                                    target="_blank"
                                    style="color: var(--color-purple); font-weight: 600;">@heladeriaarcoiristocaima</a>
                            </p>
                        </div>
                    </div>

                    <a href="https://wa.me/573134292831" target="_blank" class="whatsapp-btn">
                        <i class="fa-brands fa-whatsapp"></i> Pedir por WhatsApp
                    </a>
                </div>

                <div class="map-container">
                    <!-- Embed a placeholder map for Tocaima -->
                    <iframe
                        src="https://maps.google.com/maps?q=calle%204%20%236-55,%20tocaima,%20colombia&t=&z=17&ie=UTF8&iwloc=&output=embed"
                        width="100%" height="100%" style="border:0;" allowfullscreen="" loading="lazy"
                        referrerpolicy="no-referrer-when-downgrade"></iframe>
                </div>
            </div>
        </section>
    </main>


    <section id="equipo de trabajo" class="about-section"></section>
    <h2 style="text-align: center;">EQUIPO DE TRABAJO</h2>
    <br>

    <div class="contenedor-equipo">

        <div class="miembro">
            <img src="images/astrit.jpeg"
                height="150" width="150" alt="Astrit">
            <h3>ASTRIT BAUTISTA</h3>
            <p>LIDER DE EQUIPO</p>
            <p>PROGRAMADORA</p>
        </div>

        <div class="miembro">
            <img src="images/daniela.jpeg"
                height="150" width="150" alt="Daniela">
            <h3>DANIELA DUARTE</h3>
            <p>PRESENTADORA</p>
        </div>

        <div class="miembro">
            <img src="images/esteban.jpeg"
                height="150" width="150" alt="Esteban">
            <h3>ESTEBAN MIRANDA</h3>
            <p>DISEÑADOR GRAFICO</p>
        </div>

        <div class="miembro">
            <img src="images/nicolas.jpeg"
                height="150" width="150" alt="Nicolas">
            <h3>NICOLAS TRUJILLO</h3>
            <p>DISEÑADOR UX</p>
        </div>

        <div class="miembro">
            <img src="images/wilbert.jpeg"
                height="150" width="150" alt="WILBERT">
            <h3>WILBERT</h3>
            <p>TESTER</p>

        </div>
    </div> <!-- FIN CONTENEDOR EQUIPO -->

    <style>
        .equipo {
            text-align: center;
            padding: 30px;
        }

        .contenedor-equipo {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
        }

        .miembro {
            background: white;
            border-radius: 15px;
            width: 200px;
            padding: 15px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.15);
            transition: transform 0.2s;
        }

        .miembro:hover {
            transform: scale(1.05);
        }

        .miembro img {
            border-radius: 50%;
            object-fit: cover;
            margin-bottom: 10px;
        }

        .miembro h3 {
            margin: 5px 0;
        }

        .miembro p {
            color: gray;
        }
    </style>

    <!-- Footer -->
    <footer>
        <div class="footer-content">
            <div class="footer-brand">
                <div class="logo">
                    <i class="fa-solid fa-rainbow logo-icon"></i>
                    <div class="logo-text">
                        <h2>Arcoíris</h2>
                    </div>
                </div>
                <p>Sabor, color y frescura en cada bocado.</p>
            </div>
            <div class="social-links">
                <a href="https://www.facebook.com/share/1Etc48D2zr/" target="_blank" aria-label="Facebook"><i
                        class="fa-brands fa-facebook-f"></i></a>
                <a href="https://www.instagram.com/heladeriaarcoiristocaima" target="_blank" aria-label="Instagram"><i
                        class="fa-brands fa-instagram"></i></a>
                <a href="https://wa.me/573134292831" target="_blank" aria-label="WhatsApp"><i
                        class="fa-brands fa-whatsapp"></i></a>
            </div>
        </div>
        <div class="footer-bottom">
            <p>&copy; 2024 Heladería y Frutería Arcoíris. Todos los derechos reservados. Diseñado en Tocaima.</p>
        </div>
    </footer>

    <!-- Custom JS -->
    <script src="script.js"></script>
</body>

</html><!DOCTYPE html>
<html lang="es">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Heladería y Frutería Arcoíris</title>
    <meta name="description"
        content="Sabor, color y frescura en cada bocado. Disfruta de los mejores helados y frutas en Tocaima.">
    <!-- Google Fonts -->
    <link
        href="https://fonts.googleapis.com/css2?family=Fredoka:wght@400;600;700&family=Nunito:wght@400;600;700&display=swap"
        rel="stylesheet">
    <!-- FontAwesome for icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Custom CSS -->
    <link rel="stylesheet" href="styles.css">
</head>

<body>

    <!-- Cart Widget -->
    <div id="cart-widget" class="cart-widget minimized">
        <div class="cart-header" id="cart-header">
            <h3><i class="fa-solid fa-cart-shopping"></i> Mi Pedido</h3>
            <span id="cart-count" class="cart-count">0</span>
            <button id="toggle-cart" class="toggle-cart-btn"><i class="fa-solid fa-chevron-up"></i></button>
        </div>
        <div class="cart-body" id="cart-body">
            <ul id="carrito" class="cart-list">
                <li class="empty-cart">El carrito está vacío</li>
            </ul>
            <div class="cart-total">
                <span>Total:</span>
                <span>$<span id="total">0</span></span>
            </div>
            <a href="https://wa.me/573134292831" target="_blank" class="btn btn-primary cart-checkout-btn"
                id="checkout-btn">
                <i class="fa-brands fa-whatsapp"></i> Pedir por WhatsApp
            </a>
        </div>
    </div>
    <!-- Header -->
    <header class="header">
        <div class="header-container">
            <div class="logo">
                <i class="fa-solid fa-rainbow logo-icon"></i>
                <div class="logo-text">
                    <h1>Arcoíris</h1>
                    <span>Heladería y Frutería</span>
                </div>
            </div>
            <button class="mobile-menu-btn" aria-label="Abrir menú">
                <i class="fa-solid fa-bars"></i>
            </button>
            <nav class="nav-menu">
                <ul>
                    <li><a href="#inicio" class="active">Inicio</a></li>
                    <li><a href="#productos">Productos</a></li>
                    <li><a href="#nosotros">Nosotros</a></li>
                    <li><a href="#contacto">
                            <class="nav-link">Contacto</a></li>
                    <li><a href="#equipo de trabajo">
                            <class="nav-link">equipo de trabajo</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <main>
        <!-- Inicio Section -->
        <section id="inicio" class="hero">
            <div class="hero-content">
                <h2 class="slogan">Sabor, color y frescura en cada bocado con la heladeria maya</h2>
                <p class="welcome-text">Descubre la magia de lo natural con nuestros deliciosos helados y frutas frescas
                    de la mejor calidad. ¡Te esperamos en Tocaima para endulzar tu día!</p>
                <div class="hero-buttons">
                    <a href="#productos" class="btn btn-primary"><i class="fa-solid fa-ice-cream"></i> Ver Menú</a>
                    <a href="#contacto" class="btn btn-secondary"><i class="fa-solid fa-location-dot"></i> Visítanos</a>
                </div>
            </div>
            <div class="hero-image-container">
                <div class="blob-shape"></div>
                <img id="foto" src="https://images.unsplash.com/photo-1501443762994-82bd5dace89a?auto=format&fit=crop&w=600&q=80" width="200" class="circulo">

                <script>


                    let imagenes = [
                        "https://images.unsplash.com/photo-1501443762994-82bd5dace89a?auto=format&fit=crop&w=600&q=80",
                        "https://images.unsplash.com/photo-1563805042-7684c019e1cb?auto=format&fit=crop&w=600&q=80",
                        "https://images.unsplash.com/photo-1579954115545-a95591f28bfc?auto=format&fit=crop&w=600&q=80"
                    ];
                    let i = 0;

                    setInterval(() => {
                        i = (i + 1) % imagenes.length;
                        document.getElementById("foto").src = imagenes[i];
                    }, 2000); // cambia cada 2 segundos

                </script>

            </div>
            <style>
                .contenedor {
                    position: relative;
                    width: 100%;
                    max-width: 300px;
                    height: 200px;
                    margin: 0 auto;
                }

                .circulo {
                    width: 100%;
                    height: 100%;
                    background: orange;
                    border-radius: 100px;
                    display: flex;
                    justify-content: center;
                    align-items: center;
                }

                .foto {
                    width: 180px;
                    border-radius: 10px;
                }
            </style>



        </section>

        <!-- Productos Section -->
        <section id="productos" class="products-section">
            <div class="section-header">
                <h2>Nuestros Productos</h2>
                <div class="rainbow-divider"></div>
            </div>

            <h3 class="category-title">Ensaladas</h3>
            <div class="products-grid">
                <div class="product-card" data-category="ensaladas">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1540420773420-3366772f4999?auto=format&fit=crop&w=500&q=80"
                            alt="ensalada mini">
                        <span class="category-helado-badge">ensaladas</span>
                    </div>
                    <div class="card-content">
                        <h3>ensalada mini</h3>
                        <div class="price-row">
                            <span class="price">$8.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>

                <div class="product-card" data-category="ensaladas">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1511690656952-34342bb7c2f2?auto=format&fit=crop&w=500&q=80"
                            alt="ensalada sencilla">
                        <span class="category-badge helados-badge">ensaladas</span>
                    </div>
                    <div class="card-content">
                        <h3>ensalada sencilla</h3>
                        <div class="price-row">
                            <span class="price">$10.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>

                <div class="product-card" data-category="ensaladas">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1498837167922-ddd27525d352?auto=format&fit=crop&w=500&q=80"
                            alt="ensalada especial">
                        <span class="category-badge helados-badge">ensaladas</span>
                    </div>
                    <div class="card-content">
                        <h3>ensalada especial</h3>
                        <div class="price-row">
                            <span class="price">$13.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>

                <!-- Ensaladas de frutas -->
                <div class="product-card" data-category="frutas">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1505576399279-565b52d4ac71?auto=format&fit=crop&w=500&q=80"
                            alt="Ensalada super maya">
                        <span class="category-badge frutas-badge">Ensaladas</span>
                    </div>
                    <div class="card-content">
                        <h3>Ensalada super mayal</h3>
                        <div class="price-row">
                            <span class="price">$15.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>

                <div class="product-card" data-category="frutas">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1519996521430-02b798c1d881?auto=format&fit=crop&w=500&q=80"
                            alt="ensalada maya suprema">
                        <span class="category-badge frutas-badge">Ensaladas</span>
                    </div>
                    <div class="card-content">
                        <h3>ensalada maya super</h3>
                        <div class="price-row">
                            <span class="price">$20.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>

                <!-- Jugos -->
                <div class="product-card" data-category="frutas">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1516685018646-549198525c1b?auto=format&fit=crop&w=500&q=80"
                            alt="ensalada full fruta">
                        <span class="category-badge jugos-badge">ensaladas</span>
                    </div>
                    <div class="card-content">
                        <h3>ensalada full fruta</h3>
                        <div class="price-row">
                            <span class="price">$10.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>
            </div>

            <h3 class="category-title">Preparaciones con Helado</h3>
            <div class="products-grid">
                <div class="product-card" data-category="preparaciones con helado">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1579954115545-a95591f28bfc?auto=format&fit=crop&w=500&q=80"
                            alt="banana split">
                        <span class="category-badge jugos-badge">preparaciones con helado</span>
                    </div>
                    <div class="card-content">
                        <h3>banana split</h3>
                        <div class="price-row">
                            <span class="price">$14.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>

                <div class="product-card" data-category="preparaciones con helado">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1501443762994-82bd5dace89a?auto=format&fit=crop&w=500&q=80"
                            alt="Jugo Natural en Leche">
                        <span class="category-badge jugos-badge">preparaciones con helado</span>
                    </div>
                    <div class="card-content">
                        <h3>banana split super</h3>
                        <div class="price-row">
                            <span class="price">$17.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>

                <div class="product-card" data-category="preparaciones con helado">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1606313564200-e75d5e30476c?auto=format&fit=crop&w=500&q=80"
                            alt="Jugo Natural en Leche">
                        <span class="category-badge jugos-badge">preparaciones con helado</span>
                    </div>
                    <div class="card-content">
                        <h3>brownie con helado</h3>
                        <div class="price-row">
                            <span class="price">$13.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>

                <div class="product-card" data-category="preparaciones con helado">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1488477181946-6428a0291777?auto=format&fit=crop&w=500&q=80"
                            alt="Jugo Natural en Leche">
                        <span class="category-badge jugos-badge">preparaciones con helado</span>
                    </div>
                    <div class="card-content">
                        <h3>copa de helado con fruta</h3>
                        <div class="price-row">
                            <span class="price">$15.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>

                <div class="product-card" data-category="preparaciones con helado">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1563805042-7684c019e1cb?auto=format&fit=crop&w=500&q=80"
                            alt="Jugo Natural en Leche">
                        <span class="category-badge jugos-badge">preparaciones con helado</span>
                    </div>
                    <div class="card-content">
                        <h3>copa de helado de durazno</h3>
                        <div class="price-row">
                            <span class="price">$15.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>

                <div class="product-card" data-category="preparaciones con helado">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1590080875515-8a3a8dc5735e?auto=format&fit=crop&w=500&q=80"
                            alt="Jugo Natural en Leche">
                        <span class="category-badge jugos-badge">preparaciones con helado</span>
                    </div>
                    <div class="card-content">
                        <h3>fresas con crema clasicas</h3>
                        <div class="price-row">
                            <span class="price">$10.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>

                <div class="product-card" data-category="preparaciones con helado">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1469533748051-9be432b7377c?auto=format&fit=crop&w=500&q=80"
                            alt="Jugo Natural en Leche">
                        <span class="category-badge jugos-badge">preparaciones con helado</span>
                    </div>
                    <div class="card-content">
                        <h3>fresas con crema y helado</h3>
                        <div class="price-row">
                            <span class="price">$13.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>

                <div class="product-card" data-category="preparaciones con helado">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1587314168485-3236d6710814?auto=format&fit=crop&w=500&q=80"
                            alt="Jugo Natural en Leche">
                        <span class="category-badge jugos-badge">preparaciones con helado</span>
                    </div>
                    <div class="card-content">
                        <h3>fresas con crema especiales</h3>
                        <div class="price-row">
                            <span class="price">$16.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>

                <div class="product-card" data-category="conos">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1567206563066-ec152f031a3a?auto=format&fit=crop&w=500&q=80"
                            alt="Jugo Natural en Leche">
                        <span class="category-badge jugos-badge">conos</span>
                    </div>
                    <div class="card-content">
                        <h3>cono doble</h3>
                        <div class="price-row">
                            <span class="price">$8.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>
            </div>



            <h3 class="category-title">Comida Rápida</h3>
            <div class="products-grid">
                <div class="product-card" data-category="comida rapida">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1568901346375-23c9450c58cd?auto=format&fit=crop&w=500&q=80"
                            alt="hamburguesa especial">
                        <span class="category-badge jugos-badge">comida rapida</span>
                    </div>
                    <div class="card-content">
                        <h3>hamburguesa especial</h3>
                        <div class="price-row">
                            <span class="price">$15.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>

                <div class="product-card" data-category="comida rapida">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1550547660-d9450f859349?auto=format&fit=crop&w=500&q=80"
                            alt="Jugo Natural en Leche">
                        <span class="category-badge jugos-badge">comida rapida</span>
                    </div>
                    <div class="card-content">
                        <h3>hamburguesa sencilla</h3>
                        <div class="price-row">
                            <span class="price">$10.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>
            </div>

            <h3 class="category-title">Bebidas</h3>
            <div class="products-grid">
                <div class="product-card" data-category="bebidas">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1497534446932-c925b458314e?auto=format&fit=crop&w=500&q=80"
                            alt="Jugo Natural en Leche">
                        <span class="category-badge jugos-badge">bebidas</span>
                    </div>
                    <div class="card-content">
                        <h3>granizado</h3>
                        <div class="price-row">
                            <span class="price">$8.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>

                <div class="product-card" data-category="bebidas">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1595981267035-7b04ca84a82d?auto=format&fit=crop&w=500&q=80"
                            alt="Jugo Natural en Leche">
                        <span class="category-badge jugos-badge">bebidas</span>
                    </div>
                    <div class="card-content">
                        <h3>michelada</h3>
                        <div class="price-row">
                            <span class="price">$10.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>

                <div class="product-card" data-category="jugos">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1572490122747-3968b75cc699?auto=format&fit=crop&w=500&q=80"
                            alt="Jugo Natural en Leche">
                        <span class="category-badge jugos-badge">Jugos</span>
                    </div>
                    <div class="card-content">
                        <h3>Jugo Natural en Leche</h3>
                        <div class="price-row">
                            <span class="price">$7.000</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>

                <div class="product-card" data-category="jugos">
                    <div class="card-image">
                        <img src="https://images.unsplash.com/photo-1512621776951-a57141f2eefd?auto=format&fit=crop&w=500&q=80"
                            alt="Jugo Natural en Leche">
                        <span class="category-badge jugos-badge">Jugos</span>
                    </div>
                    <div class="card-content">
                        <h3>limonada de coco</h3>
                        <div class="price-row">
                            <span class="price">$8.500</span>
                            <button class="btn-add"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Nosotros Section -->
        <section id="nosotros" class="about-section">
            <div class="about-container">
                <div class="about-image">
                    <img src="https://images.unsplash.com/photo-1505935428862-770b6f24f629?auto=format&fit=crop&w=800&q=80"
                        alt="Interior de la heladería">
                </div>
                <div class="about-content">
                    <h2>Sobre Nosotros</h2>
                    <div class="rainbow-divider-left"></div>
                    <p class="history">Nacimos en el corazón de Tocaima con un sueño dulce: llevar alegría y frescura a
                        cada familia. Desde nuestros inicios, nos hemos dedicado a crear los mejores helados y ensaladas
                        de frutas utilizando ingredientes 100% naturales y de la más alta calidad.</p>

                    <div class="mission-vision">
                        <div class="mv-card">
                            <div class="mv-icon"><i class="fa-solid fa-bullseye"></i></div>
                            <h3>Misión</h3>
                            <p>Brindar anuestros clientes productos frescos, saludables y de excelente
                                calidad, ofreciendo una variedad de helados y frutas que satisfagan sus
                                gustos, en un ambiente agradable, con atencion amable y precios justos que
                                generen bienestar y confianza en la comunidad
                            </p>
                        </div>
                        <div class="mv-card">
                            <div class="mv-icon"><i class="fa-solid fa-eye"></i></div>
                            <h3>Visión</h3>
                            <p>ser reconocidos como la heladeria y fruteria lider en nuestra region, destacandonos
                                por la calidad de nuestros productos, la innovacion en sabores y la preferencia de
                                nuestros clientes, contribuyendo a una alimentacion mas saludable y el crecimiento
                                de nuestro negocio.
                            </p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Contacto Section -->
        <section id="contacto" class="contact-section">
            <div class="section-header">
                <h2>Encuéntranos</h2>
                <div class="rainbow-divider"></div>
                <p>¡Ven a disfrutar de nuestros sabores o haz tu pedido a domicilio!</p>
            </div>

            <div class="contact-container">
                <div class="contact-info">
                    <div class="info-item">
                        <div class="info-icon"><i class="fa-solid fa-location-dot"></i></div>
                        <div>
                            <h4>Dirección</h4>
                            <p>calle 4 #6-55, tocaima, colombia</p>
                        </div>
                    </div>
                    <div class="info-item">
                        <div class="info-icon"><i class="fa-solid fa-phone"></i></div>
                        <div>
                            <h4>Teléfono</h4>
                            <p>313 4292831</p>
                        </div>
                    </div>
                    <div class="info-item">
                        <div class="info-icon"><i class="fa-solid fa-clock"></i></div>
                        <div>
                            <h4>Horario</h4>
                            <p>Lunes a Domingo: 11:00 AM - 11:00 PM</p>
                        </div>
                    </div>
                    <div class="info-item">
                        <div class="info-icon" style="color: #1877F2;"><i class="fa-brands fa-facebook"></i></div>
                        <div>
                            <h4>Facebook</h4>
                            <p><a href="https://www.facebook.com/share/1Etc48D2zr/" target="_blank"
                                    style="color: var(--color-blue); font-weight: 600;">Heladería Arcoíris Tocaima</a>
                            </p>
                        </div>
                    </div>
                    <div class="info-item">
                        <div class="info-icon" style="color: #E4405F;"><i class="fa-brands fa-instagram"></i></div>
                        <div>
                            <h4>Instagram</h4>
                            <p><a href="https://www.instagram.com/fruteria_maya?igsh=MXVuamFrbHdyYm02dg%3D%3D"
                                    target="_blank"
                                    style="color: var(--color-purple); font-weight: 600;">@heladeriaarcoiristocaima</a>
                            </p>
                        </div>
                    </div>

                    <a href="https://wa.me/573134292831" target="_blank" class="whatsapp-btn">
                        <i class="fa-brands fa-whatsapp"></i> Pedir por WhatsApp
                    </a>
                </div>

                <div class="map-container">
                    <!-- Embed a placeholder map for Tocaima -->
                    <iframe
                        src="https://maps.google.com/maps?q=calle%204%20%236-55,%20tocaima,%20colombia&t=&z=17&ie=UTF8&iwloc=&output=embed"
                        width="100%" height="100%" style="border:0;" allowfullscreen="" loading="lazy"
                        referrerpolicy="no-referrer-when-downgrade"></iframe>
                </div>
            </div>
        </section>
    </main>


    <section id="equipo de trabajo" class="about-section"></section>
    <h2 style="text-align: center;">EQUIPO DE TRABAJO</h2>
    <br>

    <div class="contenedor-equipo">

        <div class="miembro">
            <img src="images/astrit.jpeg"
                height="150" width="150" alt="Astrit">
            <h3>ASTRIT BAUTISTA</h3>
            <p>LIDER DE EQUIPO</p>
            <p>PROGRAMADORA</p>
        </div>

        <div class="miembro">
            <img src="images/daniela.jpeg"
                height="150" width="150" alt="Daniela">
            <h3>DANIELA DUARTE</h3>
            <p>PRESENTADORA</p>
        </div>

        <div class="miembro">
            <img src="images/esteban.jpeg"
                height="150" width="150" alt="Esteban">
            <h3>ESTEBAN MIRANDA</h3>
            <p>DISEÑADOR GRAFICO</p>
        </div>

        <div class="miembro">
            <img src="images/nicolas.jpeg"
                height="150" width="150" alt="Nicolas">
            <h3>NICOLAS TRUJILLO</h3>
            <p>DISEÑADOR UX</p>
        </div>

        <div class="miembro">
            <img src="images/wilbert.jpeg"
                height="150" width="150" alt="WILBERT">
            <h3>WILBERT</h3>
            <p>TESTER</p>

        </div>
    </div> <!-- FIN CONTENEDOR EQUIPO -->

    <style>
        .equipo {
            text-align: center;
            padding: 30px;
        }

        .contenedor-equipo {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
        }

        .miembro {
            background: white;
            border-radius: 15px;
            width: 200px;
            padding: 15px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.15);
            transition: transform 0.2s;
        }

        .miembro:hover {
            transform: scale(1.05);
        }

        .miembro img {
            border-radius: 50%;
            object-fit: cover;
            margin-bottom: 10px;
        }

        .miembro h3 {
            margin: 5px 0;
        }

        .miembro p {
            color: gray;
        }
    </style>

    <!-- Footer -->
    <footer>
        <div class="footer-content">
            <div class="footer-brand">
                <div class="logo">
                    <i class="fa-solid fa-rainbow logo-icon"></i>
                    <div class="logo-text">
                        <h2>Arcoíris</h2>
                    </div>
                </div>
                <p>Sabor, color y frescura en cada bocado.</p>
            </div>
            <div class="social-links">
                <a href="https://www.facebook.com/share/1Etc48D2zr/" target="_blank" aria-label="Facebook"><i
                        class="fa-brands fa-facebook-f"></i></a>
                <a href="https://www.instagram.com/heladeriaarcoiristocaima" target="_blank" aria-label="Instagram"><i
                        class="fa-brands fa-instagram"></i></a>
                <a href="https://wa.me/573134292831" target="_blank" aria-label="WhatsApp"><i
                        class="fa-brands fa-whatsapp"></i></a>
            </div>
        </div>
        <div class="footer-bottom">
            <p>&copy; 2024 Heladería y Frutería Arcoíris. Todos los derechos reservados. Diseñado en Tocaima.</p>
        </div>
    </footer>

    <!-- Custom JS -->
    <script src="script.js"></script>
</body>

</html>
