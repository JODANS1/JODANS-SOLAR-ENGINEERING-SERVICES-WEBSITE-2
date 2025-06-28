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
body {
    margin: 0;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background-color: #f4f6f8;
    color: #333;
}

header {
    background-color: #ff9800;
    padding: 15px 40px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

header .logo {
    font-size: 1.8em;
    color: white;
    font-weight: bold;
    text-transform: uppercase;
    animation: slideIn 1s ease-out;
}

nav ul {
    display: flex;
    gap: 15px;
    list-style: none;
    margin: 0;
    padding: 0;
}

nav a {
    text-decoration: none;
    color: white;
    font-weight: bold;
    transition: color 0.3s;
}

nav a:hover {
    color: #333;
}

.hero {
    text-align: center;
    padding: 100px 20px;
    color: white;
    background-image: url('https://source.unsplash.com/1600x700/?solar,energy');
    background-size: cover;
    background-position: center;
    position: relative;
    overflow: hidden;
}

.hero::after {
    content: "";
    position: absolute;
    top: 0; left: 0; right: 0; bottom: 0;
    background: rgba(0,0,0,0.5);
}

.hero h1, .hero p, .hero button {
    position: relative;
    z-index: 1;
    animation: fadeInDown 1s ease-in;
}

.hero button {
    background-color: #ffc107;
    color: black;
    padding: 12px 25px;
    border: none;
    cursor: pointer;
    font-weight: bold;
    margin-top: 10px;
    transition: background 0.3s, transform 0.2s;
}

.hero button:hover {
    background-color: #ff9800;
    transform: scale(1.05);
}

section {
    padding: 60px 20px;
    max-width: 1200px;
    margin: auto;
    text-align: center;
}

.services ul {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
    gap: 10px;
    list-style: none;
    padding: 0;
}

.services li {
    background: #fff8e1;
    padding: 15px;
    border-radius: 8px;
    transition: transform 0.3s;
}

.services li:hover {
    transform: translateY(-5px);
}

.projects {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
}

.project img {
    width: 100%;
    border-radius: 10px;
    transition: transform 0.3s ease, box-shadow 0.3s;
}

.project img:hover {
    transform: scale(1.05);
    box-shadow: 0 8px 16px rgba(0,0,0,0.3);
}

footer {
    background-color: #333;
    color: white;
    padding: 20px;
    text-align: center;
}

/* Animations */
@keyframes slideIn {
    from { transform: translateX(-100px); opacity: 0; }
    to { transform: translateX(0); opacity: 1; }
}

@keyframes fadeInDown {
    from { opacity: 0; transform: translateY(-20px); }
    to { opacity: 1; transform: translateY(0); }
}

/* Modal Styles */
.modal {
    display: none;
    position: fixed;
    z-index: 1000;
    left: 0; top: 0;
    width: 100%; height: 100%;
    background-color: rgba(0,0,0,0.7);
}

.modal-content {
    background: white;
    margin: 10% auto;
    padding: 20px;
    width: 90%;
    max-width: 400px;
    border-radius: 8px;
}

.modal-content input,
.modal-content textarea {
    width: 100%;
    padding: 10px;
    margin: 10px 0;
}

.modal-content button {
    background-color: #ff9800;
    border: none;
    padding: 10px 20px;
    cursor: pointer;
    color: white;
    font-weight: bold;
}

.close {
    float: right;
    cursor: pointer;
    font-size: 1.5em;
}
