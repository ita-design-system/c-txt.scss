---
title: White-space
description: Modifieurs c-txt pour la gestion des blancs au sein de l'élément.
layout: libdoc/page-split
order: 300
---
```html

<div class="c-txt m-ws-normal">Texte test pour le modifieur white-space normal</div>
<div class="c-txt m-ws-nowrap">Texte test pour le modifieur white-space avec passage à la ligne automatique supprimés</div>
<div class="c-txt m-ws-pre">Texte test pour le modifieur white-space avec séries de blancs conservées telles quelles. Les sauts de ligne ont uniquement lieu avec les caractères de saut de ligne et avec les éléments '< br >'</div>
<div class="c-txt m-ws-pre-wrap">Texte test pour le modifieur white-space avec séries de blancs conservées telles quelles. Les sauts de ligne ont lieu avec les caractères de saut de ligne, avec '< br >' et on a des passages à la ligne automatiques.</div>
<div class="c-txt m-ws-pre-line">Texte test pour le modifieur white-space avec séries de blancs regroupées, les sauts de lignes ont lieu avec les caractères de saut de ligne, les éléments '< br >' et on a des passages à la ligne automatiques.</div>
<div class="c-txt m-ws-break-spaces">Texte test pour le modifieur white-space break-spaces : comportement identique à pre-wrap mais chaque séquence de blancs continue d'occuper un espace, y compris en fin de ligne. Il y aura une opportunité de saut de ligne après chaque blanc.</div>

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
{:.playground title="Modifieurs pour la gestion des blancs"}
