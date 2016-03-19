<style>
	.code {
		font-size: 14;
		font-family: courier;
	}
</style>

<h4>SASS</h4>

Sass is a ‘pre-processing’ language. This means that the Sass documents cannot consumed by the browser, but need to be processed into another language that can. Sass is processed into CSS, similar to the way that CoffeeScript is processed into JavaScript.

The following SCSS files form the styling workflow:

<p class="code">style.css:</p> 

Do not worry about this file, it's required by WordPress. All styling are handled in the Sass files described below.

<p class="code">assets/scss/foundation.scss:</p>

Imports for Foundation components and your custom styles.

<p class="code">assets/scss/config/_settings.scss:</p>

Original Foundation 5 base settings.

<p class="code">assets/scss/config/_custom-settings.scss:</p>

Copy the settings you will modify to this file. Make it your own.

<p class="code">assets/scss/site/*.scss:</p> 

Unleash your creativity. Create the files you need (and remember to make import statements for all your files in assets/scss/foundation.scss)