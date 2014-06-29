# x-livecode

This is a web component for having a live editor AND a live area which you can half-see when the editor is visible, for impressing friends, coworkers and maybe relatives.

Nice!

Internally it uses *another component*, [x-editor](https://github.com/sole/x-editor).

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

### Live areas

TO DO

### Attributes

#### `appendcontrols`

If present, editor controls will be appended to the element that matches the query selector specified with this attribute. For example, the following:

````html
<x-livecode appendcontrols="h1"></x-livecode>
````

would append the controls to the first matched `h1` element.

#### `autoexec`

If present, the code will be automatically executed as soon as it is loaded. For example:

````
<x-livecode src="main.js" autoexec></x-livecode>
````

#### `hidecode`

If present, the code will be initially hidden. You will have to click on the `code` button to show it (this will evidently require that you show the controls). For example:

````
<x-livecode src="main.js" hidecode></x-livecode>
````

#### `src`

Specify the path of the file to be loaded. If not present, nothing will be loaded and the editor will be empty. For example:

````
<x-livecode src="main.js"></x-livecode>
````

will load the `main.js` file.


### Methods

TO DO

### Events

TO DO

## Things that need to be done

* Fill the TO DO gaps.
* Use Vulcanise or something similar to generate a distributable file with only one JavaScript file that registers the element - so it can be used either with HTML imports or with just including such file.
* TESTS

