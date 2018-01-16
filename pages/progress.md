---
title: "&lt;progress&gt;"
last_updated: 16 Januari, 2018
summary: "WIP"
sidebar: default
permalink: progress
---

#### Keep in mind

* `aria-valuemin` should always be equal to `min`
* `aria-valuemax` should always be equal to `max`
* `aria-valuenow` should always be equal to `value`
* values that are higher than the allowed max value could result in unwanted behavior

## Advised markup

### Emmet

```css
progress[role="progressbar"][aria-valuenow][value]
```

### HTML

```html
<progress role='progressbar' value="" aria-valuenow="">
</progress>
```

{% include custom/screen_reader_results.liquid stats=site.data.results.progress %}

##  Browser support

<p class="ciu_embed" data-feature="progress" data-periods="future_2,future_1,current,past_1,past_2">
  <a href="http://caniuse.com/#feat=progress">Can I Use progress?</a> Data on support for the progress feature across the major browsers from caniuse.com.
</p>
<script src="//cdn.jsdelivr.net/caniuse-embed/1.1.0/caniuse-embed.min.js"></script>

## Specifications
* [MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/progress)
* [HTML 5 - progress element](https://www.w3.org/TR/html/sec-forms.html#the-progress-element)