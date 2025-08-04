<h1>Cinder Theme Specimen</h1>

# Cinder主题样例

<h2 id="typography">Typography<a class="headerlink" href="#typography" title="Permanent link">¶</a></h2>

## 排版

<h3 id="typefaces">Typefaces<a class="headerlink" href="#typefaces" title="Permanent link">¶</a></h3>

### 字体

<ul>
<li>Headers: <a href="https://github.com/rsms/inter">Inter</a></li>
<li>Body: <a href="https://www.google.com/fonts/specimen/Open+Sans">Open Sans</a></li>
<li>Code: <a href="https://sourcefoundry.org/hack/">Hack</a></li>
</ul>
<h3 id="body-copy">Body Copy<a class="headerlink" href="#body-copy" title="Permanent link">¶</a></h3>

### 正文文本

<p>You think water moves fast? You should see ice. <strong>It moves like it has a mind</strong>. Like it knows it killed the world once and got a taste for murder. <em>After the avalanche, it took us a week to climb out</em>. Now, I don't know exactly when we turned on each other, but I know that seven of us survived the slide... and only five made it out.</p>
<p>Now we took an oath, that I'm breaking now. <a href="#">We said</a> we'd say it was the snow that killed the other two, but it wasn't.  Nature is lethal but it doesn't hold a candle to man.</p>
<p>Like inline code?  Here is a string for you <code>010101010</code>.</p>
<h3 id="lead-body-copy">Lead Body Copy<a class="headerlink" href="#lead-body-copy" title="Permanent link">¶</a></h3>

### 引导性正文文本

<p class="lead">Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor. Duis mollis, est non commodo luctus.</p>
<h3 id="headings">Headings<a class="headerlink" href="#headings" title="Permanent link">¶</a></h3>

### 标题

<p>All HTML headings, <code>&lt;h1&gt;</code> through <code>&lt;h6&gt;</code>, are available. <code>.h1</code> through <code>.h6</code> classes are also available, for when you want to match the font styling of a heading but still want your text to be displayed inline.</p>
<h1>h1. Heading</h1>

<h2>h2. Heading</h2>

<h3>h3. Heading</h3>

<h4>h4. Heading</h4>

<h5>h5. Heading</h5>

<h6>h6. Heading</h6>

<h1>h1. Heading <small>Secondary text</small></h1>

<h2>h2. Heading <small>Secondary text</small></h2>

<h3>h3. Heading <small>Secondary text</small></h3>

<h4>h4. Heading <small>Secondary text</small></h4>

<h5>h5. Heading <small>Secondary text</small></h5>

<h6>h6. Heading <small>Secondary text</small></h6>

<h3 id="blockquotes">Blockquotes<a class="headerlink" href="#blockquotes" title="Permanent link">¶</a></h3>

### 文本块

<blockquote>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.</p>
  <footer default-translate="no">Someone famous in <cite title="Source Title">Source Title</cite></footer>
</blockquote>

<h3 id="lists">Lists<a class="headerlink" href="#lists" title="Permanent link">¶</a></h3>

### 列表

<ul>
<li><code>mkdocs new [dir-name]</code> - Create a new project.</li>
<li><code>mkdocs serve</code> - Start the live-reloading docs server.</li>
<li><code>mkdocs build</code> - Build the documentation site.</li>
<li><code>mkdocs help</code> - Print this help message.</li>
</ul>
<h3 id="horizontal-description-lists">Horizontal Description Lists<a class="headerlink" href="#horizontal-description-lists" title="Permanent link">¶</a></h3>

### 水平描述列表

<dl class="dl-horizontal">
  <dt>Something</dt>
  <dd>This is something</dd>
  <dt>SomethingElse</dt>
  <dd>This is something else</dd>
</dl>

<h3 id="contextual-colors">Contextual Colors<a class="headerlink" href="#contextual-colors" title="Permanent link">¶</a></h3>

### 上下文颜色

<p class="text-muted">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.</p>

<p class="text-primary">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.</p>

<p class="text-success">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.</p>

<p class="text-info">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.</p>

<p class="text-warning">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.</p>

<p class="text-danger">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.</p>

<h2 id="code">Code<a class="headerlink" href="#code" title="Permanent link">¶</a></h2>

## 代码

<h3 id="inline-code">Inline Code<a class="headerlink" href="#inline-code" title="Permanent link">¶</a></h3>

### 内联代码

<p>This is an example of inline code <code>#import requests</code></p>
<h3>Preformatted Code Blocks <small>with Syntax Highlighting</small></h3>

### 预格式化代码块 <small>带高亮显示</small>

<pre><code class="python hljs"><span class="hljs-function"><span class="hljs-keyword">def</span> <span class="hljs-title">request</span><span class="hljs-params">(method, url, **kwargs)</span>:</span>
    <span class="hljs-string">"""Constructs and sends a :class:`Request </span><request><span class="hljs-string">`.
    Usage::
      &gt;&gt;&gt; import requests
      &gt;&gt;&gt; req = requests.request('GET', 'https://httpbin.org/get')
      </span><response [200]=""><span class="hljs-string">
    """</span>

    <span class="hljs-comment"># By using the 'with' statement we are sure the session is closed, thus we</span>
    <span class="hljs-comment"># avoid leaving sockets open which can trigger a ResourceWarning in some</span>
    <span class="hljs-comment"># cases, and look like a memory leak in others.</span>
    <span class="hljs-keyword">with</span> sessions.Session() <span class="hljs-keyword">as</span> session:
        <span class="hljs-keyword">return</span> session.request(method=method, url=url, **kwargs)

<span class="hljs-function"><span class="hljs-keyword">def</span> <span class="hljs-title">get</span><span class="hljs-params">(url, params=None, **kwargs)</span>:</span>
    <span class="hljs-string">r"""Sends a GET request.
    :param url: URL for the new :class:`Request` object.
    :param params: (optional) Dictionary, list of tuples or bytes to send
        in the body of the :class:`Request`.
    :param \*\*kwargs: Optional arguments that ``request`` takes.
    :return: :class:`Response </span><response><span class="hljs-string">` object
    :rtype: requests.Response
    """</span>

    kwargs.setdefault(<span class="hljs-string">'allow_redirects'</span>, <span class="hljs-literal">True</span>)
    <span class="hljs-keyword">return</span> request(<span class="hljs-string">'get'</span>, url, params=params, **kwargs)
</response></response></request></code></pre>

<div id="language-support"></div>

<p><small>(Source code sample from the Python <a href="https://github.com/requests/requests">requests library</a>, <a href="https://github.com/requests/requests/blob/master/LICENSE">Apache License, v2.0</a>)</small></p>
<p>Syntax highlighting support is available for and of the following languages listed on the <a href="https://highlightjs.org/download/">highlightjs website</a>. See the <a href="https://www.mkdocs.org/user-guide/styling-your-docs/">mkdocs "styling your docs"</a> hljs_languages section for info on how to load languages dynamically.</p>
<div class="bs-callout bs-callout-info">
  <h4>Note</h4>
  Include source code formatted in <a href="https://github.github.com/gfm/#fenced-code-blocks" class="alert-link">Github-flavored Markdown fenced code blocks</a> with an <a href="https://github.github.com/gfm/#info-string" class="alert-link">info string</a> that defines the supported programming language to automate syntax highlighting when your site is built.
</div>

<h2 id="tables">Tables<a class="headerlink" href="#tables" title="Permanent link">¶</a></h2>

## 表

<h3 id="striped-table">Striped Table<a class="headerlink" href="#striped-table" title="Permanent link">¶</a></h3>

### 条纹表

<table class="table table-striped table-hover">
  <thead>
      <tr>
        <th>#</th>
        <th>Head 1</th>
        <th>Head 2</th>
        <th>Head 3</th>
      </tr>
      </thead>
      <tbody>
      <tr>
        <th scope="row">1</th>
        <td>Box 1</td>
        <td>Box 2</td>
        <td>Box 3</td>
      </tr>
        <tr>
        <th scope="row">2</th>
        <td>Box 4</td>
        <td>Box 5</td>
        <td>Box 6</td>
      </tr>
      <tr>
        <th scope="row">3</th>
        <td>Box 7</td>
        <td>Box 8</td>
        <td>Box 9</td>
      </tr>
  </tbody>
</table>

<h3 id="bordered-table">Bordered Table<a class="headerlink" href="#bordered-table" title="Permanent link">¶</a></h3>

### 边界表

<table class="table table-bordered table-striped table-hover">
  <thead>
      <tr>
        <th>#</th>
        <th>Head 1</th>
        <th>Head 2</th>
        <th>Head 3</th>
      </tr>
      </thead>
      <tbody>
      <tr>
        <th scope="row">1</th>
        <td>Box 1</td>
        <td>Box 2</td>
        <td>Box 3</td>
      </tr>
        <tr>
        <th scope="row">2</th>
        <td>Box 4</td>
        <td>Box 5</td>
        <td>Box 6</td>
      </tr>
      <tr>
        <th scope="row">3</th>
        <td>Box 7</td>
        <td>Box 8</td>
        <td>Box 9</td>
      </tr>
  </tbody>
</table>

<h2 id="buttons">Buttons<a class="headerlink" href="#buttons" title="Permanent link">¶</a></h2>

## 按钮

<h3 id="default-buttons">Default Buttons<a class="headerlink" href="#default-buttons" title="Permanent link">¶</a></h3>

### 默认按钮

<p><a class="btn btn-default" href="#" role="button">Link</a>
<button class="btn btn-default" type="submit">Button</button>
<input class="btn btn-default" type="button" value="Input">
<input class="btn btn-default" type="submit" value="Submit"></p>
<h3 id="styled-buttons">Styled Buttons<a class="headerlink" href="#styled-buttons" title="Permanent link">¶</a></h3>

### 装饰按钮

<!-- Standard button -->

<p><button type="button" class="btn btn-default">Default</button> 默认</p>
<!-- Provides extra visual weight and identifies the primary action in a set of buttons -->

<p><button type="button" class="btn btn-primary">Primary</button> 主要</p>
<!-- Indicates a successful or positive action -->

<p><button type="button" class="btn btn-success">Success</button> 成功</p>
<!-- Contextual button for informational alert messages -->

<p><button type="button" class="btn btn-info">Info</button> 信息</p>
<!-- Indicates caution should be taken with this action -->

<p><button type="button" class="btn btn-warning">Warning</button> 警告</p>
<!-- Indicates a dangerous or potentially negative action -->

<p><button type="button" class="btn btn-danger">Danger</button> 危险</p>
<h3 id="button-sizes">Button Sizes<a class="headerlink" href="#button-sizes" title="Permanent link">¶</a></h3>

### 按钮尺寸

<p>
  <button type="button" class="btn btn-primary btn-lg">Large button</button>
  <button type="button" class="btn btn-default btn-lg">Large button</button>
</p>

<p>
  <button type="button" class="btn btn-primary">Default button</button>
  <button type="button" class="btn btn-default">Default button</button>
</p>

<p>
  <button type="button" class="btn btn-primary btn-sm">Small button</button>
  <button type="button" class="btn btn-default btn-sm">Small button</button>
</p>

<p>
  <button type="button" class="btn btn-primary btn-xs">Extra small button</button>
  <button type="button" class="btn btn-default btn-xs">Extra small button</button>
</p>

<h3 id="block-level-buttons">Block Level Buttons<a class="headerlink" href="#block-level-buttons" title="Permanent link">¶</a></h3>

### 区块层级

<p><button type="button" class="btn btn-primary btn-lg btn-block">Block level button</button>
<button type="button" class="btn btn-default btn-lg btn-block">Block level button</button></p>
<h2 id="alerts">Alerts<a class="headerlink" href="#alerts" title="Permanent link">¶</a></h2>

## 警告

<div class="alert alert-primary" role="alert">
  A simple primary alert—check it out!
</div>

<div class="alert alert-secondary" role="alert">
  A simple secondary alert—check it out!
</div>

<div class="alert alert-success" role="alert">
  A simple success alert—check it out!
</div>

<div class="alert alert-danger" role="alert">
  A simple danger alert—check it out!
</div>

<div class="alert alert-warning" role="alert">
  A simple warning alert—check it out!
</div>

<div class="alert alert-info" role="alert">
  A simple info alert—check it out!
</div>

<div class="alert alert-light" role="alert">
  A simple light alert—check it out!
</div>

<div class="alert alert-dark" role="alert">
  A simple dark alert—check it out!
</div>

<h2 id="callouts">Callouts<a class="headerlink" href="#callouts" title="Permanent link">¶</a></h2>

## 标注

<div class="bs-callout bs-callout-default">
  <h4>Default Callout</h4>
  This is a default callout.
</div>

<div class="bs-callout bs-callout-primary">
  <h4>Primary Callout</h4>
  This is a primary callout.
</div>

<div class="bs-callout bs-callout-success">
  <h4>Success Callout</h4>
  This is a success callout.
</div>

<div class="bs-callout bs-callout-info">
  <h4>Info Callout</h4>
  This is an info callout.
</div>

<div class="bs-callout bs-callout-warning">
  <h4>Warning Callout</h4>
  This is a warning callout.
</div>

<div class="bs-callout bs-callout-danger">
  <h4>Danger Callout</h4>
  This is a danger callout.
</div>

<h2 id="admonitions">Admonitions<a class="headerlink" href="#admonitions" title="Permanent link">¶</a></h2>

## 告诫

<p>The following admonitions are formatted like the callouts above but can be implemented in Markdown when you include the <code>admonition</code> Markdown extension in your <code>mkdocs.yml</code> file.  </p>
<p>Add the following setting to <code>mkdocs.yml</code>:</p>
<pre><code class="yaml hljs"><span class="hljs-attr">markdown_extensions:</span>
  <span class="hljs-bullet">-</span> <span class="hljs-string">admonition</span>
</code></pre>

<p>and then follow the instructions in <a href="https://python-markdown.github.io/extensions/admonition/">the extension documentation</a> to author admonitions in your documentation.</p>
<p>Cinder currently supports <code>note</code>, <code>warning</code>, and <code>danger</code> admonition types.</p>
<div class="admonition note">
<p class="admonition-title">Note</p>
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
massa, nec semper lorem quam in massa.</p>
<p></p><pre><code class="hljs ruby">
<span class="hljs-comment"># this is a note</span>
<span class="hljs-function"><span class="hljs-keyword">def</span> <span class="hljs-title">func</span><span class="hljs-params">(arg)</span></span> {
  <span class="hljs-comment"># notable things are in here!</span>
  <span class="hljs-keyword">return</span> None
}
</code></pre><p></p>
</div>
<div class="admonition warning">
<p class="admonition-title">Warning</p>
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
massa, nec semper lorem quam in massa.</p>
<p></p><pre><code class="hljs ruby">
<span class="hljs-comment"># this is a warning</span>
<span class="hljs-function"><span class="hljs-keyword">def</span> <span class="hljs-title">func</span><span class="hljs-params">(arg)</span></span> {
  <span class="hljs-comment"># be careful!</span>
  <span class="hljs-keyword">return</span> None
}
</code></pre><p></p>
</div>
<div class="admonition danger">
<p class="admonition-title">Danger</p>
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
massa, nec semper lorem quam in massa.</p>
<p></p><pre><code class="hljs ruby">
<span class="hljs-comment"># this is dangerous</span>
<span class="hljs-function"><span class="hljs-keyword">def</span> <span class="hljs-title">func</span><span class="hljs-params">(arg)</span></span> {
  <span class="hljs-comment"># BOOM!</span>
  <span class="hljs-keyword">return</span> None
}
</code></pre><p></p>
</div></div>