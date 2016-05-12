## PHP

Retrieving posts from a certain category or with a certain set of filters can be carried out in two steps - configuring a WP Query object and using this object in ‘the loop’ from the WordPress API. The following code snippet demonstrates these two steps to retrieve the latest post thumbnail from the “Featured” category. 

	```php
	<?php
		function get_featured_thumbnail() {

		$args = array (
				'posts_per_page' => 1, 
				'category_name' => 'featured', 
				'meta_key' => '_thumbnail_id'
				);

			$the_query = new WP_Query($args);

			if ( $the_query->have_posts() ) {
				while ( $the_query->have_posts() ) {
					$the_query->the_post();
					// Link
					echo '<a href="' . get_permalink() . '" title="' . esc_attr( get_post()->post_title ) . '">';
					
		// Thumbnail
					echo get_the_post_thumbnail( get_post()->ID, 'size-thumbnail-medium', array('class' => "headline-img") );
						echo '</a>';
				}
			}
			else {
				// no posts found
			}

			wp_reset_postdata();
		}
	?>
	```

In this example, the arguments passed to an object of the WP Query class consist of the number of posts, the category and an attribute determining whether or not the post has an attachment associated with it.

The if and while statements that follow consist of what is referred to in the WordPress API as ‘the_loop’. The WP Query class filters the posts to display, which are then displayed by ‘the loop’. Through ‘the loop’, you can configure what attributes of the post to display, such as the post title, thumbnail, post author, etc.