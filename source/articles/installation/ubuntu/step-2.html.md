---

title: Installing Prerequsites for SplashKit
tags: installation,ubuntu

---

Once you have
[confirmed that your version of Ubuntu is supported](/articles/installation/ubuntu/step1/)
you will need to install a list of required software packages in order
for SplashKit to operate on Ubuntu.

1. Open up a terminal.

    ![Opening a terminal in Ubuntu](images/install-gifs/Ubuntu/open-terminal.gif)

2. Update your system's package manager cache.

    Copy and paste the code below into your terminal and press enter.

    ```bash
    sudo apt-get update
    ```

3. Install the pre-requisites for SplashKit

    Copy and paste the code below into your terminal and press enter.

    ```bash
    sudo apt-get install \
    git libsdl2-dev libsdl2-gfx-dev libsdl2-mixer-dev libsdl2-ttf-dev \
    libsdl2-net-dev libsdl2-image-dev libncurses-dev libpng-dev \
    libcurl4-openssl-dev libbz2-dev libflac-dev libvorbis-dev libmikmod-dev \
    libwebp-dev libfreetype6-dev cmake libgconf-2.0 clang
    ```

    You will be asked to confirm the installation of the selected packages. Review
    the list of packages, and confirm by typing "Y" and pressing enter.

    ![Confirm package installation](images/install-gifs/Ubuntu/confirm-packages.jpg)

    The pre-requisite packages will now be downloaded and installed. Wait
    for the installation process to finish before continuing to the next step.

4. Install libpng12 (Ubuntu 17.04 users only)

    If your [version of Ubuntu](/articles/installation/ubuntu/step1.html) is less than 17.04, you may skip this step.

    To install libpng12, copy and paste the code below into your terminal, one line at a time.

    ```bash
    cd /tmp
    wget http://mirrors.kernel.org/ubuntu/pool/main/libp/libpng/libpng12-0_1.2.54-1ubuntu1_amd64.deb
    sudo dpkg -i libpng12-0_1.2.54-1ubuntu1_amd64.deb
    cd -
    ```


Once you have completed this step, move on to the
[next step - Install SplashKit library](/articles/installation/ubuntu/step-3.html).

Return to the
[overview of the Ubuntu Linux install](/articles/installation/ubuntu).
