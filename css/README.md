# Organize your CSS with component files
From this point, you will start organizing your CSS code with one CSS file for each component. 
Buttons are standard components, and so are avatars, cards, lists, navbar, tabs, forms, etc.. 
All these guys deserve their own separate CSS file. 

Then in style.css:

/* Importing all components file */

@import url("components/avatar.css");
@import url("components/banner.css");
@import url("components/button.css");

Then you just need one unique link to style.css in your HTML file.

# Relative / Absolute

The relative/absolute CSS pattern is important when you need to position stuff in a specific place inside a component (e.g. a card).

Putting the card as position: relative is a way to pin it and be able to position the things inside it precisely.
Then you can make the inner elements position: absolute and place them wherever you want in the card thanks to the top/bottom/left/right properties.

# Flexbox

Flexboxes are awesome. It’s a layout mode intended to accommodate different screen sizes and different display devices. 
To turn a div into a flexbox is super easy: just add display: flex on your div. Then:

* That div is the flexbox
* All of its children elements are called flex items and can be distributed vertically and horizontally within the flexbox.


# Main flexbox properties
Here are the important CSS properties on the flexbox (not on the item):

* justify-content distributes flex items horizontally (either with space-around the items or space-between the items).
align-items: center allows use to vertically align the items (very useful).
* You can also make a flex item grow and take all available space:
* flex-grow: 1 will make a flex item grow and push its neighbours on the left and on the right 💪💪💪.
