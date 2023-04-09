# css

## adding to html
* external: `<link rel="stylesheet" href="styles.css">`
* internal: `<style>`
* inline: `<div style="">`

## selectors
* universal: `*`
* type selector: `<div>`, `<p>`, and more
* class:`.class`
* id: `#id`
* can group selector with commas, or channing them
* descendents: `.ancestor .child`

## properties
* text color: `color`
* background color: `background-color`
* font: `font-family`
* font size: `font-size`
* text boldness: `font-weight`
* text alignment: `text-align`
* height: `height`
* width: `width`
* space b/w box and content: `padding`
* space b/w borders: `margin`
* space b/w margin and padding: `border`
* block and inline display

## cascade
determines which rules actually get applied to the html
* specificity  
 an id selector will always beat any number of class selectors, a class selector will always beat any number of type selectors, and a type selector will always beat any number of anything less specific than it.
* inheritance  
 properties that, when applied to an element, are inherited by that element’s descendants, even if we don’t explicitly write a rule for those descendants. the exception to this is when directly targeting an element, as this always beats inheritance.
* rule order  
 whichever rule was the last defined is the winner. sort of a tie-breaker.

