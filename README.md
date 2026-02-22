# Colorful rickroll in terminal
shows rickroll in terminal, just like ascii.live/rick or ascii.live/can-you-hear-me but colorful and with better quality. Inspired by ascii.live and parrot.live

# Usage: [Not availbale now]

## Global
-   **curl.exe rvl-vovka.github.io/rr** ― *shows shortened help message that isn't a spoiler to what will happen when you run curl rvl-vovka.github.io/rr/mini or similar*
   
-   **curl.exe rvl-vovka.github.io/rr/info** ― *shows this help message*

## windows

 - **powershell -c "curl.exe rvl-vovka.github.io/rr/hugewin | iex"** ― *shows huge rickroll with really good quality [require really good internet connection and fast terminal emulator]*
   
 -  **powershell -c "curl.exe rvl-vovka.github.io/rr/midwin | iex"** ― *shows rickroll of normal size and normal quality [recommended for above average internet speed]*
   
-   **powershell -c "curl.exe rvl-vovka.github.io/rr/midnobgwin | iex"** ― *shows rickroll of normal size and normal quality but without background [much faster than with background so it is recommended for slower internet and/or slow terminal emulator]*
   
-   **powershell -c "curl.exe rvl-vovka.github.io/rr/miniwin | iex"** ― *shows small rickroll (size of default cmd in windows) [recommended for windows]*
   
-   **powershell -c "curl.exe rvl-vovka.github.io/rr/mininobgwin | iex"** ― *shows small rickroll but without background [recommended for windows with slow internet]*
   
## linux

 - **curl rvl-vovka.github.io/rr/hugelinux | sh** ― *shows huge rickroll with really good quality [require really good internet connection and fast terminal emulator]*
   
 -  **curl rvl-vovka.github.io/rr/midlinux | sh** ― *shows rickroll of normal size and normal quality [recommended for above average internet speed]*
   
-   **curl rvl-vovka.github.io/rr/midnobglinux | sh** ― *shows rickroll of normal size and normal quality but without background [much faster than with background so it is recommended for slower internet and/or slow terminal emulator]*
   
-   **curl rvl-vovka.github.io/rr/minilinux | sh** ― *shows small rickroll (size of default cmd in windows)*
   
-   **curl rvl-vovka.github.io/rr/mininobglinux | sh** ― *shows small rickroll but without background*

# Implementation explanation
I've tried to make it work as easy as just curl like parrot.live or ascii.live but it required paying for servers, so this is the closes I came up with: when you curl it you get code that is executed and creates an animation
> Note: please don't trust everyone who recommends you to curl source code and execute it especially on windows. It could be a virus, you should always check what code you will execute by running command without "| iex" or "| sh" in the end to make sure it is not a virus
