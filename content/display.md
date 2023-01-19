---
title: Display
description: Modifieurs c-txt pour le type d'affichage utilisé pour le rendu d'un élément
layout: libdoc/page-split
order: 300
---
```html

<div class="c-txt m-d-block">Texte test pour le modifieur display block</div>
<div class="c-txt m-d-table">Texte test pour le modifieur display table</div>
<div class="c-txt m-d-table-row">Texte test pour le modifieur display table-row</div>
<div class="c-txt m-d-list-item">Texte test pour le modifieur display list-item</div>
<div class="c-txt m-d-inline">Texte test pour le modifieur display inline</div>
<div class="c-txt m-d-inline-block">Texte test pour le modifieur display inline-block</div>
<div class="c-txt m-d-flex">Texte test pour le modifieur display flex</div>
<div class="c-txt m-d-inline-flex">Texte test pour le modifieur display inline flex</div>
<div class="c-txt m-d-table-row">Texte test pour le modifieur display table-row</div>
<div class="c-txt m-d-grid">Texte test pour le modifieur display grid</div>
<div class="c-txt m-d-inline-grid">Texte test pour le modifieur display inline-grid</div>
<div class="c-txt m-d-flow-root">Texte test pour le modifieur display flow-root</div>
<div class="c-txt m-d-none">Texte test pour le modifieur display none : <span class="c-txt m-d-none"></span></div>
<div class="c-txt m-d-contents">Texte test pour le modifieur display contents</div>
<div class="c-txt m-d-table">Texte test pour le modifieur display table</div>
<div class="c-txt m-d-table-row">Texte test pour le modifieur display table-row</div>
<div class="c-txt m-d-list-item">Texte test pour le modifieur display list-item</div>

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
{:.playground title="Modifieurs pour l'affichage : display"}
