# iyf-s10-week-2-Bella1234-ai
transform your HTML portfolio into a beautifully styled, responsive website. By the end, your portfolio will look professional on any device.
# Week 2: HTML portfolio

## Author
- **Name:** ISABELLAH SIMIYU
- **GitHub:** [@MaisoriKitayama](https://github.com/MaisoriKitayama)
- **Date:** Month Day, Year

## Project Description
Brief description of what you built and why.

## Technologies Used
- HTML5
- CSS3
- JavaScript
- (list all technologies)

## Features
- Feature 1
- Feature 2
- Feature 3

## How to Run
1. Clone this repository
2. Open `index.html` in your browser
   OR
   Run `npm install` then `npm start`

## Lessons Learned
What did you learn while building this project?

## Challenges Faced
What problems did you encounter and how did you solve them?

## Screenshots (optional)
<img width="1293" height="631" alt="image" src="https://github.com/user-attachments/assets/7a205270-6d32-4a88-9491-39c2e3826749" />
Why this works:

    flex-flow: column-reverse wrap-reverse;: This is a shorthand for flex-direction and flex-wrap.

        column-reverse stacks the frogs vertically and puts the red frog at the bottom.

        wrap-reverse ensures that when the frogs wrap to a new "column," they do so towards the left side of the pond.

    justify-content: center;: Since the main axis is now vertical (due to column-reverse), this centers the frogs vertically along the right and left edges.

    align-content: space-between;: This property controls the spacing between the lines (the two columns). It pushes one column of frogs to the far left and the other to the far right, perfectly landing them on their lilypads.

Would you like me to explain the difference between align-items and align-content, as they often get confused in levels like this?

![Screenshot description](path/to/screenshot.png)

## Live Demo (if deployed)
[View Live Demo](https://your-deployed-url.com)

## Exercise 2: Debug the Layout Fix this broken CSS (the boxes should be 300px wide total):
/* This box ends up 340px wide - why? Fix it! */
.broken-box {
    width: 300px;
    padding: 20px;
    border: none;
}
The reason your box is expanding is due to the default CSS Box Model. By default, the width you set only applies to the content area. The padding and borders are then added on top of that width.
The Math

In your code, the total width is calculated as:
Total Width=Width+Left Padding+Right Padding
300px+20px+20px=340px
The Fix: box-sizing

To make the box stay exactly 300px wide including the padding, you need to use the box-sizing: border-box; property. This tells the browser to include the padding and border within the specified width.
CSS

.broken-box {
  width: 300px;
  padding: 20px;
  border: none;
  box-sizing: border-box; /* This is the fix */
}

Pro Tip

Most modern web developers apply this to every element on the page at the very top of their CSS file to avoid this headache entirely:
CSS

*, *::before, *::after {
  box-sizing: border-box;
}
