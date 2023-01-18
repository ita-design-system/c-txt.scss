---
title: Overflow
description: Modifieurs c-txt pour l'overflow : dépassement du contenu d'un élément dans son bloc
layout: libdoc/page-split
order: 300
---
```html
<h2>Overflow</h2>
<div class="c-txt m-o-visible">Texte test pour le modifieur overflow visible</div>
<div class="c-txt m-o-hidden">Texte test pour le modifieur overflow caché</div>
<div class="c-txt m-o-scroll">Texte test pour le modifieur overflow au scroll</div>
<div class="c-txt m-o-auto">Texte test pour le modifieur overflow automatique</div>

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
        width: 150px;
    }
    .c-txt + .c-txt {
        margin-top: var(--ita-spacing-4);
    }
    .c-flex + h2 {
        margin-top: var(--ita-spacing-12);
    }
</style>
```
{:.playground title="Modifieurs pour l'overflow"}
