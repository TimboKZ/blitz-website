# Blitz website

This repository contains the source code for [https://getblitz.io/](https://getblitz.io/).

You will need [Blitz](https://github.com/TimboKZ/blitz) to rebuild the static site after changing the source.


# Building the website

Assuming you have npm and git installed, you should be able to build the website by running the following commands:

```bash
git clone https://github.com/TimboKZ/blitz-website.git
cd blitz-website
npm install -g blitz-ssg
blitz build
```

If you want to browse the website offline, don't forget to change `absolute_urls` to `false` and `explicit_html_extensions` to `true` before building the website.