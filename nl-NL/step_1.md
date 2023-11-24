Je kunt nauwkeurigere bewegingswaarden verkrijgen met behulp van `rotatie`{:class='microbitinput'}.

- Je kunt het blok `rotatie`{:class='microbitinput'} vinden in het `Invoer`{:class='microbitinput'} menu in je Toolbox.

Dit kan worden gebruikt om te vergelijken met een maximale 'rol' waarde om een gebeurtenis te activeren.

Hier is een voorbeeld.

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

Hier is de code die op de simulator draait.

Rol de micro:bit naar links of rechts om het pictogram te laten veranderen. <br>

<div style="position:relative;height:0;padding-bottom:127%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:60%;height:100%;" src="https://makecode.microbit.org/---run?id=_gzvM5a8MgA4f" allowfullscreen="allowfullscreen" sandbox="allow-popups allow-forms allow-scripts allow-same-origin" frameborder="0"></iframe></div>
