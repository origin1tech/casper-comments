# Casper-Comments

The default theme for [Ghost](http://github.com/tryghost/ghost/).

To download, visit the [releases](https://github.com/origin1tech/casper-comments/releases) page.

## Extended Theme

This theme is an extended version of the Casper theme. It's sole purpose is to provide an easy way to add Disqus comments to your blog.

## Installation

To install the theme either unzip theme into your /content/themes folder. Restart your Ghost blog and the theme will then be available under "General" in your Blog Settings.

Alternatively you can use Git to pull the theme. Open a terminal at your themes directory then run

```sh
$ git clone https://github.com/origin1tech/casper-comments.git
```
Restart your blog and again simply set theme under "General" in your Blog Settings.

## Configuration

Configuration is quite simple. After you have added a new site on Disqus and have provided Disqus with your desired shortname for your site you'll need to set this variable in the "Code Injection" header under the "Settings" of your blog.

```html
<script>

    // Set Disqus short name which is
    // the first part of your Disqus url.
    window.DISQUS_NAME = 'SHORT_NAME';

    // OPTIONAL
    // Optionally you can set the disqus_config here as well.
    // This allows for defining more granular control on how
    // Disqus will handle unique comments for posts. By default
    // this is handled by the URL which is fine in most cases.

    // UNCOMMENT
    // window.DISQUS_CONFIG = function () {
    //   this.page.url = 'YOUR_PAGE_URL';
    //   this.page.identifier = 'YOUR_PAGE_IDENTIFIER';
    // };

</script>
```

## Enable Post Comments

Enabling comments is pure cake. Simply add a tag called "comments" to the post's tags and viola you'll have your Disqus comments on that page.

## Wrapping Up

This is not meant to be the end all be all solution but rather a quick and dirty way to add comments without enabling comments for every post which is not usually desired. Simply adding comments to the post.hbs template for that reason doesn't work well. If you can think of an easier way without modifying Ghost itself feel free to PR :)

## Copyright & License

Copyright (c) 2013-2016 Ghost Foundation - Released under the MIT License.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
