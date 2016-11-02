# omni-search
> A UI element for global searches

## Use Cases

Some use cases include adding quick navigation to your webapp so users can just jump to where they want to be
without leaving the keyboard or clicking several links. You can also provide a list of actions the user can perform in the application.

You just:

* Choose what triggers the global search to open, for example a keyboard shortcut.
* Provide a list of search results
* Provide a callback to handle what happens when the item is clicked by the user

## Demo

[http://pedrocatre.com/omni-search/demo/index.html](http://pedrocatre.com/omni-search/demo/index.html)

## Example project using omni-search

[WunderlistNavigator](https://github.com/pedrocatre/wunderlist-navigator/tree/feature/omni-search-lib),
quickly navigate between to-do lists in wunderlist.

![WunderlistNavigator](https://github.com/pedrocatre/wunderlist-navigator/raw/master/screenshots/demo.gif)

## Install

`npm install omni-search --save`

or

`bower install omni-search --save`

## Usage

1. Include jQuery:

	```html
	<script src="http://ajax.googleapis.com/ajax/libs/jquery/2.1.4/jquery.min.js"></script>
	```

2. Include plugin's code and style:

	```html
	<link rel="stylesheet" href="dist/css/omni.search.css"/>
	<script src="dist/js/omni.search.js"></script>
	```

3. Call the plugin:

	```javascript
	var $search = $('#element').omniSearch();
	$search.omniSearch('open', searchItems, callback);
	```

## Developing

Install dependencies by running:

`npm install`

Run `grunt build --force`to build the project (compile sass, minify css, concat javascript and uglify).

Install typescript `npm install -g typescript`

Run `tsc -w` to watch for typescript file changes.

### Run e2e-tests

Setup [nightwatchjs](http://nightwatchjs.org/getingstarted)

Nightwatch works with the Selenium standalone server so the first thing you need to do is download the selenium server jar file selenium-server-standalone-2.x.x.jar from the Selenium releases page: https://selenium-release.storage.googleapis.com/index.html

`npm install -g nightwatch`

Run `grunt serve` to serve the demo: http://localhost:9006/demo/index.html

Run `nightwatch`

## Credit

Inspired by the [TabSwitcher project](https://github.com/kamranahmedse/tab-switcher), a tab switcher for chrome.

## License

[MIT License](http://pedrodcatre.mit-license.org/) © Pedro Catré
