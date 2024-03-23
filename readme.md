<style>
    h1{background-color: #0aa; padding: 10px;}
    h2,h3{border-bottom: 4px solid;}
    blockquote{border-left: 4px solid #0aa}
</style>

# CSS Collapsing Margins Puzzle

Collapsing Margins is the cause of most grief in UI styling. Kevin Powell provides one of the best ways to
illustrate how margins collapse upon each other. Watch Kevin's video to understand more.

In the [*box* model](https://www.w3schools.com/Css/css_boxmodel.asp) the margins are on the outside of the
border and the padding is on the inside of the border. In this repo it is the *padding* that seem to
disappear and not the *margin*.

I have added multiple *display:* type to demonstrate their effect upon collapsing margins. The 
'*display: flex*' and '*display grid*' are working properly because they prevent the margins from
collapsing into each other. The goal is to have the child div span the height of the parent div 
without collapsing. In the case where there are two divs inside of the parent div, there should
not be any space between them. See if you can solve the collapsing margins issue on your own.

Kevin has a few ways to solve the collapsing margin issue. You will need to decide for yourself what is 
the best way to solve the issue.

#### *Personal Note*

This repo is a way for me to play around with it on my own and learn from it. Also, I like to work with
SCSS and that is why I use SCSS in this project.

#### *Basic Project Information*

Node modules are used to facilitate building the project. Watchers will compile scss into css and copy 
files to the dist folder.

To run the created index.html in the dist folder, right click on index.html and select 'Open with Live
Server'.

## Initial Project Setup

This project depends on Node.js utilities to automatically build
while you are working on your code. You will need to install Node.js to take advantage of the scripts
to automatically build your files. Installing Node.js only needs to be done once. If you already have
Node.js installed on your machine you can skip this step of installing Node.js.

Install Node.js - click [here](https://nodejs.org/en/download/) to go to the Node.js download page.

Once you have installed Node.js go to a terminal in your IDE and run this command:

> npm i

This will install the utilities needed to build the project.

To check the version of Node.js installed on your computer, run this command in the terminal in your IDE:

> node -v

When you install Node.js, it will also install `npm`. You can check the version of `npm` by running this
command in the terminal of your IDE:

> npm -v

## Running the File Watchers

The file watchers are utilities that will watch for changes in your source files using NPM commands to
watch and build HTML and SCSS source into a dist folder.

To start the watchers 

> run watch

## Run index.html

To see your changes in a browser:
> run serve

# Additional Resources

https://www.geeksforgeeks.org/how-to-disable-margin-collapsing-in-css/

https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Box_Model/Mastering_margin_collapsing

https://css-tricks.com/what-you-should-know-about-collapsing-margins/

https://www.joshwcomeau.com/css/rules-of-margin-collapse/

https://devdoc.net/web/developer.mozilla.org/en-US/docs/CSS/margin_collapsing.html

https://www.freecodecamp.org/news/what-is-margin-collapse-and-how-to-avoid-it/
