# Colorful rickroll in terminal
shows rickroll in terminal, just like ascii.live/rick or ascii.live/can-you-hear-me but colorful and with better quality. Inspired by ascii.live and parrot.live

# Usage:

## Global
-   **curl rvl-vovka.github.io/rr** ― *shows shortened help message that isn't a spoiler to what will happen when you run curl rvl-vovka.github.io/rr/mini or similar*
   
-   **curl rvl-vovka.github.io/rr/info** ― *shows this help message*

## windows

 - **powershell -c "(iwr -useb rvl-vovka.github.io/rr/bigwin).content | iex"** ― *shows big rickroll with really good quality [requires really good internet connection or will take some time to load]*
   
 -  **powershell -c "(iwr -useb rvl-vovka.github.io/rr/midwin).content | iex"** ― *shows rickroll of normal size and normal quality [recommended for fullscreen]*
   
-   **powershell -c "(iwr -useb rvl-vovka.github.io/rr/midnobgwin).content | iex"** ― *shows rickroll of normal size and normal quality but without background [much faster than with background so it is recommended for slower internet]*
   
-   **powershell -c "(iwr -useb rvl-vovka.github.io/rr/miniwin).content | iex"** ― *shows small rickroll (size of default terminal window in windows) [recommended for windowed mode or just fast opening in win+r box]*
   
-   **powershell -c "(iwr -useb rvl-vovka.github.io/rr/mininobgwin).content | iex"** ― *shows small rickroll but without background [recommended for windows with slow internet]*
   
## linux

 - **curl -L rvl-vovka.github.io/rr/biglinux | sh** ― *shows huge rickroll with really good quality [requires really good internet connection or will take some time to load]*
   
 -  **curl -L rvl-vovka.github.io/rr/midlinux | sh** ― *shows rickroll of normal size and normal quality [recommended for fullscreen]*
   
-   **curl -sL rvl-vovka.github.io/rr/midnobglinux | sh** ― *shows rickroll of normal size and normal quality but without background [much faster than with background so it is recommended for slower internet and/or slow terminal emulator, e.g. termux, at this point -s is recommended because width of rickroll is less than width of curl downloading progress messages]*
   
-   **curl -sL rvl-vovka.github.io/rr/minilinux | sh** ― *shows small rickroll (size of default cmd in windows) [recommended for windowed mode]*
   
-   **curl -sL rvl-vovka.github.io/rr/mininobglinux | sh** ― *shows small rickroll but without background [recommended for slow terminal emulators e.g. termux]*

# Implementation explanation
I've tried to make it work as easy as just curl like parrot.live or ascii.live but it required paying for servers, so this is the closes I came up with: when you curl it you get code that is executed and creates an animation, it is also somewhat better because it doesn't need constant internet connection
> Note: please don't trust everyone who recommends you to curl source code and execute it especially on windows. It could be a virus, you should always check what code you will execute by running command without "| iex" or "| sh" in the end to make sure it is not a virus
