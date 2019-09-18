# Instructions

Thank you for taking the Project 6 developer assessment!  The purpose of this test is to see how your experience aligns with our proccess and our projects. The goal here is to complete the test to the best of your ability and understanding; feel free to use any resources at your disposal, but all your code must be human readable.

__This test is designed to take about 2-4 hrs.__  Our expectation is that exercises 1, 3, and 4 will take about 1 hour in total and that the rest of the time will be spent on exercise 2. Let us know how you feel you did against these expectations. If the test takes longer, please let us know.

This test is meant to not be an exhaustive demonstration of your talents but rather a window in to how you approach solving problems on a time-sensitive deadline. We do not expect perfectly engineered code but we do want to see thoughtfully written solutions.

# HTML5 and CSS3

## 1. HTML5
We've created a homepage (home.html), but our resident SEO expert has told us that although the page looks good, it is not following semantic HTML5 rules. They would like to rewrite the page so that it is easier for search engines and screen readers to understand the content. Additionally, they would like to make sure that the third blog post has a red title (using the .red class)

__How to win:__
- The page follows valid, semantic HTML structure
- The page uses correct BEM rules


## 2. Homepage Layout
Recreate this layout: question-2/comp.png

Use BEM layout and write your code mobile first. Feel free to use CSS Grid, Flexbox, or floats but do not use any prebuilt frameworks or libraries (e.g. Bootstrap). For brevity, you can use any preprocessor you like. For CTA buttons, the client wants the hover effect to darken the button by 20% over 1 second. They also want the nav to be sticky on scroll. They also want the homepage hero image to fade in over 2.5s when the page loads.

Some hints:
This was designed on a grid system in a 1200px container with 80px columns and 10px gutters on each side (including the outside of the first and last columns). We used the google font Ubuntu in a regular and heavy weight. We used black and white text in 64px, 48px, 32px, and 16px. The colors used on the site were #000000, a 50% opacity of #D7D7D7, a 15% opacity of #000000, and #BBB1B1. Simple ease functions are more than sufficient, but if you want to get creative more power to you. We'd expect to see at least one animation with two keyframe states.

We'll assume  large is 992px+, medium is 768-992px, and small is is 0-767px.


__Sections:__
1. __Header:__ The site title should reduce in size on smaller devices
2. __Hero w/ title,:__ Font size should scale appropriately as the device size changes.  The background image should fill the container, regardless of device size. The aspect ratio must be maintained (no cropping). The animation effect must work for the latest versions of Firefox and Chrome with a no animation fallback for older browsers.
3. __Callouts:__  Images should be evenly divided with an appropriate gutter between.  On larger devices this should be 4-up, on medium devices this should be 2-up, and on small this should stack. Images should be in a square aspect ratio and crop out from the middle parts of the image that do not fit the ratio.
4. __Footer and copyright text:__  On larger devices, site menu and copyright text should lay out horizontally with the copyright text always aligned to the middle of the container element.  On smaller devices, the copyright text should go to the right and scale down.

__How to win:__
- The page follows valid, semantic HTML structure
- The page uses correct BEM rules
- The page scales down elegantly.
- CSS structure is easy to follow and extend.


# Javascript

## 3. Working with the DOM
__Copy and paste your solution from the question 2 directory into the question 3 directory.__
Using the layout you just created in solution 2, add on vanilla javascript to add a class to the menu on scroll that turns the logo red. Additionally, insert a new node into the page above the intro that counts the instances of the word "dog" (no matter the casing) and displays that count in realtime. It should say, "The page says dog: x times" where x is the count. It


__How to win:__
- Well formed vanilla JS that follows ES6 or ES5 rules.
- JS is modularized into component functions.



# Wordpress / PHP

## 4. Wordpress

### A) Custom Post Types & Taxonomy

In the file `5a.php`, add the necessary code to register a new custom post type with these parameters:

- The post type name should be `Movies`
- The post type should *only* support: title and author
- Has a custom dashicon

Additionally, add a new custom taxonomy with these parameters:

- The taxonomy's name should be `Genres`
- Show an admin column for this taxonomy

__How to Win:__
- Post type works as intended.
- Relationships between post type and taxonomy are valid


### B) Post Queries

Write a simple query that returns all movies with the Genre `Horror` produced between 1990 and 2001 with the author matching `wescraven`

__How to Win:__
- well-formed query
- returns expected results
