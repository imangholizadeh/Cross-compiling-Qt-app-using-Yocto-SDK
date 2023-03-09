# Cross-compiling Qt applications using Yocto Project standard SDK

[1] : add " inherit populate_sdk_qt5 " command to "qt5-image.bb" file located in "/poky/meta-licheepizero/recipes-images/images"    
(for example in my projecct address is "/home/imangh/yocto/poky/meta-licheepizero/recipes-images/images")

[2] : build the standard SDK with the command: " bitbake -c populate_sdk <image-name> "
We now obtain an installable SDK in build/tmp/deploy/sdk/<image-name>-<host-arch>-<distro-version>-toolchain.sh     
(for example for my project its located in " /home/imangh/yocto/tmp/deploy/sdk ")

[3]: Install the SDK with command : "./(image-name)-(host-arch)-(distro-version)-toolchain.sh "  
(for example for my project its " ./poky-glibc-x86_64-qt5-image-armv7vet2hf-neon-licheepizero-dock-toolchain-3.1.23.sh  ")

[4]:Configuring Qt Creator for cross-compilation

source link:https://technotes.kynetics.com/2018/Yocto-SDK-Qt/
