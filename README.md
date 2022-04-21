# Frontend Mentor - Intro section with dropdown navigation solution

This is a solution to the [Intro section with dropdown navigation challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/intro-section-with-dropdown-navigation-ryaPetHE5). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the relevant dropdown menus on desktop and mobile when interacting with the navigation links
- View the optimal layout for the content depending on their device's screen size
- See hover states for all interactive elements on the page

### Screenshot

![](./design/desktop-design.jpg)

### Links

- Solution URL: [Add solution URL here](https://github.com/Buch-dev/Intro-section.git)
- Live Site URL: [Add live site URL here](https://buch-dev.github.io/Intro-section/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

I learnt how to make drop-down menus more efficiently

```html
<h1>
  <div id="mySidenav" class="sidenav" onmouseover="hideSubmenu()">
        <img src="images/icon-close-menu.svg" alt="icon-close-menu" class="closebtn" onclick="closeNav()">
          <div class="nav-items">
            <div class="item">
              <a href="#">Features
                <img src="images/icon-arrow-down.svg" alt="icon-arrow-down" onmouseover="showSubmenu()">
              </a>
              <div class="sub-menu" id="submenu">
                <a href="#" class="submenu-item"><img src="images/icon-todo.svg" alt="icon-todo" > <span>Todo List</span></a>
                <a href="#" class="submenu-item"><img src="images/icon-calendar.svg" alt="icon-calendar" > <span>Calender</span></a>
                <a href="#" class="submenu-item"><img src="images/icon-reminders.svg" alt="icon-reminders" > <span>Reminders</span></a>
                <a href="#" class="submenu-item"><img src="images/icon-planning.svg" alt="icon-planning" > <span>Planning</span></a>
              </div>
            </div>
            <div class="item">
              <a href="#">Company
                <img src="images/icon-arrow-down.svg" alt="icon-arrow-down">
              </a>
              <div class="sub-menu">
                <a href="#" class="submenu-item company-submenu">History</a>
                <a href="#" class="submenu-item company-submenu">Our Team</a>
                <a href="#" class="submenu-item company-submenu">Blog</a>
              </div>
            </div>
            <div class="item"><a href="#">Careers</a></div>
            <div class="item"><a href="#">About</a></div>
          </div>
          <div class="login-section">
            <div class="item"><a href="#">Login</a></div>
            <div class="register"><a href="#">Register</a></div>
          </div>
      </div>
</h1>
```
```css
.proud-of-this-css {
  .sidenav {
    height: 100%;
    width: 0;
    position: fixed;
    z-index: 1;
    top: 0;
    right: 0;
    background-color: $Almost-White;
    overflow-x: hidden;
    padding-top: 100px;
    transition: .5s;
}
```
```js
const proudOfThisFunc = () => {
  function openNav() {
    document.getElementById("mySidenav").style.width = "67%";
    document.body.style.backgroundColor = "rgba(0, 0, 0, 0.4)";
  }

  function closeNav() {
    document.getElementById("mySidenav").style.width = "0";
    document.body.style.backgroundColor = "#fff";
  }
}
```

### Continued development

i would love making more complex layouts with HTML, CSS & Vanilla Javascript

### Useful resources

- [w3s NavBar Tutorial](https://www.example.com) - This helped me create the sidebar menu

## Author

- Website - [Daniel Okafor](https://buch-dev.GitHub.io/Daniel-Okafor/)
- Frontend Mentor - [@Buch-dev](https://www.frontendmentor.io/profile/Buch-dev)
- Twitter - [@bucheed](https://www.twitter.com/bucheed)
