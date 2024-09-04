Μπορείς να λάβεις πιο ακριβείς τιμές κίνησης χρησιμοποιώντας την `περιστροφ`'{:class='microbitinput'}.

- Μπορείς να βρεις το μπλοκ `περιστροφή`{:class='microbitinput'} στο μενού `Είσοδος`{:class='microbitinput'} στην Εργαλειοθήκη σου.

Αυτό μπορεί να χρησιμοποιηθεί για σύγκριση με μια μέγιστη τιμή `κύληση` για την ενεργοποίηση ενός συμβάντος.

Εδώ είναι ένα παράδειγμα.

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

Εδώ είναι ο κώδικας που εκτελείται στον προσομοιωτή.

Μετακίνησε το micro:bit αριστερά ή δεξιά για να ενεργοποιήσεις το εικονίδιο για αλλαγή. <br>

<div style="position:relative;height:0;padding-bottom:127%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:60%;height:100%;" src="https://makecode.microbit.org/---run?id=_gzvM5a8MgA4f" allowfullscreen="allowfullscreen" sandbox="allow-popups allow-forms allow-scripts allow-same-origin" frameborder="0"></iframe></div>
