# portfolio_update_v1 (Techdegree Project 1)

[Live Project is availabe Here](https://ezellfrazier.com/projects/portfoliov1)

## Project Overview

--------------------

-   Create or find an image file to represent yourself and a new image for the background. Be aware of file size: keep the profile image under  400 KB  and the background image under  1 MB(see the link in the project resources section to Picresize, an online image resizing tool).

````
<header class="index">
  <img src="images/ezell.jpg" alt="Image of Ezell Frazier." class="profile-image">
  <h1 class="tag name">Hello, I’m Ezell.</h1>
  <p class="tag location">Houston, Texas</p>
</header>
````

````
.portfolio {
  text-align: center;
  background: linear-gradient(#5c37ff, transparent 100%),
              linear-gradient(0deg, #f7f5f0, transparent 3%),
              url('images/code.PNG') no-repeat center ;

  background-size: cover;
  overflow: hidden;
  padding-top: 60px;
}
````

-   Using a text editor, modify the HTML of the index.html file:

-   Add the images you collected in step 1 to the page. Please leave the class "profile-image" intact on your profile image.

-   Don't forget to update the text for your new profile image's alt attribute!

-   Personalize all the text on the page by changing the name, background and goals. Feel free to make up the information if you do not wish to share anything personal.

````
<div class="card">
  <h2>Background</h2>
  <p>As a recent college graduate, I want to continue my life of learning and creating value for others. Joining the Treehouse
    Techdegree program feels like the right step after finishing with a bachelor's in management information systems.
    I'm super excited to be a part of this amazing experience.</p>
  <p>I have a strong background in computer hardware and customer service. However, it is time to set web development and programming as the track towards the future.</p>
</div>
````

-   Add links to your GitHub, Twitter and LinkedIn accounts. If you don't have a Twitter or LinkedIn account, or don't want to share those, then you need to delete those links.

-   Edit the href value of the Home link so it navigates to  index.html. Note: do not use root relative links, or links that begin with a leading forward slash,  /.

````
<footer>
  <ul>
    <li><a href="https://twitter.com/_Ezell_" class="social twitter">Twitter</a></li>
    <li><a href="https://www.linkedin.com/in/ezell-frazier-830a50135" class="social linkedin">LinkedIn</a></li>
    <li><a href="https://github.com/lynellf" class="social github">Github</a></li>
    <li><a href="https://teamtreehouse.com/ezellfrazier" class="social treehouse">Treehouse</a></li>
  </ul>
  <p class="copyright">Copyright 2017, Ezell Frazier</p>
</footer>
````

-   Feel free to expand on this project, by adding an additional page or two, adding more images and customizing the CSS.

-   If you do not want to add an additional page then delete the experience link in the HTML.

-   Put your project files in a new GitHub repository on your GitHub account:

-   Make sure that you're only putting the files for this project in that repository.

-   Please do not create any new folders for this project.

-   The GitHub Desktop application can automatically create a new repository for you. See the workshop 'Share Your Techdegree Projects with Github Desktop' for more info on how to put your project onto GitHub using the GitHub Desktop app (linked in the Additional Resources section).

-   Make sure to check your code is valid by running it through an HTML and CSS validator.

-   Links to the validators can be found in the Project Resources. This will help you spot any errors that might be in your code.

-   Create additional pages to expand on this online profile.

-   Edit the styling of the profile photo's CSS properties. Pick at least one of the following properties to change:

-   border

-   border-radius

-   transition

````
header .profile-image {
  margin-top: 50px;
  width: 150px;
  height: 150px;
  border-radius: 30%;
  /*A circular image did not look all too good in this case. */
  border: 3px solid yellow;
  box-shadow: 5px 5px 0 0 #222;
  transition: all .5s;
}

header .profile-image:hover {
  transform: scale(1.2) rotate(360deg);
}
````

-   Add more photos and imagery to the page

-   Add more text to the page such as a list of your hobbies.

### Extra (JavaScript-based Navigation)

Mobile displays will see a drop-down menu, configured with JavaScript.

````
<script type="text/javascript">
const navi = document.querySelector(".nav"),
      burger = document.querySelector(".hamburger"),
    toggleMainBurger = () => {
        if (navi.style.display === "") {
            navi.style.display = "flex";
        } else {
            if (navi.style.display === "flex") {
                navi.style.display = "";
            }
        }
    };
burger.addEventListener('click', () => {
    toggleMainBurger();
});
</script>
````
