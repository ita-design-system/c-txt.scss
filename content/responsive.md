---
title: Responsive
description: Fonctionnalités responsive du composant c-txt
layout: libdoc/page-split
order: 90
separator: true
---
Si le paramètre `responsive: true` est activé, les modifieurs du composant c-txt sont adaptables à chaque design token de taille d'écran `$briks-screen-sizes` comme suit.

## Classes responsives

Un modifieur peut être appliqué sur des design tokens de tailles d'écrans via des classes CSS

```html
<!-- Avec des classes CSS -->
<HTMLTag class="c-txt m-NOM_DU_MODIFIEUR--TOKEN_TAILLE_ECRAN"></HTMLTag>
```

## Attributs responsives

En parallèle des classes CSS, la syntaxe par attribut permet d'appliquer la même fonctionnalité d'un modifieur sur plusieurs tailles d'écran en une seule fois.

```html
L'attribut responsive du modifieur
<HTMLTag class="c-txt" m-NOM_DU_MODIFIEUR="TOKEN_TAILLE_ECRAN_1, TOKEN_TAILLE_ECRAN_2, TOKEN_TAILLE_ECRAN_3"></HTMLTag>

a le même effet que les classes CSS
<HTMLTag class="c-txt m-NOM_DU_MODIFIEUR--TOKEN_TAILLE_ECRAN_1 m-NOM_DU_MODIFIEUR--TOKEN_TAILLE_ECRAN_2 m-NOM_DU_MODIFIEUR--TOKEN_TAILLE_ECRAN_3"></HTMLTag>
```

```html
<!-- Avec des classes responsives -->
<p class="c-txt m-ta-right--xs">
    Je m'aligne à droite<br> sur la taille d'écran xs<br> via des classes CSS.</div>
</p>
<!-- Avec l'attribut responsive - multiples tailles d'écrans -->
<p class="c-txt" m-ta-right="xs,sm">
    Je m'aligne à droite<br> sur les tailles d'écran xs et sm<br> via l'attribut responsive.</div>
</p>
<!-- DEMO UNIQUEMENT -->
<style>
    body {
        padding: var(--ita-spacing-4);
        background-color: var(--ita-color-primary-100);
        color: var(--ita-color-primary-800);
        font-family: var(--ita-font-family-mono);
        font-size: 1rem;
        line-height: 1.5rem;
        padding-bottom: 50vh;
    }
    .c-txt {
        background-color: var(--ita-color-primary-500);
        color: var(--ita-color-neutral-100);
        padding: var(--ita-spacing-4);
    }
    .c-txt + .c-txt {
        margin-top: var(--ita-spacing-4);
    }
</style>
```
{:.playground title="Exemples responsives"}