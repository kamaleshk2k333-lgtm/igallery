# Ex.07 Design of Interactive Image Gallery
## Date:7-1-2026

## AIM:
To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for positioning and styling.

### Step 4:
Write JavaScript program for implementing interactivity.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
index.html:

<html>
<head>

    <title>Interactive Image Gallery</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header>
        <h1>Interactive Image Gallery</h1>
    </header>

    <div class="gallery-container">
        <img id="galleryImage" src="die.jpeg" alt="Gallery Image">
        <p id="caption">3D Printing Lab</p>

        <div class="buttons">
            <button onclick="prevImage()">Previous</button>
            <button onclick="nextImage()">Next</button>
        </div>
    </div>

    <footer>
        Designed & Developed by Kamalesh Kumar . &copy; 2025
    </footer>

    <script src="scripts.js"></script>
</body>
</html>

scripts.js

let images = [
    {
        src: "die.jpeg",
        caption: "Diablo"
    },
    {
        src: "asta.jpeg",
        caption: "asta"
    },
    {
        src: "eee.jpeg",
        caption: "Gingka"
    }
];

let currentIndex = 0;

function showImage() {
    document.getElementById("galleryImage").src = images[currentIndex].src;
    document.getElementById("caption").innerText = images[currentIndex].caption;
}

function nextImage() {
    currentIndex++;
    if (currentIndex >= images.length) {
        currentIndex = 0;
    }
    showImage();
}

function prevImage() {
    currentIndex--;
    if (currentIndex < 0) {
        currentIndex = images.length - 1;
    }
    showImage();
}

style.css:

body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f4;
    text-align: center;
}

h1 {
    margin-top: 20px;
}

.gallery-container {
    width: 500px;
    margin: 30px auto;
    background: white;
    padding: 15px;
    border-radius: 10px;
    box-shadow: 0 0 10px rgba(0,0,0,0.2);
}

.gallery-container img {
    width: 100%;
    height: 300px;
    object-fit: cover;
    border-radius: 5px;
}

.buttons {
    margin-top: 15px;
}

button {
    padding: 10px 20px;
    font-size: 16px;
    margin: 5px;
    border: none;
    border-radius: 5px;
    background-color: #007bff;
    color: white;
    cursor: pointer;
}

button:hover {
    background-color: #0056b3;
}
footer {
    margin-top: auto;
    background-color: #333;
    color: white;
    padding: 15px 0;
    font-size: 14px;
}
footer a {
    color: #ffcc00;
    text-decoration: none;
}
footer a:hover {
    text-decoration: underline;
}
footer {
    margin-top: auto;
    background-color: #333;
    color: white;
    padding: 15px 0;
    font-size: 14px;
}
footer a {
    color: #ffcc00;
    text-decoration: none;
}
footer a:hover {
    text-decoration: underline;
}
footer {
    margin-top: auto;
    background-color: #333;
    color: white;
    padding: 15px 0;
    font-size: 14px;
}
footer a {
    color: #ffcc00;
    text-decoration: none;
}
footer a:hover {
    text-decoration: underline;
}
```

## OUTPUT:

<img width="1919" height="1079" alt="Screenshot 2026-01-07 215145" src="https://github.com/user-attachments/assets/2701270d-3445-4481-abaf-b7f2202e9125" />
<img width="1919" height="1079" alt="Screenshot 2026-01-07 215126" src="https://github.com/user-attachments/assets/e2bdee9d-dc99-4d25-bd3e-f9a89f555a3c" />
<img width="1919" height="1079" alt="Screenshot 2026-01-07 215056" src="https://github.com/user-attachments/assets/e652b784-cd12-4fc6-b8d7-c1df460cc58f" />


## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
