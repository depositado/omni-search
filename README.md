# omni-search
> A UI element for global searches

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
	$search.omniSearch('open', searchItems, callback);
	```

## Developing

Run `grunt build --force`to build the project (compile sass, minify css, concat javascript and uglify).

Install typescript `npm install -g typescript`

Run `tsc -w` to watch for typescript file changes.

### Run e2e-tests

Setup [nightwatchjs](http://nightwatchjs.org/getingstarted)

Nightwatch works with the Selenium standalone server so the first thing you need to do is download the selenium server jar file selenium-server-standalone-2.x.x.jar from the Selenium releases page: https://selenium-release.storage.googleapis.com/index.html

`npm install -g nightwatch`

Run `grunt serve` to serve the demo: http://localhost:9006/demo/index.html

Run `nightwatch`


## License

[MIT License](http://pedrodcatre.mit-license.org/) © Pedro Catré
