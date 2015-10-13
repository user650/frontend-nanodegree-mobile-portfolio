NANO DEGREE - FRONT END WEB DEVERLOPER
PROJECT 4
SCOTT STUBBS
10-12-2015


PROJECT DESCRIPTION:
## Website Performance Optimization portfolio project
Your challenge, if you wish to accept it (and we sure hope you will), is to optimize this online portfolio for speed! In particular, optimize the critical rendering path and make this page render as quickly as possible by applying the techniques you've picked up in the [Critical Rendering Path course](https://www.udacity.com/course/ud884).


####Part 1: Optimize PageSpeed Insights score for index.html

> I made the following modifications to enable the index.html run faster:
o Reduced the size of the image profilepic.jpg and pizzeria.jpg
o Changed the font family 
o Changed the js to run async on several
o Inlined the css to run after the js

> I hosted the webpage from my computer using Python and Ngrok.  (this was a little bit of a challenge to do on my Windows 10 installation with 4 shared users, but it was fun).
 
> I tested the performance of the page on Google – PageSpeed Insights.  Both the desktop and mobile were over 90 when I tested.


####Part 2: Optimize Frames per Second in pizza.html

> In order to reduce the frames per second on the pizza.html I did the following items:
o Reduced the number of pizzas that float around from 200 to a number that is proportional to the screen height.
o Got rid of the time consuming determine dx function
o Made the change size slider pick a size as a direct percentage.
o Used webkitTransform instead of the style.left to move floating pizzas.
o Reduced the size of floating pizza .png by a lot
o Put some of the style in the css instead of in the java script
o Used the ever popular “will-change: transform” style thing for the .mover class.

Some other notes:

> I could not easily find a way to minify the code.  Google Page insights refers you to a link to a chrome extension that is no longer supported then that refers you back to page speed insights.  Since the files are so small I don’t think that the minify is going to really do much any way.

> In some cases I got dramatically different fps when I re-ran my tests.  The floating pizzas via the scroll seemed to change fps a lot on different runs.  Rebooting, running the tests with a slower scroll vs a longer on, waiting before I scrolled all of these had a different effect on the FPS.  The changes for “will-change: tranform;” did not seem to do a whole lot. Neither did putting the style height and width in the style sheet instead of within the javascript.
