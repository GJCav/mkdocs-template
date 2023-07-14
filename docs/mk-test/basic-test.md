# Use Markdown

[TOC]

Yes, Doxygen can processing `.md` files !! 



## h2

This is `h2` title.



### h3

#### h4

## basic function test

**bold text**

*italic text*

> quote

ordered list test:

1. list 1

2. list 2

3. list 3, nested list test

   1. list 1.a
   2. list 1.b
      1. list 1.b.i
         1. list 1.b.8.alpha
      2. list 1.b.ii
   3. list 1.c

4. list 4, nested block test

   > quote, asdfasdfasdfeeee. Not supported yet. Doxygen treated nested quote blocks as if there were not nested: no indent is added to the left. But common markdown editors, such as typora, correctly render the nested hierarchy and add the indent.

   * hello
   * unordered list



horizontal division

---------------------

code block

```cpp
Student::Student(int name, int address) {
    this->name = name;
    this->address = address;
    this->cls = nullptr;
}
```

```python
import numpy as np
import scipy.signal

def hello(name):
   print(f"hello {name}")

```


## image test

![](typora/test-image.png)


## table test

| hello    | effae  | bdef       |
| -------- | ------ | ---------- |
| alsekjlf | lklkje |            |
| lkke     |        | lkjldkjkfe |
| ---      | --     | dfe        |





## html test

If rendered correctly, there is a red block on the `some text here` and a yellow block on the right.

<div style="display: flex;">
    <div style="display: block; width: 30px; height: 30px; background-color: red;"></div>
    <div>some text here</div>
    <div style="display: block; width: 30px; height: 30px; background-color: yellow;"></div>
</div>


## hide sidebars

See [official guide: hide sidebars](https://squidfunk.github.io/mkdocs-material/setup/setting-up-navigation/#hiding-the-sidebars)
