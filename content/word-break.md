---
title: Word-break
description: Modifieurs c-txt pour word-break : définit la façon dont la césure s'applique pour les endroits où le texte dépasserait de sa boîte de contenu
layout: libdoc/page-split
order: 300
---
```html
<h2>Overflow</h2>
<div class="c-txt m-wb-normal">Texte test pour le modifieur word-break normal</div>
<div class="c-txt m-wb-break-all">Texte test pour le modifieur word-break break-all</div>
<div class="c-txt m-wb-keep-all">Texte test pour le modifieur word-break keep-all</div>

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
{:.playground title="Modifieurs pour word-break"}
