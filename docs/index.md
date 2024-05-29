# Welcome to MkDocs

* Basic documentation [mkdocs.org](https://www.mkdocs.org).
* Useful documentation [material](https://squidfunk.github.io/mkdocs-material/reference/)
* Advanced extensions [PyMdown Extension](https://facelessuser.github.io/pymdown-extensions/extensions/arithmatex/)

# Installation

`pip install mkdocs-material pymdown-extensions pygments`

## Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.

## Admonitor styles:

Create **highlighted blocks** with `!!!` followed by type of block and an optional quoted "Title".  
Make them **collapsable** with `???`  instead of `!!!`  
Use `???+ note "Title"` for collapsable, but by default **open** blocks.

!!! note

??? info "info collapsable"
    Some content

???+ abstract "abstrac with ???+"
    Some content

!!! tip

!!! success

!!! question

!!! warning

!!! failure

!!! danger

!!! bug

!!! example

!!! quote


## Latex

* Inline

`$k=\frac{k_bT}{h} \exp(\frac{dG}{RT})$`

$k=\frac{k_bT}{h} \exp(\frac{dG}{RT})$

* or bigger blocks

```
$$
k=\frac{k_bT}{h} \exp(\frac{dG}{RT})
$$
```


$$
k=\frac{k_bT}{h} \exp(\frac{dG}{RT})
$$

## SSH access

`.ssh/config` on remote machine. Allowes accessing the documentation in the browser.

```bash title=".ssh/config" hl_lines="6"
Host mypc
    HostName mypc
    User ...
    ForwardX11 yes
    Compression yes 
    LocalForward 8000 localhost:8000
```

## Markdown cheatsheet

Heading starts with #

Subheading starts with ##

**bold** `**bold**`

*italic* `*italic*`

`inline code` ``` `inline code` ```

[link text](to.some.website) `[link text](to.some.website)`

![embedded images](image.jpg) `![embedded images](image.jpg)`

> quote block, can span multiple lines  
`> quote block`

Superscript^link^ `Superscript^link^`

Subscript H~2~O `H~2~O`

* [ ] Task lists `* [ ] Task lists`
* [x] Task lists `* [x] Task lists`

--> `-->` +/- `+/-` =/= `=/=`


### Longer code blocks
```
    ```python
    import numpy
    ```
```

### Tables

| Syntax | Description |
| ----------- | ----------- |
| Header | Title |
| Paragraph | Text |

```
| Syntax | Description |
| ----------- | ----------- |
| Header | Title |
| Paragraph | Text |
```
