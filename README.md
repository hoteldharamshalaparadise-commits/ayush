# ayush
Ayush Health Paradise
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hotel Dharamshala Ayush Health Paradise | Wellness & Ayurveda Retreat</title>
    <style>
        :root {
            --primary: #2C5E3B;
            --primary-dark: #1E3F27;
            --accent: #D4A373;
            --light-bg: #F4F7F4;
            --text-dark: #333333;
            --text-light: #666666;
            --white: #FFFFFF;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            scroll-behavior: smooth;
        }

        body {
            color: var(--text-dark);
            background-color: var(--white);
            line-height: 1.6;
        }

        /* Header & Navigation */
        header {
            background: var(--white);
            box-shadow: 0 2px 10px rgba(0,0,0,0.08);
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            z-index: 1000;
        }

        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 2rem;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: var(--primary);
            text-decoration: none;
        }

        .logo span {
            color: var(--accent);
        }

        .nav-links {
            list-style: none;
            display: flex;
            gap: 2rem;
        }

        .nav-links a {
            text-decoration: none;
            color: var(--text-dark);
            font-weight: 600;
            transition: color 0.3s;
        }

        .nav-links a:hover {
            color: var(--primary);
        }

        .btn-book {
            background-color: var(--primary);
            color: var(--white);
            padding: 0.6rem 1.2rem;
            border-radius: 4px;
            text-decoration: none;
            font-weight: 600;
            transition: background 0.3s;
        }

        .btn-book:hover {
            background-color: var(--primary-dark);
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(0,0,0,0.4), rgba(0,0,0,0.4)), url('https://images.unsplash.com/photo-1540555700478-4be289fbecef?auto=format&fit=crop&w=1920&q=80') no-repeat center center/cover;
            height: 90vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: var(--white);
            padding: 0 1rem;
            margin-top: 70px;
        }

        .hero-content {
            max-width: 800px;
        }

        .hero h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
        }

        .hero p {
            font-size: 1.2rem;
            margin-bottom: 2rem;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.5);
        }

        .btn-main {
            background-color: var(--accent);
            color: var(--white);
            padding: 0.8rem 2rem;
            border-radius: 4px;
            text-decoration: none;
            font-weight: bold;
            font-size: 1.1rem;
            transition: background 0.3s;
        }

        .btn-main:hover {
            background-color: #bc8e60;
        }

        /* Section Layouts */
        section {
            padding: 5rem 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }

        .section-title {
            text-align: center;
            margin-bottom: 3rem;
        }

        .section-title h2 {
            font-size: 2.5rem;
            color: var(--primary);
            margin-bottom: 0.5rem;
        }

        .section-title p {
            color: var(--text-light);
            font-size: 1.1rem;
        }

        /* About / Philosophy */
        .about-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 3rem;
            align-items: center;
        }

        .about-text h3 {
            font-size: 1.8rem;
            color: var(--primary-dark);
            margin-bottom: 1rem;
        }

        .about-text p {
            color: var(--text-light);
            margin-bottom: 1.5rem;
        }

        .about-img img {
            width: 100%;
            border-radius: 8px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
        }

        /* Packages Grid */
        .packages-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 2rem;
        }

        .package-card {
            background: var(--light-bg);
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 4px 10px rgba(0,0,0,0.05);
            border-top: 4px solid var(--primary);
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }

        .package-header {
            background: var(--primary);
            color: var(--white);
            padding: 1.5rem;
            text-align: center;
        }

        .package-body {
            padding: 1.5rem;
            flex-grow: 1;
        }

        .package-body ul {
            list-style: none;
            margin-top: 1rem;
        }

        .package-body ul li {
            padding: 0.4rem 0;
            border-bottom: 1px solid #e0e0e0;
            font-size: 0.95rem;
        }

        .pricing {
            padding: 1.5rem;
            background: #eaeede;
            text-align: center;
            font-weight: bold;
            font-size: 1.2rem;
            color: var(--primary-dark);
        }

        /* Daily Schedule Table */
        .schedule-container {
            background: var(--light-bg);
            padding: 2rem;
            border-radius: 8px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.05);
        }

        .schedule-table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 1rem;
        }

        .schedule-table th, .schedule-table td {
            padding: 12px 15px;
            text-align: left;
            border-bottom: 1px solid #ddd;
        }

        .schedule-table th {
            background-color: var(--primary);
            color: var(--white);
        }

        .schedule-table tr:hover {
            background-color: rgba(44, 94, 59, 0.05);
        }

        /* Rooms Section */
        .rooms-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .room-card {
            background: var(--white);
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 4px 15px rgba(0,0,0,0.08);
            border: 1px solid #eee;
        }

        .room-img {
            height: 200px;
            background-size: cover;
            background-position: center;
        }

        .room-details {
            padding: 1.5rem;
        }

        .room-details h3 {
            color: var(--primary);
            margin-bottom: 0.5rem;
        }

        .room-price {
            font-size: 1.2rem;
            font-weight: bold;
            color: var(--accent);
            margin: 1rem 0;
        }

        /* Contact & Footer */
        .contact-section {
            background-color: var(--primary-dark);
            color: var(--white);
            padding: 4rem 2rem;
        }

        .contact-grid {
            max-width: 1200px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 3rem;
        }

        .contact-form input, .contact-form textarea {
            width: 100%;
            padding: 0.8rem;
            margin-bottom: 1rem;
            border: none;
            border-radius: 4px;
        }

        .contact-form button {
            background-color: var(--accent);
            color: var(--white);
            padding: 0.8rem 2rem;
            border: none;
            border-radius: 4px;
            font-weight: bold;
            cursor: pointer;
        }

        footer {
            background-color: #15271a;
            color: #aaa;
            text-align: center;
            padding: 1.5rem;
            font-size: 0.9rem;
        }

        @media (max-width: 768px) {
            .nav-links { display: none; }
            .about-grid, .contact-grid { grid-template-columns: 1fr; }
            .hero h1 { font-size: 2rem; }
        }
    </style>
</head>
<body>

    <!-- Header -->
    <header>
        <div class="nav-container">
            <a href="#" class="logo">Ayush Health <span>Paradise</span></a>
            <ul class="nav-links">
                <li><a href="#about">About Us</a></li>
                <li><a href="#packages">Health Packages</a></li>
                <li><a href="#schedule">Daily Schedule</a></li>
                <li><a href="#rooms">Rooms & Stay</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
            <a href="#contact" class="btn-book">Book Retreat</a>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="hero-content">
            <h1>Natural Healing, Yoga & Panchakarma</h1>
            <p>Experience holistic wellness, pure Sattvic lifestyle, and rejuvenation nestled in the peaceful mountains of Dharamshala.</p>
            <a href="#packages" class="btn-main">Explore Health Packages</a>
        </div>
    </section>

    <!-- About Section -->
    <section id="about">
        <div class="section-title">
            <h2>Welcome to Ayush Health Paradise</h2>
            <p>Your gateway to traditional Ayurveda, mental clarity, and deep relaxation.</p>
        </div>
        <div class="about-grid">
            <div class="about-text">
                <h3>A Sanctuary for Body, Mind & Soul</h3>
                <p>Set amidst serene natural environments near Dharamshala, our wellness centre blends classical Ayurvedic treatments, expert doctor consultations, therapeutic yoga sessions, and mindful meditation practices.</p>
                <p>Whether you seek relief from chronic stress, structured physical detoxification via Panchakarma, or a peaceful vacation escape, our team is dedicated to exceeding your wellness expectations.</p>
                <a href="#contact" class="btn-book">Get Free Consultation</a>
            </div>
            <div class="about-img">
                <img src="https://images.unsplash.com/photo-1506126613408-eca07ce68773?auto=format&fit=crop&w=800&q=80" alt="Yoga and meditation retreat landscape">
            </div>
        </div>
    </section>

    <!-- Health Packages Section -->
    <section id="packages" style="background-color: var(--light-bg);">
        <div class="section-title">
            <h2>Holistic Health Packages</h2>
            <p>Comprehensive healing routines complete with therapy, yoga, and organic nutrition.</p>
        </div>
        <div class="packages-grid">
            <!-- 7 Days Package -->
            <div class="package-card">
                <div class="package-header">
                    <h3>7 Days Wellness Program</h3>
                </div>
                <div class="package-body">
                    <p>Designed for complete rejuvenation, stress relief, and dosha balance.</p>
                    <ul>
                        <li>✓ Daily Morning & Evening Yoga</li>
                        <li>✓ Abhyanga (Full Body Oil Massage)</li>
                        <li>✓ Swedana (Herbal Steam Therapy)</li>
                        <li>✓ Rotation: Shirodhara / Basti / Udvartana</li>
                        <li>✓ Fresh Satvik Diet & Herbal Teas</li>
                    </ul>
                </div>
                <div class="pricing">
                    Shared: ₹25,000 | Individual: ₹32,000
                </div>
            </div>

            <!-- 10 Days Package -->
            <div class="package-card" style="border-top-color: var(--accent);">
                <div class="package-header" style="background-color: var(--accent);">
                    <h3>10 Days Healing Package</h3>
                </div>
                <div class="package-body">
                    <p>An extended program for deep cellular detoxification and structural recovery.</p>
                    <ul>
                        <li>✓ Extended Daily Yoga & Pranayama</li>
                        <li>✓ Daily Ayurvedic Therapeutic Massages</li>
                        <li>✓ Advanced Shirodhara & Kati Basti</li>
                        <li>✓ Wellness Talks & Meditation Sessions</li>
                        <li>✓ Complete Satvik Meal Routine</li>
                    </ul>
                </div>
                <div class="pricing">
                    Shared: ₹35,000 | Individual: ₹45,000
                </div>
            </div>
        </div>
    </section>

    <!-- Daily Schedule Section -->
    <section id="schedule">
        <div class="section-title">
            <h2>Typical Daily Schedule</h2>
            <p>A disciplined and harmonious rhythm designed to reset your biological clock.</p>
        </div>
        <div class="schedule-container">
            <table class="schedule-table">
                <thead>
                    <tr>
                        <th>Time</th>
                        <th>Activity / Program</th>
                    </tr>
                </thead>
                <tbody>
                    <tr><td>6:00 – 6:30 AM</td><td>Morning Meditation (Breath Awareness & Mindfulness)</td></tr>
                    <tr><td>6:30 – 7:30 AM</td><td>Yogasana Session (Gentle Stretching + Surya Namaskar)</td></tr>
                    <tr><td>7:30 – 8:00 AM</td><td>Herbal Tea & Rest</td></tr>
                    <tr><td>8:00 – 9:00 AM</td><td>Panchakarma Therapy – Abhyanga (Full Body Oil Massage)</td></tr>
                    <tr><td>9:00 – 10:00 AM</td><td>Swedana (Herbal Steam Therapy)</td></tr>
                    <tr><td>10:00 – 11:00 AM</td><td>Breakfast (Nourishing Satvik Diet)</td></tr>
                    <tr><td>11:00 – 12:00 PM</td><td>Relaxation / Nature Walk / Journaling</td></tr>
                    <tr><td>12:00 – 1:00 PM</td><td>Specialized Therapy (Shirodhara / Kati Basti / Udvartana)</td></tr>
                    <tr><td>1:00 – 2:00 PM</td><td>Lunch (Light Ayurvedic Diet)</td></tr>
                    <tr><td>4:00 – 5:00 PM</td><td>Evening Yoga & Pranayama (Nadi Shodhana, Bhramari)</td></tr>
                    <tr><td>7:00 – 7:30 PM</td><td>Guided Meditation / Yoga Nidra</td></tr>
                </tbody>
            </table>
        </div>
    </section>

    <!-- Rooms Section -->
    <section id="rooms" style="background-color: var(--light-bg);">
        <div class="section-title">
            <h2>Comfortable Rooms & Stay</h2>
            <p>Rest peacefully surrounded by clean mountain air and calm natural views.</p>
        </div>
        <div class="rooms-grid">
            <div class="room-card">
                <div class="room-img" style="background-image: url('https://images.unsplash.com/photo-1591088398332-8a7791972843?auto=format&fit=crop&w=600&q=80');"></div>
                <div class="room-details">
                    <h3>Deluxe Room</h3>
                    <p>Clean, cozy, and well-maintained room equipped with modern amenities for a relaxing stay.</p>
                    <div class="room-price">₹3,000 / night</div>
                    <a href="#contact" class="btn-book">Book Room</a>
                </div>
            </div>
            <div class="room-card">
                <div class="room-img" style="background-image: url('https://images.unsplash.com/photo-1582719478250-c89cae4dc85b?auto=format&fit=crop&w=600&q=80');"></div>
                <div class="room-details">
                    <h3>Family Suite</h3>
                    <p>Spacious accommodation featuring a scenic view, modern comfort, and high-speed internet.</p>
                    <div class="room-price">₹5,800 / night</div>
                    <a href="#contact" class="btn-book">Book Suite</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact-section">
        <div class="section-title" style="color: white;">
            <h2 style="color: white;">Connect With Us</h2>
            <p style="color: #ccc;">Book your health package or request a free doctor consultation today.</p>
        </div>
        <div class="contact-grid">
            <div>
                <h3>Hotel Dharamshala Ayush Health Paradise</h3>
                <p style="margin-top: 1rem; color: #ddd;">Located in Village Narwana Khas, near L&T Guest House, Dharamshala, Himachal Pradesh.</p>
                <p style="margin-top: 1rem; color: #ddd;"><strong>Phone:</strong> +91-8894109619</p>
                <p style="margin-top: 0.5rem; color: #ddd;"><strong>Email:</strong> hoteldharamshalaparadise@gmail.com</p>
            </div>
            <div class="contact-form">
                <input type="text" placeholder="Your Full Name">
                <input type="email" placeholder="Your Email Address">
                <input type="text" placeholder="Phone Number">
                <textarea rows="4" placeholder="Select Package or Inquiry Details..."></textarea>
                <button type="submit">Submit Request</button>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2026 Hotel Dharamshala Ayush Health Paradise. All rights reserved.</p>
    </footer>

</body>
</html>
