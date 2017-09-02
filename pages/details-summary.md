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
details>summary[role=button tabindex=0 aria-controls=content]{title}+#content[hidden=""]{content}
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

<!-- ## Your browser support
<script>
var res = {};

var summary = document.createElement("summary");
var details = document.createElement("details");
details.appendChild(summary);

res.detailsElementExists = Object.prototype.toString.call(details) == '[object HTMLDetailsElement]';
res.hasOpenProperty = details.open !== undefined;
res.hasCorrectValue = details.open === false;
res.hasntOpenAttributeWhenClosed = !details.hasAttribute("open");

var prevOpenValue = details.open;

summary.addEventListener("click", console.log);
details.addEventListener("toggle", (ev) => {
	res.toggleEventIsTriggeredWhenClicket = true;
});

// var observer = new MutationObserver((mutations) => {
//   mutations.forEach((mutation) => {
//     console.log(mutation);
//   });    
// });
// observer.observe(details, {attributeFilter: ["open"]});

var event = document.createEvent('KeyboardEvent');
event.initKeyEvent("keypress", true, true, null, false, false, false,  false, 32, 0);
// summary.dispatchEvent(event);

var event = document.createEvent('KeyboardEvent');
event.initKeyEvent("keypress", true, true, null, false, false, false,  false, 13, 0);
summary.dispatchEvent(event);
res.hasOpenValueAfterClicked = details.open !== undefined;
res.hasCorrectValueAfterClicked = details.open === !prevOpenValue;
res.hasOpenAttributeAfterOpened = details.hasAttribute("open");

var output = document.createElement("p");
output.innerHTML = JSON.stringify(res, null, 2);
document.currentScript.parentNode.insertBefore(output, document.currentScript.nextSibling);
</script> -->

{% include custom/screenReaderResults.liquid stats=site.data.details.stats %}

##  Browser support

<p class="ciu_embed" data-feature="details" data-periods="future_2,future_1,current,past_1,past_2">
  <a href="http://caniuse.com/#feat=details">Can I Use details?</a> Data on support for the details feature across the major browsers from caniuse.com.
</p>
<script src="//cdn.jsdelivr.net/caniuse-embed/1.1.0/caniuse-embed.min.js"></script>

## Specifications
* [MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/details)
* [HTML 5.1 #details](https://www.w3.org/TR/html/interactive-elements.html#the-details-element)
* [HTML 5.1 #summary](https://www.w3.org/TR/html/interactive-elements.html#the-summary-element)
* [WAI-ARIA #disclosure](https://www.w3.org/TR/wai-aria-practices/#disclosure)
