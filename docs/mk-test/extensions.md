# Markdown Extensions

## icons & emojis

[official guide: icon & emoji](https://squidfunk.github.io/mkdocs-material/reference/icons-emojis/)

:smile: :fontawesome-regular-face-laugh-wink:

:fontawesome-brands-twitter:{ .twitter }


## admonition

!!! note "Phasellus posuere in sem ut cursus"

    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.

???+ note

    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.

other admonition types: refer to this [list](https://squidfunk.github.io/mkdocs-material/reference/admonitions/#supported-types) for all types

???+ danger

    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor massa, nec semper lorem quam in massa.


## Annotations

[official guide](https://squidfunk.github.io/mkdocs-material/reference/annotations/)

**in admonition**

!!! note annotate "annotation in admonition (1)"

    Lorem ipsum dolor sit amet, (2) consectetur adipiscing elit. Nulla et
    euismod nulla. Curabitur feugiat, tortor non consequat finibus, justo
    purus auctor massa, nec semper lorem quam in massa.

1.  I'm an annotation!
2.  I'm an annotation as well!


**nested annotations**

Lorem ipsum dolor sit amet, (1) consectetur adipiscing elit.
{ .annotate }

1.  I'm an annotation! (1)(2)
    { .annotate }

    1.  I'm an annotation as well!
    2.  2nd annotation


## Buttons

[link as a button :fontawesome-solid-paper-plane:](https://squidfunk.github.io/mkdocs-material/reference/buttons/){.md-button}

## Code blocks

[official guide: code blocks](https://squidfunk.github.io/mkdocs-material/reference/code-blocks/)

In addition to markdown code block, this extension offers advanced features:

* a copy button
* annotation in code block
* code block title
* line numbers
* line highlight

``` python title="block title" linenums="1" hl_lines="1 4"
def func():
    printf("hello world") # (1)

func()
```

1.  :man_raising_hand: I'm a code annotation!


and, import data from external file:

``` title="file code-example.py"

--8<-- "code-example.py"

```

NOT WORKING


## Content tabs



=== "tab 1"

    [guide: tabs](https://squidfunk.github.io/mkdocs-material/reference/content-tabs/)

    !!! example embedded tab

        === "nested tab 1"

            some text here.

        === "nested tab 2"

            some text there.

=== "tab 2"

    ``` py title="code in tab"
    print("hello tabs!")
    ```

## Diagrams

[guide: diagrams](https://squidfunk.github.io/mkdocs-material/reference/diagrams/)

Supported by `Mermaid.js`

``` mermaid
sequenceDiagram
  autonumber
  Alice->>John: Hello John, how are you?
  loop Healthcheck
      John->>John: Fight against hypochondria
  end
  Note right of John: Rational thoughts!
  John-->>Alice: Great!
  John->>Bob: How about you?
  Bob-->>John: Jolly good!
```


## Footnote

[guide: footnote](https://squidfunk.github.io/mkdocs-material/reference/footnotes/)

``` markdown
Lorem ipsum[^1] dolor sit amet, consectetur adipiscing elit.[^2]

[^1]: Lorem ipsum dolor sit amet, consectetur adipiscing elit.
[^2]:
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.
```

Lorem ipsum[^1] dolor sit amet, consectetur adipiscing elit.[^2]

[^1]: Lorem ipsum dolor sit amet, consectetur adipiscing elit.
[^2]:
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.

NOTE: the content of footnote can be placed at arbitary position but is rendered at the end of the page.

## Advanced list

**Task list**:

- [x] Lorem ipsum dolor sit amet, consectetur adipiscing elit
- [ ] Vestibulum convallis sit amet nisi a tincidunt
    * [x] In hac habitasse platea dictumst
    * [x] In scelerisque nibh non dolor mollis congue sed et metus
    * [ ] Praesent sed risus massa
- [ ] Aenean pretium efficitur erat, donec pharetra, ligula non scelerisque





**Definition list**:

`Lorem ipsum dolor sit amet`

:   Sed sagittis eleifend rutrum. Donec vitae suscipit est. Nullam tempus
    tellus non sem sollicitudin, quis rutrum leo facilisis.

`Cras arcu libero`

:   Aliquam metus eros, pretium sed nulla venenatis, faucibus auctor ex. Proin
    ut eros sed sapien ullamcorper consequat. Nunc ligula ante.

    Duis mollis est eget nibh volutpat, fermentum aliquet dui mollis.
    Nam vulputate tincidunt fringilla.
    Nullam dignissim ultrices urna non auctor.
