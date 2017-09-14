---
title: "&lt;svg&gt;"
last_updated: 2 September, 2017
summary: "WIP"
sidebar: default
permalink: svg
---

{% assign svg-inline =  site.data.results.svg[2] %}
{% assign svg-symbol =  site.data.results.svg[4] %}

## Advised markup

## Emmet

```css
{{ svg-inline.emmet }}
```

### Symbols

```css
{{ svg-symbol.emmet }}
```

## HTML

```html
{{ svg-inline.code }}
```

### Symbols

```html
{{ svg-symbol.code }}
```

{% include custom/screen_reader_results.liquid stats=site.data.results.svg %}

## Specifications

* [Paciello group](https://www.paciellogroup.com/blog/2013/12/using-aria-enhance-svg-accessibility/)
* [MDN](https://developer.mozilla.org/en-US/docs/Web/SVG/Element/svg)
* [SVG Accessibility API Mappings](https://w3c.github.io/aria/svg-aam/svg-aam.html#mapping_role_table)
