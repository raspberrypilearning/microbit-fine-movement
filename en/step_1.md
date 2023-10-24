You can get more accurate movement values using `rotation`{:class='microbitinput'}.

- You can find the `rotation`{:class='microbitinput'} block in the `Input`{:class='microbitinput'} menu in your Toolbox.

This can be used to compare against a maximum `roll` value to trigger an event.

Here is an example.

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

Here is the code running on the simulator.

Roll the micro:bit left or right to trigger the icon to change.
<br>
<div style="position:relative;height:0;padding-bottom:127%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:60%;height:100%;" src="https://makecode.microbit.org/---run?id=_gzvM5a8MgA4f" allowfullscreen="allowfullscreen" sandbox="allow-popups allow-forms allow-scripts allow-same-origin" frameborder="0"></iframe></div>
