---
title: Line-height
description: Modifieurs c-txt pour la gestion des hauteurs de lignes.
layout: libdoc/page-split
order: 300
---
```html

<div class="c-txt m-lh-0">Texte test pour le modifieur line-height 0</div>
<div class="c-txt m-lh-1">Texte test pour le modifieur line-height 1 : 1 em</div>
<div class="c-txt m-lh-2">Texte test pour le modifieur line-height 2 : 1.2 em</div>
<div class="c-txt m-lh-3">Texte test pour le modifieur line-height 3 : 1.3 em</div>
<div class="c-txt m-lh-4">Texte test pour le modifieur line-height 4 : 1.4 em</div>
<div class="c-txt m-lh-5">Texte test pour le modifieur line-height 5 : 1.5 em</div>
<div class="c-txt m-lh-6">Texte test pour le modifieur line-height 6 : 1.6 em</div>

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
{:.playground title="Modifieurs pour la hauteur des lignes"}
