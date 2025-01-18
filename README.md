# rifyn-website
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Rifyn - Solar made simple with no sales calls. Get your solar proposal in minutes.">
    <title>Rifyn - Solar Made Simple</title>
    <link rel="stylesheet" href="styles.css">
    <script src="script.js" defer></script>
</head>
<body>
    <!-- Header / Navbar -->
    <header>
        <div class="container">
            <div class="logo">
                <a href="/">Rifyn</a>
            </div>
            <nav>
                <ul>
                    <li><a href="#how-it-works">How It Works</a></li>
                    <li><a href="#about-us">About Us</a></li>
                    <li><a href="#contact-us">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="container">
            <h1>Regulated IT for You Now — Solar Made Simple</h1>
            <p>No salesmen, no cold calls. Just quick, transparent solar proposals tailored for your home.</p>
            <a href="#proposal-form" class="cta-button">Get Your Solar Proposal</a>
        </div>
    </section>

    <!-- How It Works Section -->
    <section id="how-it-works" class="how-it-works">
        <div class="container">
            <h2>How It Works</h2>
            <div class="steps">
                <div class="step">
                    <h3>1. Upload Your Bill</h3>
                    <p>Easily upload your electric bill to get started.</p>
                </div>
                <div class="step">
                    <h3>2. Confirm Home Ownership</h3>
                    <p>Verify that you're the homeowner.</p>
                </div>
                <div class="step">
                    <h3>3. Instant Proposal</h3>
                    <p>Get a personalized solar proposal instantly, with options to lease or finance.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Solar Proposal Form -->
    <section id="proposal-form" class="proposal-form">
        <div class="container">
            <h2>Get Your Solar Proposal</h2>
            <form id="solar-form">
                <label for="bill-upload">Upload Your Electric Bill</label>
                <input type="file" id="bill-upload" name="bill" required>

                <label for="home-owner">Confirm Home Ownership</label>
                <input type="checkbox" id="home-owner" required>
                <label for="home-owner">I confirm that I am the homeowner</label>

                <button type="submit" class="cta-button">Get My Proposal</button>
            </form>
            <div id="proposal-result" class="proposal-result" style="display:none;">
                <h3>Your Solar Proposal</h3>
                <p>Estimated Savings: $X per month</p>
                <p>Choose a financing option: Lease or Finance</p>
                <button>Request More Info</button>
            </div>
        </div>
    </section>

    <!-- About Us Section -->
    <section id="about-us" class="about-us">
        <div class="container">
            <h2>About Us</h2>
            <p>Rifyn is here to offer homeowners an easy, hassle-free solar experience. We believe in transparency, speed, and customer satisfaction. We've partnered with leading solar providers to offer competitive pricing and quick service.</p>
        </div>
    </section>

    <!-- Contact Us Section -->
    <section id="contact-us" class="contact-us">
        <div class="container">
            <h2>Contact Us</h2>
            <form id="contact-form">
                <label for="name">Name</label>
                <input type="text" id="name" name="name" required>

                <label for="email">Email</label>
                <input type="email" id="email" name="email" required>

                <label for="message">Message</label>
                <textarea id="message" name="message" required></textarea>

                <button type="submit" class="cta-button">Send Message</button>
            </form>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <p>&copy; 2025 Rifyn. All rights reserved.</p>
        </div>
    </footer>
</body>
</html>

/* Global Styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background-color: #fff;
    color: #333;
}

.container {
    width: 80%;
    margin: 0 auto;
}

header {
    padding: 20px 0;
    border-bottom: 1px solid #ccc;
}

header .logo a {
    font-size: 32px;
    text-decoration: none;
    color: #000;
}

nav ul {
    list-style: none;
    display: flex;
    justify-content: flex-end;
}

nav ul li {
    margin-left: 20px;
}

nav ul li a {
    text-decoration: none;
    color: #000;
    font-weight: bold;
}

.hero {
    background-color: #f0f0f0;
    padding: 60px 0;
    text-align: center;
}

.hero h1 {
    font-size: 36px;
    margin-bottom: 20px;
}

.hero p {
    font-size: 18px;
    margin-bottom: 20px;
}

.cta-button {
    background-color: #28a745;
    color: #fff;
    padding: 15px 30px;
    font-size: 18px;
    border: none;
    cursor: pointer;
    text-decoration: none;
}

.cta-button:hover {
    background-color: #218838;
}

.how-it-works {
    padding: 60px 0;
    background-color: #fafafa;
    text-align: center;
}

.how-it-works h2 {
    font-size: 32px;
    margin-bottom: 40px;
}

.steps {
    display: flex;
    justify-content: space-around;
}

.step {
    max-width: 250px;
}

.step h3 {
    font-size: 24px;
    margin-bottom: 10px;
}

.proposal-form {
    padding: 60px 0;
    text-align: center;
}

.proposal-form h2 {
    font-size: 32px;
    margin-bottom: 20px;
}

.proposal-form form {
    margin-top: 20px;
    text-align: left;
    display: inline-block;
}

.proposal-form label {
    font-size: 18px;
    display: block;
    margin: 10px 0 5px;
}

.proposal-form input, .proposal-form textarea {
    width: 300px;
    padding: 10px;
    margin-bottom: 15px;
    font-size: 16px;
    border: 1px solid #ccc;
    border-radius: 5px;
}

.proposal-result {
    margin-top: 20px;
}

.about-us, .contact-us {
    padding: 60px 0;
}

footer {
    padding: 20px 0;
    text-align: center;
    background-color: #f0f0f0;
    border-top: 1px solid #ccc;
}

/* Responsive Design */
@media (max-width: 768px) {
    .steps {
        flex-direction: column;
    }

    .step {
        margin-bottom: 20px;
    }

    .cta-button {
        width: 100%;
    }

    .proposal-form form {
        text-align: center;
    }
}
// Handle solar proposal form submission
document.getElementById('solar-form').addEventListener('submit', function(event) {
    event.preventDefault();

    const bill = document.getElementById('bill-upload').files[0];
    const isHomeowner = document.getElementById('home-owner').checked;

    if (!bill || !isHomeowner) {
        alert('Please upload your bill and confirm home ownership.');
        return;
    }

    // Simulate proposal generation (In production, this would be API-driven)
    document.getElementById('proposal-form').style.display = 'none';
    document.getElementById('proposal-result').style.display = 'block';
});

// Handle contact form submission (basic alert for demo)
document.getElementById('contact-form').addEventListener('submit', function(event) {
    event.preventDefault();
    alert('Your message has been sent. We will get back to you soon.');
});
