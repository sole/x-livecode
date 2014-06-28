# x-livecode

This is a web component for having a live editor AND a live area which you can half-see when the editor is visible, for impressing friends, coworkers and maybe relatives.

Nice!

## Usage

Web Components are not ready yet in all browsers, so the safest bet for now is to just and simply include `platform.js` to polyfill gaps in the platform (get it? get it?), and then you can safely include the element as an HTML import:

````html
<script src="js/platform.js"></script>
<link rel="import" href="x-livecode/element.html">
````

And then you can do this in your code:

````html
<x-livecode src="mycode.js"></x-livecode>
````

Which will hopefully work and the code will be loaded.

Look at the example to see a complete configuration. Sadly you will need to run it over a local server (or a 'real' server) because there is some XMLHttpRequest in action to load files.

Example: TODO.

### Other examples

You can see it in action in [my presentation for LXJS](https://github.com/sole/lxjs2014).

## Styling

Use CSS.

## API

### Methods

TO DO

### Events

TO DO

## Things that need to be done

* Fill the TO DO gaps.
* Use Vulcanise or something similar to generate a distributable file with only one JavaScript file that registers the element - so it can be used either with HTML imports or with just including such file.


