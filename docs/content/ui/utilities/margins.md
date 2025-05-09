---
title: Margins
summary: Use margin utilities to control the space between elements.
description: Control the space between elements with margin utilities.
---

Margin utilities allow you to control the space between elements, providing flexibility to suit different design needs. These utilities are especially useful for creating spacing between components or aligning them consistently. Below are examples of how to use margin utilities for various directions and sizes.


### Margin size

In the table below you can see the available margin sizes.

Name|Value
-|-
0|0
1|0.25rem
2|0.5rem
3|1rem
4|1.5rem
5|2rem
6|3rem
7|5rem
8|8rem


### Margin

Use the `.m-*` utilities to control the margin of an element. Margin utilities are used to create consistent spacing around an element, ensuring that the layout is visually balanced.

{% capture html -%}
<div class="d-flex">
  <div class="bg-purple-lt">
    <div class="px-3 py-2 m-0 bg-purple rounded text-white font-monospace">.m-0</div>
  </div>
</div>
<div class="d-flex">
  <div class="bg-purple-lt">
    <div class="px-3 py-2 m-4 bg-purple rounded text-white font-monospace">.m-4</div>
  </div>
</div>
<div class="d-flex">
  <div class="bg-purple-lt">
    <div class="px-3 py-2 m-8 bg-purple rounded text-white font-monospace">.m-8</div>
  </div>
</div>
{%- endcapture %}
{% include "docs/example.html" html=html %}

### Start margin

Start margins control the spacing to the left of an element, helping to create consistent horizontal gaps between elements. Start margin class names are prefixed with `ms-`.

```html
<div class="ms-4">...</div>
```

{% capture html -%}
<div class="d-flex">
  <div class="bg-red-lt">
    <div class="px-3 py-2 ms-0 bg-red rounded text-white font-monospace">.ms-0</div>
  </div>
</div>
<div class="d-flex">
  <div class="bg-red-lt">
    <div class="px-3 py-2 ms-4 bg-red rounded text-white font-monospace">.ms-4</div>
  </div>
</div>
<div class="d-flex">
  <div class="bg-red-lt">
    <div class="px-3 py-2 ms-8 bg-red rounded text-white font-monospace">.ms-8</div>
  </div>
</div>
{%- endcapture %}
{% include "docs/example.html" html=html %}

### End margin

End margins control the spacing on the right side of an element. These utilities are helpful for creating visual separation between elements that flow horizontally. End margin class names are prefixed with `me-`.

```html
<div class="me-4">...</div>
```

{% capture html -%}
<div class="d-flex">
  <div class="bg-orange-lt">
    <div class="px-3 py-2 ms-0 bg-orange rounded text-white font-monospace">.me-0</div>
  </div>
</div>
<div class="d-flex">
  <div class="bg-orange-lt">
    <div class="px-3 py-2 me-4 bg-orange rounded text-white font-monospace">.me-4</div>
  </div>
</div>
<div class="d-flex">
  <div class="bg-orange-lt">
    <div class="px-3 py-2 me-8 bg-orange rounded text-white font-monospace">.me-8</div>
  </div>
</div>
{%- endcapture %}
{% include "docs/example.html" html=html %}

### Top margin

Top margins define the spacing above an element. This is useful for separating stacked components or creating vertical spacing between sections. Top margin class names are prefixed with `mt-`.

```html
<div class="mt-4">...</div>
```

{% capture html -%}
<div class="d-flex">
  <div class="bg-yellow-lt">
    <div class="px-3 py-2 mt-0 bg-yellow rounded text-white font-monospace">.mt-0</div>
  </div>
</div>
<div class="d-flex">
  <div class="bg-yellow-lt">
    <div class="px-3 py-2 mt-4 bg-yellow rounded text-white font-monospace">.mt-4</div>
  </div>
</div>
<div class="d-flex">
  <div class="bg-yellow-lt">
    <div class="px-3 py-2 mt-8 bg-yellow rounded text-white font-monospace">.mt-8</div>
  </div>
</div>
{%- endcapture %}
{% include "docs/example.html" html=html %}

### Bottom margin

Bottom margins control the spacing below an element, helping to create consistent vertical gaps between stacked elements. Bottom margin class names are prefixed with `mb-`.

```html
<div class="mb-4">...</div>
```

{% capture html -%}
<div class="d-flex">
  <div class="bg-lime-lt">
    <div class="px-3 py-2 mb-0 bg-lime rounded text-white font-monospace">.mb-0</div>
  </div>
</div>
<div class="d-flex">
  <div class="bg-lime-lt">
    <div class="px-3 py-2 mb-4 bg-lime rounded text-white font-monospace">.mb-4</div>
  </div>
</div>
<div class="d-flex">
  <div class="bg-lime-lt">
    <div class="px-3 py-2 mb-8 bg-lime rounded text-white font-monospace">.mb-8</div>
  </div>
</div>
{%- endcapture %}
{% include "docs/example.html" html=html %}

### Horizontal margin

Use the `mx-*` utilities to control the horizontal margin of an element. Horizontal margin utilities are used to create consistent spacing between elements that flow horizontally.

```html
<div class="mx-4">...</div>
```

{% capture html -%}
<div class="d-flex">
  <div class="bg-azure-lt">
    <div class="px-3 py-2 mx-0 bg-azure rounded text-white font-monospace">.mx-0</div>
  </div>
</div>
<div class="d-flex">
  <div class="bg-azure-lt">
    <div class="px-3 py-2 mx-4 bg-azure rounded text-white font-monospace">.mx-4</div>
  </div>
</div>
<div class="d-flex">
  <div class="bg-azure-lt">
    <div class="px-3 py-2 mx-8 bg-azure rounded text-white font-monospace">.mx-8</div>
  </div>
</div>
{%- endcapture %}
{% include "docs/example.html" html=html %}


### Vertical margin

Use the `my-*` utilities to control the vertical margin of an element. Vertical margin utilities are used to create consistent spacing between elements that flow vertically.

```html
<div class="my-4">...</div>
```

{% capture html -%}
<div class="d-flex">
  <div class="bg-blue-lt">
    <div class="px-3 py-2 my-0 bg-blue rounded text-white font-monospace">.my-0</div>
  </div>
</div>
<div class="d-flex">
  <div class="bg-blue-lt">
    <div class="px-3 py-2 my-4 bg-blue rounded text-white font-monospace">.my-4</div>
  </div>
</div>
<div class="d-flex">
  <div class="bg-blue-lt">
    <div class="px-3 py-2 my-8 bg-blue rounded text-white font-monospace">.my-8</div>
  </div>
</div>
{%- endcapture %}
{% include "docs/example.html" html=html %}

## Horizontal centering

Additionally, Tabler also includes an `.mx-auto` class for horizontally centering fixed-width block level content — that is, content that has `display: block` and a width set — by setting the horizontal margins to `auto`.

```html
<div class="mx-auto">...</div>
```

{% capture html -%}
<div class="bg-teal-lt w-100 d-flex">
  <div class="px-3 py-2 mx-auto bg-teal rounded text-white font-monospace">.mx-auto</div>
</div>
{%- endcapture %}
{% include "docs/example.html" html=html %}

## Gap

Use the `.gap-*` utilities to control the space between elements in a grid layout. The gap utilities are used to create consistent spacing between grid items, ensuring that the layout is visually balanced.

```html
<div class="d-grid gap-6">...</div>
```

```html example 
<div class="d-grid gap-6 bg-indigo-lt">
  <div class="px-3 py-2 bg-indigo text-white rounded">Grid item 1</div>
  <div class="px-3 py-2 bg-indigo text-white rounded">Grid item 2</div>
  <div class="px-3 py-2 bg-indigo text-white rounded">Grid item 3</div>
</div>
```
