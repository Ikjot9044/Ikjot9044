<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Singh's Auto Works</title>
    <link rel="stylesheet" href="styles.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
</head>
<body>
    <header>
        <div class="container">
            <h1>Singh's Auto Works</h1>
            <nav>
                <ul>
                    <li><a href="#home">Home</a></li>
                    <li><a href="#gallery">Custom Cars Gallery</a></li>
                    <li><a href="#accessories">Accessories</a></li>
                    <li><a href="#appointments">Appointments</a></li>
                    <li><a href="#contact">Contact Us</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <section id="home" class="hero">
        <div class="container">
            <h2>Welcome to Singh's Auto Works</h2>
            <p>Transforming Your Vehicles with Precision and Passion</p>
            <a href="#appointments" class="cta-button">Book an Appointment</a>
        </div>
    </section>

    <section id="gallery" class="gallery">
        <div class="container">
            <h2>Custom Cars Gallery</h2>
            <div class="gallery-slider">
                <div class="slide">
                    <img src="https://via.placeholder.com/800x400" alt="Custom Car 1">
                    <p>Custom Car 1 Description</p>
                </div>
                <div class="slide">
                    <img src="https://via.placeholder.com/800x400" alt="Custom Car 2">
                    <p>Custom Car 2 Description</p>
                </div>
                <!-- Add more slides as needed -->
            </div>
        </div>
    </section>

    <section id="accessories" class="accessories">
        <div class="container">
            <h2>Accessories</h2>
            <div class="accessories-list">
                <div class="accessory-item">
                    <img src="https://via.placeholder.com/400x300" alt="Accessory 1">
                    <h3>Accessory 1</h3>
                    <p>Description of accessory 1.</p>
                </div>
                <div class="accessory-item">
                    <img src="https://via.placeholder.com/400x300" alt="Accessory 2">
                    <h3>Accessory 2</h3>
                    <p>Description of accessory 2.</p>
                </div>
                <!-- Add more accessories as needed -->
            </div>
        </div>
    </section>

    <section id="appointments" class="appointments">
        <div class="container">
            <h2>Book an Appointment</h2>
            <form id="appointmentForm">
                <label for="name">Name:</label>
                <input type="text" id="name" name="name" required>

                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required>

                <label for="date">Preferred Date:</label>
                <input type="date" id="date" name="date" required>

                <label for="message">Additional Details:</label>
                <textarea id="message" name="message"></textarea>

                <button type="submit" class="cta-button">Submit</button>
            </form>
        </div>
    </section>

    <section id="contact" class="contact">
        <div class="container">
            <h2>Contact Us</h2>
            <div class="contact-info">
                <p><i class="fas fa-envelope"></i> Email: info@singhsautoworks.com</p>
                <p><i class="fas fa-phone"></i> Phone: (123) 456-7890</p>
                <p><i class="fas fa-map-marker-alt"></i> Address: 123 Garage Lane, City, Country</p>
            </div>
            <div id="map"></div>
        </div>
    </section>

    <footer>
        <div class="container">
            <p>&copy; 2024 Singh's Auto Works</p>
        </div>
    </footer>

    <script src="scripts.js"></script>
</body>
</html>
/* Reset some default styles */
body, h1, h2, h3, p, ul, li, form {
    margin: 0;
    padding: 0;
}

body {
    font-family: 'Arial', sans-serif;
    line-height: 1.6;
}

header {
    background: #333;
    color: #fff;
    padding: 1rem 0;
    position: fixed;
    width: 100%;
    top: 0;
    z-index: 1000;
}

header .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 1rem;
}

header h1 {
    margin: 0;
}

nav ul {
    display: flex;
    list-style: none;
}

nav ul li {
    margin-left: 1rem;
}

nav ul li a {
    color: #fff;
    text-decoration: none;
}

.hero {
    background: url('https://via.placeholder.com/1920x800') no-repeat center center/cover;
    color: #fff;
    text-align: center;
    padding: 100px 0;
    margin-top: 60px;
}

.hero h2 {
    font-size: 3rem;
    margin-bottom: 1rem;
}

.hero p {
    font-size: 1.5rem;
    margin-bottom: 2rem;
}

.cta-button {
    background: #e74c3c;
    color: #fff;
    padding: 0.5rem 1rem;
    text-decoration: none;
    border-radius: 5px;
}

.cta-button:hover {
    background: #c0392b;
}

.container {
    width: 90%;
    max-width: 1200px;
    margin: 0 auto;
}

.gallery-slider {
    display: flex;
    overflow: hidden;
    position: relative;
}

.slide {
    min-width: 100%;
    transition: transform 0.5s ease-in-out;
}

.slide img {
    width: 100%;
    height: auto;
}

.accessories {
    background: #f9f9f9;
    padding: 2rem 0;
}

.accessories-list {
    display: flex;
    flex-wrap: wrap;
}

.accessory-item {
    flex: 1 1 45%;
    margin: 1rem;
    background: #fff;
    padding: 1rem;
    border-radius: 8px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.accessory-item img {
    width: 100%;
    height: auto;
    border-radius: 8px;
}

.appointments form {
    display: flex;
    flex-direction: column;
}

.appointments label {
    margin-top: 1rem;
}

.appointments input, .appointments textarea {
    padding: 0.75rem;
    margin-bottom: 1rem;
    border: 1px solid #ddd;
    border-radius: 5px;
}

.contact {
    background: #fff;
    padding: 2rem 0;
}

.contact-info {
    font-size: 1.1rem;
}

.contact-info p {
    margin-bottom: 1rem;
}

#map {
    height: 300px;
    background: #eaeaea;
}

footer {
    background: #333;
    color: #fff;
    text-align: center;
    padding: 1rem 0;
    margin-top: 2rem;
}
document.addEventListener('DOMContentLoaded', function () {
    // Slider functionality
    const slides = document.querySelectorAll('.slide');
    let currentSlide = 0;

    function showSlide(index) {
        slides.forEach((slide, i) => {
            slide.style.transform = `translateX(${(i - index) * 100}%)`;
        });
    }

    function nextSlide() {
        currentSlide = (currentSlide + 1) % slides.length;
        showSlide(currentSlide);
    }

    setInterval(nextSlide, 3000); // Change slide every 3 seconds

    // Appointment form handling
    document.getElementById('appointmentForm').addEventListener('submit', function(event) {
        event.preventDefault();
        alert('Appointment request submitted!');
        // Handle form submission here, e.g., send data to server
    });
});
