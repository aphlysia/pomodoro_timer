# Pomodoro Timer

A Pomodoro timer with a simple micro:bit-inspired appearance, implemented in a single HTML file.

## Requirements

- Count down from 25 minutes.
- Opening the HTML file displays the timer.

## Controls

| State | Action | Result |
| --- | --- | --- |
| Ready | Press the left button | Start the timer. |
| Running | Press the left button | Pause the timer. |
| Paused | Press the left button | Resume the countdown. |
| Paused | Press the right button | Return to the ready state. |
| Complete | Press the left button | Return to the ready state. |
| Complete | Press the right button | Start a new timer. |

## LED display

| State | Display |
| --- | --- |
| Ready | All LEDs are lit. |
| Running | LEDs for elapsed minutes are off, the current minute blinks, and the remaining LEDs are lit. |
| Paused | LEDs for elapsed minutes are off; the current and remaining LEDs blink together. |
| Complete | All LEDs are off. |

Examples:

- At the start, the top-left LED blinks and all other LEDs are lit.
- After one minute, the top-left LED is off, the next LED blinks, and all other LEDs are lit.
- After two minutes, the first two LEDs are off, the next LED blinks, and all other LEDs are lit.
- After five minutes, the top row is off, the first LED in the second row blinks, and all other LEDs are lit.
- After 25 minutes, all LEDs are off.

## Appearance

- Use a simple micro:bit-inspired design.
- Use a black board with a button on each side.
- Each button is a black circle inside a gray square.
- Arrange 25 red square LEDs in a 5 × 5 grid at the center.
- Do not display text on the page.
