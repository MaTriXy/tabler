---
title: Alerts
summary: Alert messages are used to inform users of the status of their action and help them solve any problems that might have occurred. Good design of alert modals is very important for the overall user experience of a website or app.
bootstrapLink: components/alerts/
description: Alert messages for user notifications.
---

## Default markup

Depending on the information you need to convey, you can use one of the following types of alert messages - **success**, **info**, **warning** or **danger**. Using the right type of alert modal will help draw users' attention to the message and prompt them to take action.

Combine `alert` class with one of the following: `alert-success`, `alert-info`, `alert-warning`, `alert-danger` to get the alert that you need.

Alert classes affect the color of all the text inside an alert. Use another class, e.g. `text-secondary` to change the color of the alert's content.

{% capture html -%}
{% include "ui/alert.html" type="success" title="Wow! Everything worked!" description="Your account has been saved!" %}
{% include "ui/alert.html" type="info" title="Did you know?" description="Here is something that you might like to know." %}
{% include "ui/alert.html" type="warning" title="Uh oh, something went wrong" description="Sorry! There was a problem with your request." %}
{% include "ui/alert.html" type="danger" title="I'm so sorry&hellip;" description="Your account has been deleted and can't be restored." %}
{%- endcapture %}
{% include "docs/example.html" html=html %}

## Alert links

Add a link to your alert message to redirect users to the details they need to complete or additional information they should read. Use `alert-link` class to style the link and match the text color.

{% capture html -%}
{% include "ui/alert.html" type="danger" title="This is a danger alert" link="check it out" %}
{%- endcapture %}
{% include "docs/example.html" html=html %}

## Dismissible alerts

Add the `x` close button to make an alert modal dismissible. Thanks to that, your alert modal will disappear only when the user closes it.

```html
<a class="btn-close" data-bs-dismiss="alert" aria-label="close"></a>
```

{% capture html -%}
{% include "ui/alert.html" type="danger" title="This is a danger alert" show-close %}
{%- endcapture %}
{% include "docs/example.html" html=html %}

## Alerts with icons

Add an icon to your alert modal to make it more user-friendly and help users easily identify the message.

Use the `alert-icon` class on an `<svg>` (or on an `<i>` when using the webfont) to provide the proper styling.

{% capture html -%}
<div class="alert alert-success" role="alert">
  <div class="d-flex">
    <div>
      <svg
        xmlns="http://www.w3.org/2000/svg"
        class="icon alert-icon"
        width="24"
        height="24"
        viewBox="0 0 24 24"
        stroke-width="2"
        stroke="currentColor"
        fill="none"
        stroke-linecap="round"
        stroke-linejoin="round"
      >
        <path stroke="none" d="M0 0h24v24H0z" fill="none" />
        <path d="M5 12l5 5l10 -10" />
      </svg>
    </div>
    <div>
      <h4 class="alert-title">Wow! Everything worked!</h4>
      <div class="text-secondary">Your account has been saved!</div>
    </div>
  </div>
</div>
<div class="alert alert-info" role="alert">
  <div class="d-flex">
    <div>
      <svg
        xmlns="http://www.w3.org/2000/svg"
        class="icon alert-icon"
        width="24"
        height="24"
        viewBox="0 0 24 24"
        stroke-width="2"
        stroke="currentColor"
        fill="none"
        stroke-linecap="round"
        stroke-linejoin="round"
      >
        <path stroke="none" d="M0 0h24v24H0z" fill="none" />
        <circle cx="12" cy="12" r="9" />
        <line x1="12" y1="8" x2="12.01" y2="8" />
        <polyline points="11 12 12 12 12 16 13 16" />
      </svg>
    </div>
    <div>
      <h4 class="alert-title">Did you know?</h4>
      <div class="text-secondary">Here is something that you might like to know.</div>
    </div>
  </div>
</div>
<div class="alert alert-warning" role="alert">
  <div class="d-flex">
    <div>
      <svg
        xmlns="http://www.w3.org/2000/svg"
        class="icon alert-icon"
        width="24"
        height="24"
        viewBox="0 0 24 24"
        stroke-width="2"
        stroke="currentColor"
        fill="none"
        stroke-linecap="round"
        stroke-linejoin="round"
      >
        <path stroke="none" d="M0 0h24v24H0z" fill="none" />
        <path d="M12 9v2m0 4v.01" />
        <path
          d="M5 19h14a2 2 0 0 0 1.84 -2.75l-7.1 -12.25a2 2 0 0 0 -3.5 0l-7.1 12.25a2 2 0 0 0 1.75 2.75"
        />
      </svg>
    </div>
    <div>
      <h4 class="alert-title">Uh oh, something went wrong</h4>
      <div class="text-secondary">Sorry! There was a problem with your request.</div>
    </div>
  </div>
</div>
<div class="alert alert-danger" role="alert">
  <div class="d-flex">
    <div>
      <svg
        xmlns="http://www.w3.org/2000/svg"
        class="icon alert-icon"
        width="24"
        height="24"
        viewBox="0 0 24 24"
        stroke-width="2"
        stroke="currentColor"
        fill="none"
        stroke-linecap="round"
        stroke-linejoin="round"
      >
        <path stroke="none" d="M0 0h24v24H0z" fill="none" />
        <circle cx="12" cy="12" r="9" />
        <line x1="12" y1="8" x2="12" y2="12" />
        <line x1="12" y1="16" x2="12.01" y2="16" />
      </svg>
    </div>
    <div>
      <h4 class="alert-title">I'm so sorry&hellip;</h4>
      <div class="text-secondary">Your account has been deleted and can't be restored.</div>
    </div>
  </div>
</div>
{%- endcapture %}
{% include "docs/example.html" html=html %}

## Alert with avatar

Add an avatar to your alert modal to make it more personalized.

{% capture html -%}
<div class="alert alert-success" role="alert">
  <div class="d-flex">
    <div>
      <span
        class="avatar me-3"
        style="background-image: url(/static/avatars/039m.jpg)"
      ></span>
    </div>
    <div>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Lorem ipsum dolor sit amet,
      consectetur adipisicing elit. Lorem ipsum dolor sit amet, consectetur adipisicing elit.
    </div>
  </div>
</div>
<div class="alert alert-info" role="alert">
  <div class="d-flex">
    <div>
      <span class="avatar me-3">JL</span>
    </div>
    <div>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Lorem ipsum dolor sit amet,
      consectetur adipisicing elit. Lorem ipsum dolor sit amet, consectetur adipisicing elit.
    </div>
  </div>
</div>
<div class="alert alert-warning" role="alert">
  <div class="d-flex">
    <div>
      <span
        class="avatar me-3"
        style="background-image: url(/static/avatars/035f.jpg)"
      ></span>
    </div>
    <div>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Lorem ipsum dolor sit amet,
      consectetur adipisicing elit. Lorem ipsum dolor sit amet, consectetur adipisicing elit.
    </div>
  </div>
</div>
<div class="alert alert-danger" role="alert">
  <div class="d-flex">
    <div>
      <span
        class="avatar me-3"
        style="background-image: url(/static/avatars/056f.jpg)"
      ></span>
    </div>
    <div>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Lorem ipsum dolor sit amet,
      consectetur adipisicing elit. Lorem ipsum dolor sit amet, consectetur adipisicing elit.
    </div>
  </div>
</div>
{%- endcapture %}
{% include "docs/example.html" html=html %}

## Alert with buttons

Add primary and secondary buttons to your alert modals if you want users to take a particular action based on the information included in the modal message.

Buttons don't inherit the alert's color, so you should set the proper class if you want it to be matched. For example, `btn-success` for `alert-success`.

{% capture html -%}
<div class="alert alert-success alert-dismissible" role="alert">
  <h3 class="mb-1">Some Title</h3>
  <p class="text-secondary">
    Lorem ipsum Minim ad pariatur eiusmod ea ut nulla aliqua est quis id dolore minim voluptate.
  </p>
  <div class="btn-list">
    <a href="#" class="btn btn-success">Okay</a>
    <a href="#" class="btn">Cancel</a>
  </div>
  <a class="btn-close" data-bs-dismiss="alert" aria-label="close"></a>
</div>
<div class="alert alert-info alert-dismissible" role="alert">
  <h3 class="mb-1">Some Title</h3>
  <p class="text-secondary">
    Lorem ipsum Minim ad pariatur eiusmod ea ut nulla aliqua est quis id dolore minim voluptate.
  </p>
  <div class="btn-list">
    <a href="#" class="btn btn-info">Okay</a>
    <a href="#" class="btn">Cancel</a>
  </div>
  <a class="btn-close" data-bs-dismiss="alert" aria-label="close"></a>
</div>
<div class="alert alert-warning alert-dismissible" role="alert">
  <h3 class="mb-1">Some Title</h3>
  <p class="text-secondary">
    Lorem ipsum Minim ad pariatur eiusmod ea ut nulla aliqua est quis id dolore minim voluptate.
  </p>
  <div class="btn-list">
    <a href="#" class="btn btn-warning">Okay</a>
    <a href="#" class="btn">Cancel</a>
  </div>
  <a class="btn-close" data-bs-dismiss="alert" aria-label="close"></a>
</div>
<div class="alert alert-danger alert-dismissible" role="alert">
  <h3 class="mb-1">Some Title</h3>
  <p class="text-secondary">
    Lorem ipsum Minim ad pariatur eiusmod ea ut nulla aliqua est quis id dolore minim voluptate.
  </p>
  <div class="btn-list">
    <a href="#" class="btn btn-danger">Okay</a>
    <a href="#" class="btn">Cancel</a>
  </div>
  <a class="btn-close" data-bs-dismiss="alert" aria-label="close"></a>
</div>
{%- endcapture %}
{% include "docs/example.html" html=html %}

## Important alerts

If you want your alert to be really eye-catching, you can add an `alert-important` class. It will use the selected color as a background for the alert.

```html
<div class="alert alert-important alert-success alert-dismissible" role="alert">...</div>
```

You can also use other elements, like icons and dismissible buttons, with this type of alert.

{% capture html -%}
<div class="alert alert-important alert-success alert-dismissible" role="alert">
  <div class="d-flex">
    <div>
      <svg
        xmlns="http://www.w3.org/2000/svg"
        class="icon alert-icon"
        width="24"
        height="24"
        viewBox="0 0 24 24"
        stroke-width="2"
        stroke="currentColor"
        fill="none"
        stroke-linecap="round"
        stroke-linejoin="round"
      >
        <path stroke="none" d="M0 0h24v24H0z" fill="none"></path>
        <path d="M5 12l5 5l10 -10"></path>
      </svg>
    </div>
    <div>Wow! Everything worked!</div>
  </div>
  <a class="btn-close btn-close-white" data-bs-dismiss="alert" aria-label="close"></a>
</div>
<div class="alert alert-important alert-danger alert-dismissible" role="alert">
  <div class="d-flex">
    <div>
      <svg
        xmlns="http://www.w3.org/2000/svg"
        class="icon alert-icon"
        width="24"
        height="24"
        viewBox="0 0 24 24"
        stroke-width="2"
        stroke="currentColor"
        fill="none"
        stroke-linecap="round"
        stroke-linejoin="round"
      >
        <path stroke="none" d="M0 0h24v24H0z" fill="none" />
        <circle cx="12" cy="12" r="9" />
        <line x1="12" y1="8" x2="12" y2="12" />
        <line x1="12" y1="16" x2="12.01" y2="16" />
      </svg>
    </div>
    <div>Your account has been deleted and can't be restored.</div>
  </div>
  <a class="btn-close btn-close-white" data-bs-dismiss="alert" aria-label="close"></a>
</div>
{%- endcapture %}
{% include "docs/example.html" html=html %}

## Custom alert color

You're not limited to the 4 default alert colors. You can use any [base or social color](../base/colors) you want.

{% capture html -%}
<div class="alert alert-lime" role="alert">
  <h4 class="alert-title">Wow! Everything worked!</h4>
  <div class="text-secondary">Your account has been saved!</div>
</div>
<div class="alert alert-cyan" role="alert">
  <h4 class="alert-title">Did you know?</h4>
  <div class="text-secondary">Here is something that you might like to know.</div>
</div>
<div class="alert alert-facebook" role="alert">
  <h4 class="alert-title">You have a new friend on Facebook</h4>
  <div class="text-secondary">Say hello to your new friend!</div>
</div>
<div class="alert alert-instagram alert-dismissible alert-important" role="alert">
  <div class="d-flex">
    <div>
      <span
        class="avatar me-3"
        style="background-image: url(/static/avatars/035f.jpg)"
      ></span>
    </div>
    <div>
      <h4 class="alert-title">Sophia just added a new post on Instagram</h4>
      <div>Be the first to see it!</div>
    </div>
  </div>
  <a class="btn-close" data-bs-dismiss="alert" aria-label="close"></a>
</div>
{%- endcapture %}
{% include "docs/example.html" html=html %}

## SASS variables

You can customize the alert colors by changing the SASS variables. The default values are:

{% scss-docs "alert-variables" "ui/_alerts.scss" %}