# mesa-20.2.6-linux-ultra-pefomance-wayland-graphics
ubuntu , debian , fedora , arch , all  , test  , distro , meson , ninja-build , perfomance wayland new , griggorii , quality color grafic , quality audio

Download source mesa + my include: https://github.com/Griggorii/mesa-20.2.6-linux-ultra-pefomance-wayland-graphics/releases/tag/20.2.6

Dev install example 20.04

$ sudo apt install binfmt-support glslang-tools lib32gcc-s1 lib32stdc++6 libc6-i386 libclang-10-dev libclang-common-10-dev libclang-cpp10 libclang1-10 libclc-dev libdrm-dev libegl-dev libelf-dev libexpat1-dev libgl-dev libgles-dev libgles1 libglvnd-dev libglx-dev libncurses-dev libobjc-10-dev libobjc4 libopengl-dev libopengl0 libpfm4 libpthread-stubs0-dev libsensors4-dev libset-scalar-perl libtinfo-dev libva-dev libva-glx2 libvdpau-dev libvulkan-dev libwayland-bin libwayland-dev libwayland-egl-backend-dev libx11-dev libx11-xcb-dev libxau-dev libxcb-dri2-0-dev libxcb-dri3-dev libxcb-glx0-dev libxcb-present-dev libxcb-randr0-dev libxcb-render0-dev libxcb-shape0-dev libxcb-sync-dev libxcb-xfixes0-dev libxcb1-dev libxdamage-dev libxdmcp-dev libxext-dev libxfixes-dev libxrandr-dev libxrender-dev libxshmfence-dev libxxf86vm-dev libz3-4 libz3-dev libzstd-dev llvm-10 llvm-10-dev llvm-10-runtime llvm-10-tools python3-pygments python3-setuptools quilt spirv-tools valgrind wayland-protocols x11proto-xf86vidmode-dev meson ninja-build cmake

$ tar xvpf mesa-20.2.6_dump.tar.xz -C /tmp

Sudo and root backup:

$ cd ~/ && sudo XZ_OPT=-9 tar -Jcvf backup_original_include.tar.xz /usr/include

$ sudo tar xvpf include_griggorii_collection_patent_all_my_job_build_20.04_new.tar.xz -C /

$ cd /tmp/mesa-20.2.6/griggorii

$ meson --reconfigure

$ ninja install

install mesa build replace reinstall original security include | возвращение оригинальных инклюдов что бы было безопаснее пусть корпорации качают инклюды тут потом заплатят за всю сборку инклюдов которые я подобрал чем они будут собирать имея доступ к компьютерам через керберос на ваших компьютерах используя инклюды как хост инклюды они конечно могут сказать что они кристально чисты и никуда не лезут если все выключено и фаирволл , но если у вас останутся именно эти инклюды то вы заметите что компьютер начнет тормозить значат на вас что то собирают удаленно , мне пока не удалось выбить инвестиции что бы собирать именно свою ос по этому пока так.  

$ cd ~/ && sudo rm -rf /usr/include && sudo tar xvpf backup_original_include.tar.xz -C /  




