---
title: SVG version
description: Download Tabler Icons in SVG format.
---

![](/img/icons/package-svg.png)

## Installation

{% include "docs/tabs-package.html" name="@tabler/icons" %}

or just [download from Github](https://github.com/tabler/tabler-icons/releases).

## Usage

All icons are built with SVG, so you can place them as `<img>`, `background-image` and inline in HTML code.

### HTML image

If you load an icon as an image, you can modify its size using CSS.

```html
<img src="path/to/icon.svg" alt="icon title" />
```

### Inline HTML

You can paste the content of the icon file into your HTML code to display it on the page.

```html
<a href="">
  {% include "ui/icon.html" icon="disabled" %}
  Click me
</a>
```

Thanks to that, you can change the size, color and the `stroke-width` of the icons with CSS code.

```css
.icon-tabler {
color: red;
width: 32px;
height: 32px;
stroke-width: 1.25;
}
```

### SVG sprite

Add an icon to be displayed on your page with the following markup (`activity` in the above example can be replaced with any valid icon name):

```html
<svg width="24" height="24">
  <use xlink:href="path/to/tabler-sprite.svg#tabler-activity" />
</svg>
```

## CDN

#### Outline version

```html
<img src="https://unpkg.com/@tabler/icons@$ICONS_VERSION/icons/outline/home.svg" />
```

#### Filled version

```html
<img src="https://unpkg.com/@tabler/icons@$ICONS_VERSION/icons/filled/home.svg" />
```

Instead of a specific version, you can use `latest` to always get the newest icons.
