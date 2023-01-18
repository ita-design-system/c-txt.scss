---
title: Text-Decoration
description: Modifieurs c-txt pour les décorations de texte
layout: libdoc/page-split
order: 300
---
```html

<div class="c-txt m-td-under">Texte test pour le modifieur text-decoration en dessous</div>
<div class="c-txt m-td-line">Texte test pour le modifieur text-decoration barré</div>
<div class="c-txt m-td-none">Texte test pour le modifieur text-decoration inexistant</div>

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
{:.playground title="Modifieurs pour les décorations de texte"}
