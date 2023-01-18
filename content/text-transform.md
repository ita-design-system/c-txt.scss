---
title: Text-transform
description: Modifieurs c-txt pour le text-transform : gestion des minuscules ou majuscules
layout: libdoc/page-split
order: 300
---
```html
<h2>Overflow</h2>
<div class="c-txt m-tt-none">Texte test pour le modifieur sans transformation de texte</div>
<div class="c-txt m-tt-capitalize">Texte test pour le modifieur avec lettres capitales</div>
<div class="c-txt m-tt-uppercase">Texte test pour le modifieur texte en majuscules</div>
<div class="c-txt m-tt-lowercase">Texte test pour le modifieur texte en minuscules</div>

<!-- DEMO UNIQUEMENT -->
<style>
    body {
        padding: var(--ita-spacing-4);
        background-color: var(--ita-color-primary-900);
        color: var(--ita-color-primary-200);
        font-family: var(--ita-font-family-mono);
        font-size: 1rem;
        line-height: 1.5rem;
        padding-bottom: 50vh;
    }
    .c-txt {
        background-color: var(--ita-color-primary-800);
    }
    .c-txt > * {
        background-color: var(--ita-color-primary-500);
        color: var(--ita-color-primary-900);
        border: var(--ita-border-6);
        padding: var(--ita-spacing-4);
    }
    .c-txt + .c-txt {
        margin-top: var(--ita-spacing-4);
    }
    .c-flex + h2 {
        margin-top: var(--ita-spacing-12);
    }
</style>
```
{:.playground title="Modifieurs pour text-transform"}
