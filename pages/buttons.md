---
title: Buttons
tags: [formatting]
keywords: notes, tips, cautions, warnings, admonitions
last_updated: July 3, 2016
summary: "You can insert notes, tips, warnings, and important alerts in your content. These notes are stored as shortcodes made available through the linksrefs.hmtl include."
sidebar: mydoc_sidebar
permalink: buttons
---

## Button

## Toggle Button

```html
<button type="button" aria-pressed="false">Test</button>
```
```html
<div role="button" aria-pressed="false" tabindex="0">Test</div>
```

|| Safari 10 + VoiceOver | Firefox 55 + VoiceOver | Chrome 62 + VoiceOver | Chrome 62 + ChromeVox 53 |
|:---|:---|:---|:---|:---|
| Spoken output   | Test, toggle button | Test, button | Test, toggle button | Test, button not pressed
| Title / Name    | Test | Test | Test | Test |
| Label           |||||
| Type / Role     | toggle button | button | toggle button | button |
| Value / Pressed | 0 | | 0 | false |
| API             | Role: AXCheckbox <br/> Subrole: AXToggle | Role: AXButton | Role: AXCheckbox <br/> Subrole: AXToggleButton ||

```html
<button type="button" aria-pressed="true">Test</button>
```
```html
<div role="button" aria-pressed="true" tabindex="0">Test</div>
```

|| Safari 10 + VoiceOver | Firefox 55 + VoiceOver | Chrome 62 + VoiceOver | Chrome 62 + ChromeVox 53 |
|:---|:---|:---|:---|:---|
| Spoken output   | Test, selected, toggle button | Test, button | Test, selected, toggle button | Test, button pressed |
| Title / Name    | Test | Test | Test | Test |
| Label           |||||
| Type / Role     | toggle button | button | toggle button | button |
| Value / Pressed | 1 | | 1 | true |
| API             | Role: AXCheckbox <br/> Subrole: AXToggle | Role: AXButton | Role: AXCheckbox <br/> Subrole: AXToggleButton ||

### Menu Button
