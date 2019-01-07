---
id: 29
title: How to use the plugin
date: 2017-09-30T02:07:07+00:00
author: Geordi
layout: post
guid: 127.0.0.1/?p=29
permalink: /how-to-use-the-mmdb-plugin/
---
<img class="alignright wp-image-322 size-thumbnail" src="{{site.baseurl}}/wp-content/uploads/2017/11/icon-256x256-white-150x150.png" alt="mmdb-logo" width="150" height="150" srcset="{{site.baseurl}}/wp-content/uploads/2017/11/icon-256x256-white-150x150.png 150w, {{site.baseurl}}/wp-content/uploads/2017/11/icon-256x256-white-100x100.png 100w, {{site.baseurl}}/wp-content/uploads/2017/11/icon-256x256-white.png 256w" sizes="(max-width: 150px) 100vw, 150px" />The My-Movie-Database (mmdb) plugin can be used via  [**shortcodes**](#shortcodes) or  inside [**wordpress posts**](#post_types) (and post types).

After installing the plugin three custom post types are created in wordpress: Movies, TvShows and Persons.

You can disable any one of them (or all of them if you want to use this plugin _only_ via shortcode) by going into the Advanced options tab of the Movie Database options and selecting &#8220;No&#8221; for the post types you don&#8217;t want.

The shortcode method will always be available for all resource types (Movies, TvShows, etc) regardless of the state of the mmdb options for each post type.

Below is an outline of the two methods: WordPress posts and shortcodes

<div id="post_types">
  <h2>
    <strong>Using the plugin with WordPress posts</strong>
  </h2>
</div>

So as was mentioned above, by default the plugin will create three custom post types in wordpress: Movies, TvShows and Persons.

These custom post types are just like your regular wordpress posts except that they have a Movie, TvShow or Person section .

##### **Adding a New Movie (or editing a Movie post):**

Below the content textarea of your Movie post you will find the search  field.

_1-) Enter the title of the movie you are looking for and click on search._

_2-) You will then be presented with the search results._

<img class="size-full wp-image-306" src="{{site.baseurl}}/wp-content/uploads/2017/09/search.png" alt="search-results" width="982" height="827" srcset="{{site.baseurl}}/wp-content/uploads/2017/09/search.png 982w, {{site.baseurl}}/wp-content/uploads/2017/09/search-300x253.png 300w, {{site.baseurl}}/wp-content/uploads/2017/09/search-768x647.png 768w" sizes="(max-width: 706px) 89vw, (max-width: 767px) 82vw, 740px" /> 

_ _

_3-) Click on the desired movie._ A pop up will appear asking you to confirm your selection or to return to the previous page.

<img class="wp-image-305 size-large" src="{{site.baseurl}}/wp-content/uploads/2017/09/confirm-selection-1024x442.png" alt="confirm-selection" width="525" height="227" srcset="{{site.baseurl}}/wp-content/uploads/2017/09/confirm-selection-1024x442.png 1024w, {{site.baseurl}}/wp-content/uploads/2017/09/confirm-selection-300x129.png 300w, {{site.baseurl}}/wp-content/uploads/2017/09/confirm-selection-768x331.png 768w, {{site.baseurl}}/wp-content/uploads/2017/09/confirm-selection.png 1085w" sizes="(max-width: 525px) 100vw, 525px" /> 

_4-) Once you have confirmed your selection click to save (or update) your post._

That&#8217;s it! Now if you navigate to the url of your post (front-end), the movie information will be displayed.

##### Configuration and customization of display

From the plugin option page you can select:

  * which template will be used to display your resource, and
  * if this should appear before or after the post content
  * which sections to display/hide, as well as
  * the header and body  colors for the available templates

For the Movie posts only  (in the advanced configuration option tab) :

  * You have the option of using the default wordpress posts instead of a new custom post type.
  * You also have the option of renaming the default WP posts into movies or leaving them as is (&#8216;Posts&#8217;).

See the [configuration documentation page]({{site.baseurl}}/plugin-configuration-mmdb-options-page/)  for more detailed info.

> **All the of the above apply for TvShows and Persons as well.**

<div id="shortcodes">
  <h2>
    <strong>Using the plugin with shortcodes</strong>
  </h2>
</div>

The plugin shortcode is [my\_movie\_db].

  * The basic parameters that you need to set are  **id**  and **type**.
  * Optional parameters to override the global plugin settings are : **template,** **size, body** (color) and **header** (color).

{% include docs/shortcodes.html %}