---
layout: "docs_api"
version: "unstable"
versionHref: "/docs/unstable"
path: "api/directive/ngDblclick/"
title: "ng-dblclick"
header_sub_title: "Directive in module scripts"
doc: "ngDblclick"
docType: "directive"
---

<div class="improve-docs">
  <a href='https://github.com/Famous/famous-angular/edit/master/src/scripts/directives/fa-input.js#L275'>
    Improve this doc
  </a>
</div>





<h1 class="api-title">

  ng-dblclick



</h1>





This wrapped on `ngDblclick` directive allows you to specify custom behavior on a dblclick event on a fa-surface .






  
<h2 id="usage">Usage</h2>
  
```html
<ANY ng-dblclick="expression">

</ANY>
```
  
  
<h2 id="api" style="clear:both;">API</h2>

<table class="table" style="margin:0;">
  <thead>
    <tr>
      <th>Attr</th>
      <th>Type</th>
      <th>Details</th>
    </tr>
  </thead>
  <tbody>
    
    <tr>
      <td>
        ngDblclick
        
        
      </td>
      <td>
        
  <code>expression</code>
      </td>
      <td>
        <p><a href="guide/expression">Expression</a> to evaluate upon
a dblclick. (The Event object is available as <code>$event</code>)</p>

        
      </td>
    </tr>
    
  </tbody>
</table>

  

  



<h2 id="example">Example</h2><p>

{% assign lvl = page.url | append:'X' | split:'/' | size %}
{% capture relative %}{% for i in (3..lvl) %}../{% endfor %}{% endcapture %}

<div>
  <a ng-click="openPlunkr('{{ relative }}examples/example-example')" class="btn pull-right">
    <i class="glyphicon glyphicon-edit">&nbsp;</i>
    Edit in Plunker</a>
  <div class="runnable-example" path="examples/example-example"
      
  >

   
    <div class="runnable-example-file"
      
        name="index.html"
      
        language="html"
      
        type="html"
      
    >
      <pre><code>&lt;fa-surface ng-dblclick=&quot;count = count + 1&quot; ng-init=&quot;count=0&quot;&gt;&#13;&#10;  Increment (on double click), count: {{count}}&#13;&#10;&lt;/fa-surface&gt;&#13;</code></pre>
    </div>
  
    <div class="runnable-example-file"
      
        name="style.css"
      
        language="css"
      
        type="css"
      
    >
      <pre><code>body {&#13;&#10;  -webkit-user-select: none;&#13;&#10;  -moz-user-select: none;&#13;&#10;  -ms-user-select: none;&#13;&#10;  user-select: none;&#13;&#10;}&#13;&#10;fa-surface {&#13;&#10;  cursor: pointer;&#13;&#10;}&#13;</code></pre>
    </div>
  

    <iframe class="runnable-example-frame" src="{{ relative }}examples/example-example/index.html" name="example-example"></iframe>
  </div>
</div>


</p>


