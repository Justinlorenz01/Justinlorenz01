Find what you need faster … Home is your new landing page and surfaces your most relevant files and folders
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Valentine's Day Question</title>
    <style>
        body {
            font-family: 'Old English Text MT', sans-serif;
            margin: 0;
            text-align: center;
            background-image: url(https://static.vecteezy.com/system/resources/previews/001/927/754/large_2x/paper-heart-on-pink-background-for-valentine-s-day-greeting-card-free-photo.jpg);
            background-size: 1920px 1080px;
            background-position: side;
            color: black; /* Change text color to contrast with the background */
        }

        h1 {
            color: #333;
            text-align: center; /* Center the text */
        }

        p {
            color: #666;
        }

        button {
            font-size: 16px;
            padding: 10px 20px;
            margin: 10px;
            cursor: pointer;
            border: none;
            border-radius: 5px;
        }

        /* Color for Yes button */
        button.yes {
            background-color: red;
            color: white;
        }

        /* Color for No button */
        button.no {
            background-color: green;
            color: white;
        }

        #response {
            font-size: 18px;
            margin: 20px;
            color: black; /* Set the font color to black */
        }

        /* Style for the GIF container */
        #gif-container {
            display: none; /* Hide by default */
            position: relative;
        }

        /* Style for the GIF image */
        #gif-image {
            max-width: 100%; /* Ensure it doesn't exceed the container width */
            max-height: 300px; /* Set a maximum height */
            mix-blend-mode: lighten; /* Blend mode to lighten the GIF with the background */
        }
    </style>
</head>

<body>
    <h1>Will you be my Valentine?</h1>

    <button class="yes" onclick="answer('Yes')">Yes</button>
    <button class="no" onclick="answer('No')">No</button>

    <!-- Container for the GIF -->
    <div id="gif-container">
        <!-- GIF image for Yes -->
        <img id="gif-image" src="https://i.pinimg.com/originals/8a/96/62/8a9662c17622af94d458485c8ee136d4.gif" alt="Yay GIF">
    </div>

    <p id="response"></p>

    <script>
        function answer(choice) {
            // Get the response element
            var responseElement = document.getElementById('response');

            // Get the GIF container element
            var gifContainer = document.getElementById('gif-container');

            // Get the GIF image element
            var gifImage = document.getElementById('gif-image');

            if (choice === 'Yes') {
                // Set the response text
                responseElement.innerHTML = 'Yay! ❤️😘';

                // Set the GIF source for Yes
                gifImage.src = 'https://i.pinimg.com/originals/8a/96/62/8a9662c17622af94d458485c8ee136d4.gif';
            } else {
                // Set the response text
                responseElement.innerHTML = 'Sad 😢';

                // Set the GIF source for No
                gifImage.src = 'https://c.tenor.com/HYjlr2O2riUAAAAC/milk-and-mocha-bear-comfort.gif';
            }

            // Show the GIF container
            gifContainer.style.display = 'block';
        }
    </script>
</body>

</html>
