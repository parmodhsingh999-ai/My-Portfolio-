<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Parmodh Singh | Graphic Designer</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;700&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
    <style>
        :root {
            --bg-color: #0a0a0a;
            --accent-color: #007AFF; /* Apple Blue */
            --text-white: #ffffff;
            --glass: rgba(255, 255, 255, 0.05);
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-white);
            font-family: 'Inter', sans-serif;
            margin: 0;
            padding: 0;
            scroll-behavior: smooth;
        }

        /* --- Header --- */
        nav {
            padding: 20px 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: fixed;
            width: 90%;
            top: 0;
            z-index: 1000;
            backdrop-filter: blur(10px);
            background: rgba(10, 10, 10, 0.8);
        }

        .logo {
            font-family: 'Playfair Display', serif;
            font-size: 1.5rem;
            letter-spacing: 2px;
        }

        /* --- Hero Section --- */
        .hero {
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            background: radial-gradient(circle at center, #1a1a1a 0%, #0a0a0a 100%);
        }

        .hero h1 {
            font-size: clamp(3rem, 8vw, 6rem);
            margin: 0;
            font-family: 'Playfair Display', serif;
            background: linear-gradient(to right, #fff, #555);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        /* --- Services --- */
        .section-title { text-align: center; margin-bottom: 50px; font-size: 2.5rem; }
        
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
            padding: 50px 10%;
        }

        .service-card {
            background: var(--glass);
            padding: 40px;
            border-radius: 20px;
            border: 1px solid rgba(255,255,255,0.1);
            transition: 0.3s;
            text-align: center;
        }

        .service-card:hover {
            border-color: var(--accent-color);
            transform: translateY(-10px);
        }

        /* --- Contact Form --- */
        .contact-container {
            max-width: 600px;
            margin: 100px auto;
            padding: 40px;
            background: var(--glass);
            border-radius: 30px;
        }

        input, select, textarea {
            width: 100%;
            padding: 15px;
            margin: 10px 0;
            background: rgba(255,255,255,0.1);
            border: none;
            border-radius: 10px;
            color: white;
            box-sizing: border-box;
        }

        .btn {
            background: var(--accent-color);
            color: white;
            padding: 15px 30px;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            font-weight: bold;
            width: 100%;
            margin-top: 20px;
            transition: 0.3s;
        }

        .btn:hover { opacity: 0.8; }

        footer { text-align: center; padding: 50px; font-size: 0.9rem; color: #666; }

    </style>
</head>
<body>

    <nav>
        <div class="logo">PARMODH SINGH</div>
        <div>Contact: 7889810285</div>
    </nav>

    <section class="hero">
        <h1 data-aos="zoom-in">Graphic & Motion</h1>
        <p data-aos="fade-up" data-aos-delay="300">Premium Visual Identities by Parmodh Singh</p>
    </section>

    <h2 class="section-title">Exclusive Services</h2>
    <div class="services-grid">
        <div class="service-card" data-aos="fade-up">
            <h3>Logo Design</h3>
            <p>Minimalist and impactful brand marks.</p>
        </div>
        <div class="service-card" data-aos="fade-up" data-aos-delay="100">
            <h3>Motion Graphics</h3>
            <p>Smooth 2D/3D animations for your brand.</p>
        </div>
        <div class="service-card" data-aos="fade-up" data-aos-delay="200">
            <h3>UI/UX Design</h3>
            <p>Modern and user-friendly web interfaces.</p>
        </div>
    </div>

    <div class="contact-container" data-aos="flip-left">
        <h2 style="text-align: center;">Get in Touch</h2>
        <form action="#">
            <input type="text" placeholder="Full Name" required>
            <input type="email" placeholder="Email Address" required>
            <select>
                <option>Select Service</option>
                <option>Animation</option>
                <option>Branding</option>
                <option>Social Media</option>
            </select>
            <textarea rows="5" placeholder="Tell me about your project..."></textarea>
            <button type="submit" class="btn">Send Message</button>
        </form>
    </div>

    <footer>
        <p>Created for Parmodh Singh | Phone: 7889810285</p>
        <p>© 2026 Premium Design Studio</p>
    </footer>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });
    </script>
</body>
</html>
