---
title: Ellipses
description: Modifieurs c-txt dédiés aux ellipses avec c-dim et c-dis
layout: libdoc/page-split
order: 160
---
```html
<!-- Pour les besoins de la démo, ajout du CSS du composant générique c-dis et c-dim -->
<link rel="stylesheet" href="https://ita-design-system.github.io/c-dis.scss/content/css/c-dis.generic.css">
<link rel="stylesheet" href="https://ita-design-system.github.io/c-dim.scss/content/css/c-dim.generic.css">

<p>Important! Les ellipses requièrent c-dis et c-dim pour fonctionner correctement.</p>
<p class="
    c-dis
    c-dim m-o-hidden
    c-txt m-ellipsis">c-dim m-o-hidden avec c-txt m-ellipsis<br>Ellipse 1 ligne. Sed sanctus tempor diam eos elitr, clita takimata vero sit sea magna dolores lorem gubergren diam. Et consetetur labore amet sadipscing justo magna, no diam dolor dolor eirmod diam clita.</p>
<p class="
    c-dis m-webkit-box
    c-dim m-o-hidden
    c-txt m-ellipsis-2">m-ellipsis-2<br>Ellipse 2 lignes. Sed sanctus tempor diam eos elitr, clita takimata vero sit sea magna dolores lorem gubergren diam. Et consetetur labore amet sadipscing justo magna, no diam dolor dolor eirmod diam clita.</p>
<p class="
    c-dis m-webkit-box
    c-dim m-o-hidden
    c-txt m-ellipsis-3">m-ellipsis-3<br>Ellipse 3 lignes. Sed sanctus tempor diam eos elitr, clita takimata vero sit sea magna dolores lorem gubergren diam. Et consetetur labore amet sadipscing justo magna, no diam dolor dolor eirmod diam clita.</p>
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
    }
</style>
```
{:.playground title="Modifieurs ellipses"}


