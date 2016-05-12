## SASS

Sass is a ‘pre-processing’ language. This means that the Sass documents cannot consumed by the browser, but need to be processed into another language that can. Sass is processed into CSS, similar to the way that CoffeeScript is processed into JavaScript.

The following SCSS files form the styling workflow:

	```
	style.css:
	```

Do not worry about this file, it's required by WordPress. All styling are handled in the Sass files described below.

	```
	assets/scss/foundation.scss:
	```

Imports for Foundation components and your custom styles.

	```
	assets/scss/config/_settings.scss:
	```

Original Foundation 5 base settings.

	```
	assets/scss/config/_custom-settings.scss:
	```

Copy the settings you will modify to this file. Make it your own.

	```
	assets/scss/site/*.scss:
	```

Unleash your creativity. Create the files you need (and remember to make import statements for all your files in assets/scss/foundation.scss)