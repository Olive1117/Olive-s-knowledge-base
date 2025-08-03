# Welcome to MkDocs
# <p id="anchor-name">标题</p>
这是一个需要添加锚点的段落 {id = "paragraph-id"}
For full documentation visit [mkdocs.org](https://www.mkdocs.org).

## Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.

## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.
[跳转到标题](#anchor-name)
[跳转到段落](#paragraph-id)

[跳转到说明](#explanation)

## 说明 {#explanation}
<a name="锚点名称">A</a>
<button type="button" class="btn btn-primary">Primary</button>
<div class="alert alert-dark" role="alert">
  A simple dark alert—check it out!
</div>
<div class="bs-callout bs-callout-warning">
  <h4>Warning Callout</h4>
  This is a warning callout.
</div>
<div class="bs-callout bs-callout-info">
  <h4>Note</h4>
  Include source code formatted in <a href="https://github.github.com/gfm/#fenced-code-blocks" class="alert-link">Github-flavored Markdown fenced code blocks</a> with an <a href="https://github.github.com/gfm/#info-string" class="alert-link">info string</a> that defines the supported programming language to automate syntax highlighting when your site is built.
</div>
<code>mkdocs new [dir-name]</code>