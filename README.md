
# Site Under Development

This repository contains a simple “coming soon” or “site under development” static page built with **HTML**, **CSS**, and **Particles.js**. The goal is to display an elegant page with an animated particle background and a message informing visitors that the site is currently being built.

---

<p align="center">
  <img src="https://github.com/yuvayna/Waiting-HTML-Website/blob/main/mto8Q.png" alt="Under Construction Preview" width="800"/>
</p>


## 📋 Description

The main file is `index.html`, which includes:

1. An animated background using the [Particles.js](https://github.com/VincentGarreau/particles.js/) library.
2. A central content area displaying:
   - A 🚧 “Site Under Development” 🚧 headline
   - A paragraph asking visitors to check back later
   - A button linking to your GitHub profile
3. Inline CSS (inside the `<style>` tag) to:
   - Set the typography (Orbitron font)
   - Handle the layout (vertical/horizontal centering, fade-in animation)
   - Style the “View my GitHub” button with hover effects

---

## Config 


Open the page in a browser

Double-click index.html or right-click ► “Open with” ► choose your preferred browser.

The page will immediately display with the particle animation in the background.

Customize the GitHub button link

By default, the button opens:

````
https://github.com/yuvayna
````

To modify this, update the ``onclick="window.open('https://github.com/yuvayna', '_blank')"`` attribute in ``index.html`` to point to your own GitHub profile or any desired URL.


## 🎨 Customization

### 1. Change the text

Update the headline text ``(🚧 Site Under Development 🚧)`` in the ``<h1>`` tag.

Adjust the paragraph ``<p>`` to provide more context or details.

### 2. Change the background or text color 

In the ``<style>`` section:

````css
html, body {
  background-color: #0d0d0d; /* Background color */
  color: #fff;               /* Text color */
  /* … */
}
````

- Replace #0d0d0d with your desired hex color (e.g., #1a1a1a, #22202A, etc.).

- Replace #fff with the color you want for the text.

### 3. Tweak the particle animation

````js
particlesJS("particles-js", {
  particles: {
    number: { value: 80, density: { enable: true, value_area: 800 } },
    color: { value: "#ffffff" },
    shape: { /* … */ },
    opacity: { /* … */ },
    size: { /* … */ },
    line_linked: { /* … */ },
    move: { /* … */ }
  },
  interactivity: {
    detect_on: "canvas",
    events: {
      onhover: { enable: true, mode: "repulse" },
      onclick: { enable: true, mode: "push" },
      resize: true
    },
    modes: { repulse: { distance: 100, duration: 0.4 }, push: { particles_nb: 4 } }
  },
  retina_detect: true
});
````

- Particle count: ``number.value`` (default: 80)

- Color: ``color.value`` (default: "#ffffff")

- Shape: ``shape.type`` (“circle”, “edge”, “triangle”, etc.)

- Speed: ``move.speed`` (default: 2)

- Hover effect: ``onhover.mode`` (“grab”, “repulse”, “bubble”)

- Click effect: ``onclick.mode`` (“push”, “remove”, “bubble”, “repulse”)

- Adjust these values to get the desired effect (fewer or more particles, different color, different behavior, etc.).

### 4. Change the font
  
The page imports Google Fonts:

````html
<link href="https://fonts.googleapis.com/css2?family=Orbitron&display=swap" rel="stylesheet">
````

To use a different font, replace this URL with the Google Fonts link (or a locally served font).

Don’t forget to update ``font-family: 'Orbitron', sans-serif;`` in the CSS if you switch to another font.



## 📌 Key Points

No back-end: This page is completely static and does not collect user data.

Responsiveness: Thanks to the meta viewport tag and the CSS flex layout, the page adapts to most screen sizes (desktop, tablet, mobile).

Accessibility: High contrast between text and background improves readability, and the button is large enough for easy clicking.


## 📄 License

This project is licensed under the MIT License. You are free to use, modify, and redistribute. See the LICENSE file for details. @yuvayna

Credit me if you use this template.

<p align="center"> ✨ Thanks and happy customizing! https://yuvayna.com ✨ </p>


