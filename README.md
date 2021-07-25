# Article preview component

- Live website -(https://carlospwd-article-preview-component.netlify.app/)

## Table of contents

- [The challenge](#the-challenge)
- [Screenshot](#screenshot)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)

### The challenge

Users should be able to:

- View the optimal layout for the component depending on their device's screen size
- See the social media share links when they click the share icon

## My process

### Screenshot

### End Result

![result](https://user-images.githubusercontent.com/85038929/126907816-320ddabb-9c34-4884-b93b-7d6e6c94fd50.JPG)

### Active image

![active](https://user-images.githubusercontent.com/85038929/126907810-60ee74c9-1e60-4686-9adc-b4ca97935ab1.JPG)

### Built with

- Semantic HTML5 markup
- CSS custom properties
- CSS Grid
- JavaScript
- Media Queries

### What I learned

This was a fairly challenging project for me. I learned how to use the z-index property in css along with the display: relative property. Once I figured out how to complete the project in chrome, I opened up the file in firefox and noticed it looked different in the mobile view, so I learned how to use queries for specific browsers.

Here is some code that I wrote in order to complete this task

```HTML
        <!-- start of pop up -->
        <div class="pop-positioning">
          <div class="popup" id="popup-1">
            <div class="icons">
                <p>SHARE</p>
                <a href="https://www.facebook.com/" target="_blank"><i class="fab fa-facebook-square "></i></a>
                <a href="https://twitter.com/WDCarlosP" target="_blank"><i class="fab fa-twitter " ></i></a>
                <a href="https://www.pinterest.com/" target="_blank"><i class="fab fa-pinterest "></i></a>
            </div>
            <div class="shape"></div>
          </div>
        </div>
      <!-- pop up end -->

```

```Javascript
function togglePopup(){
    // this will add the class "active" to my element with the id popup-1 which replaces display hidden with display block and makes my content transition in when scaled back to regular size"
    document.getElementById("popup-1").classList.toggle("active");
}
```

```CSS
.popup .icons {
	display: flex;
	align-items: center;
	padding: 0 30px;
	background-color: var(--vdgBlue);
	width: inherit;
	height: 60px;
	border-radius: 0 0 10px 10px;
	box-shadow: 0 5px 10px rgba(184, 184, 184, 0.6);
	z-index: 1;
}

@-moz-document url-prefix() {
	.content {
		height: 257px;
	}
}
```

### Questions

- how can I change the color of my share arrow svg icon?
- is there a way to make sure all of the browsers look the same instead of using individual media queries?

### Useful resources

- [How to Create Simple Popup Box / Modal using HTML CSS & JavaScript](https://www.youtube.com/watch?v=iE_6pQ3RlZU&ab_channel=Codingflag) - this is a tutorial that demonstrates how to create a popup box with a smooth transition using CSS, HTML, and JavaScript

- [Using media queries](https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries/Using_media_queries) - this documentation shows how media queries work and the different types

- [display](https://developer.mozilla.org/en-US/docs/Web/CSS/display) -this documentation shows how to use the display element in css

- [z-index](https://developer.mozilla.org/en-US/docs/Web/CSS/z-index) -this documentation shows how to use the z-index element in css

- [Debugging JavaScript in Visual Studio Code and Google Chrome](https://www.youtube.com/watch?v=AX7uybwukkk&ab_channel=JamesQQuick) - this video taught me how to debug my javascript using the debugger tool in developer tools

## Author

- Website - [Carlos Perez](https://www.site.com)
- Frontend Mentor - [@Carlos-A-P](https://www.frontendmentor.io/profile/yourusername)
- Twitter - [@WDCarlosP](https://www.twitter.com/WDCarlosP)
