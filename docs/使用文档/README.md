<center>嵌入官方的使用文档，以备不时之需</center>

> 官方中文文档：https://docsify.js.org/#/zh-cn/deploy

<link rel="stylesheet" href="https://fastly.jsdelivr.net/npm/docsify-themeable@0/dist/css/theme-simple.css" title="simple">
<link rel="stylesheet" href="https://fastly.jsdelivr.net/npm/docsify-themeable@0/dist/css/theme-simple-dark.css" title="simple-dark" disabled="">
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/docsify-themeable@0/dist/css/theme-defaults.css" title="defaults" disabled="">
<link rel="stylesheet" href="//cdn.jsdelivr.net/npm/docsify/lib/themes/vue.css" title="vue" disabled="">
<link rel="stylesheet" href="//cdn.jsdelivr.net/npm/docsify/lib/themes/buble.css" title="buble" disabled="">
<link rel="stylesheet" href="//cdn.jsdelivr.net/npm/docsify/lib/themes/dark.css" title="dark" disabled="">
<link rel="stylesheet" href="//cdn.jsdelivr.net/npm/docsify/lib/themes/pure.css" title="pure" disabled="">
<link rel="stylesheet" href="//cdn.jsdelivr.net/npm/docsify/lib/themes/dolphin.css" title="dolphin" disabled="">

## 主题切换
<div class="demo-theme-preview">
  <a data-theme="simple">simple</a>
  <a data-theme="simple-dark">simple-dark</a>
		<a data-theme="vue">vue</a>
		<a data-theme="buble">buble</a>
		<a data-theme="dark">dark</a>
		<a data-theme="pure">pure</a>
		<a data-theme="dolphin">dolphin</a>
</div>

<script>
  var preview = Docsify.dom.find('.demo-theme-preview');
  var themes = Docsify.dom.findAll('[rel="stylesheet"]');

  preview.onclick = function (e) {
    var title = e.target.getAttribute('data-theme')

    themes.forEach(function (theme) {
      theme.disabled = theme.title !== title
    });
  };
</script>
