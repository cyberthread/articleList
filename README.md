# Article List
One unique feature of an article list is that you often have an unknown amount of articles in that list and need an efficient way to build a consistent layout for that module. There are two different ways you can implement this sort of layout: Flexbox or Grid. The Flexbox implementation requires media queries, however the grid implementation does not. For this assignment *you can choose the layout method you'd like to implement*. The goal in either case is to implement a layout that starts with one column of articles and as the screen width increases, and as space allows, you should add additional columns.

## Flexbox Implementation
The Flexbox implementation requires styles to be set for the flex container by default (not in a media query) and rules for the flex items to be be set both by default and in media queries.

Use the [CSS-Tricks Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) to help you with this implentation. You'll need properties applied to the flex container:
- display
- flex-wrap
- justify-content
- row-gap
- column-gap

You'll need the following properties applied to flex items by default and in media queries:
- flex-basis
- for flex-basis to work well you may also need to use the [calc](https://css-tricks.com/a-complete-guide-to-calc-in-css/) property

## Grid Implementation
What is particularly cool about using a grid implementation is that you can create flexible and dynamic layouts that are responsive without ever needing to write a media query! This requires using a very small percentage of what grid is capable of, so full guides to the grid like the [CSS-Tricks Complete Grid Guide](https://css-tricks.com/snippets/css/complete-guide-grid/) will introduce far more ways of using grid than what is needed for this particular type of layout. Use this guide to limit the scope on what you explore.

For grid implementation you'll need to set the following properties on the grid container:
- display
- grid-gap
- grid-template columns (note that you'll want to use sizing and repeat functions to avoid the use of media queries)
	- [minmax()](https://gridbyexample.com/video/series-minmax/)
	- [repeat()](https://gridbyexample.com/video/series-repeat/)

As part of the grid-template-columns notation you will also need: 
- CSS Keyword [auto-fill](https://gridbyexample.com/video/series-auto-fill-auto-fit/)
- CSS Unit [fr](https://gridbyexample.com/video/series-the-fr-unit/)

## TASKS
- Implement a flexible article list layout using either flexbox or grid (you choose). The columns in the layout should:
	- All be the same width
	- Increase the number of columns as the screen width gets wider and as space allows
	- Have 2rem of space between them
- If there is not enough articles for a complete bottom row, make sure those articles are aligned to the left
- Make the site live

## Submission
- URL to live site on Blackboard
- Show your work to Instructor or TA in class for immediate feedback
