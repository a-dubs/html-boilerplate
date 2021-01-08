# html-boilerplate
This is the boilerplate (starter template) that I use for all new sites I create. I wish I would have taken the time to make this years ago...

This boilerplate includes 2 core files: `index.html` and `index.css`. The SASS file, `custom.scss`, is also included for customizing the Bootsrap breakpoints and container max-widths. An additional CSS file, `util.css`, is included for common utility class stylings and foundation/default settings used across all my sites.

### index.html
The HTML file has a neatly organized `<head>` section with all the imports and `<meta>` tags your heart could ever desire, and features a very simple starter layout tempalate that fits most basic sites I create (at least for home or landing pages). 

Note: The two Bootstrap import lines are commented out by default, and **both** lines must be uncommented for Bootstrap to fully function

### index.css
A CSS file with clearly sectioned media queries for each breakpoint dictated in `custom.scss`, each with empty, commented-out, style blocks for every element included in `index.html`. In addition, a main / universal section is present above the media query sections such that any styling done here will apply to any size screen, until it is later overriden in one of the media query sections. 

### custom.scss
This file allows for setting custom Bootsrap min-width screen breakpoints and their respective container max-width values.
Not that this file will only be utilized if the Bootsrap framework is being used. And even if Bootstrap is used, this file is completely optional (if you are satisfied with Bootstrap's default breakpoints).

### util.css
This file has 3 main functions:
1. Adjusting the root font size of html files for use with REM and EM units for responsive content-size adjusting. All breakpoints featured here are consistent with the breakpoints set in `custom.scss`.
1. Declaring foundation/default settings to be used across all HTML pages. Note that all of these stylings are easily overridden since `util.css` is imported before any other css files (in CSS, preceding style values are always overriden by the final value).
1. Creating common utility classes that can be used across all sites, such as automatic vertical centering of a block element, even if it's not fixed width, using the class `.v-center`. 
