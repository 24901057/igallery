# Ex.05 Design of Interactive Image Gallery
## Date: 06-05-2025

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
<html>
    <head>
        <title>Image Gallery</title>
        <style>
            body {
                font-family: Arial, sans-serif;
                display: flex;
                flex-direction: column;
                align-items: center;
                margin: 0;
                background-size: cover;
                background-image: url('bb2.jpg');
                padding: 15px;
                min-height: 100vh;
                position: relative;
                background-color: #f7f7f7;
            }
            h1 {
                margin-top: 20px;
                color: #ff4800;
                font-size: xx-large;
                font-weight: bold;
                text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2);
            }
            .gallery {
                display: grid;
                grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
                gap: 20px;
                max-width: 800px;
                width: 100%;
                margin-top: 30px;
                transition: all 0.3s ease-in-out;
            }
            .photo {
                display: flex;
                flex-direction: column;
                align-items: center;
                text-align: center;
                cursor: pointer;                   
                padding: 10px; 
                border-radius: 10px;
                background-color: whitesmoke;
                box-shadow: 0 3px 6px rgba(0, 0, 0, 0.1); 
                transition: background-color 0.3s ease, transform 0.3s ease;                    
                max-width: 120px; 
            }

            .photo:hover {
                transform: scale(1.05);
                background-color: #eaf8ff;
            }
            .photo img {
                width: 120px;
                height: 140px;
                border-radius: 8px;
                object-fit: cover;
                transition: transform 0.3s, box-shadow 0.3s ease;
            }

            .photo img:hover {
                transform: scale(1.1);
                box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);
            }
            .photo p {
                margin-top: 8px;
                font-size: 16px;
                color: #4f4f4f;
                font-weight: bold;
                transition: color 0.3s ease;
            }
            .photo:hover p {
                color: #ff7f50;
            }
            footer {
                position: absolute;
                bottom: 0;
                width: 100%;
                text-align: center;
                background-color: rgba(255, 255, 255, 0.8);
                color: #333;
                padding: 10px 0;
                font-size: 14px;
                box-shadow: 0 -4px 8px rgba(0, 0, 0, 0.1);
            }
        </style>
    </head>
    <body>
        <h1>Interactive Image Gallery</h1>
        <div class="gallery">
            <div class="photo" onclick="openImage('games.jpg')">
                <img src="games.jpg" alt="Games">
                <p>Games</p>
            </div>
            <div class="photo" onclick="openImage('movie.jpg')">
                <img src="movie.jpg" alt="Wednesday Addams">
                <p>Movies</p>
            </div>
            <div class="photo" onclick="openImage('book.jpg')">
                <img src="book.jpg" alt="Book">
                <p>Books</p>
            </div>
            <div class="photo" onclick="openImage('music.jpg')">
                <img src="music.jpg" alt="Music">
                <p>Music</p>
            </div>
            <div class="photo" onclick="openImage('birds.jpg')">
                <img src="birds.jpg" alt="Birds">
                <p>Birds</p>
            </div>
            <div class="photo" onclick="openImage('pets.jpg')">
                <img src="pets.jpg" alt="Pets">
                <p>Pets</p>
            </div>
            <div class="photo" onclick="openImage('animals.jpg')">
                <img src="animals.jpg" alt="Animals">
                <p>Animals</p>
            </div>
            <div class="photo" onclick="openImage('tourist.jpg')">
                <img src="tourist.jpg" alt="tourist">
                <p>Tourist</p>
            </div>
        </div>
        <footer>
            &copy; Designed and Developed by S.Thejashree.
        </footer>
        <script>
            function openImage(src) {
                const newWindow = window.open("", "_blank");
                newWindow.document.write(`
                    <html>
                        <head><title>Image Preview</title></head>
                        <body style="margin:0;display:flex;justify-content:center;align-items:center;height:100vh;background-color:#f7f7f7;">
                            <img src="${src}" style="max-width:90%;max-height:90%;border-radius:10px;box-shadow: 0px 4px 15px rgba(0, 0, 0, 0.2);">
                        </body>
                    </html>
                `);
            }
        </script>
    </body>
</html>

```
## OUTPUT:

![alt text](<Screenshot (32).png>)

## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
