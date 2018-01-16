---
title: "&lt;meter&gt;"
last_updated: 16 Januari, 2018
summary: "WIP"
sidebar: default
permalink: meter
---

The aria specification does not specify an native mapping or aria role to the meter element. 

I would propose to use the role `slider` with `aria-readonly="true"` as fallback. As the both supposed to show a range that is not changeable by the user.

{% include note.html content="IE doesn't natively support the meter elements" %}

## Advised markup

### Emmet

```css
meter[role="slider"][aria-valuemin="0"][aria-valuemax="1"][aria-readonly="true"][aria-valuenow][value]
```

### HTML

```html
<meter role='slider' aria-readonly="true" aria-valuemin="0" aria-valuemax="1" value="0.3" aria-valuenow="0.3">
</meter>
```

{% include custom/screen_reader_results.liquid stats=site.data.results.meter %}

##  Browser support

<p class="ciu_embed" data-feature="meter" data-periods="future_2,future_1,current,past_1,past_2">
  <a href="http://caniuse.com/#feat=meter">Can I Use meter?</a> Data on support for the meter feature across the major browsers from caniuse.com.
</p>
<script src="//cdn.jsdelivr.net/caniuse-embed/1.1.0/caniuse-embed.min.js"></script>

## Specifications
* [MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/meter)
* [HTML 5 - meter element](https://www.w3.org/TR/html/interactive-elements.html#the-meter-element)