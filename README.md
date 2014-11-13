pk-slider
========
[![deprecated](http://badges.github.io/stability-badges/dist/deprecated.svg)](https://github.com/sw4/pocketknife) 

Functionality now integrated into [pocketknife ui](https://github.com/sw4/pocketknife)

--------------


[![Build Status](https://travis-ci.org/sw4/pk-slider.svg?branch=master)](https://travis-ci.org/sw4/pk-slider)

Lightweight javascript input slider

**Licensed under [cc by-sa 3.0](http://creativecommons.org/licenses/by-sa/3.0/) with attribution required**

#####[Demo](http://sw4.github.io/pk-slider/)

###Features

- HTML form compliant (input value can be submitted like with any other `input` element
- Mousewheel support

###Requires

- `pk-core.js`
- `pk-core.css`
- `pk-draggable.js`
- `pk-draggable.css`


###Usage

`pk.slider(opt);`

Returns a new slider object.

`opt` is an object consisting of:

```
element: \\ DOM element to replace with a slider - the elements attributes are carried over
axis: \\ can be `x` or `y`, determines vertical or horizontal slider
name: \\ the name to use for the slider input form element (can also be set as attribute on original element)
units: \\ the units postfix
value: \\ the starting value (defaults to 0)
disabled: \\ boolean, whether the toggle is disabled (can also be set as attribute on original element)
min: \\ minimum value (defaults to 0)
max: \\ maximum value (defaults to 100)
tabindex: \\ tabindex value (can also be set as attribute on original element) - defaults to 0
listeners: \\ object consisting of regular event functions for input elements as well as slidestart, slideend and sliding - passed the originating element and event
```

###Methods

`slider.val(value)`

Where `slider` is a slider object and value is either blank/null to get the current value, or a numeric value to set it

`slider.disabled(value)`

Where `slider` is a toggleswitch slider and value is either blank/null to get the current state, or a boolean value to set it
