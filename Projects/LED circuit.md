# LED circuit

## Aim
To create a circuit using;
- 9V battery
- Resistor(s)
- LED
- Jumper wires
- Breadboard

## Setup
Started with some breadboard research and trial and error to understand the layout and use of a breadboard.
Research how to calculate the resistors required (and why they're required).
I calculated the resistance required to be 360 ohms but didn't have a 360 ohms resistor.
R = (battery voltage 9V - LED forward voltage 1.8V) / LED operating current 0.02 amps
I read that resistors place in series sum. So I used a 330 and 100 ohms resistors in series.

![alt text](image.png)














## Testing
The LED lit up to confirm the circuit was working correctly.

### Voltage

The voltage of the battery was 9V as expected.
The voltage over the led 2.056V
The voltage over the 330 ohm resistor was 5.490V
The voltage over the 100 ohm resistor was 1.626V

2.056V + 5.490V + 1.626V = 9.172V

Close enough for a first try.

## Investigation
#### Many resistors
I discovered that I could add many resistors without affecting the brightness of the battery. Which isn't what I expected.

It didn't make sense because I assumed the voltage drop observered over one resistor would be the same over others.

### Voltage drop of resistors and LEDs in series
The total voltage across the circuit is always around 5V.

LEDs \ Resistors | 1 | 2 | 3
--- | --- | --- | ---
2 | 1.49V \ 2.05V | 0.57V \ 1.95V | 0.003V \ 1.68V 
3 | 1.01V \ 2.01V | 0.40V \ 1.92V | 0.003V \ 1.67V
4 | 0.76V \ 1.98V | 0.31V \ 1.90V | 0.003V \ 1.67V

