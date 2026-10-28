let humor = 0

input.onButtonPressed(Button.A, function () {
    if (humor == 0) {
        basic.showLeds(`
            . . . . .
            . # . # .
            . . . . .
            # . . . #
            . # # # .
        `)
    } else if (humor == 1) {
        basic.showLeds(`
            . . . . .
            . # . # .
            . . . . .
            . # # # .
            # . . . #
        `)
    } else if (humor == 2) {
        basic.showLeds(`
            . # . # .
            . . . . .
            . . # . .
            . # . # .
            . . # . .
        `)
    } else {
        basic.showLeds(`
            . . . . .
            . # . # .
            . . . . .
            # . # . #
            . # . # .
        `)
    }

    humor += 1
    if (humor == 4) {
        humor = 0
    }
})

basic.forever(function () {
})
