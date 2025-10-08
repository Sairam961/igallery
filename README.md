# Ex.08 Design of Interactive Image Gallery
## Date: 8-10-2025

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
    <!DOCTYPE html>
    <html lang="en">
    <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Image Gallery</title>
    </head>
    <body>
    <header style="text-align: center; background-color: #333; color: white; padding: 1rem 0;">
        <h1>My favorite games</h1>
    </header>

    <div style="white-space: nowrap; overflow-x: auto; padding: 1rem;">
        <div style="display: inline-block; margin-right: 10px;" onclick="openModal(this)">
            <img width="202" height="250" alt="image" src="https://github.com/user-attachments/assets/a28423e4-11e8-442d-88e1-d0921c1b68c9" />

        </div>
        <div style="display: inline-block; margin-right: 10px;" onclick="openModal(this)">
            <img width="202" height="249" alt="image" src="https://github.com/user-attachments/assets/4e623c1c-7721-4a17-a872-234297f5c006" />

        </div>
        <div style="display: inline-block; margin-right: 10px;" onclick="openModal(this)"> 
        <img width="196" height="257" alt="image" src="https://github.com/user-attachments/assets/f784b333-1f06-4183-9482-27027bbe28b8" />

        </div>
        <div style="display: inline-block;" onclick="openModal(this)"> 
        <img width="194" height="259" alt="image" src="https://github.com/user-attachments/assets/9873ff4e-c4fb-4862-bb47-6efb84c8f839" />

        </div>
    </div>

    <div id="modal" style="display: none; position: fixed; z-index: 1; left: 0; top: 0; width: 100%; height: 100%; background-color: rgba(0,0,0,0.9);">
        <span style="position: absolute; top: 15px; right: 35px; color: white; font-size: 40px; font-weight: bold; cursor: pointer;" onclick="closeModal()">&times;</span>
        <img id="modalImage" style="display: block; margin: 5% auto; max-width: 80%;">
    </div>

    <script>
        function openModal(element) {
            var modal = document.getElementById("modal");
            var modalImg = document.getElementById("modalImage");
            modal.style.display = "block";
            modalImg.src = element.querySelector("img").src;
        }

        function closeModal() {
            document.getElementById("modal").style.display = "none";
        }
    </script>
</body>
</html>

## OUTPUT:

## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
