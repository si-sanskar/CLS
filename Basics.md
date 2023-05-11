# CLS

CLS (Cumulative Layout Shift) is a performance metric that measures the visual stability of a web page. It quantifies the amount of unexpected layout shift that occurs during the loading of a page.

## Layout Shifts in detail

Layout shifts occur when the content on a web page moves around unexpectedly. This can happen due to a variety of reasons, such as images and videos loading slowly or incorrect sizing of elements. Layout shifts can be measured using the Layout Shift score, which takes into account the Impact fraction and Distance fraction.

### Layout Shift score and it's calculation

The Layout Shift score is calculated by multiplying the Impact fraction by the Distance fraction. The Impact fraction is the proportion of the viewport that is affected by the layout shift, while the Distance fraction is the distance that the content moves.

### Impact fraction

The Impact fraction ranges from 0 to 1 and represents the proportion of the viewport that is affected by the layout shift. A layout shift that affects the entire viewport would have an Impact fraction of 1, while a layout shift that only affects a small part of the viewport would have an Impact fraction close to 0.

### Distance fraction

The Distance fraction ranges from 0 to 1 and represents the distance that the content moves due to the layout shift. A layout shift that moves the content a long distance would have a Distance fraction close to 1, while a layout shift that only moves the content a short distance would have a Distance fraction close to 0.

### Example calculation of LS Score 

For example, if a layout shift affects 50% of the viewport (Impact fraction = 0.5) and moves the content 200 pixels (Distance fraction = 0.2), the Layout Shift score would be 0.1 (0.5 * 0.2).

To calculate the CLS score, each individual LS scores are summed up.

Example: 
LS Score 1: 0.5, LS Score 2: 0.5, LS Score 3: 0.2. 
CLS Score: 0.5 + 0.5 + 0.2 = 1.2

### What is a good CLS Score?
A good CLS score is less than 0.1. This means that the amount of unexpected layout shift that occurs during the loading of a page is minimal, which provides a better user experience.

## Expected vs Unexpected Layout Shifts
Expected layout shifts occur when the user interacts with the page, such as clicking a button or scrolling. These types of layout shifts are not considered to be unexpected and do not negatively impact the user experience.

### User Initiated layout shifts
User initiated layout shifts can be minimized by using predictive loading, where the web page anticipates the user's actions and preloads the necessary content.

### Animations and Transitions
Animations and transitions can also cause layout shifts, but these are expected and can be optimized by using CSS animations and transitions instead of JavaScript animations, and by preloading assets to reduce loading times.


