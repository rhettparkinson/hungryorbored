# hungryorbored.com

A simple web application that tells you if you're hungry, bored, or something else entirely.

## Project Setup

### Step 1: Create the Basic HTML Structure

The initial step was to create a basic HTML file with a structure that includes a heading, a placeholder where the random response will be displayed, and sections for future CSS and JavaScript.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta
      name="viewport"
      content="width=device-width, initial-scale=1.0"
    />
    <title>Are You Hungry or Just Bored?</title>
    <style>
      /* CSS will be added here */
    </style>
  </head>
  <body>
    <h1>Are You Hungry or Bored?</h1>
    <p id="response"></p>

    <script>
      // JavaScript will go here
    </script>
  </body>
</html>
```

### Step 2: Set up Git Respository

Create an empty respository on GitHub, and then in the command line:

```sh
git init
git remote add origin git@github.com:rhettparkinson/hungryorbored.git
git add .
git commit -m "Initial commit"
git branch -M main
git push -u origin main
```

### Step 3: Add JavaScript to Display Random Response

Added JavaScript within the HTML file to randomly select and display one of the predefined responses when the page loads.

```html
<script>
  // Array of responses
  const responses = ["hungry", "bored", "both", "hangry", "go to bed"];

  // Function to get a random response
  function getRandomResponse() {
    const randomIndex = Math.floor(Math.random() * responses.length);
    return responses[randomIndex];
  }

  // Function to display a random response
  function displayResponse() {
    const responseParagraph = document.getElementById("response");
    responseParagraph.textContent = getRandomResponse();
  }

  // Call displayResponse when the page loads
  window.onload = displayResponse;
</script>
```

### Step 4: A Little CSS

Added [The New CSS Reset](https://github.com/elad2412/the-new-css-reset) by elad2412 as well as the following:

```css
body {
  display: grid;
  place-items: center;
  height: 100%;
  min-height: 100dvh;
  font-family: "Urbanist", sans-serif;
  margin: 0;
  padding: 0;
  background-color: blanchedalmond;
}
#response {
  margin: 0 0 0.175em 0;
  padding: 1rem;
  font-size: 25vw;
  line-height: 1em;
}
```

### Step 5: Deploy to DigitalOcean App Platform

https://www.digitalocean.com/community/tutorials/how-to-deploy-a-static-site-from-github-with-digitalocean-app-platform-quickstart

https://www.digitalocean.com/landing/use-cases
