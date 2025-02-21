# :focus-visible Browser Compatibility Issue

This repository demonstrates a common CSS issue related to the `:focus-visible` pseudo-class and provides a solution for broader browser compatibility.  The `:focus-visible` pseudo-class is a relatively new addition to CSS and is not supported by all browsers.  This can lead to unexpected styling behaviors, especially regarding focused elements.  This repo shows how to handle this incompatibility using feature detection.

## Bug:

The `focus-bug.css` file contains CSS that relies solely on `:focus-visible`.  In older browsers, this will either not apply the styles, or will apply them incorrectly, producing unexpected results.

## Solution:

The `focus-solution.css` file provides a solution that utilizes a JavaScript polyfill to simulate the functionality of `:focus-visible` in older browsers.  This ensures consistent styling across a wider range of browsers.