---

---
### Notes about the config

* Every single property of the config is optional, i.e. an empty YAML file is still a valid Blitz config. If some property is not defined Blitz will just use its own predefined values. It will also warn you about it, and you'll see something like this in the console:
    ```bash
    [Blitz WRN] `blitz_version` is not defined: Using current Blitz version (`0.2.0`)
    [Blitz WRN] `site_url` is not defined: Using an empty string (``)
    ```
* As seen above, Blitz validates the config before using it to generate the website. In theory, this process should catch all of the mistakes made in the config and abort site generation if any errors will be found. That said, keep in mind it's still an experimental feature.