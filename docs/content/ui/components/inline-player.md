---
title: Inline player
docs-libs: plyr
summary: A simple, lightweight, accessible and customizable HTML5, YouTube and Vimeo media player that supports modern browsers.
description: Lightweight media player for websites.
---


## Overview

The Inline Player is a versatile, modern media player designed for seamless integration into websites. It supports HTML5, YouTube, and Vimeo content, offering a lightweight and accessible solution for media playback. Built with customization and ease of use in mind, this player ensures compatibility with modern browsers and enhances user experience.

## Installation

To use the Inline Player, you need to include the Plyr library in your project. You can install it via npm or include it directly from a CDN. The following example demonstrates how to include the Plyr library from a CDN:

```html
<script src="{{ cdnUrl }}/dist/libs/plyr/dist/plyr.min.js"></script>
```

## Sample demo

Integrating the Inline Player into your website is straightforward. Below is a sample implementation for a YouTube video:

```html
<div id="player-youtube" data-plyr-provider="youtube" data-plyr-embed-id="dQw4w9WgXcQ"></div>
<script>
  document.addEventListener("DOMContentLoaded", function () {
    window.Plyr && new Plyr("#player-youtube");
  });
</script>
```

Look at the example below to see how the Inline Player works with a YouTube video.

{% capture html -%}
<div id="player-youtube" data-plyr-provider="youtube" data-plyr-embed-id="dQw4w9WgXcQ"></div>
<script src="{{ cdnUrl }}/dist/libs/plyr/dist/plyr.min.js"></script>
<script>
  document.addEventListener("DOMContentLoaded", function () {
    window.Plyr && new Plyr("#player-youtube");
  });
</script>
{%- endcapture %}
{% include "docs/example.html" html=html %}

## Vimeo file

Here’s how to embed a Vimeo video using the Inline Player:

{% capture html -%}
<div id="player-vimeo" data-plyr-provider="vimeo" data-plyr-embed-id="515937365"></div>
<script src="{{ cdnUrl }}/dist/libs/plyr/dist/plyr.min.js"></script>
<script>
  document.addEventListener("DOMContentLoaded", function () {
    window.Plyr && new Plyr("#player-vimeo");
  });
</script>
{%- endcapture %}
{% include "docs/example.html" html=html %}
