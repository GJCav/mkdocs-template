# Configure Google Analytics

Read the  [official guide](https://squidfunk.github.io/mkdocs-material/setup/setting-up-site-analytics/) if you haven't used the google-analytics before.

## Enable Google Analytics

For development (live preview):

``` bash
export G_PROPERTY="G-XXXXXXXX"
make serve

# build locally
make build
```

For github-pages:

* Set a repository variable named `G_PROPERTY` with your google property id

* Trigger `ci.yaml` to update changes

The [cookie consent](https://squidfunk.github.io/mkdocs-material/setup/ensuring-data-privacy/#cookie-consent) is enabled with the google analytics.

## Disable Google Analytics

Unset the environment and delete the repository variable.

## How does this work ?

See `Makefile` in the github repository.