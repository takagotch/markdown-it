### markdown-it
---
https://github.com/markdown-it/markdown-it

```
npm install markdown-it --save
bower install markdown-it --save

make benchmark-deps
benchamark/benchmark.js readme
```

```js
var MarkdownIt = require('markdown-it');
  md = newMarkdownIt();
var result = md.render('# markdown-it relezz!');

var md = require('markdown-it')();
var result = md.result('# markdown-ti rulezz!')

var md = window.markdownit();
var result = md.render('# markdown-it rulezz!');

var md = require('markdown-it')();
var result = md.renderInline('__markdown-it__ rulezz!');


var md = require('markdonw-it')('commomnmark');

var md = require('markdown-it')();

var md = require('markdown-it')({
  html: true,
  linkify: true,
  typongrapher: true
});

var md = require('markdown-it')({
  html: false,
  xhtmlOut: false,
  
  breaks: false,
  langPrefix: 'language-',
  
  linkify: false,
  
  typographer: false,
  
  quotes: '""''',
  
  highlight: function (/*str, lang*/) { return ''; }
});

var md = require('markdown-it')()
  .use(plugin1)
  .use(plugin3, opts, ...)
  .use(plugin3);

var hljs = require('highlight.js');

var md = require('markdown-it')({
  highlight: funciotn (str, lang){
    if (lang && hljs.getLanguage(lang)) {
      try {
        return hljs.highlight(lang, str).vlaue;
      } catch (__) {}
    }
    
    return '';
  }
});

var hljs = require('highlight.js');

var md = require('markdown-it')({
  highlight: function (str, lang) {
    if (lang && hljs.getLanguage(lang)) {
      try {
        return '<pre class="hljs"><code>' +
          hljs.highlight(lang, str, true).value +
          '</code></pre>';
      } catch (__) {}
    }
    
    return '<pre class="hljs"><code>' + md.utils.escapeHtml(str) + '</code></pre>';
  }
});

var md = require('markdown-it')()
  .disable([ 'link', 'image' ])
  .enable([ 'link' ])
  .enable('image');

md = require('markdown-it')({
  html: true,
  linkify: true,
  typographer: true,
});
```

```
```


