---
title: 'Installing Blitz'
menu_title: 'Installation'
---
## Installation

##### Installing Node.js

Since Blitz relies on [Node.js](https://nodejs.org/en/) and its package manager, [NPM](https://www.npmjs.com/), you will have to install both of them. Fortunately, NPM is installed automatically when you install Node.js (unless you tweak the settings), so following [these instructions](https://docs.npmjs.com/getting-started/installing-node) should be enough.

##### Installing Blitz globally (recommended)

To install Blitz globally run the following command:

```bash
npm install -g blitz-ssg
```

If you didn't receive any errors from NPM, you've successfully installed Blitz. You can check that it works by running the following command:

```bash
blitz -h
```

##### Installing Blitz locally

Although it is recommended to install Blitz globally, local installation should also work. Run the following command:

```bash
npm install --save blitz-ssg
```

Keep in mind, this will **not** create the global `blitz` command, so to run it you'll have to switch to the directory where `package.json` for your NPM project is located and run the following:

```bash
node node_modules/blitz-ssg/blitz-cli
```

##### Updating Blitz

To get the most recent version, just run this command again:

```bash
npm install -g blitz-ssg
```