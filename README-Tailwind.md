# Tailwind CSS Installation Guide

This guide explains how to install and configure Tailwind CSS in your project.

## Step 1: Install Node.js and npm

Before installing Tailwind CSS, you need to have **Node.js** and **npm** installed. If you haven't installed them yet, you can download and install Node.js from [nodejs.org](https://nodejs.org/). This will automatically install npm as well.

## Step 2: Initialize Your Project

If you don't have a project set up yet, create a new project directory and initialize it:

## Step 3: Install Tailwind CSS
```bash
npm install -D tailwindcss
npx tailwindcss init

```

## Step 4: Configure Tailwind
```html
module.exports = {
  content: ["./src/*.css", "./index.html"],
  theme: {
    extend: {},
  },
  plugins: [],
}

```

## Add the Tailwind directives to your input.CSS file
```html
@tailwind base;
@tailwind components;
@tailwind utilities;
```

## Start the Tailwind CLI build process
```bash
npx tailwindcss -i ./src/input.css -o ./src/output.css --watch

```
## Start using Tailwind in your HTML
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

