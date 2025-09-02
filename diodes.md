# Diodes

Despite common thought, diodes do leak current
- **Normal Diodes**: Leak voltage about 0.6V (Silicon) forward and 0.3V (Germanium) backward 
- **Shottky Diodes**: Good ones are about 1/2 of Silicon at about 0.3-0.4V forward but bad ones are like 10x that.
- **Zener Diodes**: Very similar to Normal except that they can recover rather than burnout like Normal diodes. 
    - Often used as reverse biased at Zener Voltage to hold voltage constant for a device or node in its circuit. And does require a bit of current going through it. (Negative current will cause it to lose the Zener voltage and become forward biased)
        - Will split naturally split the current when doing that, and must be above zero to maintain the Zener voltage else it will hit the breakdown region and leakage will occur. May even be forward biased

Most Diodes rated to about half a watt

Diode Reverse Recovery:
- When you shut it off, still has some time of sending current. Almost like a bounce back to equilibrium. 
    - Shottky- Basically 0 (nanoseconds), Normal- Aobut a microsecond (noticeable in microcontroller as noise), Fast Recovery- in between at about hundreds of nanoseconds