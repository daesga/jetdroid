### Preamble: Regular user _**should not use it**_! ###
This project is not finished yet. It is under active development. Thus this page is intended for developers who want to help with programing. Regular users _**should not use it**_ now!

Currently you will not find any instructions here on how to run Android on the Jet. Moreover it is so far _**not possible**_ to run Android now. None of the hardcore actions described below _**will not bring the android to the phone**_ yet!

### Install Linux ###
Currently all Android related development needs a Linux environment (or may be any other `*`nix environment including cygwin. But it may be more difficult and this way is not guaranteed to work). If you are mainly using Windows it is an option to run Linux inside a virtual machine (e.g. using [VirtualBox](http://www.virtualbox.org/)). An usefull (small) Linux distribution is Ubuntu Netbook Remix. Install images can be found here: [http://www.ubuntu.com/getubuntu/download-netbook](http://www.ubuntu.com/getubuntu/download-netbook).

### Installation of the toolchain ###
It is needed to use arm-eabi cross toolchain. It is easy to obtain a prebuilt toolchain with the Android sources. Next instructions should help you with it. Similar instructions can be found in other places like [android.com](http://source.android.com/download/) and [CyanogenMod](http://wiki.cyanogenmod.com/index.php/Building_from_source). The steps shon here should not be taken as a strict recipie. There is always a chance that tomething may be different on your system or your setup. You can find a short version of these instructions [here](JetDroidBuildEnvironmentShort.md).

### Install + Setup Repo ###
  1. Open a terminal and run the following comands to install the various tools you will need.<pre>sudo aptitude install git-core gnupg sun-java6-jdk flex bison gperf libsdl-dev ncurses-dev libc6-dev-i386</pre><pre>sudo aptitude install libesd0-dev libwxgtk2.6-dev build-essential zip curl libncurses5-dev zlib1g-dev valgrind</pre>
  1. Make sure you have a /bin directory in your /home directory <pre>cd ~/</pre><pre>mkdir bin</pre><pre>echo $PATH</pre> You should see something like ':/home/user\_name/bin:' in a line of text. If you don't see this, try restarting your computer or add it to your path (in case you are using the bash shell) by executing <pre>echo "export PATH=$PATH:$HOME/bin" >>~/.bashrc</pre> and restarting your terminal. (we should admit that adding a user writable directory into the path may decrease your computer security)
  1. Download repo and make it executable<pre>curl http://android.git.kernel.org/repo >~/bin/repo</pre><pre>chmod a+x ~/bin/repo</pre>

### Setup your working directories ###
  1. Create directories to hold your working files:<pre>mkdir ~/JetDroid</pre><pre>cd ~/JetDroid</pre><pre>mkdir android</pre>

### Download the Android source ###
  1. Change to the Android source directory <pre>cd ~/JetDroid/android</pre>
  1. Download the Android 2.1 (Eclair) Repo:<pre>repo init -u git://android.git.kernel.org/platform/manifest.git -b eclair</pre>If everything was successful, you should see a message like 'repo initialized in ~/JetDroid/android'
  1. Next, get the latest files:<pre>repo sync</pre>This step may take a while as this command will download approx 4 Gb of data.

### Enable read-write access to the repositories ###
  1. If you don't want write access to the repository please skip this section
  1. For read-write access to the github repository you need to have a github account. If you do not already have one you can create a free account [here](https://github.com/signup/free). Your github account needs to be write enabled for the JetDroid repositories in order to make changes. Please write to dopi711 (at) googlemail.com if you need write access,
  1. Your ssh public keys need to be set up inside your github account as described [here](http://help.github.com/linux-key-setup/).

### Download the JetQi bootloader source ###
  1. Change to the JetDroid working directory<pre>cd ~/JetDroid</pre>
  1. Use git to fetch the current source from the repository at github. Execute <pre>git clone -n git://github.com/Dopi/JetQi.git</pre> if you want to go with read-only access or execute <pre>git clone -n git@github.com:Dopi/JetQi.git</pre> if you have everything set up for read-write accees.
  1. Checkout the testing branch <pre>cd JetQi</pre><pre>git checkout -b testing origin/testing</pre>
  1. Please note that you will need to download the kernel source (as described in the following section) prior to compiling the JetQi bootloader as the kernel include directory is required for the bootloader build process.

### Download the JetKernel linux kernel source ###
  1. Change to the JetDroid working directory<pre>cd ~/JetDroid</pre>
  1. Use git to fetch the current source from the repository at github. Execute <pre>git clone -n git://github.com/Dopi/JetKernel.git</pre> if you want to go with read-only access or execute <pre>git clone -n git@github.com:Dopi/JetKernel.git</pre> if you have everything set up for read-write accees.
  1. Create a link inside the JetDroid working directory to point to the active kernel directory <pre>ln -s JetKernel kernel</pre> This link is requires by the JetQi build environment to find the kernel includes.
  1. Checkout the testing branch <pre>cd JetKernel</pre><pre>git checkout -b testing origin/testing</pre>

### Building the JetQi bootloader ###
  1. Type `./build.sh` (`./make_qi.sh` for old versions) when you are in JetQi directory and all should be builded without any messages
  1. You will find new bootloader in the image directory. The bootloader image to flash is called `qi-s3c6410-YYYYMMDD-JetQi.mbn` with YYYY, MM and DD corresponding to the build date. Before flashing you need to replace the `boot_loader.mbn` of your firmware with this file.
If you use other names for directories then after downloading of JetQi you may need to change something in `config.mk` and `make_qi.sh` files to set up building process closely to your toolchain installation. It is known that variables named `CROSS_PATH` and `KERNEL_PATH` may vary from one installation to another. So do not be afraid to change them for your purposes if something fails. And there is one important note: you need to download kernel sources (JetKernel) in order to build JetQi. You can download JetKernel sources in the same way as JetQi sources just with other git file. Without JetKernel sources or with bad `KERNEL_PATH` build process may fail with very strange messages like: ``Error: bad instruction `bswapl r3'``.

Please see JetQiFlashing page for instructions how to flash the bootloader to your phone.

### Building the android sources ###

To build sources just type make in android's folder:

<pre>cd ~/JetDroid/android</pre>
<pre>make</pre>

If you are building under x86\_64 you may encounter the following errors:

<pre>/usr/bin/ld: skipping incompatible /usr/lib/gcc/x86_64-linux-gnu/4.2.3/libstdc++.a when searching for -lstdc++<br>
/usr/bin/ld: cannot find -lstdc++<br>
collect2: ld returned 1 exit status</pre>

You should install g++-multilib:

<pre>sudo apt-get install g++-multilib</pre>

If you are experiencing the following errors:

<pre>/usr/bin/ld: skipping incompatible /usr/lib/gcc/x86_64-linux-gnu/4.4.3/../../../libz.so when searching for -lz<br>
/usr/bin/ld: skipping incompatible /usr/lib/gcc/x86_64-linux-gnu/4.4.3/../../../libz.a when searching for -lz<br>
/usr/bin/ld: skipping incompatible /usr/lib/libz.so when searching for -lz<br>
/usr/bin/ld: skipping incompatible /usr/lib/libz.a when searching for -lz<br>
/usr/bin/ld: cannot find -lz</pre>

You should install lib32z1-dev:

<pre>sudo apt-get install lib32z1-dev</pre>

If you are experiencing the following errors:

<pre>
/usr/bin/ld: skipping incompatible /usr/lib/gcc/x86_64-linux-gnu/4.4.3/../../../libncurses.so when searching for -lncurses<br>
/usr/bin/ld: skipping incompatible /usr/lib/gcc/x86_64-linux-gnu/4.4.3/../../../libncurses.a when searching for -lncurses<br>
/usr/bin/ld: skipping incompatible /usr/lib/libncurses.so when searching for -lncurses<br>
/usr/bin/ld: skipping incompatible /usr/lib/libncurses.a when searching for -lncurses<br>
/usr/bin/ld: cannot find -lncurses</pre>

You should install lib32ncurses5-dev:

<pre>sudo apt-get install lib32ncurses5-dev</pre>