# JODANS-SOLAR-ENGINEERING-SERVICES-WEBSITE-2
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jodans Solar Engineering Services | Solar Energy Solutions</title>
    <meta name="description" content="Expert solar and engineering services across Nigeria. Trusted solar energy solutions by Jodans Solar Engineering Services.">
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <div class="logo">Jodans Solar Engineering</div>
        <nav>
            <ul>
                <li><a href="#about">About</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#portfolio">Portfolio</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section class="hero">
        <h1>Reliable Solar Energy Solutions ☀️</h1>
        <p>Affordable | Professional | Clean Energy</p>
        <button onclick="openContactForm()">Contact Us</button>
    </section>

    <section id="about" class="about">
        <h2>About Jodans Solar</h2>
        <p>We deliver engineering excellence in solar panel installations, energy audits, power backup systems, and much more.</p>
    </section>

    <section id="services" class="services">
        <h2>Our Services</h2>
        <ul>
            <li>Solar Panel Installations</li>
            <li>Solar Inverter Setups</li>
            <li>Battery Storage Systems</li>
            <li>Energy Audits and Consultancy</li>
            <li>Electrical Engineering Solutions</li>
        </ul>
    </section>

    <section id="portfolio" class="portfolio">
        <h2>Our Projects</h2>
        <div class="projects">
            <div class="project">
                <img src="https://source.unsplash.com/400x300/?solar,commercial" alt="Commercial Solar Project">
                <p>Commercial Solar Installation - Lagos</p>
            </div>
            <div class="project">
                <img src="https://source.unsplash.com/400x300/?solar,home" alt="Residential Solar Project">
                <p>Residential Solar Setup - Abuja</p>
            </div>
            <div class="project">
                <img src="https://source.unsplash.com/400x300/?solar,farm" alt="Solar Farm">
                <p>Solar Farm Deployment - Ogun State</p>
            </div>
        </div>
    </section>

    <section id="contact" class="contact">
        <h2>Contact Us</h2>
        <p>📞 07035416258 | 08060473621</p>
        <p>📧 <a href="mailto:jodansolarengr@gmail.com">jodansolarengr@gmail.com</a></p>
        <button onclick="openContactForm()">Send a Message</button>
    </section>

    <div id="contactFormModal" class="modal">
        <div class="modal-content">
            <span class="close" onclick="closeContactForm()">&times;</span>
            <h2>Get in Touch</h2>
            <form>
                <input type="text" placeholder="Your Name" required>
                <input type="email" placeholder="Your Email" required>
                <textarea placeholder="Your Message" required></textarea>
                <button type="submit">Send</button>
            </form>
        </div>
    </div>

    <footer>
        <p>&copy; 2025 Jodans Solar Engineering Services | Powered by the Sun ☀️</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
