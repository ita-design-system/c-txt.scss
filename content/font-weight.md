---
title: Graisses
description: Modifieurs c-txt dédiés à la propriété font-weight
layout: libdoc/page-split
order: 120
weights:
    - Thin (Hairline)
    - Extra Light (Ultra Light)
    - Light
    - Normal
    - Medium
    - Semi Bold (Demi Bold)
    - Bold
    - Extra Bold (Ultra Bold)
    - Black (Heavy)
---
```html
{% for i in (1..9) %}
<p class="c-txt m-fw-{{ i }}00">m-fw-{{ i }}00<br><i>{{ page.weights[forloop.index0] }}</i><br><br>Sed sanctus tempor diam eos elitr, clita takimata vero sit sea magna dolores lorem gubergren diam. Et consetetur labore amet sadipscing justo magna, no diam dolor dolor eirmod diam clita.</p>
{% endfor %}
<!-- DEMO UNIQUEMENT -->
<style>
    body {
        padding: var(--ita-spacing-4);
        background-color: var(--ita-color-primary-100);
        color: var(--ita-color-primary-800);
        font-family: var(--ita-font-family-mono);
        font-size: 1rem;
        line-height: 1.5rem;
        min-height: 100vh;
    }
    .c-txt {
        background-color: var(--ita-color-primary-500);
        color: var(--ita-color-neutral-100);
        padding: var(--ita-spacing-4);
        max-width: 30ch;
        margin-left: auto;
        margin-right: auto;
    }
</style>
```
{:.playground title="Modifieurs line-height"}


