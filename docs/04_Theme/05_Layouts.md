## Layouts

![](layouts.png =450x)

The code for the layout shown above is found in the

```
parts/sections/desktop-tablet/featured.php
```

file and is included below:
	
```html
<!-- // Featured // -->

<div class="row" data-equalizer>
<div class="medium-5 columns" data-equalizer-watch>	

<!-- Latest post thumbnail -->
<?php get_featured_thumbnail(); ?>

</div>

<div class="medium-7 columns" data-equalizer-watch>

<!-- Latest post title -->
<h3>
	<?php get_featured_title(); ?>
</h3>

<!-- Single sentence excerpt -->
<p class="featured-excerpt">
	<?php get_featured_excerpt(); ?>
</p>

<!-- Three posts with thumbnails --> 
<?php get_featured_list(); ?>

</div>

</div>

<!-- Get more posts -->
<div class="row" data-equalizer>
<div class="medium-12 columns" data-equalizer-watch>
<?php get_more_posts("featured"); ?>
</div>
</div>
```

There are two rows, one for the content and another for displaying a link to get more posts from that category. The content row consists of two columns which have a 5:7 ratio in terms of length. The left column contains a call to the function which displays the latest post thumbnail from the “Featured” category. The right column displays the post title and an excerpt from the same post used in the left column. Additionally, it also includes a call to a function which displays the three latest posts with their thumbnails using Foundation’s “Block Grid” element.

At a higher level, the layout for the front page consists of calls to partials in the parts/layouts/desktop-tablet.php file:
	
```html
<div class="show-for-medium-up">
<?php get_template_part('parts/sections/desktop-tablet/featured'); ?>
<?php get_template_part('parts/sections/desktop-tablet/news-opinion-multimedia'); ?>
<?php get_template_part('parts/sections/desktop-tablet/culture-sports'); ?>
</div>
```

The folder structure can be summed up as follows:

```
parts/sections:
```

Contains the low-level grid layout for each section (category).

```
parts/layouts:
```

Contains the top-level grid layout for all the sections.

```
library/sections:
```

Contains the functions for each section that have been called in the section files. 

