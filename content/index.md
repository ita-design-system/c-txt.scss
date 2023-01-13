---
layout: libdoc/page-codemirror
permalink: index.html
unlisted: true
---
<section class="c-flex"
    m-nowrap="sm,md,lg,xl">
    <menu class="c-flex" 
        m-column="sm,md,lg,xl">
        <li><a href="#">Lien</a></li>
        <li><a href="#">Lien</a></li>
        <li><a href="#">Lien</a></li>
    </menu>
    <header class="c-flex m-column">
        <h1>c-flex</h1>
        <p>Composant CSS de grille flexbox polyvalent, cascadable et personnalisable en fonction du projet.</p>
    </header>
</section>
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
    .c-flex {
        background-color: var(--ita-color-primary-800);
    }
    .c-flex > * {
        background-color: var(--ita-color-primary-500);
        color: var(--ita-color-primary-900);
        border: var(--ita-border-6);
        padding: var(--ita-spacing-4);
    }
    menu, h1, p {
        margin: 0;
        padding: 0;
        list-style: none;
    }
    a {
        color: var(--ita-color-primary-900);
        text-underline-offset: 0.2em;
    }
</style>
