/* General Styles */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
}

/* Navigation Bar */
.navbar {
    background-color: #333;
    padding: 10px;
}

.navbar ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
}

.navbar ul li {
    margin: 0 20px;
}

.navbar ul li a {
    color: white;
    text-decoration: none;
    font-size: 16px;
}

/* Main Content */
.main-content {
    display: flex;
    justify-content: space-between;
    padding: 20px;
}

/* Left Section */
.left {
    flex: 1;
    padding: 20px;
    background-color: #f4f4f4;
    margin-right: 20px;
}

/* Right Section */
.right {
    flex: 2;
    padding: 20px;
    background-color: #e2e2e2;
}

/* Grid Layout for Right Section */
.grid-container {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;
}

.grid-item {
    background-color: #ccc;
    padding: 20px;
    text-align: center;
}

/* Footer */
footer {
    text-align: center;
    background-color: #333;
    color: white;
    padding: 10px 0;
}

/* Media Queries for Responsiveness */
@media screen and (max-width: 768px) {
    .main-content {
        flex-direction: column;
        align-items: center;
    }

  .left, .right {
        flex: 1;
        margin-right: 0;
        margin-bottom: 20px;
    }

  .grid-container {
        grid-template-columns: repeat(2, 1fr);
    }

  .navbar ul {
        flex-direction: column;
    }

  .navbar ul li {
        margin-bottom: 10px;
    }
}

@media screen and (max-width: 480px) {
    .grid-container {
        grid-template-columns: 1fr;
    }

    .navbar ul {
        padding: 0;
    }
}

