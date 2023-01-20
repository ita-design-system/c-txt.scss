# c-txt.scss

[Démo et documentation](https://ita-design-system.github.io/c-txt.scss/)

Composant CSS dédié aux textes. 

## Scope

Liste des propriétés CSS utilisées par le composant


* [font-family](https://developer.mozilla.org/fr/docs/Web/CSS/font-family)
* [font-size](https://developer.mozilla.org/fr/docs/Web/CSS/font-size)
* [font-style](https://developer.mozilla.org/fr/docs/Web/CSS/font-style)
* [font-weight](https://developer.mozilla.org/fr/docs/Web/CSS/font-weight)
* [letter-spacing](https://developer.mozilla.org/fr/docs/Web/CSS/letter-spacing)
* [line-height](https://developer.mozilla.org/fr/docs/Web/CSS/line-height)
* [overflow](https://developer.mozilla.org/fr/docs/Web/CSS/overflow)
* [text-align](https://developer.mozilla.org/fr/docs/Web/CSS/text-align)
* [text-decoration](https://developer.mozilla.org/fr/docs/Web/CSS/text-decoration)
* [text-overflow](https://developer.mozilla.org/fr/docs/Web/CSS/text-overflow)
* [text-transform](https://developer.mozilla.org/fr/docs/Web/CSS/text-transform)
* [vertical-align](https://developer.mozilla.org/fr/docs/Web/CSS/vertical-align)
* [white-space](https://developer.mozilla.org/fr/docs/Web/CSS/white-space)
* [word-break](https://developer.mozilla.org/fr/docs/Web/CSS/word-break)
* [-webkit-box-orient](https://developer.mozilla.org/fr/docs/Web/CSS/box-orient)
* [-webkit-line-clamp](https://developer.mozilla.org/fr/docs/Web/CSS/-webkit-line-clamp)


## Typologie d'un composant générique

```scss
// SCSS map
$briks-components-generic: ( 
    // SCSS map | Nom du composant
    NOM_DU_COMPOSANT: ( 
        // Boolean | Composant activé true ou false
        enabled: true, 
        // Boolean | Responsive activé true ou false
        responsive: true, 
        // SCSS map | Liste des propriétés du composant par défaut (c-txt seul)
        defaults: (), 
        // SCSS map | Liste des modifieurs
        modifiers: () 
    )
);
```

## Configuration

Organisation et description du fichier de configuration [_sass/_txt_generic.scss](_sass/_txt_generic.scss).

```scss
/*
    C-TXT
    v0.1.0
    Composant générique CSS ITADS
    https://github.com/ita-design-system/c-txt.scss
*/
// SCSS map
$briks-components-generic: ( 
    // Nom du composant
    txt: ( 
        // Composant activé true ou false
        enabled: true, 
        // Responsive activé true ou false
        responsive: true, 
        // Liste des propriétés c-txt par défaut
        defaults: (),
        // Rendu: 
        // c-txt {
        // }
        // Liste des modifieurs contenant chacun une liste de propriétés qui 
        // soit surchargent les propriétés par défaut
        // soit ajoutent des propriétés
        // soit les deux
        modifiers: ( 
            // TEXT ALIGN
            // c-txt m-ta-left
            ta-left: (
                text-align: left
            ),
            // c-txt m-ta-center
            ta-center: (
                text-align: center
            ),
            // c-txt m-ta-right
            ta-right: (
                text-align: right
            ),
            // c-txt m-ta-justify
            ta-justify: (
                text-align: justify
            ),
            // TEXT DECORATION
            // c-txt m-td-underline
            td-underline: (
                text-decoration: underline
            ),
            // c-txt m-td-none
            td-none: (
                text-decoration: none
            ),
            // c-txt m-td-line-through
            td-line-through: (
                text-decoration: line-through
            ),
            // TEXT TRANSFORM
            // c-txt m-tt-uppercase
            tt-uppercase: (
                text-transform: uppercase
            ),
            // c-txt m-tt-lowercase
            tt-lowercase: (
                text-transform: lowercase
            ),
            // FONT STYLE
            // c-txt m-fstyle-italic
            fstyle-italic: (
                font-style: italic
            ),
            // ELLIPSE 1 ligne
            // c-txt m-ellipsis
            ellipsis: (
                white-space: nowrap,
                text-overflow: ellipsis,
                overflow: hidden
            ),
            // ELLIPSE 2 lignes
            // c-txt m-ellipsis-2
            ellipsis-2: (
                overflow: hidden,
                text-overflow: ellipsis,
                display: -webkit-box,
                '-webkit-box-orient': vertical,
                '-webkit-line-clamp': 2
            ),
            // ELLIPSE 3 lignes
            // c-txt m-ellipsis-3
            ellipsis-3: (
                overflow: hidden,
                text-overflow: ellipsis,
                display: -webkit-box,
                '-webkit-box-orient': vertical,
                '-webkit-line-clamp': 3
            ),
            // LINE HEIGHT
            // c-txt m-lh-0
            lh-0:(
                line-height: 0
            ),
            // c-txt m-lh-1
            lh-1:(
                line-height: 1em
            ),
            // c-txt m-lh-2
            lh-2:(
                line-height: 1.2em
            ),
            // c-txt m-lh-3
            lh-3:(
                line-height: 1.3em
            ),
            // c-txt m-lh-4
            lh-4:(
                line-height: 1.4em
            ),
            // c-txt m-lh-5
            lh-5:(
                line-height: 1.5em
            ),
            // c-txt m-lh-6
            lh-6:(
                line-height: 1.6em
            ),
            // VERTICAL ALIGN
            // c-txt m-va-top
            va-top: (
                vertical-align: top
            ),
            // c-txt m-va-middle
            va-middle: (
                vertical-align: middle
            ),
            // c-txt m-va-bottom
            va-bottom: (
                vertical-align: bottom
            ),
            // c-txt m-va-super
            va-super: (
                vertical-align: super
            ),
            // c-txt m-va-sub
            va-sub: (
                vertical-align: sub
            ),
            // CÉSURES
            // c-txt m-wb-break-all
            wb-break-all: (
                word-break: break-all
            ),
            // c-txt m-wb-break-word
            wb-break-word: (
                word-break: break-word
            ),
            // RETOURS À LA LIGNE
            // c-txt m-ws-nowrap
            ws-nowrap: (
                white-space: nowrap
            ),
            // LISSAGE TYPO
            antialiased: (
                -webkit-font-smoothing: antialiased,
                -moz-osx-font-smoothing: grayscale
            )
        )
    )
);
``` 

## Extensions

Il est possible d'étendre les fonctionnalités du composant en ajoutant simplement un point d'entrée avec une déclaration `$briks-components-generic` à la typologie identique mais avec des propriétés par défaut et des modifieurs qui surchargent ou ajoutent des propriétés CSS.

Exemple:

```scss
/*
    C-TXT EXTENSION
    Extension du composant générique c-txt
    https://github.com/ita-design-system/c-txt.scss
    Ce fichier doit servir à étendre ou surcharger les fonctionnalités
    du composant c-txt selon les besoins du projet
*/
$briks-components-generic: (
    // Nom du composant, obligatoirement txt
    txt: ( 
        // Extension activée true ou false
        enabled: true, 
        // Responsive activée true ou false pour l'extension
        responsive: true, 
        // Valeurs par défaut de l'extension
        defaults: (),
        // Liste des modifieurs contenant chacun une liste de propriétés qui 
        // soit surchargent les propriétés par défaut
        // soit ajoutent des propriétés
        // soit les deux
        modifiers: ( 
            ff-lead-400: (
                font-family: my-font-family(lead-400),
                font-weight: 400
            ),
            fs-1: (
                font-size: my-font-size(1)
            ),
            fs-2: (
                font-size: my-font-size(2)
            )
        )
    )
);
```
