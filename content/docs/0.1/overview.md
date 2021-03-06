---
title: 'Overview'
menu_title: 'Overview'
version: '0.1.x'
---
## Overview

> This section is still being written up. Come back in a couple of days for complete documentation.

##### Understanding Blitz

The way Blitz works is really pretty simple. You have [Blitz content files](https://www.getblitz.io/docs/0.1/writing-content), which describes the contents of your website. Then, you have [Pug templates](https://www.getblitz.io/docs/0.1/making-templates) which describe how said contents should look. Finally, you have [the main config file](https://www.getblitz.io/docs/0.1/config), `blitz.yml` — it tells Blitz how to combine content files and templates to produce your static website. You can reuse both as much as you want, and even parse all content files in a directory!

##### Features

v0.1 was the first stable release of Blitz and it introduced a lot of key features.

* YAML configuration file. `blitz.yml` is the core configuration file for Blitz. It uses YAML syntax and is the only file required for Blitz to function (in minimal configuration).  
* Pug (formerly Jade) templates support. As of version v0.1.1, Pug is the only templating engine supported by Blitz. The templates can use all of the Pug features as long as the result is valid Pug markup.
* Markdown and YAML support for content creation. Blitz's content files have the `.md` extension but they are not your usual Markdown files. Read [Writing content] for more information about them.
* Nested and duplicate pages. Using `blitz.yml`, you can nest as many pages as you own. Having duplicate pages isn't an issue either, a single page or template can be reused an infinite amount of times. Blitz caches as much data as possible, so duplicates shouldn't cause any significant performance impact either.
* Pagination and loading content from a directory. 
* Global menus that work offline and know what the current menu point is. In `config.yml` you can specify which menu each page belongs to (if any) and then use the generated menus in every single template.

##### Known issues

* No known issues with versions 0.1.x yet.

##### Upcoming features

* Live preview/reload. One of the features I think people might find useful is making a `blitz preview` command, that will boot up an HTML server and reload the pages in real time whenever a change is detected.
* `blitz watch` command that will watch project files for changes and rebuild the website whenever a change is detected. Perforamnce is likely to suffer on big projects but for small one it should be quite feasible.
* Add page numbers and separate pages to the current pagination engine. The idea is to allow you to specify the amount of records per page when retrieving data from a directory and then pass all page numbers with URLs to your templates.
* Refine CLI workflow. At the moment it is not quite intuitive and is quite different from other similar applications, which can have a negative impact on user experience.
* Instead of passing a boolean as the `active` property of each menu item, I'm planning to pass a number instead. This way, the value of `active` will be `0` when the page is not active, which is treated as `false` in `if` clauses. Otherwise, the number will be `1` if the current page is the active one, `2` if the immediate child of the page is active, `3` if a child of a child is active and so on.