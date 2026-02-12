# 🚀 Tailwind CSS – Simple English Notes

## 1. What will we learn in this course?

We will learn Tailwind CSS from scratch.

Hands-on approach → write code along with video.

Understand:

* What Tailwind is
* How to install it
* How to design responsive websites
* How to use hover, dark mode, utilities

---

## 2. Prerequisites for Tailwind CSS

Before learning Tailwind, you should know:

* Basic HTML
* Basic CSS concepts like:

  * Padding
  * Margin
  * Background color
  * Flexbox
  * Grid

👉 You don’t need to be CSS master, but basics are required.

---

## 3. What is Tailwind CSS?

Tailwind is a Utility-First CSS Framework.

Instead of writing CSS in separate file, we use predefined classes directly in HTML.

Example:

<div class="flex pt-4 text-center rotate-90"></div>

Why Tailwind became popular?

* Writing CSS is easier & faster
* Code becomes maintainable
* Only used CSS is exported → optimized performance
* Built-in responsive & dark mode support

---

## 4. Tailwind vs Bootstrap

* Bootstrap → ready-made components
* Tailwind → utilities to create your own design

Tailwind gives more custom control.

---

## 5. Setup Tailwind (Recommended Method)

### Step 1 – Check Node installed

node -v

If not installed → install Node.js first.

### Step 2 – Initialize Tailwind

npx tailwindcss init

This creates:

* tailwind.config.js

### Step 3 – Create folder structure

project
│── dist
│   └── index.html
│── src
│   └── input.css

### Step 4 – Write in input.css

@tailwind base;
@tailwind components;
@tailwind utilities;

### Step 5 – Build CSS

npx tailwindcss -i ./src/input.css -o ./dist/style.css --watch

### Step 6 – Link in HTML

<link rel="stylesheet" href="style.css">

---

## 6. First Tailwind Example

<h1 class="bg-slate-950 text-white text-xl m-4">
  Hello Tailwind
</h1>

bg-slate-950 → background
text-white → text color
m-4 → margin

---

## 7. Center Content using Grid

<body class="grid place-content-center h-screen">
  <h1 class="text-white">Centered Text</h1>
</body>

grid place-content-center → center vertically & horizontally
h-screen → full height

---

## 8. Build Simple Card

<div class="p-6 max-w-sm mx-auto bg-white rounded-xl shadow flex items-center space-x-4">
  <img class="h-12 w-12" src="logo.png" />
  <div>
    <h1 class="text-2xl font-medium">Tailwind CSS</h1>
    <p class="text-slate-500">Easy & Fast</p>
  </div>
</div>

---

## 9. Hover Effects

<button class="bg-sky-500 text-white p-2 rounded hover:bg-white hover:text-black">
  Buy Now
</button>

hover: → applies on mouse hover

---

## 10. Dark Mode

<button class="bg-sky-500 dark:bg-red-600 text-white"></button>

dark: → style for dark mode

---

## 11. Responsive Design (Mobile First)

Tailwind is mobile-first.

<p class="text-white sm:text-red-600 md:text-green-600">
  Responsive Text
</p>

Default → mobile
sm: → small screens
md: → medium screens

---

## 12. Responsive Card Example

<div class="max-w-sm md:max-w-2xl bg-white rounded-xl">
  <div class="md:flex">
    <img class="w-full md:w-48" src="img.jpg" />
    <div class="p-4">
      <h1 class="text-2xl">Card Title</h1>
      <p class="text-slate-500">Description</p>
    </div>
  </div>
</div>

Mobile → image top
Desktop → image left

---

## 13. Useful Tailwind Classes

### Text

* text-sm, text-xl, text-3xl
* text-center
* font-bold

### Spacing

* p-4 → padding
* m-4 → margin
* space-x-4

### Flex & Grid

* flex, grid
* items-center
* justify-between

### Colors

* bg-slate-900
* text-gray-500

---

## 14. Project Idea

Create:

* Navbar
* Hero section
* Cards
* Footer

Using only Tailwind classes.

---

## 🎯 Summary

* Tailwind = utility-first framework
* Write classes directly in HTML
* Mobile-first responsive
* Hover + Dark mode built-in
* Optimized CSS output

