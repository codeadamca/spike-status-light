# LEGO Spike Hub and the Hub Status Light

A Python snippet utilizing the LEGO Spike status light, [MicroPython](https://lego.github.io/MINDSTORMS-Robot-Inventor-hub-API/), and the `on()` and `off()` commands.

## Sample Code

```py
from mindstorms import MSHub
from mindstorms.control import wait_for_seconds

hub = MSHub()

colors = [
    'azure',
    'black',
    'blue',
    'cyan',
    'green',
    'orange',
    'pink',
    'red',
    'violet',
    'white',
    'yellow'
]

for color in colors:

    print(color)

    hub.status_light.on(color)

    wait_for_seconds(1)

hub.status_light.off()

hub.speaker.beep()
```

***

## Repo Resources

* [Visual Studio Code](https://code.visualstudio.com/)
* [MicroPython for LEGO Robot Inventor](https://www.lego.com/en-ca/themes/mindstorms/downloads)
* [LEGO Mindstorms](https://www.lego.com/en-ca/themes/mindstorms)
* [LEGO Mindstorms App for Mac](https://apps.apple.com/us/app/lego-mindstorms-inventor/id1515448947)
* [LEGO Mindstorms App for Android](https://play.google.com/store/apps/details?id=com.lego.retail.mindstorms)
* [LEGO Mindstorms App for Windows](https://www.microsoft.com/store/apps/9N7GN3KC2GK6)

<a href="https://codeadam.ca">
<img src="https://codeadam.ca/images/code-block.png" width="100">
</a>
