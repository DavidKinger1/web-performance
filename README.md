Improvements added to Web Site

1) Moved remote images to local web resources. Compressed images and set the widths when neccesary of:
	pizzeria.jpg
	2048.jpg
	cam_be_like.jpg
	mobilewebdev.jpg
	profilepic.jpg
	project-mobile.jpg
	web-performance.jpg

2) Removed google font download because font did not enhance the web pages but created serious timing issues

3) Function changes

function changeSliderLabel(size)
// Changed document.querySelectore to document.getElementByID and removed leading #

function updatePositions()
// declared top = document height
// declared phase outside of loop
// get array of pizzas outside for loop
// calculate approximate number of pizzas needed according to viewport height and width

function changePizzaSizes()
// Moved static calculations pizzaDiv, numPizzas, dx, and newwidth out of for loop
// retrieved objects of randomPizzas ID outside of loop and stored in container var

event window.addEventListener
stored common element img in d outside of for loop. 

4) Moved css and script to below the html rendering and made them asynch to try and eliminate render blocking

5) Minified bootstrap-grid.css and print.css as I didn't do anything with them for final submition. 

6) Modified all getElementByClassName by removing the period in front of the class names. Eg. .randomPizzaContainer is changed to randomPizzaContainer.

7) replaced querySelector with getElementById for ID queries as the later call is faster

8) added -webkit- and -ms to translateZ(0); for CSS .mover

9) calculated background pizzas by using window.inner(Height/Width) to scale the number with the viewport.

10) Fixed typo in main.js dx was using wrong syntax and parameter to:
  var dx = determineDx(container[0],size);