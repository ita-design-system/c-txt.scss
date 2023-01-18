---
title: Display
description: Modifieurs c-txt pour le type d'affichage utilisé pour le rendu d'un élément
layout: libdoc/page-split
order: 300
---
```html

<div class="c-txt m-d-block">Texte test pour le modifieur vertical-align baseline</div>
<div class="c-txt m-d-table">Texte test pour le modifieur vertical-align sub : aligne la ligne de base sur la ligne de base inférieure</div>
<div class="c-txt m-d-table-row">Texte test pour le modifieur vertical-align super : aligne la ligne de base sur la ligne de base supérieure</div>
<div class="c-txt m-d-list-item">Texte test pour le modifieur vertical-align text-top : aligne le haut de l'élément avec le haut de la police de l'élément parent</div>
<div class="c-txt m-d-inline">Texte test pour le modifieur vertical-align text-bottom : aligne le bas de l'élément avec le bas de la police de l'élément parent.</div>
<div class="c-txt m-d-inline-block">Texte test pour le modifieur vertical-align middle : aligne le milieu de l'élément avec la hauteur donnée par la ligne de base de l'élément parent à laquelle on ajoute la moitié de sa hauteur en x.</div>
<div class="c-txt m-d-flex">Texte test pour le modifieur vertical-align top : aligne le haut de l'élément et de ses descendants avec le haut de la ligne entière.</div>
<div class="c-txt m-d-inline-flex">Texte test pour le modifieur vertical-align bottom : aligne le bas de l'élément et de ses descendants avec le bas de la ligne entière.</div>
<div class="c-txt m-d-table-row">Texte test pour le modifieur vertical-align super : aligne la ligne de base sur la ligne de base supérieure</div>
<div class="c-txt m-d-grid">Texte test pour le modifieur vertical-align text-top : aligne le haut de l'élément avec le haut de la police de l'élément parent</div>
<div class="c-txt m-d-inline-grid">Texte test pour le modifieur vertical-align text-bottom : aligne le bas de l'élément avec le bas de la police de l'élément parent.</div>
<div class="c-txt m-d-flow-root">Texte test pour le modifieur vertical-align middle : aligne le milieu de l'élément avec la hauteur donnée par la ligne de base de l'élément parent à laquelle on ajoute la moitié de sa hauteur en x.</div>
<div class="c-txt m-d-none">Texte test pour le modifieur vertical-align top : aligne le haut de l'élément et de ses descendants avec le haut de la ligne entière.</div>
<div class="c-txt m-d-contents">Texte test pour le modifieur vertical-align bottom : aligne le bas de l'élément et de ses descendants avec le bas de la ligne entière.</div>
<div class="c-txt m-d-table">Texte test pour le modifieur vertical-align middle : aligne le milieu de l'élément avec la hauteur donnée par la ligne de base de l'élément parent à laquelle on ajoute la moitié de sa hauteur en x.</div>
<div class="c-txt m-d-table-row">Texte test pour le modifieur vertical-align top : aligne le haut de l'élément et de ses descendants avec le haut de la ligne entière.</div>
<div class="c-txt m-d-list-item">Texte test pour le modifieur vertical-align bottom : aligne le bas de l'élément et de ses descendants avec le bas de la ligne entière.</div>

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
