# Tailwind CSS Installation Guide

This guide explains how to install and configure Tailwind CSS in your project.

## Step 1: Install Node.js and npm

Before installing Tailwind CSS, you need to have **Node.js** and **npm** installed. If you haven't installed them yet, you can download and install Node.js from [nodejs.org](https://nodejs.org/). This will automatically install npm as well.

## Step 2: Initialize Your Project

If you don't have a project set up yet, create a new project and make a empty file called index.html

## Step 3: Install Tailwind CSS
```bash
npm install -D tailwindcss
npx tailwindcss init

```
## Step 3: Create INPUT.CSS FILE
Make a new folder called "src" and make a new file inside called input.css

## Step 5: Configure Tailwind
```html
module.exports = {
  content: ["./src/*.css", "./index.html"],
  theme: {
    extend: {},
  },
  plugins: [],
}

```

## Step 6: Add the Tailwind directives to your input.CSS file
```html
@tailwind base;
@tailwind components;
@tailwind utilities;
```

## Step 7: Start the Tailwind CLI build process
```bash
npx tailwindcss -i ./src/input.css -o ./src/output.css --watch

```
## Step 8: Start using Tailwind in your HTML
```html
<!doctype html>
    <html>
    <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="./output.css" rel="stylesheet">
    </head>
    <body>
    <h1 class="text-3xl font-bold underline">
        Hello world!
    </h1>
    </body>
</html>
```


## EXCERCISE 1: DESIGN SOMETHING USING TAILWINDCSS
Task: Your task is to design something using tailwindcss no matter how big or small. Some example are buttons, forms, inputs etc.

