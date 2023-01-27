---
title: Césures
description: Modifieurs c-txt dédiés aux césures
layout: libdoc/page-split
order: 180
---
```html
<p class="c-txt">Texte standard sans césure.<br>Sedsanctustempordiameoselitrclitatakimataverositseamagnadoloresloremgubergrendiam. Et consetetur labore amet sadipscing justo magna, no diam dolor dolor eirmod diam clita.</p>
<p class="c-txt m-wb-break-all">m-wb-break-all<br>Césure. Sedsanctustempordiameoselitrclitatakimataverositseamagnadoloresloremgubergrendiam. Et consetetur labore amet sadipscing justo magna, no diam dolor dolor eirmod diam clita.</p>
<p class="c-txt m-wb-break-word">m-wb-break-word<br>Césure mot. Sedsanctustempordiameoselitrclitatakimataverositseamagnadoloresloremgubergrendiam. Et consetetur labore amet sadipscing justo magna, no diam dolor dolor eirmod diam clita.</p>

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
        padding: var(--ita-spacing-4);
        max-width: 30ch;
        margin-left: auto;
        margin-right: auto;
    }
</style>
```
{:.playground title="Modifieurs césures"}


