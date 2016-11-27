---
title: 'Getting started with Blitz: Starting from scratch'
menu_title: 'Getting started from scratch'
---
## Getting started from scratch

To function, Blitz needs the `blitz.yml` file to be present in the working directory. To achieve that, you can either create an empty `blitz.yml` file and copy the example config from [here](https://getblitz.io/docs/0.1/config/#example-blitz-yml-), or, if you know what you're doing, you can try writing `blitz.yml` from scratch yourself.

Another option you have is to use the `config` template:

```bash
blitz init -t config
```

Running this command will create a standard Blitz config in the current directory.

Remember that you'll have to create the `content`, `templates` and `assets` folders yourself.