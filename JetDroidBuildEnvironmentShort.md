### Alternative short description to setup the build environment ###
  1. In any directory you want make JetDroid directory by `mkdir JetDroid`
  1. All work will be done inside this direcrory so change directory by `cd JetDroid`
  1. Download repo script by `curl http://android.git.kernel.org/repo > repo`
  1. Make sure that the script is executable by `chmod +x repo`
  1. Make directory for android standart parts including prebuilt toolchain by `mkdir android`
  1. Change directory by `cd android`
  1. Download repository by `../repo init -u git://android.git.kernel.org/platform/manifest.git -b eclair`
  1. Initiate repository by `../repo sync`. This command may take a long time because it downloads all stuff
  1. Come back to the JetDroid directory by `cd ..`
  1. Work with this directory should not bring any problems in the future