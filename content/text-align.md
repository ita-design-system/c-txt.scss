---
title: Text-Align
description: Modifieurs c-txt pour l'alignement du texte
layout: libdoc/page-split
order: 300
---
```html

<div class="c-txt m-ta-center">Texte test pour le modifieur alignement au centre</div>
<div class="c-txt m-ta-left">Texte test pour le modifieur alignement à gauche</div>
<div class="c-txt m-ta-right">Texte test pour le modifieur alignement à droite</div>
<div class="c-txt m-ta-justify">Texte test pour le modifieur de justification du texte</div>

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
{:.playground title="Modifieurs pour l'alignement du texte"}
