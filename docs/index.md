# Welcome to my Mkdocs-template project

This is a MkDocs-template project.

## Features

out-of-box features

* theme: [mkdocs-material](https://squidfunk.github.io/mkdocs-material/) with version `9.2.0b0`
* math support with MathJax3
* markdown extension: [example](./mk-test/extensions.md)
* fine-grained navigation control with [awesome-pages](https://github.com/lukasgeiter/mkdocs-awesome-pages-plugin) 
* search: both English and Chinese

    !!! warning
        
        Chinese language is supported by Japanese language. So unwanted effects may occur.


## Quick start

**Install**

1. Create a virtual environment

    Installing `mkdocs-material` from pip results in a legacy `mkdocs-material` version but this template adopts the latest mkdocs-material so locally installation is necessary and unavoidable mess your python environment. Thus a virtual python environment is HIGHLY recommended.

    In 2023, please select a modern virtual env manager. Personally, I prefer `miniconda`.
    
    Make sure that you have activated a virtual environment before continue the installation.

2. Clone repo

    ``` bash
    git clone --recursive https://github.com/GJCav/mkdocs-template.git
    ```
    

3. Install `mkdocs-material`

    ``` bash
    cd mkdocs-material
    git checkout 9.2.0b0
    pip3 install -e .
    ```

4. Install `awesome-pages`

    ``` bash
    pip3 install mkdocs-awesome-pages-plugin
    ```

4. Customize

    Open file `mkdocs.yml` and modify the `site_name`, `site_url` and `repo_url`.


**Live preview**
``` bash
mkdocs serve
```

**Build**
``` bash
mkdocs build
```

## LICENSE

```
MIT License

Copyright (c) 2023 GJCav(https://github.com/GJCav)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```