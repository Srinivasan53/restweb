# Ex.07 Restaurant Website
## Date:12.12.24

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
        <title>Admin Dashboard - Velvet Bistro</title>
        <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&family=Roboto:wght@300;400;500&family=Gloock&display=swap" rel="stylesheet">
        <style>
            body {
                font-family: 'Roboto', sans-serif;
                margin: 0;
                padding: 0;
                background-color: black;
                color: white;
            }

            .header {
                background-color: black;
                padding: 15px 30px;
                display: flex;
                justify-content: space-between;
                align-items: center;
                color: whitesmoke;
            }

            .header .logo h1 {
                margin: 0;
                font-family: 'Poppins', sans-serif;
                font-size: 26px;
            }

            .header .logo img {
                height: 40px;
                width: auto;
                margin-left: 10px;
            }

            .header .search-bar input {
                padding: 10px;
                width: 350px;
                border-radius: 20px;
                border: 1px solid grey;
                margin-right: 10px;
                font-size: 1em;
                background-color: bla;
                color: white;
            }

            .header .search-bar button {
                padding: 10px 20px;
                background-color: orange;
                border: none;
                cursor: pointer;
                border-radius: 5px;
                font-size: 1em;
                color: white;
            }

            .nav {
                background-color: grey;
                color: white;
                padding: 15px 0;
            }

            .nav ul {
                display: flex;
                justify-content: center;
                list-style: none;
                margin: 0;
                padding: 0;
            }

            .nav ul li {
                margin: 0 25px;
                cursor: pointer;
            }

            .nav ul li a {
                text-decoration: none;
                color: white;
                font-size: 1.1em;
                transition: color 0.3s;
            }

            .nav ul li a:hover {
                color: orange;
            }

            .admin-dashboard {
                padding: 60px 30px;
                text-align: center;
                background-color: black;
                margin: 30px 0;
                border-bottom: 5px solid orange;
            }

            .admin-dashboard h2 {
                font-family: 'Gloock', sans-serif;
                font-size: 3.5em;
                color: orange;
                margin-bottom: 20px;
                text-transform: uppercase;
            }

            .admin-dashboard p {
                font-size: 1.1em;
                color: grey;
                margin-bottom: 30px;
            }

            .admin-team {
                display: flex;
                justify-content: space-around;
                flex-wrap: wrap;
                margin-top: 40px;
            }

            .admin-card {
                background-color: green;
                width: 250px;
                margin: 20px;
                padding: 20px;
                text-align: center;
                border-radius: 10px;
                box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
                transition: transform 0.3s;
            }

            .admin-card:hover {
                transform: translateY(-10px);
            }

            .admin-card img {
                width: 100px;
                height: 100px;
                border-radius: 50%;
                object-fit: cover;
                margin-bottom: 15px;
            }

            .admin-card h3 {
                color: peru;
                font-size: 1.5em;
                margin-bottom: 10px;
            }

            .admin-card p {
                color: white;
                font-size: 1em;
                margin-bottom: 15px;
            }

            .admin-card .position {
                font-size: 1.1em;
                color: cyan;
            }

            footer {
                background-color: black;
                color: whitesmoke;
                padding: 20px 0;
                text-align: center;
            }

            footer a {
                color: peachpuff;
                text-decoration: none;
                margin: 0 10px;
            }

            footer a:hover {
                text-decoration: underline;
            }
        </style>
    </head>
    <body>
        <header class="header">
            <div class="logo">
                <img src="logo (2).jpg" alt="logo">
                <h1>Velvet Bistro</h1>
            </div>
            <div class="search-bar">
                <input type="text" placeholder="Search for reservations...">
                <button>Search</button>
            </div>
        </header>

        <nav class="nav">
            <ul>
                <li><a href="home.html">Home</a></li>
                <li><a href="menu.html">Menu</a></li>
                <li><a href="reservation.html">Make a Reservation</a></li>
                <li><a href="contact.html">Contact Us</a></li>
                <li><a href="admin.html">Admin Dashboard</a></li>
            </ul>
        </nav>

        <section class="admin-dashboard">
            <h2>Admin Dashboard</h2>
            <p>Manage your restaurant's reservations, menu, and staff. Welcome, admin!</p>

            <div class="admin-team">
                <!-- Admin 1 -->
                <div class="admin-card">
                    <img src="admin1.jpeg" alt="Admin 1">
                    <h3>Srinivasan S</h3>
                    <p class="position">CEO</p>
                    <p>Responsible for overall functioning of the restaurant setting and executing the organization's strategy, allocating capital, and building and overseeing the executive team.</p>
                </div>

                <!-- Admin 2 -->
                <div class="admin-card">
                    <img src="admin2.jpg" alt="Admin 2">
                    <h3>Koushik Shankar</h3>
                    <p class="position">Chef</p>
                    <p>Head of kitchen operations, ensuring quality control, menu design, and food preparation standards.</p>
                </div>

                <!-- Admin 3 -->
                <div class="admin-card">
                    <img src="admin3.jpg" alt="Admin 3">
                    <h3>Damodharan Kothandaraman</h3>
                    <p class="position">Reservation Manager</p>
                    <p>Manages all reservations, coordinates with guests, and ensures smooth seating arrangements.</p>
                </div>

                <!-- Admin 4 -->
                <div class="admin-card">
                    <img src="admin4.jpg" alt="Admin 4">
                    <h3>Venkatesh Bhat</h3>
                    <p class="position">Marketing Manager</p>
                    <p>Handles restaurant promotions, social media presence, and marketing campaigns.</p>
                </div>

                <!-- Admin 5 -->
                <div class="admin-card">
                    <img src="admin5.jpg" alt="Admin 5">
                    <h3>Madhampatty Rangaraj









                    </h3>
                    <p class="position">Operations Manager</p>
                    <p>Responsible for maintaining restaurant operations, supplies, and day-to-day management.</p>
                </div>
            </div>
        </section>

        <footer>
            <p>&copy; 2024 Velvet Bistro | <a href="privacy.html">Privacy Policy</a> | <a href="terms.html">Terms & Conditions</a></p>
        </footer>
    </body>
</html>

```

## OUTPUT:
![alt text](<srini/Screenshot (709).png>)
![alt text](<srini/Screenshot (710).png>)
![alt text](<srini/Screenshot (711).png>)
![alt text](<srini/Screenshot (712).png>)
![alt text](<srini/Screenshot (713).png>)
## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
