# Configure Navigation 

Navigation is enhanced with [awesome-pages](https://github.com/lukasgeiter/mkdocs-awesome-pages-plugin). Refer to official site for complete information. 

Here is a quick guide:

For EVERY directory, no matter root or sub-directory, create a `.pages` file for it. List the files and subdirectories in the order that they should appear in navigation.

``` yaml title=".pages"
nav:
- page1.md
- page2.md
- subdir      # and create `.pages` under `subdir` for further navigation.
- ...         # list other files in this folder
```

If a directory doesn't have a `.pages` file, all files and sub-directories are added to navigation recursively.