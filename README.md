# Ex.08 Design of Interactive Image Gallery
## Date: 14/05/2025

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
image.html
<html>

<head>
    <title> Nostalgic cartoons </title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #db1a1a;
            margin: 0;
            padding: 0;

        }

        .gallery {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            padding: 20px;
            justify-content: center;
        }

        .gallery-item {
            margin: 20px;
            width: 300px;
            height: auto;
            cursor: pointer;
            border-radius: 15px;
            border: 2px solid #4bc8c8;
            transition: transform 0.01s;
        }

        .gallery-item:hover {
            transform: scale(1.2);
        }

        .modal {
            display: none;
            position: fixed;
            z-index: 1;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.8);
            justify-content: center;
            align-items: center;
        }

        .modal-content {
            max-width: 80%;
            max-height: 80%;
        }

        .close {
            position: absolute;
            top: 20px;
            right: 30px;
            font-size: 30px;
            color: rgb(167, 61, 61);
            cursor: pointer;
        }

        .back {
            background-color: rgb(14, 14, 14);
        }
    </style>
    <script>
        function openModal(image) {
            const modal = document.getElementById('imageModal');
            const modalImg = document.getElementById('modalImage');

            modal.style.display = "flex";
            modalImg.src = image.src;
        }
        function closeModal() {
            const modal = document.getElementById('imageModal');
            modal.style.display = "none";
        }
    </script>
</head>

<body class="back">

    <h1 align="center" style="font-family: Georgia, 'Times New Roman', Times, serif;color: rgb(246, 236, 233);">
        Nostalgic cartoons</h1>
    <div class="gallery">
        <br><br><br>
        <img src="sample 1.webp" alt="Image 1" class="gallery-item" onclick="openModal(this)">
        <img src="sample 2.webp" alt="Image 2" class="gallery-item" onclick="openModal(this)">
        <img src="sample 3.webp" alt="Image 3" class="gallery-item" onclick="openModal(this)">
        <img src="sample 4.webp" alt="Image 4" class="gallery-item" onclick="openModal(this)">
        <img src="sam 5.webp" alt="Image 5" class="gallery-item" onclick="openModal(this)">
        <img src="sam 6.webp" alt="Image 6" class="gallery-item" onclick="openModal(this)">
        
    </div>
    <div id="imageModal" class="modal" onclick="closeModal()">
        <span class="close">&times;</span>
        <img class="modal-content" id="modalImage">
    </div>

</body>

</html>
```

## OUTPUT:
![alt text](<Screenshot 2025-05-14 184000.png>)
![alt text](<Screenshot 2025-05-14 184038.png>)
![alt text](<Screenshot 2025-05-14 184051.png>)
## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
