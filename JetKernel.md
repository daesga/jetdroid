# Kernel repositories #
  * [JetDroid kernel repository](http://github.com/Dopi/JetKernel)
  * [Samsung kernel development repository](http://git.kernel.org/pub/scm/linux/kernel/git/kki_ap/linux-2.6-samsung.git/)
  * [Samsung OpenSource](http://opensource.samsungmobile.com/index.jsp?page=1). GT-I5700 (Spica) and SPH-M900 (Moment) source code can be downloaded from this page.

# Setting up a build environment #
See JetDroidBuildEnvironment.

# Kernel building instructions #
Here are the current kernel build instructions:
  * download kernel sources from repo:
```
    git clone -n git://github.com/Dopi/JetKernel.git
    cd JetKernel
    git checkout -b testing-2.6.29 origin/testing-2.6.29
```
  * make jet's config to be current
```
     cp arch/arm/configs/jet_android_defconfig .config
```
  * enter menu config:
```
     make menuconfig
```
> > and disable `General setup -> Initial RAM filesystem and RAM disk...`
  * after it you are ready to build kernel

# Some notes about crosscompilation #
JetKernel has one crosscompilation specific setting set up in makefile.
It is `ARCH` option. So to build other kernel for jet it is needed to call `make` like:
```
make CROSS_COMPILE=pathtocc ARCH=arm ...
```
So it is possible to use following script (named `make.sh` and placed into kernel directory) with predefined path to crosscompiler (if you set up your environment as it is described here: JetDroidBuildEnvironment, then such path should be correct):
```
#! /bin/sh
CCOMPILER=../android/prebuilt/linux-x86/toolchain/arm-eabi-4.4.0/bin/arm-eabi-
make CROSS_COMPILE=$CCOMPILER ARCH=arm $@
```
`make` commands then should look like:
```
./make.sh menuconfig
./make.sh
```

# Kernel building links #
  * [Building cyanogen from source](http://wiki.cyanogenmod.com/index.php/Building_from_source)
  * [Compile Android kernel from the source](http://whyandroid.com/android/221-compile-android-kernel-from-the-source.html)
  * [http://blog.csdn.net/hongjiujing/archive/2009/08/18/4460044.aspx](http://blog.csdn.net/hongjiujing/archive/2009/08/18/4460044.aspx)