---
title: 'Getting started with Blitz: Using a template'
menu_title: 'Getting started from a template'
---
## Getting started from a template

##### Choosing your template

Using a template is probably the fastest way to get started with Blitz. Templates provide useful boilerplates to speed up your development project. Additionally, you can study these templates to understand what Blitz is capable of and how you can achieve certain this.

The following templates are bundled with v0.1:

* `config`: Blitz configuration file only. You'll have to create all other directories on your own.
* `minimal`: As the name implies, this is a minimal configuration of Blitz. It has an oversimplified config and only a single Pug template.
* `portfolio`: A simple portfolio site built using Bootstrap. Uses menus, globals, layouts and fetches information about projects from a directory. Might be useful if you want to understand how these features work.

##### Initialising a project

First you, have to switch to the directory you want to initialise Blitz in. For the sake of this example, we will create a directory called `blitz-example` and initialise a new project inside it:

```bash
mkdir blitz-example
cd blitz-example
blitz init -t portfolio
```

Replace `portfolio` with the name of your desired template from the list above and you're good to go! The default template is `minimal`.