# Colorful rickroll in terminal
shows rickroll in terminal, just like ascii.live/rick or ascii.live/can-you-hear-me but colorful and with better quality. Inspired by ascii.live and parrot.live

# Usage:

## Global
-   **curl -sL rvl-vovka.github.io/rr** ― *shows shortened help message that isn't a spoiler to what will happen when you run curl rvl-vovka.github.io/rr/mini or similar*
   
-   **curl -sL rvl-vovka.github.io/rr/info** ― *shows this help message*

## Windows

 - **powershell -c "(iwr -useb rvl-vovka.github.io/rr/bigwin).content | iex"** ― *shows big rickroll with really good quality [requires really good internet connection or will take some time to load]*
   
 -  **powershell -c "(iwr -useb rvl-vovka.github.io/rr/midwin).content | iex"** ― *shows rickroll of normal size and normal quality [recommended for fullscreen]*
   
-   **powershell -c "(iwr -useb rvl-vovka.github.io/rr/midnobgwin).content | iex"** ― *shows rickroll of normal size and normal quality but without background [much faster than with background so it is recommended for slower internet]*
   
-   **powershell -c "(iwr -useb rvl-vovka.github.io/rr/miniwin).content | iex"** ― *shows small rickroll (size of default terminal window in windows) [recommended for windowed mode or just fast opening in win+r box]*
   
-   **powershell -c "(iwr -useb rvl-vovka.github.io/rr/mininobgwin).content | iex"** ― *shows small rickroll but without background [recommended for windows with slow internet]*
   
## Linux

 - **curl -sL rvl-vovka.github.io/rr/biglinux | sh** ― *shows huge rickroll with really good quality [requires really good internet connection or will take some time to load]*
   
 -  **curl -sL rvl-vovka.github.io/rr/midlinux | sh** ― *shows rickroll of normal size and normal quality [recommended for fullscreen]*
   
-   **curl -sL rvl-vovka.github.io/rr/midnobglinux | sh** ― *shows rickroll of normal size and normal quality but without background [much faster than with background so it is recommended for slower internet and/or slow terminal emulator, e.g. termux, at this point -s is recommended because width of rickroll is less than width of curl downloading progress messages]*
   
-   **curl -sL rvl-vovka.github.io/rr/minilinux | sh** ― *shows small rickroll (size of default cmd in windows) [recommended for windowed mode]*
   
-   **curl -sL rvl-vovka.github.io/rr/mininobglinux | sh** ― *shows small rickroll but without background [recommended for slow terminal emulators e.g. termux]*

# Implementation explanation
I've tried to make it work as easy as just curl like parrot.live or ascii.live but it required paying for servers, so this is the closes I came up with: when you curl it you get code that is executed and creates an animation, it is also somewhat better because it doesn't need constant internet connection
> Note: please don't trust everyone who recommends you to curl source code and execute it especially on windows. It could be a virus, you should always check what code you will execute by running command without "| iex" or "| sh" in the end to make sure it is not a virus

# Other
All windows versions of animation work with newer powershell and it is recommended to use newer versions if they are available because they are faster (replace powershell with pwsh).

All windows versions should work on other operating systems as long as they have powershell installed.

If you want to have local version that doesn't require internet connection you can download "index.html" file from folder that you want or put "> animation.txt" in the end instead of "| iex" or "| sh". Then rename file to for example OpenMe.ps1 (for windows versions) or OpenMe.sh (for linux versions) and run it locally anytime you want (if you used "> animation.txt" method file will be in start position folder of terminal, usually your home folder).

All linux versions are **NOT** compatable with bash. you have to add "-e" ater each "echo" in the local script you downloaded for it to be compatable but it is not recommended because sh if faster and more supported.

Some terminals (e.g. jackpal android terminal) don't support unicode characters by default (or maybe at all), I can't fix that.
