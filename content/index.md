## What is Blitz?

Blitz is a static site generator. This means it can combine the text you write with templates produced by you or
someone else to generate HTML pages. Once the pages are generated, you can browse your site using any browser, online or
offline.

Blitz has a lot of built-in features such as menus, pagination, fetching content from directories, relative URLs to
other pages (useful for offline websites) and much more! That said, Blitz can be very simple when it counts and setting
up a single page website shouldn't take longer than a minute.

## How does Blitz work?

Blitz is a command line application that uses Node.js. To generate static sites it relies on 3 main components:

* The main configuration file, `blitz.yml`. It contains everything Blitz needs to know about your website, including
the description of pages. In minimal configuration, this is the only file Blitz needs.
* Page templates written using [Pug](https://www.npmjs.com/package/pug) templating engine. These will suit as the
skeleton of your website.
* Content files that will be used to populate the templates and generate the website.

Once these are ready, Blitz uses the config to build pages, piping content into templates. The beauty of this approach is that you can reuse content files and templates as many times as you want! Additionally, [Pug](https://pugjs.org/), the templating engine used by Blitz, supports such amazing things as [layouts](https://pugjs.org/language/extends.html), [includes](https://pugjs.org/language/includes.html) and [mixins](https://pugjs.org/language/mixins.html).

## Super quick start

Don't want to read the whole [quick start guide](https://getblitz.io/docs/0.1/getting-started-template)? No problems, here's how you can get started with Blitz right now —
first, [make sure you have Node and NPM installed](https://docs.npmjs.com/getting-started/installing-node). Then run the
following command in terminal to install Blitz:

```bash
npm install -g blitz-ssg
```

Congratulations, you've just installed Blitz! Now, you can create a new directory, initialise a minimal Blitz project
inside it and build your first site:

```bash
mkdir blitz-example
cd blitz-example
blitz init -t minimal
blitz build
```

Now, if you open the newly created `build` directory you should see an `index.html` file, which you can open to view
the website you've just generated. You can find `index.md` in the `content` folder and change the contents inside to
update the website. Don't forget to run `blitz build` once you're done.
 
 To see what else can be done, head to the [docs](https://getblitz.io/docs/0.1/). By the way, this website was also built using Blitz, so you might want
 to check out [its source code](https://github.com/TimboKZ/blitz-website) to see how I acheieved certain things.