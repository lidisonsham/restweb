# Ex.07 Restaurant Website
## Date:

## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
```

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gourmet Haven | Fine Dining Experience</title>
    <style>
        /* Global Styles */
        :root {
            --primary: #e63946;
            --secondary: #f1faee;
            --dark: #1d3557;
            --light: #a8dadc;
            --accent: #457b9d;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Playfair Display', serif;
        }
        
        body {
            background-color: #f8f9fa;
            color: #333;
            line-height: 1.6;
        }
        
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
        }
        
        /* Header Styles */
        header {
            background: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)), url('https://images.unsplash.com/photo-1517248135467-4c7edcad34c4?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80');
            background-size: cover;
            background-position: center;
            height: 100vh;
            color: white;
            display: flex;
            flex-direction: column;
            justify-content: center;
            text-align: center;
        }
        
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
            position: absolute;
            top: 0;
            width: 90%;
            max-width: 1200px;
        }
        
        .logo {
            font-size: 2rem;
            font-weight: 700;
            color: var(--secondary);
        }
        
        .nav-links {
            display: flex;
            list-style: none;
        }
        
        .nav-links li {
            margin-left: 30px;
        }
        
        .nav-links a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: all 0.3s ease;
        }
        
        .nav-links a:hover {
            color: var(--primary);
        }
        
        .hero-content {
            margin-top: 60px;
        }
        
        .hero-content h1 {
            font-size: 4rem;
            margin-bottom: 20px;
            animation: fadeIn 1.5s ease;
        }
        
        .hero-content p {
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto 30px;
            animation: fadeIn 2s ease;
        }
        
        .btn {
            display: inline-block;
            background: var(--primary);
            color: white;
            padding: 12px 30px;
            border: none;
            border-radius: 30px;
            font-size: 1rem;
            cursor: pointer;
            transition: all 0.3s ease;
            text-decoration: none;
            animation: fadeIn 2.5s ease;
        }
        
        .btn:hover {
            background: #c1121f;
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
        }
        
        /* Menu Section */
        .menu-section {
            padding: 100px 0;
            background-color: white;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 60px;
        }
        
        .section-title h2 {
            font-size: 2.5rem;
            color: var(--dark);
            position: relative;
            display: inline-block;
            padding-bottom: 15px;
        }
        
        .section-title h2::after {
            content: '';
            position: absolute;
            width: 50%;
            height: 3px;
            background-color: var(--primary);
            bottom: 0;
            left: 25%;
        }
        
        .menu-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .menu-item {
            background: #fff;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease;
        }
        
        .menu-item:hover {
            transform: translateY(-10px);
        }
        
        .menu-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }
        
        .menu-item-content {
            padding: 20px;
        }
        
        .menu-item-content h3 {
            font-size: 1.5rem;
            margin-bottom: 10px;
            color: var(--dark);
        }
        
        .menu-item-content p {
            color: #666;
            margin-bottom: 15px;
        }
        
        .price {
            font-weight: 700;
            color: var(--primary);
            font-size: 1.2rem;
        }
        
        /* About Section */
        .about-section {
            padding: 100px 0;
            background-color: var(--secondary);
        }
        
        .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 50px;
            align-items: center;
        }
        
        .about-text h2 {
            font-size: 2.5rem;
            color: var(--dark);
            margin-bottom: 20px;
        }
        
        .about-text p {
            margin-bottom: 20px;
            font-size: 1.1rem;
        }
        
        .about-image img {
            width: 100%;
            border-radius: 10px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
        }
        
        /* Contact Section */
        .contact-section {
            padding: 100px 0;
            background-color: white;
        }
        
        .contact-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 50px;
        }
        
        .contact-info h3 {
            font-size: 1.8rem;
            margin-bottom: 20px;
            color: var(--dark);
        }
        
        .contact-info p {
            margin-bottom: 15px;
            display: flex;
            align-items: center;
        }
        
        .contact-info i {
            margin-right: 10px;
            color: var(--primary);
        }
        
        .contact-form input,
        .contact-form textarea {
            width: 100%;
            padding: 15px;
            margin-bottom: 20px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 1rem;
        }
        
        .contact-form textarea {
            height: 150px;
        }
        
        /* Footer */
        footer {
            background-color: var(--dark);
            color: white;
            padding: 50px 0 20px;
            text-align: center;
        }
        
        .social-links {
            margin-bottom: 30px;
        }
        
        .social-links a {
            color: white;
            font-size: 1.5rem;
            margin: 0 15px;
            transition: all 0.3s ease;
        }
        
        .social-links a:hover {
            color: var(--primary);
        }
        
        .copyright {
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            padding-top: 20px;
        }
        
        /* Animations */
        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        /* Responsive Design */
        @media (max-width: 768px) {
            .hero-content h1 {
                font-size: 2.5rem;
            }
            
            .about-content {
                grid-template-columns: 1fr;
            }
            
            .about-image {
                order: -1;
            }
            
            nav {
                flex-direction: column;
            }
            
            .nav-links {
                margin-top: 20px;
            }
            
            .nav-links li {
                margin: 0 10px;
            }
        }
    </style>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css">
</head>
<body>
    <!-- Header/Hero Section -->
    <header>
        <nav class="container">
            <div class="logo">Gourmet Haven</div>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#menu">Menu</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
        
        <div class="hero-content container">
            <h1>Exquisite Dining Experience</h1>
            <p>Discover culinary perfection with our chef's seasonal creations, crafted from the finest locally-sourced ingredients</p>
            <a href="#menu" class="btn">View Our Menu</a>
        </div>
    </header>
    
    <!-- Menu Section -->
    <section id="menu" class="menu-section">
        <div class="container">
            <div class="section-title">
                <h2>Our Signature Dishes</h2>
            </div>
            
            <div class="menu-grid">
                <!-- Menu Item 1 -->
                <div class="menu-item">
                    <img src="https://images.unsplash.com/photo-1546069901-ba9599a7e63c?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Salmon Dish">
                    <div class="menu-item-content">
                        <h3>Pan-Seared Salmon</h3>
                        <p>Fresh Atlantic salmon with lemon butter sauce, seasonal vegetables, and herb-infused rice</p>
                        <span class="price">$28.50</span>
                    </div>
                </div>
                
                <!-- Menu Item 2 -->
                <div class="menu-item">
                    <img src="https://images.unsplash.com/photo-1512621776951-a57141f2eefd?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Salad Dish">
                    <div class="menu-item-content">
                        <h3>Mediterranean Salad</h3>
                        <p>Fresh greens with cherry tomatoes, cucumber, olives, feta cheese, and balsamic dressing</p>
                        <span class="price">$18.00</span>
                    </div>
                </div>
                
                <!-- Menu Item 3 -->
                <div class="menu-item">
                    <img src="https://images.unsplash.com/photo-1504674900247-0877df9cc836?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Pasta Dish">
                    <div class="menu-item-content">
                        <h3>Truffle Pasta</h3>
                        <p>Handmade pasta with wild mushrooms, truffle oil, parmesan, and fresh herbs</p>
                        <span class="price">$24.75</span>
                    </div>
                </div>
                
                <!-- Menu Item 4 -->
                <div class="menu-item">
                    <img src="https://images.unsplash.com/photo-1559847844-5315695dadae?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Steak Dish">
                    <div class="menu-item-content">
                        <h3>Filet Mignon</h3>
                        <p>8oz premium cut with red wine reduction, garlic mashed potatoes, and grilled asparagus</p>
                        <span class="price">$36.00</span>
                    </div>
                </div>
                
                <!-- Menu Item 5 -->
                <div class="menu-item">
                    <img src="https://images.unsplash.com/photo-1563805042-7684c019e1cb?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Dessert Dish">
                    <div class="menu-item-content">
                        <h3>Chocolate Soufflé</h3>
                        <p>Warm chocolate soufflé with vanilla bean ice cream and raspberry coulis</p>
                        <span class="price">$12.50</span>
                    </div>
                </div>
                
                <!-- Menu Item 6 -->
                <div class="menu-item">
                    <img src="https://images.unsplash.com/photo-1560717843-60cb77e8d2e6?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Wine Selection">
                    <div class="menu-item-content">
                        <h3>Wine Pairing</h3>
                        <p>Sommelier-selected wine pairing for each course (3 glasses)</p>
                        <span class="price">$25.00</span>
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <!-- About Section -->
    <section id="about" class="about-section">
        <div class="container">
            <div class="about-content">
                <div class="about-text">
                    <h2>Our Culinary Story</h2>
                    <p>Founded in 2010, Gourmet Haven has been serving exceptional cuisine in a warm, inviting atmosphere. Our executive chef, with over 20 years of international experience, creates dishes that blend traditional techniques with innovative flavors.</p>
                    <p>We pride ourselves on sourcing ingredients from local farmers and producers, ensuring the freshest seasonal offerings while supporting our community.</p>
                    <p>Our restaurant has been awarded the "Best Fine Dining Experience" by City Magazine for three consecutive years.</p>
                    <a href="#contact" class="btn">Reserve a Table</a>
                </div>
                <div class="about-image">
                    <img src="https://images.unsplash.com/photo-1581349485608-9469926a8e5e?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Restaurant Interior">
                </div>
            </div>
        </div>
    </section>
    
    <!-- Contact Section -->
    <section id="contact" class="contact-section">
        <div class="container">
            <div class="section-title">
                <h2>Make a Reservation</h2>
            </div>
            
            <div class="contact-container">
                <div class="contact-info">
                    <h3>Contact Information</h3>
                    <p><i class="fas fa-map-marker-alt"></i> 123 Culinary Street, Foodie City, FC 12345</p>
                    <p><i class="fas fa-phone"></i> (555) 123-4567</p>
                    <p><i class="fas fa-envelope"></i> info@gourmethaven.com</p>
                    <p><i class="fas fa-clock"></i> Open Tuesday-Sunday: 5:00 PM - 11:00 PM</p>
                    <div class="social-links">
                        <a href="#"><i class="fab fa-facebook-f"></i></a>
                        <a href="#"><i class="fab fa-instagram"></i></a>
                        <a href="#"><i class="fab fa-twitter"></i></a>
                    </div>
                </div>
                
                <div class="contact-form">
                    <form>
                        <input type="text" placeholder="Your Name" required>
                        <input type="email" placeholder="Your Email" required>
                        <input type="tel" placeholder="Phone Number">
                        <input type="date" placeholder="Date">
                        <input type="time" placeholder="Time">
                        <input type="number" placeholder="Number of Guests" min="1">
                        <textarea placeholder="Special Requests"></textarea>
                        <button type="submit" class="btn">Book Now</button>
                    </form>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="social-links">
                <a href="#"><i class="fab fa-facebook-f"></i></a>
                <a href="#"><i class="fab fa-instagram"></i></a>
                <a href="#"><i class="fab fa-twitter"></i></a>
                <a href="#"><i class="fab fa-yelp"></i></a>
            </div>
            <div class="copyright">
                <p>&copy; 2023 Gourmet Haven. All Rights Reserved.</p>
            </div>
        </div>
    </footer>
</body>
</html>
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/474e38e4-0fbf-4ecf-9108-910a44d4e42d)
![image](https://github.com/user-attachments/assets/63d030f8-9ffd-41ab-8b90-b2ba68b5fee8)


## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
