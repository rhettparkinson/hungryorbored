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
    <title>Are You Hungry or Bored?</title>
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

## Set up Git Resposity.

Create an empty respository on GitHub, and then in the command line:

```sh
git init
git remote add origin git@github.com:rhettparkinson/hungryorbored.git
git add .
git commit -m "Initial commit"
git branch -M main
git push -u origin main
```
