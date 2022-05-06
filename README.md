4. After it's installed, click _Activate_ to activate the plugin on your site.

### Install the plugin manually

1. Download the plugin from [WordPress.org](https://wordpress.org/plugins/wp-parsely/) or get the latest release from our [Github Releases page](https://github.com/Parsely/wp-parsely/releases).
2. Unzip the downloaded archive.
3. Upload the entire `wp-parsely` folder to your `/wp-content/plugins` directory.
4. Visit the Plugins page from your WordPress dashboard and look for the newly installed Parse.ly plugin.
5. Click _Activate_ to activate the plugin on your site.

Note that this method is the recommended one for installing old versions of the plugin. Those can be downloaded from [WordPress.org](https://wordpress.org/plugins/wp-parsely/advanced/) or the GitHub Releases page.

## Local development

Development, code hosting and issue tracking of this plugin happens on the [wp-parsely GitHub repository](https://github.com/Parsely/wp-parsely/). Active development happens on the `develop` branch and releases are made off the `trunk` branch.

To run the plugin locally or to contribute to it, please check the instructions in the [CONTRIBUTING](https://github.com/parsely/wp-parsely/blob/trunk/CONTRIBUTING.md) file.

## Sample Parse.ly metadata

The standard Parse.ly JavaScript tracker inserted before the closing `body` tag:

~~~html
<script id="parsely-cfg" data-parsely-site="example.com" src="https://cdn.parsely.com/keys/example.com/p.js"></script>
~~~

A sample `JSON-LD` structured data for a home page or section page:

~~~html
<script type="application/ld+json">
{"@context":"http:\/\/schema.org","@type":"WebPage","headline":"WordPress VIP","url":"http:\/\/wpvip.com\/"}
</script>
~~~

A sample `JSON-LD` meta tag and structured data for an article or post:

~~~html
<script type="application/ld+json">
{"@context":"http:\/\/schema.org","@type":"NewsArticle","mainEntityOfPage":{"@type":"WebPage","@id":"http:\/\/wpvip.com\/2021\/04\/09\/how-the-wordpress-gutenberg-block-editor-empowers-enterprise-content-creators\/"},"headline":"How the WordPress Gutenberg Block Editor Empowers Enterprise Content Creators","url":"http:\/\/wpvip.com\/2021\/04\/09\/how-the-wordpress-gutenberg-block-editor-empowers-enterprise-content-creators\/","thumbnailUrl":"https:\/\/wpvip.com\/wp-content\/uploads\/2021\/04\/ladyatdesk.png?w=120","image":{"@type":"ImageObject","url":"https:\/\/wpvip.com\/wp-content\/uploads\/2021\/04\/ladyatdesk.png?w=120"},"dateCreated":"2021-04-09T15:13:13Z","datePublished":"2021-04-09T15:13:13Z","dateModified":"2021-04-09T15:13:13Z","articleSection":"Gutenberg","author":[{"@type":"Person","name":"Sam Wendland"}],"creator":["Sam Wendland"],"publisher":{"@type":"Organization","name":"The Enterprise Content Management Platform | WordPress VIP","logo":"https:\/\/wpvip.com\/wp-content\/uploads\/2020\/11\/cropped-favicon-dark.png"},"keywords":[]}
</script>
~~~

## The Parse.ly Recommendations Block

**IMPORTANT:** The Recommendations Block is available only in WordPress 5.9 and later.

The plugin includes a Recommendations Block that uses the [Parse.ly API](https://www.parse.ly/help/api/recommendations#get-related) to showcase links to content on your site. More information about the Block [can be found here](https://www.parse.ly/help/integration/recommendations-block).

## Screenshots

1. Parse.ly plugin main settings for easy setup. For the plugin to start working, only the website ID is needed.  
   ![The main settings screen of the wp-parsely plugin](.wordpress-org/screenshot-1.png)
2. Parse.ly plugin settings that require you to submit a website recrawl request whenever you update them.  
   ![The main settings screen of the wp-parsely plugin](.wordpress-org/screenshot-2.png)
3. Parse.ly plugin advanced settings. To be used only if instructed by Parse.ly staff.  
   ![The main settings screen of the wp-parsely plugin](.wordpress-org/screenshot-3.png)
