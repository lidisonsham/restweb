# Ex.07 Restaurant Website
## Date: 17/05/2025

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
~~~
INDEX.HTML

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Virundhagam - Home</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body class="home">
  <nav>
    <ul>
      <li><a href="index.html">Home</a></li>
      <li><a href="menu.html">Menu</a></li>
      <li><a href="team.html">Team</a></li>
      <li><a href="contact.html">Contact</a></li>
    </ul>
  </nav>
  <header class="hero">
    <h1>Welcome to Virundhagam</h1>
    <p><b>Savor the authentic taste of India</b></p>
  </header>
</body>
</html>
 
 MENU.HTML

 <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Menu - Virundhagam</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body class="menu-page">
  <nav>
    <ul>
      <li><a href="index.html">Home</a></li>
      <li><a href="menu.html">Menu</a></li>
      <li><a href="team.html">Team</a></li>
      <li><a href="contact.html">Contact</a></li>
    </ul>
  </nav>
  <h1 class="page-title">Our Indian Specials</h1>
  <div class="menu-grid">
    <div class="menu-item"><img src="chickenbiryani-1.webp" alt="Biryani"><p>Hyderabadi Dum Biryani</p></div>
    <div class="menu-item"><img src="Shemins-Butter-Chicken-LR.jpg" alt="Butter Chicken"><p>Butter Chicken</p></div>
    <div class="menu-item"><img src="palak-panner.jpeg" alt="Palak Paneer"><p>Palak Paneer</p></div>
    <div class="menu-item"><img src="homemade-samosa-recipe1.jpg" alt="Samosa"><p>Punjabi Samosa</p></div>
    <div class="menu-item"><img src="dosa.jpg" alt="Dosa"><p>Masala Dosa</p></div>
    <div class="menu-item"><img src="chole-bhature.jpg" alt="Chole Bhature"><p>Chole Bhature</p></div>
    <div class="menu-item"><img src="Rajma-Chawal.jpg" alt="Rajma"><p>Rajma Chawal</p></div>
    <div class="menu-item"><img src="Rasmalai-recipe-01-500x375.jpg" alt="Rasmalai"><p>Rasmalai</p></div>
    <div class="menu-item"><img src="gulab-jamun-desi-ghee.jpg" alt="Gulab Jamun"><p>Gulab Jamun</p></div>
    <div class="menu-item"><img src="bhel-poori-gravy-re2.jpg" alt="Chaat"><p>Chennai Street Chaat</p></div>
  </div>
</body>
</html>

TEAM.HTML

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Our Team</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body class="team-page">
  <nav>
    <ul>
      <li><a href="index.html">Home</a></li>
      <li><a href="menu.html">Menu</a></li>
      <li><a href="team.html">Team</a></li>
      <li><a href="contact.html">Contact</a></li>
    </ul>
  </nav>
  <section class="team-section">
    <h2 style="text-align: center;">Meet Our Culinary Experts</h2>
    <div class="team-grid">
      <div class="team-member">
        <img src="manager.jpg" alt="Ahamed">
        <h3>Ahamed - Restaurant Manager</h3>
      </div>
      <div class="team-member">
        <img src="lead chef.jpg" alt="Chef Nishanth">
        <h3>Chef Nishanth - Head Chef</h3>
      </div>
      <div class="team-member">
        <img src="Sous chef.jpg" alt="Aakil">
        <h3>Aakil - Sous Chef</h3>
      </div>
      <div class="team-member">
        <img src="server.jpg" alt="Sanjaiganth">
        <h3>Sanjaiganth - Lead Server</h3>
      </div>
      <div class="team-member">
        <img src="chai expert.jpg" alt="Kevin">
        <h3>Kevin - Chai Expert</h3>
      </div>
      <div class="team-member">
        <img src="recepionist.jpg" alt="Jebin">
        <h3>Jebin - Receptionist</h3>
      </div>
    </div>
  </section>
</body>
</html>

CONTACT.HTML

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Our Team</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body class="team-page">
  <nav>
    <ul>
      <li><a href="index.html">Home</a></li>
      <li><a href="menu.html">Menu</a></li>
      <li><a href="team.html">Team</a></li>
      <li><a href="contact.html">Contact</a></li>
    </ul>
  </nav>
  <section class="team-section">
    <h2 style="text-align: center;">Meet Our Culinary Experts</h2>
    <div class="team-grid">
      <div class="team-member">
        <img src="manager.jpg" alt="Ahamed">
        <h3>Ahamed - Restaurant Manager</h3>
      </div>
      <div class="team-member">
        <img src="lead chef.jpg" alt="Chef Nishanth">
        <h3>Chef Nishanth - Head Chef</h3>
      </div>
      <div class="team-member">
        <img src="Sous chef.jpg" alt="Aakil">
        <h3>Aakil - Sous Chef</h3>
      </div>
      <div class="team-member">
        <img src="server.jpg" alt="Sanjaiganth">
        <h3>Sanjaiganth - Lead Server</h3>
      </div>
      <div class="team-member">
        <img src="chai expert.jpg" alt="Kevin">
        <h3>Kevin - Chai Expert</h3>
      </div>
      <div class="team-member">
        <img src="recepionist.jpg" alt="Jebin">
        <h3>Jebin - Receptionist</h3>
      </div>
    </div>
  </section>
</body>
</html>

STYLING.CSS

body {
  font-family: 'Segoe UI', sans-serif;
  margin: 0;
  background-color: #111;
  color: #eee;
}

nav {
  background-color: #000;
  padding: 15px;
  text-align: center;
}

nav ul {
  list-style: none;
  padding: 0;
}

nav ul li {
  display: inline-block;
  margin: 0 15px;
}

nav ul li a {
  color: #f2c94c;
  text-decoration: none;
  font-weight: bold;
}

.hero {
  background: url('images/hero_indian.jpg') no-repeat center center/cover;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.hero h1 {
  font-size: 70px;
  color: #f2c94c;
}

.hero p {
  font-size: 1.5rem;
  color: #ccc;
}

.page-title {
  text-align: center;
  font-size: 2.5rem;
  margin: 30px 0;
  color: #f2c94c;
}

.menu-grid, .team-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 20px;
  padding: 30px;
  text-align: center;
}

.menu-item, .team-member {
  background: #222;
  padding: 15px;
  border-radius: 12px;
  box-shadow: 0 4px 10px rgba(255, 255, 255, 0.1);
}

.menu-item img, .team-member img {
  width: 100%;
  height: 160px;
  object-fit: cover;
  border-radius: 10px;
}

.menu-item p, .team-member h3 {
  color: #f2c94c;
  margin-top: 10px;
}

.team-section h2 {
  color: #f2c94c;
}

.contact-page {
  background: url('images/contact_indian.jpg') no-repeat center center/cover;
  color: white;
}

~~~


## OUTPUT:

HOME 
![alt text](<Screenshot 2025-05-18 160723.png>)\
MENU
![alt text](<Screenshot 2025-05-18 160736.png>)
TEAM
![alt text](<Screenshot 2025-05-18 160750.png>)
CONTACT
![alt text](<Screenshot 2025-05-18 160958.png>)


## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
