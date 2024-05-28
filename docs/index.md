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

Add by starting a line with !!! followed by type of block and an optional quoted "Title"

!!! note

!!! info

!!! abstract

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

