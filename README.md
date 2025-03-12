HTML (index.html)

Save this as index.html:

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Modern Webpage</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>

    <header>
        <h1>My Website</h1>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section id="home" class="hero">
        <h2>Welcome to My Website</h2>
        <p>Your journey starts here.</p>
    </section>

    <section id="about" class="container">
        <h2>About Us</h2>
        <p>We provide quality services to make your life easier and more enjoyable.</p>
    </section>

    <section id="services" class="container">
        <h2>Our Services</h2>
        <div class="services">
            <div class="service">
                <h3>Web Design</h3>
                <p>We create stunning and responsive websites.</p>
            </div>
            <div class="service">
                <h3>SEO Optimization</h3>
                <p>Improve your online presence with our SEO services.</p>
            </div>
            <div class="service">
                <h3>Marketing</h3>
                <p>Grow your business with digital marketing strategies.</p>
            </div>
        </div>
    </section>

    <section id="contact" class="container">
        <h2>Contact Us</h2>
        <form>
            <input type="text" name="name" placeholder="Your Name" required>
            <input type="email" name="email" placeholder="Your Email" required>
            <textarea name="message" placeholder="Your Message" rows="5" required></textarea>
            <button type="submit">Send Message</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2025 My Website | All Rights Reserved</p>
    </footer>

</body>
</html>


---

CSS (styles.css)

Save this as styles.css:

/* Global Styles */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    background-color: #f5f5f5;
    color: #333;
}

/* Header */
header {
    background: #333;
    color: white;
    padding: 20px;
    text-align: center;
}

nav ul {
    list-style: none;
    padding: 0;
}

nav ul li {
    display: inline;
    margin: 0 15px;
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-size: 18px;
}

/* Hero Section */
.hero {
    background: url('https://source.unsplash.com/1600x900/?technology') no-repeat center center/cover;
    text-align: center;
    color: white;
    padding: 100px 20px;
}

.hero h2 {
    font-size: 36px;
}

/* Container */
.container {
    padding: 40px 20px;
    text-align: center;
}

.services {
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
    margin-top: 20px;
}

.service {
    background: white;
    padding: 20px;
    width: 30%;
    border-radius: 5px
