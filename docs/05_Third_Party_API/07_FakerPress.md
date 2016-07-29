### FakerPress

In order to inject filler content into a local development environment of the MSU Exponent website, we use Fakerpress. Fakerpress is a Wordpress plugin that generates random content for development usage. Fakerpress works nicely because it has support for generating posts that have almost the exact post format that is used on the MSU Exponent site. Fakerpress can be downloaded using the following [link](https://wordpress.org/plugins/fakerpress/). Once the plugin is downloaded, go to the wordpress dashboard and on the left sidebar, navigate to Plugins->Add New, at the top click Upload Plugin and choose the Fakerpress zip file. Click the Fakerpress->Posts button on the left sidebar in the Wordpress dashboard and enter in the following settings:

* Quantity: 10-30
* Date: 10 day range (in current year)
* Post Type: Posts
* Parents: none
* Comment Status: Allow Comments
* HTML tags: Leave as default
* Featured Image Rate: 90
* Image Providers: leave as default
* Author: User that you are logged in as on your local dev environment
* Taxonomies: Tags, Categories
* Terms: opinion, sports, culture, msu, montana state university
* Rate: 85
* Quantity: 1-5
* No Meta Field Rules

Click the Generate button