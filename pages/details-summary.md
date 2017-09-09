---
title: details and summary elements
last_updated: 2 September, 2017
summary: "WIP"
sidebar: default
permalink: details-summary
---

## Advised markup

### Emmet
```css
details>summary[role="button"][tabindex="0"][aria-controls="content"]{title}+#content[hidden=""]{content text}
```

### HTML
```html
<details>
	<summary role="button" tabindex="0" aria-controls="content">
		Title here
	</summary>
	<div id="content" hidden>
		Content here
	</div>
</details>
```

{% include custom/screen_reader_results.liquid stats=site.data.results.details.stats %}

##  Browser support

<p class="ciu_embed" data-feature="details" data-periods="future_2,future_1,current,past_1,past_2">
  <a href="http://caniuse.com/#feat=details">Can I Use details?</a> Data on support for the details feature across the major browsers from caniuse.com.
</p>
<script src="//cdn.jsdelivr.net/caniuse-embed/1.1.0/caniuse-embed.min.js"></script>

## Specifications
* [MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/details)
* [HTML 5.1 - details element](https://www.w3.org/TR/html/interactive-elements.html#the-details-element)
* [HTML 5.1 - summary element](https://www.w3.org/TR/html/interactive-elements.html#the-summary-element)
* [HTML Accessibility mapping - summary element](https://w3c.github.io/html-aam/#summary-element)
* [HTML Accessibility mapping - feature implementation](https://w3c.github.io/html-aam/#summary-and-details-elements)
* [WAI-ARIA - disclosure](https://www.w3.org/TR/wai-aria-practices/#disclosure)
