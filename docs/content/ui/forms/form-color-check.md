---
title: Color check
summary: The color check is a great way to make your form more user-friendly and engaging. You can use the color check to create a visually appealing form that will help users make decisions quickly and easily.
description: Enhance forms with color checks.
---

Your input controls can come in a variety of colors, depending on your preferences. Click [here](/img/ui/base/colors) to see the list of available colors.

```html
<label class="form-colorinput">
  <input name="..." type="radio" value="..." class="form-colorinput-input" />
  <span class="form-colorinput-color bg-lime"></span>
</label>
```

There is also an example of a color input:

{% capture html -%}
<div class="mb-3">
  <label class="form-label">Color Input</label>
  <div class="row g-2">
    <div class="col-auto">
      <label class="form-colorinput">
        <input name="color" type="radio" value="dark" class="form-colorinput-input" />
        <span class="form-colorinput-color bg-dark"></span>
      </label>
    </div>
    <div class="col-auto">
      <label class="form-colorinput form-colorinput-light">
        <input name="color" type="radio" value="white" class="form-colorinput-input" checked />
        <span class="form-colorinput-color bg-white"></span>
      </label>
    </div>
    <div class="col-auto">
      <label class="form-colorinput">
        <input name="color" type="radio" value="blue" class="form-colorinput-input" />
        <span class="form-colorinput-color bg-blue"></span>
      </label>
    </div>
    <div class="col-auto">
      <label class="form-colorinput">
        <input name="color" type="radio" value="azure" class="form-colorinput-input" />
        <span class="form-colorinput-color bg-azure"></span>
      </label>
    </div>
    <div class="col-auto">
      <label class="form-colorinput">
        <input name="color" type="radio" value="indigo" class="form-colorinput-input" />
        <span class="form-colorinput-color bg-indigo"></span>
      </label>
    </div>
    <div class="col-auto">
      <label class="form-colorinput">
        <input name="color" type="radio" value="purple" class="form-colorinput-input" />
        <span class="form-colorinput-color bg-purple"></span>
      </label>
    </div>
    <div class="col-auto">
      <label class="form-colorinput">
        <input name="color" type="radio" value="pink" class="form-colorinput-input" />
        <span class="form-colorinput-color bg-pink"></span>
      </label>
    </div>
    <div class="col-auto">
      <label class="form-colorinput">
        <input name="color" type="radio" value="red" class="form-colorinput-input" />
        <span class="form-colorinput-color bg-red"></span>
      </label>
    </div>
    <div class="col-auto">
      <label class="form-colorinput">
        <input name="color" type="radio" value="orange" class="form-colorinput-input" />
        <span class="form-colorinput-color bg-orange"></span>
      </label>
    </div>
    <div class="col-auto">
      <label class="form-colorinput">
        <input name="color" type="radio" value="yellow" class="form-colorinput-input" />
        <span class="form-colorinput-color bg-yellow"></span>
      </label>
    </div>
    <div class="col-auto">
      <label class="form-colorinput">
        <input name="color" type="radio" value="lime" class="form-colorinput-input" />
        <span class="form-colorinput-color bg-lime"></span>
      </label>
    </div>
    <div class="col-auto">
      <label class="form-colorinput">
        <input name="color" type="radio" value="green" class="form-colorinput-input" />
        <span class="form-colorinput-color bg-green"></span>
      </label>
    </div>
  </div>
</div>
{%- endcapture %}
{% include "docs/example.html" html=html %}

If you need to select only one color, you can use the radio input type:


{% capture html -%}
<div class="mb-3">
  <label class="form-label">Color Input</label>
  <div class="row g-2">
    <div class="col-auto">
      <label class="form-colorinput">
        <input name="color-rounded" type="radio" value="dark" class="form-colorinput-input" />
        <span class="form-colorinput-color bg-dark rounded-circle"></span>
      </label>
    </div>
    <div class="col-auto">
      <label class="form-colorinput form-colorinput-light">
        <input
          name="color-rounded"
          type="radio"
          value="white"
          class="form-colorinput-input"
          checked
        />
        <span class="form-colorinput-color bg-white rounded-circle"></span>
      </label>
    </div>
    <div class="col-auto">
      <label class="form-colorinput">
        <input name="color-rounded" type="radio" value="blue" class="form-colorinput-input" />
        <span class="form-colorinput-color bg-blue rounded-circle"></span>
      </label>
    </div>
    <div class="col-auto">
      <label class="form-colorinput">
        <input name="color-rounded" type="radio" value="azure" class="form-colorinput-input" />
        <span class="form-colorinput-color bg-azure rounded-circle"></span>
      </label>
    </div>
    <div class="col-auto">
      <label class="form-colorinput">
        <input name="color-rounded" type="radio" value="indigo" class="form-colorinput-input" />
        <span class="form-colorinput-color bg-indigo rounded-circle"></span>
      </label>
    </div>
    <div class="col-auto">
      <label class="form-colorinput">
        <input name="color-rounded" type="radio" value="purple" class="form-colorinput-input" />
        <span class="form-colorinput-color bg-purple rounded-circle"></span>
      </label>
    </div>
    <div class="col-auto">
      <label class="form-colorinput">
        <input name="color-rounded" type="radio" value="pink" class="form-colorinput-input" />
        <span class="form-colorinput-color bg-pink rounded-circle"></span>
      </label>
    </div>
    <div class="col-auto">
      <label class="form-colorinput">
        <input name="color-rounded" type="radio" value="red" class="form-colorinput-input" />
        <span class="form-colorinput-color bg-red rounded-circle"></span>
      </label>
    </div>
    <div class="col-auto">
      <label class="form-colorinput">
        <input name="color-rounded" type="radio" value="orange" class="form-colorinput-input" />
        <span class="form-colorinput-color bg-orange rounded-circle"></span>
      </label>
    </div>
    <div class="col-auto">
      <label class="form-colorinput">
        <input name="color-rounded" type="radio" value="yellow" class="form-colorinput-input" />
        <span class="form-colorinput-color bg-yellow rounded-circle"></span>
      </label>
    </div>
    <div class="col-auto">
      <label class="form-colorinput">
        <input name="color-rounded" type="radio" value="lime" class="form-colorinput-input" />
        <span class="form-colorinput-color bg-lime rounded-circle"></span>
      </label>
    </div>
    <div class="col-auto">
      <label class="form-colorinput">
        <input name="color-rounded" type="radio" value="green" class="form-colorinput-input" />
        <span class="form-colorinput-color bg-green rounded-circle"></span>
      </label>
    </div>
  </div>
</div>
{%- endcapture %}
{% include "docs/example.html" html=html %}

```html
<label class="form-colorinput">
  <input name="..." type="radio" value="..." class="form-colorinput-input" />
  <span class="form-colorinput-color bg-dark rounded-circle"></span>
</label>
```

## Input color picker

Add an color picker to your form to let users customize it according to their preferences.

```html
<input
  type="color"
  class="form-control form-control-color"
  value="#066fd1"
  title="Choose your color"
/>
```

There is also an example of a color picker input:

{% capture html -%}
<div class="mb-3">
  <label class="form-label">Color picker</label>
  <input
    type="color"
    class="form-control form-control-color"
    value="#066fd1"
    title="Choose your color"
  />
</div>
{%- endcapture %}
{% include "docs/example.html" html=html %}

