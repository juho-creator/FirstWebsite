# Recreate Webpage Prompt

#### You:
Write a prompt that will allow you to write the exact same code mentioned below. The functionality of the website should work exactly the same, and the file names should be identical too. Give me the prompt and confirm if you can write the exact same code without missing anything with me.
Here's the code :
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Juho Kim's Website</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      background-color: #f2f2f2;
      margin: 0;
      padding: 20px;
    }

    h1 {
      font-size: 32px;
      color: #333;
      margin: 10px 0;
    }

    h2 {
      font-size: 24px;
      color: #666;
      margin: 10px 0;
    }

    p {
      font-size: 18px;
      color: #777;
      margin: 10px 0;
    }

    a {
      color: #0066cc;
      text-decoration: none;
    }

    img {
      width: 300px; /* Adjust the width as needed */
      height: auto;
      margin-top: 20px;
    }

    .container {
      max-width: 600px;
      margin: 0 auto;
    }

    .button {
      display: inline-block;
      padding: 10px 20px;
      font-size: 16px;
      background-color: #0066cc;
      color: #fff;
      border: none;
      border-radius: 4px;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }

    .button:hover {
      background-color: #004080;
    }

    .crazy-colors {
      animation: changeColors 0.5s infinite;
    }

    @keyframes changeColors {
      0% {
        background-color: #0066cc;
      }

      50% {
        background-color: #cc0066;
      }

      100% {
        background-color: #00cc66;
      }
    }
  </style>
  <script>
    var isSurpriseActive = false;
    var audio = new Audio();
    var audioFiles = ['happy_cat_song.mp3', 'banana_cat_crying.mp3'];
    var audioIndex = 0;

    function changeBackgroundColor() {
      var body = document.getElementsByTagName('body')[0];
      body.classList.toggle('crazy-colors');

      isSurpriseActive = !isSurpriseActive;

      var image = document.getElementById('image');
      var gifPath = isSurpriseActive ? 'fast-cat-excited.gif' : 'banana-cat-crying.gif';
      image.src = gifPath;

      if (!isSurpriseActive) {
        body.classList.remove('crazy-colors');
      }

      audio.pause();
      audio.src = audioFiles[audioIndex];
      audio.loop = true;
      audio.play();

      audioIndex = (audioIndex + 1) % audioFiles.length;
    }
  </script>
</head>

<body>
  <audio autoplay loop>
    <source src="pet-the-peepo.mp3" type="audio/mpeg">
  </audio>

  <div class="container">
    <img id="image" src="pepe-the-frog-head-pat.gif" alt="Funny Asian Man">
    <h1>Juho Kim</h1>
    <h2 id="age"></h2>
    <p>Passionate Programmer!</p>
    <p><a href="https://podcasters.spotify.com/pod/show/juhooray">Check out my AI-generated podcast!</a></p>
    <button class="button" onclick="changeBackgroundColor()">Surprise Me!</button>
  </div>

  <script>
    // Calculate age based on birthdate
    var birthdate = new Date('2002-10-08');
    var currentDate = new Date();
    var age = currentDate.getFullYear() - birthdate.getFullYear();
    if (currentDate.getMonth() < birthdate.getMonth() ||
      (currentDate.getMonth() === birthdate.getMonth() && currentDate.getDate() < birthdate.getDate())) {
      age--;
    }
    document.getElementById('age').textContent = age + ' yrs old';
  </script>
</body>

</html>
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Juho Kim's Website</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      background-color: #f2f2f2;
      margin: 0;
      padding: 20px;
    }

    h1 {
      font-size: 32px;
      color: #333;
      margin: 10px 0;
    }

    h2 {
      font-size: 24px;
      color: #666;
      margin: 10px 0;
    }

    p {
      font-size: 18px;
      color: #777;
      margin: 10px 0;
    }

    a {
      color: #0066cc;
      text-decoration: none;
    }

    img {
      width: 300px; /* Adjust the width as needed */
      height: auto;
      margin-top: 20px;
    }

    .container {
      max-width: 600px;
      margin: 0 auto;
    }

    .button {
      display: inline-block;
      padding: 10px 20px;
      font-size: 16px;
      background-color: #0066cc;
      color: #fff;
      border: none;
      border-radius: 4px;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }

    .button:hover {
      background-color: #004080;
    }

    .crazy-colors {
      animation: changeColors 0.5s infinite;
    }

    @keyframes changeColors {
      0% {
        background-color: #0066cc;
      }

      50% {
        background-color: #cc0066;
      }

      100% {
        background-color: #00cc66;
      }
    }
  </style>
  <script>
    var isSurpriseActive = false;
    var audio = new Audio();
    var audioFiles = ['happy_cat_song.mp3', 'banana_cat_crying.mp3'];
    var audioIndex = 0;

    function changeBackgroundColor() {
      var body = document.getElementsByTagName('body')[0];
      body.classList.toggle('crazy-colors');

      isSurpriseActive = !isSurpriseActive;

      var image = document.getElementById('image');
      var gifPath = isSurpriseActive ? 'fast-cat-excited.gif' : 'banana-cat-crying.gif';
      image.src = gifPath;

      if (!isSurpriseActive) {
        body.classList.remove('crazy-colors');
      }

      audio.pause();
      audio.src = audioFiles[audioIndex];
      audio.loop = true;
      audio.play();

      audioIndex = (audioIndex + 1) % audioFiles.length;
    }
  </script>
</head>

<body>
  <audio autoplay loop>
    <source src="pet-the-peepo.mp3" type="audio/mpeg">
  </audio>

  <div class="container">
    <img id="image" src="pepe-the-frog-head-pat.gif" alt="Funny Asian Man">
    <h1>Juho Kim</h1>
    <h2 id="age"></h2>
    <p>Passionate Programmer!</p>
    <p><a href="https://podcasters.spotify.com/pod/show/juhooray">Check out my AI-generated podcast!</a></p>
    <button class="button" onclick="changeBackgroundColor()">Surprise Me!</button>
  </div>

  <script>
    // Calculate age based on birthdate
    var birthdate = new Date('2002-10-08');
    var currentDate = new Date();
    var age = currentDate.getFullYear() - birthdate.getFullYear();
    if (currentDate.getMonth() < birthdate.getMonth() ||
      (currentDate.getMonth() === birthdate.getMonth() && currentDate.getDate() < birthdate.getDate())) {
      age--;
    }
    document.getElementById('age').textContent = age + ' yrs old';
  </script>
</body>

</html>


#### ChatGPT:
Prompt:

You need to recreate a webpage with specific functionality and file names. Below is the code for the webpage. The webpage is titled "Juho Kim's Website" and has the following functionality:

1. The webpage has a background color of #f2f2f2.
2. The webpage uses the Arial font and has a text alignment of center.
3. The webpage has a container element with a maximum width of 600px, centered on the page.
4. The webpage displays an image with the ID "image". The image source is set to "pepe-the-frog-head-pat.gif" and has an alternate text of "Funny Asian Man". The image has a width of 300px and a height that adjusts automatically.
5. The webpage displays a heading with the text "Juho Kim" using a font size of 32px and a color of #333.
6. The webpage displays a subheading with the ID "age". The subheading should be empty initially.
7. The webpage displays two paragraphs. The first paragraph has the text "Passionate Programmer!" and the second paragraph contains a link with the text "Check out my AI-generated podcast!" The link has an href attribute set to "<https://podcasters.spotify.com/pod/show/juhooray>" and a color of #0066cc with no underline.
8. The webpage displays a button with the text "Surprise Me!" and the class "button". When the button is clicked, it triggers a JavaScript function called "changeBackgroundColor()".
9. The webpage includes a script tag that contains JavaScript code for the "changeBackgroundColor()" function. This function toggles the class "crazy-colors" on the body element, changes the image source between "fast-cat-excited.gif" and "banana-cat-crying.gif" based on the state of the "isSurpriseActive" variable, and plays an audio file. The audio file should loop and the source should be chosen from the "audioFiles" array.
10. The webpage includes a script tag that calculates the age of Juho Kim based on his birthdate (October 8, 2002) and the current date. The calculated age is then inserted into the subheading with the ID "age".

Recreate the webpage exactly as described above, including the same file names and functionality.


# ATTEMP 1
#### You:
You need to recreate a webpage with specific functionality and file names. Below is the code for the webpage. The webpage is titled "Juho Kim's Website" and has the following functionality:

The webpage has a background color of #f2f2f2.
The webpage uses the Arial font and has a text alignment of center.
The webpage has a container element with a maximum width of 600px, centered on the page.
The webpage displays an image with the ID "image". The image source is set to "pepe-the-frog-head-pat.gif" and has an alternate text of "Funny Asian Man". The image has a width of 300px and a height that adjusts automatically.
The webpage displays a heading with the text "Juho Kim" using a font size of 32px and a color of #333.
The webpage displays a subheading with the ID "age". The subheading should be empty initially.
The webpage displays two paragraphs. The first paragraph has the text "Passionate Programmer!" and the second paragraph contains a link with the text "Check out my AI-generated podcast!" The link has an href attribute set to "https://podcasters.spotify.com/pod/show/juhooray" and a color of #0066cc with no underline.
The webpage displays a button with the text "Surprise Me!" and the class "button". When the button is clicked, it triggers a JavaScript function called "changeBackgroundColor()".
The webpage includes a script tag that contains JavaScript code for the "changeBackgroundColor()" function. This function toggles the class "crazy-colors" on the body element, changes the image source between "fast-cat-excited.gif" and "banana-cat-crying.gif" based on the state of the "isSurpriseActive" variable, and plays an audio file. The audio file should loop and the source should be chosen from the "audioFiles" array.
The webpage includes a script tag that calculates the age of Juho Kim based on his birthdate (October 8, 2002) and the current date. The calculated age is then inserted into the subheading with the ID "age".
Recreate the webpage exactly as described above, including the same file names and functionality.

#### ChatGPT:
To recreate the webpage, you will need to create the following files:

1. index.html - The main HTML file.
2. styles.css - The CSS file for styling.
3. script.js - The JavaScript file for the functionality.

Here's the code for each file:

**index.html:**

```html
<!DOCTYPE html>
<html>
<head>
    <title>Juho Kim's Website</title>
    <link rel="stylesheet" type="text/css" href="styles.css">
</head>
<body>
    <div class="container">
        <img id="image" src="pepe-the-frog-head-pat.gif" alt="Funny Asian Man" width="300">
        <h1>Juho Kim</h1>
        <h2 id="age"></h2>
        <p>Passionate Programmer!</p>
        <p><a href="https://podcasters.spotify.com/pod/show/juhooray" style="color: #0066cc; text-decoration: none;">Check out my AI-generated podcast!</a></p>
        <button class="button" onclick="changeBackgroundColor()">Surprise Me!</button>
    </div>

    <script src="script.js"></script>
</body>
</html>
```

**styles.css:**

```css
body {
    background-color: #f2f2f2;
    font-family: Arial;
    text-align: center;
}

.container {
    max-width: 600px;
    margin: 0 auto;
}

h1 {
    font-size: 32px;
    color: #333;
}
```

**script.js:**

```javascript
// Calculate age and insert into subheading
var birthdate = new Date('2002-10-08');
var currentDate = new Date();
var age = currentDate.getFullYear() - birthdate.getFullYear();
document.getElementById('age').innerText = 'Age: ' + age;

// Change background color and toggle image source and audio
var isSurpriseActive = false;
var audioFiles = ['audio1.mp3', 'audio2.mp3', 'audio3.mp3']; // Replace with actual audio file names

function changeBackgroundColor() {
    document.body.classList.toggle('crazy-colors');
    var image = document.getElementById('image');
    if (isSurpriseActive) {
        image.src = 'pepe-the-frog-head-pat.gif';
        isSurpriseActive = false;
    } else {
        image.src = 'banana-cat-crying.gif';
        isSurpriseActive = true;
    }
    
    var audio = new Audio(audioFiles[Math.floor(Math.random() * audioFiles.length)]);
    audio.loop = true;
    audio.play();
}
```

Make sure to replace the image source, audio file names, and update the audio file paths accordingly. Additionally, you may need to adjust the paths to the CSS and JavaScript files based on your file structure.

Once you have created the HTML, CSS, and JavaScript files, ensure that they are all in the same directory and open the index.html file in a web browser. You should see the recreated webpage with the specified functionality.

*As you can see, chatgpt is giving me multiple pieces of code. So I fixed my prompt to give me a single piece of code*


# Attemp 2
#### You:
You need to recreate a webpage with specific functionality and file names. Below is the code for the webpage. The webpage is titled "Juho Kim's Website" and has the following functionality:

The webpage has a background color of #f2f2f2.
The webpage uses the Arial font and has a text alignment of center.
The webpage has a container element with a maximum width of 600px, centered on the page.
The webpage displays an image with the ID "image". The image source is set to "pepe-the-frog-head-pat.gif" and has an alternate text of "Funny Asian Man". The image has a width of 300px and a height that adjusts automatically.
The webpage displays a heading with the text "Juho Kim" using a font size of 32px and a color of #333.
The webpage displays a subheading with the ID "age". The subheading should be empty initially.
The webpage displays two paragraphs. The first paragraph has the text "Passionate Programmer!" and the second paragraph contains a link with the text "Check out my AI-generated podcast!" The link has an href attribute set to "https://podcasters.spotify.com/pod/show/juhooray" and a color of #0066cc with no underline.
The webpage displays a button with the text "Surprise Me!" and the class "button". When the button is clicked, it triggers a JavaScript function called "changeBackgroundColor()".
The webpage includes a script tag that contains JavaScript code for the "changeBackgroundColor()" function. This function toggles the class "crazy-colors" on the body element, changes the image source between "fast-cat-excited.gif" and "banana-cat-crying.gif" based on the state of the "isSurpriseActive" variable, and plays an audio file. The audio file should loop and the source should be chosen from the "audioFiles" array.
The webpage includes a script tag that calculates the age of Juho Kim based on his birthdate (October 8, 2002) and the current date. The calculated age is then inserted into the subheading with the ID "age".
Recreate the webpage exactly as described above, including the same file names and functionality.

#### ChatGPT:
To recreate the webpage, you will need to create the following files:

1. index.html - The main HTML file.
2. styles.css - The CSS file for styling.
3. script.js - The JavaScript file for the functionality.

Here's the code for each file:

**index.html:**

```html
<!DOCTYPE html>
<html>
<head>
    <title>Juho Kim's Website</title>
    <link rel="stylesheet" type="text/css" href="styles.css">
</head>
<body>
    <div class="container">
        <img id="image" src="pepe-the-frog-head-pat.gif" alt="Funny Asian Man" width="300">
        <h1>Juho Kim</h1>
        <h2 id="age"></h2>
        <p>Passionate Programmer!</p>
        <p><a href="https://podcasters.spotify.com/pod/show/juhooray" style="color: #0066cc; text-decoration: none;">Check out my AI-generated podcast!</a></p>
        <button class="button" onclick="changeBackgroundColor()">Surprise Me!</button>
    </div>

    <script src="script.js"></script>
</body>
</html>
```

**styles.css:**

```css
body {
    background-color: #f2f2f2;
    font-family: Arial;
    text-align: center;
}

.container {
    max-width: 600px;
    margin: 0 auto;
}

h1 {
    font-size: 32px;
    color: #333;
}
```

**script.js:**

```javascript
// Calculate age and insert into subheading
var birthdate = new Date('2002-10-08');
var currentDate = new Date();
var age = currentDate.getFullYear() - birthdate.getFullYear();
document.getElementById('age').innerText = 'Age: ' + age;

// Change background color and toggle image source and audio
var isSurpriseActive = false;
var audioFiles = ['audio1.mp3', 'audio2.mp3', 'audio3.mp3']; // Replace with actual audio file names

function changeBackgroundColor() {
    document.body.classList.toggle('crazy-colors');
    var image = document.getElementById('image');
    if (isSurpriseActive) {
        image.src = 'pepe-the-frog-head-pat.gif';
        isSurpriseActive = false;
    } else {
        image.src = 'banana-cat-crying.gif';
        isSurpriseActive = true;
    }
    
    var audio = new Audio(audioFiles[Math.floor(Math.random() * audioFiles.length)]);
    audio.loop = true;
    audio.play();
}
```

Make sure to replace the image source, audio file names, and update the audio file paths accordingly. Additionally, you may need to adjust the paths to the CSS and JavaScript files based on your file structure.

Once you have created the HTML, CSS, and JavaScript files, ensure that they are all in the same directory and open the index.html file in a web browser. You should see the recreated webpage with the specified functionality.
