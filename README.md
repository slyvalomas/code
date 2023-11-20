# code

Brief description of the project.

## Table of Contents

- [Introduction](#introduction)
- [HTML Explanation](#html-explanation)
- [CSS Explanation](#css-explanation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

# Carckas Explore

Carckas Explore is a web project that showcases a creative exploration of buttons with emojis. It includes a simple layout with a header, navigation, buttons section, and a footer.

## Table of Contents

- [Introduction](#introduction)
- [HTML Explanation](#html-explanation)
- [CSS Explanation](#css-explanation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Carckas Explore is a project designed to experiment with button designs using emojis. The webpage features a header, navigation bar, a section with interactive buttons, and a footer with links.

## HTML Explanation

The HTML structure defines the layout of the webpage, including the header, navigation, main content section with buttons, and a footer. The buttons are creatively designed with emojis for a visually engaging experience.

```css
html {
    scroll-behavior: smooth;
}
###Universal Reset
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
###Variables

:root {
    /* -I box general sittings */
    --border-curve: min(3vh, 50px);
    --border-outline-D: 2px dashed;
    --border-outline-S: 2px solid;
    --border-r-50: 50%;
    --fit-width-hight: fit-content;
    --padding-margin-N: 1rem;
    --padding-margin-O-RL: 0 1rem;
    --padding-margin-O-TB: 1rem 0;
    --S-box: 100PX;
    --XS-box: 200PX;
    --M-box: 400PX;
    --XM-box: 600PX;
    --L-box: 800PX;
    --XL-box: 1000PX;

    /* - II background-------------------------------------------------- */

    /* -1 BACK IMAGE------------------------- */

    --back-img-chorok-yawm: url(../pictures/400213258_740785247890832_4006886130926015080_n.jpg);
    --back-img-rayen-goslin: url(../pictures/c0bd9398e69af42eef3b220cb4f20a30.png);
    --back-img-real-2: url(../pictures/f58edcec638d593a8e8ecb1777a96b8e.png);
    --back-img-real-3: url(../pictures/ee252efb83d584a4d584cfff23bfaa3c.png);
    --back-img-real1: url(../pictures/e635d99f59cabb7131cbce30db1220e8.png);
    --back-img-siraj-eddin: url(../pictures/bff448d56cdda3e1c096b7e6fda1ce9f.png);
    --back-video-eddpeacer: url(../pictures/ddaa8de9eebc633916f20c9279cab95a.mp4);

    /* -2 BACK COLOR ------------------------ */

    --back-color-BLACK: hsl(0, 0%, 0%);
    --back-color-WHITE: hsl(0, 0%, 100%);
    --back-color-BLUE: hsl(229, 100%, 50%);
    --back-color-RED: hsl(0, 100%, 50%);
    --back-color-YELLOW: hsl(53, 100%, 50%);

    /*-III box advanced sittings--------------------------------------------*/

    --justify-align-items-C: center;
    --justify-C-align-items-E: end;
    --justify-SA: space-around;
    --justify-SE: space-evenly;
    --justify-SB: space-between;

    /* -1 flex box --------------------------- */

    --flex: flex;
    --flexy-boxes: row wrap;
    --non-flexy-boxes: row nowrap;
    --flexy-coulumn: column wrap;
    --non-flexy-coulumn: column nowrap;

    /*-IV TEXT SITTINGS------------------------------*/

    /*-1 font-size--------------------*/

    --S-font: 1rem;
    --XS-font: 2rem;
    --M-font: 4rem;
    --XM-font: 6rem;
    --L-font: 8rem;
    --XL-font: 10rem;

    /*-2 text shadow---------------*/

    --S-shadow: 1px 1px 2px;
    --XS--shadow: 2px 2px 3px;
    --M--shadow: 2.5px 2.5px 3.5px;
    --XM--shadow: 3px 3px 4px;
    --L--shadow: 3.25px 3.25px 4.5px;
    --XL--shadow: 3.5px 3.5px 5px;
}
###General Block Settings
section {
    align-items: var(--justify-align-items-C);
    display: var(--flex);
    flex-flow: var(--non-flexy-coulumn);
    grid-template-columns: 1fr;
    justify-content: var(--justify-align-items-C);
    padding: var(--padding-margin-O-TB);
}

##Advanced Header Settings
###
.header {
    border: var(--border-outline-S) black;
    /* ... (other styles) */
}
###Profile Link
.header__nav {
    /* ... (styles for header navigation) */
    display: var(--flex);
    justify-content: var(--justify-align-items-C);
    position: sticky;
    top: 0;
    background-color: aquamarine;
    z-index: 1;
}

.profile_link {
    margin-top: 1rem;
    color: #000000;
    text-decoration: none;
    font-weight: 800;
    padding: var(--padding-margin-N);
}

###Profile Link Animation
.profile_link:hover {
    text-shadow: var(--XS--shadow);
    box-shadow: var(--XS--shadow);
    font-size: var(--XS-font);
    transition: all 1s;
    transform: skew(-5deg) rotateY(360deg);
    margin: var(--padding-margin-N);
    border: var(--border-outline-S) #0000002d;
    border-radius: var(--border-curve);
    padding: var(--padding-margin-N);
    background-color: rgba(0, 0, 0, 0.036);
}

###Logo
.header_logo_container {
    display: var(--flex);
    justify-content: var(--justify-align-items-C);
}

.header_logo {
    display: var(--flex);
    justify-content: var(--justify-align-items-C);
    align-items: var(--justify-align-items-C);
    font-size: 1.5rem;
    margin: 0.5rem;
    width: 100px;
    height: 100px;
    border-radius: var(--border-r-50);
    border: var(--border-outline-S);
}
##Advanced Footer Settings
###Footer Container
.footer {
    position: sticky;
    bottom: 0;
    background-color: blueviolet;
    border: var(--border-outline-S) black;
    display: var(--flex);
    flex-flow: var(--flexy-boxes);
    justify-content: var(--justify-align-items-C);
}

###Footer Links
.footer_link {
    text-decoration: none;
    color: #000000;
    font-size: var(--XS-font);
    padding: var(--padding-margin-N);
    margin-top: 0.5rem;
}

###Links Animation
.footer_link:hover {
    padding: 0.25rem;
    transform

```html
<!-- Include your HTML code here -->
<!DOCTYPE html>
<html lang="en">
<head>
    <link rel="stylesheet" href="explore.css">
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <!-- Header Section -->
    <header class="header">
        <div class="header_logo_container"><h1 class="header_logo">carckas</h1></div>
    </header>

    <!-- Navigation Section -->
    <nav class="header__nav"><a class="profile_link" target="_blank" href="https://github.com/slyvalomas">brahim abdelmoumn</a></nav>

    <!-- Main Content Section -->
    <section class="divsec">
        <!-- Buttons for Emojis -->
        <button id="one" class="div div1">🧑🏽‍⚕️</button>
        <button id="tow" class="div div2">🧑🏾🌹</button>
        <button id="three" class="div div3">🧑🏾‍🚀</button>
        <button id="four" class="div div4">🤴🏾</button>
    </section>

    <!-- Footer Section -->
    <footer class="footer">
        <!-- Links with Emoji Names -->
        <a href="#one" class="footer_link">snake 🧑🏽‍⚕️</a>
        <a href="#tow" class="footer_link">rose 🧑🏾🌹</a>
        <a href="#three" class="footer_link">rocket 🧑🏾‍🚀</a>
        <a href="#four" class="footer_link">king 🤴🏾</a>
    </footer>
</body>
</html>
