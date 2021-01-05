# CSS Layout
## Types of Boxes/Elements
1. BLock-level elements: start on a new line, organised like lego.
2. Inline elements: flow between the surrounding text
## Element Position
We can control the posiotion of those elements on the web page in different ways:
1. Normal flow: every block-level element appears on a new line. {position: static;
2. Relative positioning: shifts elements to top, bottom, right, left. {position: relative;
3. Absolute positioning: positioned in relation to its containing element and moves when we scroll. {position: absolute;
4. Fixed positioning: positioned in relation to the web browser page and does not move when scrolling.   GIT{position: fixed;
5. Floating elements: position to the far right or left. {float: right/left;

## Types of Layouts:

1. Fixed width layout: these designs do notchange size when the user changes
the size of their browser window.
2. Liquid layout: these designs stretch and contract as the user increases or decreases the size of their browser window.

# How to add multiple style sheets to a page:
1. Our HTML page can link to one style sheet and that stylesheet can use the @import rule to import other style sheets.
2. In the HTML we can use a
separate <link> element for each style sheet.

## Notes: 
* If a containing element only contains floated elements, some browsers will treat it as if it is zero pixels tall. To fix this: 
-Set the overflow property is
given a value auto.
-Set the width property is set to
100%.
* Screen Resolution: It refers to the number of dots a screen shows per inch.
* You can create pages of around 960-1000 pixels wide because most users will be able to see designs this wide on their screens.
* You need to indicate what the site is about within the top 600 pixles.
