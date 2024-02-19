# slidev-theme-vatisv2

[![NPM version](https://img.shields.io/npm/v/slidev-theme-vatisv2?color=3AB9D4&label=)](https://www.npmjs.com/package/slidev-theme-vatisv2)

A Normal theme for [Slidev](https://github.com/slidevjs/slidev).

<!--
  Learn more about how to write a theme:
  https://sli.dev/themes/write-a-theme.html
--->

<!--
  run `npm run dev` to check out the slides for more details of how to start writing a theme
-->

<!--
  Put some screenshots here to demonstrate your theme

  Live demo: [...]
-->

## Install

Add the following frontmatter to your `slides.md`. Start Slidev then it will prompt you to install the theme automatically.

<pre><code>---
theme: <b>vatisv2</b>
---</code></pre>

Learn more about [how to use a theme](https://sli.dev/themes/use).

## Layouts

This theme provides the following layouts:

* Cover
* Contents
* default
* end

具体效果参见 `example.pdf` 及 `example.md`。

Contents为目录页，为自动生成的页面。只需在扉页填写好 `sections` 字段，并在需要的地方插入：

```yaml
---
layout: contents
---

---
```

即可。

end为结束的致谢页面，其中此页的一级标题会放大居中，如有其他紧随其后的内容会往下居中放置。

在默认页面中会有页面指示器，这依赖于扉页的`sections` 字段：


```yaml
sections: 
  - [研究背景,3]
  - [研究内容,4]
  - [技术路线,5]
```


其中的每一条为一个section的标志，每一条写作一个列表，列表的第一个内容为section的名称，第二个内容为相应的起始页码。

## Components

This theme provides the following components:

> TODO:

## Contributing

- `npm install`
- `npm run dev` to start theme preview of `example.md`
- Edit the `example.md` and style to see the changes
- `npm run export` to generate the preview PDF
- `npm run screenshot` to generate the preview PNG
