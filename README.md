# My-account
Cafeshop
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Roasted Bean | Organic Coffee & Pastries</title>
    <style>
        /* CSS STYLES */
        :root {
            --primary: #4a332d;
            --accent: #d4a373;
            --light: #fefae0;
            --dark: #1a120b;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            background-color: var(--light);
            color: var(--dark);
            line-height: 1.6;
        }

        /* Navigation */
        nav {
            background: var(--primary);
            color: white;
            padding: 1rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        nav .logo { font-weight: bold; font-size: 1.5rem; letter-spacing: 1px; }
        nav ul { list-style: none; display: flex; margin: 0; }
        nav ul li { margin-left: 20px; }
        nav ul li a { color: white; text-decoration: none; font-size: 0.9rem; }

        /* Hero Section */
        header {
            background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)), 
                        url('https://images.unsplash.com/photo-1509042239860-f550ce710b93?auto=format&fit=crop&w=1200&q=80');
            background-size: cover;
            background-position: center;
            height: 80vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            color: white;
            text-align: center;
            padding: 0 20px;
        }

        header h1 { font-size: 3.5rem; margin-bottom: 10px; }
        header p { font-size: 1.2rem; margin-bottom: 25px; }
        .btn {
            background: var(--accent);
            color: var(--dark);
            padding: 12px 30px;
            text-decoration: none;
            font-weight: bold;
            border-radius: 5px;
        }

        /* Info Bar */
        .info-bar {
            background: var(--accent);
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            text-align: center;
            padding: 20px;
        }

        /* Menu Section */
        .menu { padding: 50px 20px; max-width: 800px; margin: auto; }
        .menu h2 { text-align: center; color: var(--primary); }
        .menu-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 30px; margin-top: 30px; }
        .menu-item { display: flex; justify-content: space-between; border-bottom: 1px solid #ccc; padding-bottom: 5px; }
        
        /* Footer */
        footer { background: var(--dark); color: white; text-align: center; padding: 40px 20px; }

        @media (max-width: 600px) {
            .menu-grid { grid-template-columns: 1fr; }
            header h1 { font-size: 2.5rem; }
            nav ul { display: none; } /* Simplified for mobile code example */
        }
    </style>
</head>
<body>

    <nav>
        <div class="logo">THE ROASTED BEAN</div>
        <ul>
            <li><a href="#menu">Menu</a></li>
            <li><a href="#location">Location</a></li>
            <li><a href="tel:5550123">Call Us</a></li>
        </ul>
    </nav>

    <header>
        <h1>Freshly Brewed Excellence</h1>
        <p>Crafting the perfect cup in the heart of the city since 2015.</p>
        <a href="#menu" class="btn">View Full Menu</a>
    </header>

    <section class="info-bar">
        <div>
            <strong>Hours</strong><br>
            Mon-Fri: 7am - 7pm
        </div>
        <div>
            <strong>Address</strong><br>
            456 Espresso Ave, Coffee Town
        </div>
        <div>
            <strong>Contact</strong><br>
            (555) 123-4567
        </div>
    </section>

    <section id="menu" class="menu">
        <h2>Our Favorites</h2>
        <div class="menu-grid">
            <div class="menu-item"><span>Caramel Macchiato</span> <strong>$4.50</strong></div>
            <div class="menu-item"><span>Cold Brew</span> <strong>$3.75</strong></div>
            <div class="menu-item"><span>Avocado Toast</span> <strong>$9.00</strong></div>
            <div class="menu-item"><span>Almond Croissant</span> <strong>$3.25</strong></div>
            <div class="menu-item"><span>Flat White</span> <strong>$4.00</strong></div>
            <div class="menu-item"><span>Chai Latte</span> <strong>$4.25</strong></div>
        </div>
    </section>

    <footer id="location">
        <h3>Visit Us Today</h3>
        <p>Come for the coffee, stay for the community.</p>
        <p>&copy; 2026 The Roasted Bean Cafe</p>
    </footer>

</body>
</html>
