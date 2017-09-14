---
title: "Buttons"
last_updated: 2 September, 2017
summary: "WIP"
sidebar: default
permalink: buttons
---

## `<button type="menu">`

While in the HTML 5.1 spec, it is removed in the HTML living standard. Dropped because lack of support by browsers.  
It was only used opening [menus][1]. At this moment there isn't a spec. for adding menu items to the context menu.

## Advised markup

### Emmet

```css
button[type="button"]
```

#### Toggle button
```css
button[type="button"][aria-pressed]
```

#### Menu button
```css
button[type="button"][aria-haspopup][aria-expanded]
```

### HTML
```html
<button type="button"></button>
```

#### Toggle button
```html
<button type="button" aria-pressed="false"></button>
```

#### Menu button
```html
<!-- when closed -->
<button type="button" aria-haspopup="true"></button>

<!-- when opened -->
<button type="button" aria-haspopup="true" aria-expanded="true"></button>
```

{% include custom/screen_reader_results.liquid stats=site.data.results.buttons %}

### Menu Button

## Specifications
* [HTML 5.1 - button element](https://www.w3.org/TR/html/sec-forms.html#the-button-element)
* [HTML living standard - button element](https://html.spec.whatwg.org/multipage/form-elements.html#the-button-element)
* [HTML 5.1 - input[type=submit] element](https://www.w3.org/TR/html/sec-forms.html#submit-button-state-typesubmit)
* [HTML 5.1 - input[type=reset] element](https://www.w3.org/TR/html/sec-forms.html#reset-button-state-typereset)
* [HTML 5.1 - input[type=button] element](https://www.w3.org/TR/html/sec-forms.html#button-state-typebutton)
* [HTML living standard - input[type=button] element](https://html.spec.whatwg.org/multipage/input.html#button-state-(type=button))
* [HTML Accessibility mapping - input[type=submit], input[type=reset], input[type=button]](https://www.w3.org/TR/html-aam-1.0/#input-type-button-input-type-submit-and-input-type-reset)
* [HTML Accessibility mapping - button](https://w3c.github.io/html-aam/#button-element)
* [WAI-ARIA practices - button](https://www.w3.org/TR/wai-aria-practices/#button)
* [WAI-ARIA practices - Menu Button](https://www.w3.org/TR/wai-aria-practices/#button)

[1]: {{ site.baseurl }}/menu#menu
