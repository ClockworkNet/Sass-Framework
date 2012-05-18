Sass-Framework
==============

A modular framework based on [SASS/SCSS](http://sass-lang.com/ "Syntactically Awesome Stylesheets"). 

Documentation & Demos
-----

### Requirements

Sass 3.2 (alpha)

### File Structure

	_sass/
		|_ _config.scss <------------------ configuration lives here. 
		|_ _main.scss <-------------------- You will mostly be working in this one.
		|_ common/ <----------------------- Common style rules for your convenience.
			|_ base.scss
			|_ font-face.scss
			|_ layout.scss
			|_ mobile.scss
			|_ reset.scss
			|_ typography.scss
		|_ lib/ <-------------------------- The sweet stuff.
			|_ _lib.scss
			|_ functions/ <---------------- Helper functions.
				|_ browser-compatibilities.scss
				|_ measurements.scss
			|_ mixins/ <------------------- Partial stylesheets to include in your main.scss.
				|_ css3-prefixes.scss
				|_ media-queries.scss
				|_ utilities.scss
			|_ packages/ <----------------- Custom styles for various common web components.
				|_ buttons.scss
				|_ grid.scss
				|_ navigation.scss
	|_ css/
		|_ main.css
	|_ example.html
	|_ fonts/
		|_ (Empty)
	|_ images/
		|_ (Empty)
	|_ README.md

### Compiling the SASS/SCSS

To compile your SASS/SCSS into pure CSS; run the following command in the parent directory of this file

	# Example (project styles directory)
	sass --watch _sass/_main.scss:css/[desired-css-file-name].css