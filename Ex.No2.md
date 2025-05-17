# Ex02 Commercial Website
## Date:

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
INDEX.HTML:
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>BookTech - Appointment Booking</title>
  <link rel="stylesheet" href="s.css" />
</head>
<body>

  <!-- Header -->
  <header class="header">
    <div class="container flex header-wrap">
      <div class="logo">
        <span class="logo-icon"></span>
        <span class="logo-text">Book<span class="highlight">Tech</span></span>
      </div>
      <nav>
        <ul class="nav flex">
          <li><a href="#">Home</a></li>
          <li><a href="#booking">Book Appointment</a></li>
          <li><a href="#about">About</a></li>
        </ul>
      </nav>
    </div>
  </header>

  <!-- Hero Section -->
  <section class="hero center flex-column">
    <h2>Professional Appointments Made Easy</h2>
    <p>Schedule your IT consultation in just a few clicks.</p>
    <a href="#booking" class="btn">Book Now</a>
  </section>

  <!-- Booking Form -->
  <section id="booking" class="booking container">
    <h3 class="section-title">Book an Appointment</h3>
    <form class="booking-form flex-column">
      <input type="text" placeholder="Full Name" required />
      <input type="email" placeholder="Email Address" required />
      <input type="tel" placeholder="Phone Number" required />
      <input type="date" required />
      <input type="time" required />
      <select required>
        <option value="">Select Service</option>
        <option>IT Consultation</option>
        <option>Software Development</option>
        <option>Cloud Setup</option>
      </select>
      <textarea rows="4" placeholder="Additional Notes"></textarea>
      <button type="submit" class="btn">Confirm Appointment</button>
    </form>
  </section>

  <!-- About -->
  <section id="about" class="about container flex">
    <div class="about-text">
      <h3>About BookTech</h3>
      <p>We are a leading provider of smart IT booking solutions. Our goal is to streamline your tech consultations through seamless online scheduling with our expert team.</p>
    </div>
  </section>

  <!-- Footer -->
  <footer class="footer center">
    <p>&copy; 2025 BookTech. All rights reserved.</p>
  </footer>

</body>
</html>
```

STYLE.CSS:
```

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Segoe UI', sans-serif;
  background: #fff;
  color: #333;
}

a {
  text-decoration: none;
  color: inherit;
}

ul {
  list-style: none;
}

.container {
  max-width: 1200px;
  margin: auto;
  padding: 0 20px;
}

.flex {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.flex-column {
  display: flex;
  flex-direction: column;
}

.center {
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.logo-icon {
  font-size: 2rem;
  margin-right: 8px;
}

.highlight {
  color: #0077cc;
}

.header {
  background: #1b1f3b;
  color: white;
  padding: 20px 0;
}

.nav {
  gap: 25px;
}

.nav a {
  color: white;
  padding: 8px 14px;
  transition: background 0.3s;
}

.nav a:hover {
  background: rgba(255, 255, 255, 0.2);
  border-radius: 5px;
}

.hero {
  background: linear-gradient(to right, #e0f7fa, #ffffff);
  padding: 100px 20px;
  flex-direction: column;
}

.hero h2 {
  font-size: 2.5rem;
  color: #1b1f3b;
  margin-bottom: 10px;
}

.hero p {
  font-size: 1.2rem;
  color: #555;
}

.btn {
  margin-top: 20px;
  padding: 12px 28px;
  background: #1b1f3b;
  color: white;
  border: none;
  border-radius: 5px;
  font-weight: bold;
  cursor: pointer;
  transition: background 0.3s;
}

.btn:hover {
  background: #2c365e;
}

.booking {
  padding: 80px 20px;
}

.section-title {
  text-align: center;
  font-size: 2rem;
  color: #1b1f3b;
  margin-bottom: 40px;
}

.booking-form {
  max-width: 600px;
  margin: auto;
  gap: 15px;
}

.booking-form input,
.booking-form select,
.booking-form textarea {
  padding: 12px;
  border: 1px solid #ccc;
  border-radius: 4px;
  font-size: 1rem;
  width: 100%;
}

.about {
  padding: 80px 20px;
  gap: 40px;
  flex-wrap: wrap;
}

.about-text {
  flex: 1;
  min-width: 300px;
}

.about-img {
  flex: 1;
  max-width: 400px;
  border-radius: 8px;
}

.footer {
  background: #1b1f3b;
  color: white;
  padding: 30px 0;
  font-size: 0.9rem;
}

@media (max-width: 768px) {
  .flex {
    flex-direction: column;
    gap: 20px;
  }

  .nav {
    flex-direction: column;
  }

  .about {
    text-align: center;
  }

  .about-img {
    width: 100%;
  }
}
```


## OUTPUT
![image](https://github.com/user-attachments/assets/921fb0d6-b9db-46b7-806a-d9f2ee0076f2)
![image](https://github.com/user-attachments/assets/7632ca8e-a803-4cf9-acd6-4f1fb98e5170)


## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
