# Polymer Theme Issue

## Repro Steps

1. `bower install`
2. `polyserve`
3. open browser to http://localhost:8080/components/polymer-theme-issue/index.html


The expectation (which may be unreasonable) is that there is a way to
get polymer-theme to apply to custom elements and not just the surface
document. You'll see that the button in the surface document is
colored as primary, but the button in the custom element is partly
styled (has a drop shadow, font, etc) but is not styled as primary. So
it seems like some of the styles are piercing the shadow dom and some
aren't.

Tested on Ubuntu 14.04, Chrome 44.0.2403.107 and Firefox 39.0.
