# Comment System

Comment system is support by [giscus](https://giscus.app/). The majority of 
the configuration follows the [official guide](https://squidfunk.github.io/
mkdocs-material/setup/adding-a-comment-system/). But there are some changes.


## Giscus configuration

Recommended configuration:

* Page Mapping: `pathname`

    :bulb: The page URL is bind to relative path to the page code. Thus don't change 
    the file name if there have been comments already.

* Strict title matching: `enabled`
* Discussion Category:
    1.  Create a new category named `Comments` with the format `Announcements`

        :bulb: A new category avoids messing up normal discussions and the format 
        `Announcements` ensures that new discussions can only be created by 
        maintainers and giscus.

    2.  Select this `Comments`


* Features: 
    * :white_check_mark: Enable reactions for the main post 
    * :white_check_mark: Place the comment box above the comments 
    * :white_check_mark: Load the comments lazily 


Now the snippet should look similar to this

``` html
<script src="https://giscus.app/client.js"
    data-repo="<user>/<repo>"
    data-repo-id="<id>"
    data-category="Comments"
    data-category-id="..."
    data-mapping="pathname"
    data-strict="1"
    data-reactions-enabled="1"
    data-emit-metadata="0"
    data-input-position="bottom"
    data-theme="preferred_color_scheme"
    data-lang="en"
    data-loading="lazy"
    crossorigin="anonymous"
    async>
</script>
```

Finally, enable giscus in `mkdocs.yml`:

``` yaml title="mkdocs.yml"
giscus: true
```


## Customize `comments.html` partial

Follow the official guide but edit the `comments.html` from

``` html title="official snippet" hl_lines="1"
{% if page.meta.comments %}
  <h2 id="__comments">{{ lang.t("meta.comments") }}</h2>
  ...
{% endif %}
```

to 

``` html title="revision" hl_lines="1"
{% if config.giscus and not (page and page.meta and page.meta.disable_comments) %}
  <h2 id="__comments">{{ lang.t("meta.comments") }}</h2>
  ...
{% endif %}
```

The revision enables comment system for all pages without use of paid plugin 
`meta`. To disable the feature for certain page, add the following meta to 
the head of the markdown code.

``` yaml
---
disable_comments: true
---
```