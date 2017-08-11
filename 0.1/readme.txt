=== Query From Content Shortcode ===
Contributors: bbuster79 
Tags: WP_Query, query, shortcode, related posts, custom query, query shortcode
Requires at least: 3.0
Tested up to: 3.4.2
Stable tag: 0.1
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Feature specific posts and categories inside your post-content

== Description ==

QFC is a shortcode plugin that allows you to target exactly the posts you’re looking for and list them in your content. Further, you can specify your own list header, include your current CSS styles to format the search results, and even specify whether or not you want your results to display their thumbnails and excerpts.

Basic format of the QFC shortcode should follow the example below:

[qfc]A Basic Header[/qfc]

The above example defaults to showing your five latest blog posts, no styling, no excerpt, no featured image. To customize your results, we can tell QFC to add some CSS and the images and excerpts we’ve been talking about. That shortcode should be placed inside your post content like so:

[qfc class=”my-css-class” id=”my-css-id” image=”yes” excerpt=”yes”]Some Bells & Whistles[/qfc]

Further, you can format your QFC search results with more than just one CSS class or ID: 

[qfc class=”my-css-class, another-css-class” id=”my-css-id, another-css-id”]We Like CSS![/qfc]

Query From Content can list more than just your latest blog posts. With basic use, you can specify things like tags, categories, authors and custom post types.

Here’s another quick example. This one specifies a category, a tag and an author:

[qfc category\_name=”Italian-recipes” tag=”lasagna” author\_name=”luigi”]Great Italian Recipes![/qfc]

QFC reads the parameters above and feeds them to the WP\_Query class. If you are familiar with the WP\_Query class, you may’ve recognized the parameters used in the above QFC code match exactly the parameters used in WP\_Query. All your QFC search parameters must match exactly with the WP\_Query parameters. 

For information on advanced usage of Query From Content, visit the Wordpress codex page for <a href=\"https://codex.wordpress.org/Class\_Reference/WP\_Query\">WP_Query</a>.

<div>
  <br />
</div>

== Installation ==

Extract the zip file and just drop the contents in the wp-content/plugins/ directory of your WordPress installation and then activate the Plugin from Plugins page.

==Readme Generator== 

This Readme file was generated using <a href = 'http://sudarmuthu.com/wordpress/wp-readme'>wp-readme</a>, which generates readme files for WordPress Plugins.