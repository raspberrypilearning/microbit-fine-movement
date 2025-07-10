Tu peux obtenir des valeurs de mouvement plus précises en utilisant `rotation`{:class='microbitinput'}.

- Tu peux trouver le bloc `rotation`{:class='microbitinput'} dans le menu `Entrée`{:class='microbitinput'} dans ta boîte à outils.

Cela peut être utilisé pour comparer une valeur `rouler` maximale pour déclencher un événement.

Voici un exemple.

```microbit
basic.forever(function () {
    if (input.rotation(Rotation.Roll) < -10 || input.rotation(Rotation.Roll) > 10) {
        basic.showIcon(IconNames.EighthNote)
    } else {
        basic.showLeds(`
            . # # # .
            . . . # .
            . . # # .
            . . . . .
            . . # . .
            `)
    }
})
```

Voici le code exécuté sur le simulateur.

Fais rouler le micro:bit vers la gauche ou la droite pour déclencher le changement d'icône. <br>

<div style="position:relative;height:0;padding-bottom:127%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:60%;height:100%;" src="https://makecode.microbit.org/---run?id=_gzvM5a8MgA4f" allowfullscreen="allowfullscreen" sandbox="allow-popups allow-forms allow-scripts allow-same-origin" frameborder="0"></iframe></div>
