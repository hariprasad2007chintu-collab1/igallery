# Ex.07 Design of Interactive Image Gallery
## Date:28.12.2025

## AIM:
To design a web application for an inteactive image gallery for a minimum five images with next and previous buttons.

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

## PROGRAM:
```
gallery.html

<html>
<head>
    <title>Interactive Image Gallery</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <h1>Interactive Image Gallery</h1>

    <div class="gallery-container">
        <img id="galleryImage" src="image1.png" alt="Gallery Image">

        <div class="buttons">
            <button id="prevBtn">Previous</button>
            <button id="nextBtn">Next</button>
        </div>
    </div>


    <footer>
        <p>Designed & Developed by HariPrasad A (25005271) 2025</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>

style.css

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

script.js

const images = [
    "image2.png",
    "image3.png",
    "image4.png",
];

let currentIndex = 0;

const galleryImage = document.getElementById("galleryImage");
const nextBtn = document.getElementById("nextBtn");
const prevBtn = document.getElementById("prevBtn");

nextBtn.addEventListener("click", () => {
    currentIndex = (currentIndex + 1) % images.length;
    galleryImage.src = images[currentIndex];
});

prevBtn.addEventListener("click", () => {
    currentIndex = (currentIndex - 1 + images.length) % images.length;
    galleryImage.src = images[currentIndex];
});


```
## OUTPUT:
<img width="582" height="392" alt="Screenshot 2025-12-28 183457" src="https://github.com/user-attachments/assets/8e6c3481-390d-4b4c-a883-cec9fecee91b" />
<img width="706" height="474" alt="Screenshot 2025-12-28 183520" src="https://github.com/user-attachments/assets/321c5f48-bb4c-4f07-a8c6-710f9da4a6bf" />
<img width="610" height="467" alt="Screenshot 2025-12-28 183537" src="https://github.com/user-attachments/assets/4a1a6d37-fc28-48c8-8171-340e1f9e78ea" />


## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
