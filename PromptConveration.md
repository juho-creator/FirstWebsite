# Creating the prompt for webpage 
## Prompt Engineering_1
I told chatgpt to create a prompt for writing the exact code for my website. 
<br />
<br />

#### You:
Write a prompt that will allow you to write the exact same code mentioned below. The functionality of the website should work exactly the same, and the file names should be identical too. Give me the prompt and confirm if you can write the exact same code without missing anything with me. Here's the code :
[Website code](index.html)

<br />

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

<br />
<br />
<br />

**Chatgpt was able to create a pretty damn good prompt! It was time to test it out!**

 
  
  

# Test_1
I tested the prompt from Prompt Engineering_1 
<br />
<br />

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
<br />

#### ChatGPT:
To recreate the webpage, you will need to create the following files:

1. index.html - The main HTML file.
2. styles.css - The CSS file for styling.
3. script.js - The JavaScript file for the functionality.

Here's the code for each file:

**index.html:**
```
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

<br />
<br />
<br />

**As you can see, chatgpt succeeded in giving me multiple codes for building the website. However, I wanted a single html code.
  So I made some changes to my prompt to give me a single html code**

<br />
<br />
<br />
<br />


# Prompt_Engineering2
To make Chatgpt to write down all the necessary code on one html file, I modified the prompt slightly by indicating that we already have the necessary files. This was done simply by adding **"We have all the necessary files."** at the very beginning of the previous prompt 
<br />
<br />


  
# Test_3
 Finally, I was able to create a single prompt for creating one html code of my website! 
  <br />

  #### You:
```
We have all the necessary files. You need to write an html code with specific functionality and file names. Below is the code for the webpage. The webpage is titled "Juho Kim's Website" and has the following functionality:

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
```

#### ChatGPT:
Sure! Here's the HTML code for the webpage with the specified functionality:

```
<!DOCTYPE html>
<html>
<head>
    <title>Juho Kim's Website</title>
    <style>
        body {
            background-color: #f2f2f2;
            font-family: Arial;
            text-align: center;
        }
        .container {
            max-width: 600px;
            margin: 0 auto;
        }
        #image {
            width: 300px;
            height: auto;
        }
        h1 {
            font-size: 32px;
            color: #333;
        }
        .no-underline {
            text-decoration: none;
        }
        .button {
            cursor: pointer;
        }
    </style>
</head>
<body>
    <div class="container">
        <img id="image" src="pepe-the-frog-head-pat.gif" alt="Funny Asian Man">
        <h1>Juho Kim</h1>
        <h2 id="age"></h2>
        <p>Passionate Programmer!</p>
        <p><a href="https://podcasters.spotify.com/pod/show/juhooray" class="no-underline" style="color: #0066cc;">Check out my AI-generated podcast!</a></p>
        <button class="button" onclick="changeBackgroundColor()">Surprise Me!</button>
    </div>

    <script>
        var isSurpriseActive = false;
        var audioFiles = ["audio1.mp3", "audio2.mp3", "audio3.mp3"];

        function changeBackgroundColor() {
            var body = document.body;
            body.classList.toggle("crazy-colors");

            var image = document.getElementById("image");
            if (isSurpriseActive) {
                image.src = "fast-cat-excited.gif";
            } else {
                image.src = "banana-cat-crying.gif";
            }
            isSurpriseActive = !isSurpriseActive;

            var audio = new Audio(audioFiles[Math.floor(Math.random() * audioFiles.length)]);
            audio.loop = true;
            audio.play();
        }
    </script>

    <script>
        var birthDate = new Date(2002, 9, 8); // Month is zero-based
        var currentDate = new Date();
        var age = currentDate.getFullYear() - birthDate.getFullYear();
        if (currentDate.getMonth() < birthDate.getMonth() ||
            (currentDate.getMonth() === birthDate.getMonth() && currentDate.getDate() < birthDate.getDate())) {
            age--;
        }
        var ageElement = document.getElementById("age");
        ageElement.innerText = "Age: " + age;
    </script>
</body>
</html>
```

Make sure to save this code in an HTML file, for example, `juho_kim_website.html`, and place the corresponding image files (`pepe-the-frog-head-pat.gif`, `fast-cat-excited.gif`, and `banana-cat-crying.gif`) and audio files (`audio1.mp3`, `audio2.mp3`, and `audio3.mp3`) in the same directory as the HTML file.

