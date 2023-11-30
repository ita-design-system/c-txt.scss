# c-txt.scss

[Démo et documentation](https://ita-design-system.github.io/c-txt.scss/)

Composant CSS dédié aux textes. 

## Tableau des abréviations modifieurs

Abréviations désignant les propriétés CSS utilisées dans la version courante.

| Propriété CSS | Abréviation | Composant / modifieur associé | Utilitaire associé |
|:-|:-|:-|:-|
| font-family | `ff-` | `c-txt m-ff-` | `u-ff-` |
| font-weight | `fw-` | `c-txt m-fw-` | `u-fw-` |
| hyphens | `hy-` | `c-txt m-hy-` | `u-hy-` |
| letter-spacing | `lsp-` | `c-txt m-lsp-` | `u-lsp-` |
| line-height | `lh-` | `c-txt m-lh-` | `u-lh-` |
| text-align | `ta-` | `c-txt m-ta-` | `u-ta-` |
| text-decoration | `td-` | `c-txt m-td-` | `u-td-` |
| text-transform | `tt-` | `c-txt m-tt-` | `u-tt-` |
| vertical-align | `va-` | `c-txt m-va-` | `u-va-` |
| word-break | `wb-` | `c-txt m-wb-` | `u-wb-` |
| white-space | `ws-` | `c-txt m-ws-` | `u-ws-` |

## Scope

Liste des propriétés CSS prises en charge par le composant

* column-count
* column-fill
* column-gap
* column-rule
* column-rule-color
* column-rule-style
* column-rule-width
* column-span
* column-width
* columns
* direction
* font
* font-family
* font-feature-settings
* font-kerning
* font-language-override
* font-optical-sizing
* font-palette
* font-size
* font-size-adjust
* font-stretch
* font-style
* font-synthesis
* font-variant
* font-variant-alternates
* font-variant-caps
* font-variant-east-asian
* font-variant-emoji
* font-variant-ligatures
* font-variant-numeric
* font-variant-position
* font-variation-settings
* font-weight
* hyphenate-character
* hyphenate-limit-chars
* hyphens
* letter-spacing
* line-break
* line-height
* text-align
* text-align-last
* text-combine-upright
* text-decoration
* text-decoration-color
* text-decoration-line
* text-decoration-skip
* text-decoration-skip-ink
* text-decoration-style
* text-decoration-thickness
* text-emphasis
* text-emphasis-color
* text-emphasis-position
* text-emphasis-style
* text-indent
* text-justify
* text-orientation
* text-overflow
* text-rendering
* text-shadow
* text-size-adjust
* text-transform
* text-underline-offset
* text-underline-position
* vertical-align
* white-space
* word-break
* word-spacing
* writing-mode
* -moz-osx-font-smoothing
* -webkit-font-smoothing


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
    v0.2.0
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
            // HYPHENS Césures
            // https://developer.mozilla.org/en-US/docs/Web/CSS/hyphens
            hy-auto: (
                hyphens: auto
            ),
            hy-manual: (
                hyphens: manual
            ),
            hy-none: (
                hyphens: none
            ),
            // FONT WEIGHT
            // https://developer.mozilla.org/en-US/docs/Web/CSS/font-weight#common_weight_name_mapping
            // 100 	Thin (Hairline)
            // 200 	Extra Light (Ultra Light)
            // 300 	Light
            // 400 	Normal
            // 500 	Medium
            // 600 	Semi Bold (Demi Bold)
            // 700 	Bold
            // 800 	Extra Bold (Ultra Bold)
            // 900 	Black (Heavy)
            fw-900: (
                font-weight: 900
            ),
            fw-800: (
                font-weight: 800
            ),
            fw-700: (
                font-weight: 700
            ),
            fw-600: (
                font-weight: 600
            ),
            fw-500: (
                font-weight: 500
            ),
            fw-400: (
                font-weight: 400
            ),
            fw-300: (
                font-weight: 300
            ),
            fw-200: (
                font-weight: 200
            ),
            fw-100: (
                font-weight: 100
            ),
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
            // c-txt m-fstyle-normal
            fstyle-normal: (
                font-style: normal
            ),
            // ELLIPSE 1 ligne
            // Requiert c-dis et c-dim pour fonctionner
            // c-txt m-ellipsis c-dim m-o-hidden
            ellipsis: (
                white-space: nowrap,
                text-overflow: ellipsis
            ),
            // ELLIPSE 2 lignes
            // A utiliser avec c-txt et c-dim
            // c-dis m-webkit-box
            // c-dim m-o-hidden
            // c-txt m-ellipsis-2
            ellipsis-2: (
                text-overflow: ellipsis,
            ),
            // ELLIPSE 3 lignes
            // A utiliser avec c-txt et c-dim
            // c-dis m-webkit-box
            // c-dim m-o-hidden
            // c-txt m-ellipsis-3
            ellipsis-3: (
                text-overflow: ellipsis
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
            // c-txt m-lh-7
            lh-7:(
                line-height: 1.7em
            ),
            // c-txt m-lh-8
            lh-8:(
                line-height: 1.8em
            ),
            // c-txt m-lh-8
            lh-9:(
                line-height: 1.9em
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
