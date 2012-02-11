A CoffeeScript Class that monitors all elements in the body with `data-view` attribute and show them in a browser tooltip.

## Requirements:
- CoffeeScript
- (Backbone.js)
- (Twitter Bootstrap 2.0)

## Usage:
1. `new ViewTooltip` within for example your backbone.js View maintaining your whole app layout.
2. Make sure that you actually set the `data-view` attr on your elements. A good place is at the end of your `render` functions.

## Notes:
- Code works with current and future elements being created.
- As events fire at different times, care is taken to always show accurately the deepest nested View we are hovering over (through timeout).