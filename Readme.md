# Task 8: CSS Hamburger Menu in Mobile (Pseudo Classes)

**Author:** D P Rithvik Kumar

## Description & Learning Process
This task challenged me to build a fully functional mobile hamburger menu without using any JavaScript, relying purely on CSS pseudo-classes.

In my previous documentation, I incorrectly stated that I used a "hidden button" to trigger the menu. That was a technical inaccuracy! I learned that I am actually applying the `:focus` pseudo-class to the highly visible hamburger button itself. When the user clicks the button, it enters the `:focus` state, and I use the CSS general sibling combinator (`~`) to target the `.side-menu` and `.backdrop` div that sit next to it in the HTML, forcing them to appear.

I also iterated on the UX based on feedback. Instead of just making the menu instantly appear below the navbar, I used `position: fixed` and `top: 0` so the menu takes up the full height of the viewport. I added a `transform: translateX()` property to make the menu smoothly slide in from off-screen, and I replaced the text icon with three span elements so I could target them individually with CSS `transform: rotate` to form a cool 'X' animation when clicked!

## How to Run
1. Download or clone this repository to your local machine.
2. Ensure `index.html` and `style.css` are in the same folder.
3. Open `index.html` in a web browser.
4. Using the browser's developer tools (F12) or by dragging the window, shrink the screen width to below 768px to reveal the hamburger menu icon.
5. Click the hamburger icon to see the CSS-only X animation, the slide-in menu, and the dark backdrop overlay!
