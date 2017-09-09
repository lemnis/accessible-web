---
title: "Buttons"
last_updated: 2 September, 2017
summary: "WIP"
sidebar: default
permalink: buttons
---

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
button[type="button"][aria-controls][aria-expanded]
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
<button type="button" aria-controls="idOfElementThatWillBeOpened" aria-expanded="false">
</button>
```

{% include custom/screen_reader_results.liquid stats=site.data.results.buttons.stats %}

### Menu Button

## Specifications
* [HTML 5.1 - button element](https://www.w3.org/TR/html/sec-forms.html#the-button-element)
* [HTML 5.1 - input[type=submit] element](https://www.w3.org/TR/html/sec-forms.html#submit-button-state-typesubmit)
* [HTML 5.1 - input[type=reset] element](https://www.w3.org/TR/html/sec-forms.html#reset-button-state-typereset)
* [HTML 5.1 - input[type=button] element](https://www.w3.org/TR/html/sec-forms.html#button-state-typebutton)
* [HTML Accessibility mapping - input[type=submit], input[type=reset], input[type=button]](https://w3c.github.io/html-aam/#input-type=%22button%22,-input-type=%22submit%22-and-input-type=%22reset%22)
* [HTML Accessibility mapping - button](https://w3c.github.io/html-aam/#button-element)
* [WAI-ARIA - button](https://www.w3.org/TR/wai-aria-practices/#button)
* [WAI-ARIA - Menu Button](https://www.w3.org/TR/wai-aria-practices/#button)
