# How to install Slicer (5.8.1) in wsl?

Ask [ChatGPT](https://chatgpt.com/) OR do these ↓ ( :godmode: )

## if you don't have wsl

better to ask [ChatGPT](https://chatgpt.com/) ( 😅 )

## inside wsl (`lsb_release -a`: Ubuntu 22.04.5 LTS)

### Download 3DSlicer

1. Go to `~`

2. Download with `wget` from [3DSlicer Site](https://download.slicer.org) 

3. Extract downloaded file (e.x. `Slicer-5.8.1-linux-amd64.tar` with `tar -xvzf` to `/Slicer-5.8.1-linux-amd64`)

4. type `cd ./Slicer-5.8.1-linux-amd64/` and after that `./Slicer` to start

5. If have truble, check permisions (`chmod`) of executive file

6. If you have installed `VcXsrv` in windows, open that for see GUI window.

7. If Problem presits, do these steps:

    * change display with `export DISPLAY=:0` and try again

    *  install these packages for QT env

        ```bash
        sudo apt update

        sudo apt install -y \
        libx11-xcb1 \
        libxcb-render0 \
        libxcb-shape0 \
        libxcb-xfixes0 \
        libxcb-randr0 \
        libxcb-image0 \
        libxcb-icccm4 \
        libxcb-keysyms1 \
        libxcb-sync1 \
        libxcb-xinerama0 \
        libxcb-xkb1 \
        libxkbcommon0 \
        libxkbcommon-x11-0 \
        libglu1-mesa \
        libnss3 \
        libfontconfig1 \
        libfreetype6 \
        libxrender1 \
        libsm6 \
        libice6
        ```

        And test some qt applications before test 3DSlicer

        ```bash
        sudo apt install -y qtbase5-examples
        /usr/lib/x86_64-linux-gnu/qt5/examples/widgets/widgets/analogclock/analogclock &  
        ```


    * If you still have trouble, Ask ... [ChatGPT](https://chatgpt.com/)  :trollface:
