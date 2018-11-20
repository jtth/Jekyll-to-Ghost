Jekyll-to-Ghost Exporter
========================

Want to export your Markdown posts from [Jekyll](http://jekyllrb.com) to a format that can be easily imported into [Ghost?](http://ghost.org) This plugin will help you do that, though there are some limitations. It doesn't handle static pages, and it doesn't do anything with images. You'll have to copy those over yourself and manually adjust any URL differences.

This was built by reverse-engineering the WordPress exporter [plugin](http://wordpress.org/plugins/ghost/) to match the JSON file it outputs.

Last tested 2018-11-20 with Ghost Pro 2.6.0 and Jekyll 3.8.4.


Installation
------------

0. Clone the repo and drop the `jekylltoghost.rb` file into your Jekyll site's `_plugins` directory
1. Run `jekyll build`.
2. There should now be a `ghost_export.json` file in the `_site` directory. Open it, remove all the instances of `\n\n` or `\\n` or whatever nonsense comes out, then 
3. Import into Ghost.


License
-------

This Jekyll plugin is licensed under the MIT license.
