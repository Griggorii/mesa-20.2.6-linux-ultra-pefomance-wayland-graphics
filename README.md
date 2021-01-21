# mesa-20.2.6-linux-ultra-pefomance-wayland-graphics
ubuntu , debian , fedora , arch , all  , test  , distro , meson , ninja-build , perfomance wayland new , griggorii , quality color grafic , quality audio , quality ultra hd 10K 16K pixelization gui

13.01.2021 произведен новый революционный видео драйвер который влияет не только на улучшение картинки , но и аудио подсистемы.

Download mesa 20.2.6 ubuntu 20.04: https://github.com/Griggorii/mesa-20.2.6-linux-ultra-pefomance-wayland-graphics/releases/download/20.2.6/mesa-20.2.26_build_best_pixelization_20.04.zip libc-2.31

Download source mesa + my include: https://github.com/Griggorii/mesa-20.2.6-linux-ultra-pefomance-wayland-graphics/releases/tag/20.2.6

Test original video driver test https://linuxreviews.org/static/unity-browser-benchmarks-2018

Dev install exmp 20.04 | ubuntu old 17.04\17.10\18.04\18.10\19.04\19.10 replace libclang-common-<ver?> libclang-? libclang1-? libobjc-?-dev 

$ sudo rm /usr/share/doc/libc6/changelog.Debian.gz /usr/share/doc/libc6-i386/changelog.Debian.gz

$ sudo apt install binfmt-support glslang-tools lib32gcc-s1 lib32stdc++6 libc6-i386 libclang-10-dev libclang-common-10-dev libclang-cpp10 libclang1-10 libclc-dev libdrm-dev libegl-dev libelf-dev libexpat1-dev libgl-dev libgles-dev libgles1 libglvnd-dev libglx-dev libncurses-dev libobjc-10-dev libobjc4 libopengl-dev libopengl0 libpfm4 libpthread-stubs0-dev libsensors4-dev libset-scalar-perl libtinfo-dev libva-dev libva-glx2 libvdpau-dev libvulkan-dev libwayland-bin libwayland-dev libwayland-egl-backend-dev libx11-dev libx11-xcb-dev libxau-dev libxcb-dri2-0-dev libxcb-dri3-dev libxcb-glx0-dev libxcb-present-dev libxcb-randr0-dev libxcb-render0-dev libxcb-shape0-dev libxcb-sync-dev libxcb-xfixes0-dev libxcb1-dev libxdamage-dev libxdmcp-dev libxext-dev libxfixes-dev libxrandr-dev libxrender-dev libxshmfence-dev libxxf86vm-dev libz3-4 libz3-dev libzstd-dev llvm-10 llvm-10-dev llvm-10-runtime llvm-10-tools python3-pygments python3-setuptools quilt spirv-tools valgrind wayland-protocols x11proto-xf86vidmode-dev meson ninja-build cmake

Locate download files source + include run terminal command:

$ tar xvpf mesa-20.2.6_dump.tar.xz -C /tmp

Sudo and root backup:

$ cd ~/ && sudo XZ_OPT=-9 tar -Jcvf backup_original_include.tar.xz /usr/include && cd -

$ sudo tar xvpf include_griggorii_collection_patent_all_my_job_build_20.04_new.tar.xz -C /

$ cd /tmp/mesa-20.2.6/griggorii

$ meson --reconfigure

$ ninja install

$ cd ~/ && sudo rm -rf /usr/include && sudo tar xvpf backup_original_include.tar.xz -C /

size stip mesa root terminal command:

$ strip -s '/usr/lib/libomxil-bellagio.a' '/usr/lib/libomxil-bellagio.so' '/usr/lib/libomxil-bellagio.so.0' '/usr/lib/libomxil-bellagio.so.0.0.0' '/usr/lib/x86_64-linux-gnu/d3d/d3dadapter9.so.1.0.0' '/usr/lib/x86_64-linux-gnu/dri/i915_dri.so' '/usr/lib/x86_64-linux-gnu/dri/i965_dri.so' '/usr/lib/x86_64-linux-gnu/dri/iris_dri.so' '/usr/lib/x86_64-linux-gnu/dri/kms_swrast_dri.so' '/usr/lib/x86_64-linux-gnu/dri/nouveau_dri.so' '/usr/lib/x86_64-linux-gnu/dri/nouveau_drv_video.so' '/usr/lib/x86_64-linux-gnu/dri/nouveau_vieux_dri.so' '/usr/lib/x86_64-linux-gnu/dri/r200_dri.so' '/usr/lib/x86_64-linux-gnu/dri/r300_dri.so' '/usr/lib/x86_64-linux-gnu/dri/r600_dri.so' '/usr/lib/x86_64-linux-gnu/dri/r600_drv_video.so' '/usr/lib/x86_64-linux-gnu/dri/radeon_dri.so' '/usr/lib/x86_64-linux-gnu/dri/radeonsi_dri.so' '/usr/lib/x86_64-linux-gnu/dri/radeonsi_drv_video.so' '/usr/lib/x86_64-linux-gnu/dri/swrast_dri.so' '/usr/lib/x86_64-linux-gnu/dri/virtio_gpu_dri.so' '/usr/lib/x86_64-linux-gnu/dri/vmwgfx_dri.so' '/usr/lib/x86_64-linux-gnu/dri/zink_dri.so' '/usr/lib/x86_64-linux-gnu/gallium-pipe/pipe_nouveau.so' '/usr/lib/x86_64-linux-gnu/gallium-pipe/pipe_r300.so' '/usr/lib/x86_64-linux-gnu/gallium-pipe/pipe_r600.so' '/usr/lib/x86_64-linux-gnu/gallium-pipe/pipe_radeonsi.so' '/usr/lib/x86_64-linux-gnu/gallium-pipe/pipe_swrast.so' '/usr/lib/x86_64-linux-gnu/gallium-pipe/pipe_vmwgfx.so' '/usr/lib/x86_64-linux-gnu/libomxil-bellagio0/libomx_mesa.so' '/usr/lib/x86_64-linux-gnu/vdpau/libvdpau_nouveau.so.1.0.0' '/usr/lib/x86_64-linux-gnu/vdpau/libvdpau_r300.so.1.0.0' '/usr/lib/x86_64-linux-gnu/vdpau/libvdpau_r600.so.1.0.0' '/usr/lib/x86_64-linux-gnu/vdpau/libvdpau_radeonsi.so.1.0.0' '/usr/lib/x86_64-linux-gnu/libdrm.so.2.4.0' '/usr/lib/x86_64-linux-gnu/libdrm_amdgpu.so.1.0.0' '/usr/lib/x86_64-linux-gnu/libdrm_etnaviv.so.1.0.0' '/usr/lib/x86_64-linux-gnu/libdrm_exynos.so.1.0.0' '/usr/lib/x86_64-linux-gnu/libdrm_freedreno.so.1.0.0' '/usr/lib/x86_64-linux-gnu/libdrm_intel.so.1.0.0' '/usr/lib/x86_64-linux-gnu/libdrm_nouveau.so.2.0.0' '/usr/lib/x86_64-linux-gnu/libdrm_omap.so.1.0.0' '/usr/lib/x86_64-linux-gnu/libdrm_radeon.so.1.0.1' '/usr/lib/x86_64-linux-gnu/libdrm_tegra.so.0.0.0' '/usr/lib/x86_64-linux-gnu/libEGL.so.1.0.0' '/usr/lib/x86_64-linux-gnu/libEGL.so.1.1.0' '/usr/lib/x86_64-linux-gnu/libEGL_mesa.so.0.0.0' '/usr/lib/x86_64-linux-gnu/libgbm.so.1.0.0' '/usr/lib/x86_64-linux-gnu/libGL.so.1.2.0' '/usr/lib/x86_64-linux-gnu/libGL.so.1.7.0' '/usr/lib/x86_64-linux-gnu/libglapi.so.0.0.0' '/usr/lib/x86_64-linux-gnu/libGLESv1_CM.so.1.1.0' '/usr/lib/x86_64-linux-gnu/libGLESv2.so.2.0.0' '/usr/lib/x86_64-linux-gnu/libGLESv2.so.2.1.0' '/usr/lib/x86_64-linux-gnu/libglslang.a' '/usr/lib/x86_64-linux-gnu/libGLU.a' '/usr/lib/x86_64-linux-gnu/libGLU.so.1.3.1' '/usr/lib/x86_64-linux-gnu/libGLX_mesa.so.0.0.0' '/usr/lib/x86_64-linux-gnu/libkms.so.1.0.0' '/usr/lib/x86_64-linux-gnu/libMesaOpenCL.so.1.0.0' '/usr/lib/x86_64-linux-gnu/libOSMesa.so.8.0.0' '/usr/lib/x86_64-linux-gnu/libpng.so.3.50.0' '/usr/lib/x86_64-linux-gnu/libpng12.a' '/usr/lib/x86_64-linux-gnu/libpng12.so.0.50.0' '/usr/lib/x86_64-linux-gnu/libpng16.so.16.37.0' '/usr/lib/x86_64-linux-gnu/libswrAVX.so.0.0.0' '/usr/lib/x86_64-linux-gnu/libswrAVX2.so.0.0.0' '/usr/lib/x86_64-linux-gnu/libVkLayer_MESA_overlay.so' '/usr/lib/x86_64-linux-gnu/libvulkan_intel.so' '/usr/lib/x86_64-linux-gnu/libvulkan_radeon.so' '/usr/lib/x86_64-linux-gnu/libwayland-egl.so.1.0.0' '/usr/lib/x86_64-linux-gnu/libxatracker.so.2.5.0' '/usr/lib/x86_64-linux-gnu/libXvMCnouveau.so' '/usr/lib/x86_64-linux-gnu/libXvMCr600.so' '/usr/include/glm/libglm_shared.so' '/usr/include/glm/libglm_static.a'

Ubuntu 20.04 build mesa-20.2.26_build_20.04.zip inpack readme install

install mesa build replace reinstall original security include | возвращение оригинальных инклюдов что бы было безопаснее пусть корпорации качают инклюды тут потом заплатят за всю сборку инклюдов которые я подобрал чем они будут собирать имея доступ к компьютерам через керберос на ваших компьютерах используя инклюды как хост инклюды они конечно могут сказать что они кристально чисты и никуда не лезут если все выключено и фаирволл , но если у вас останутся именно эти инклюды то вы заметите что компьютер начнет тормозить значат на вас что то собирают удаленно , мне пока не удалось выбить инвестиции что бы собирать именно свою ос по этому пока так. Пока единственный способ сбежать ssh rpc boostrap это создавать в папке темп текстовый фаил ssh и ssh2 и убирать с них все права так же их придется создать в папке рут и домашней в папке tmp придется создать текстовый фаил только уже с точками предварительно всключить показ скрытых фаилов .ssh и .ssh2 либо делать скрипт автозапуска что бы такие фаилы создавал каждый раз либо вручную каждый раз так как оттуда все удаляется , а если будут по честному работать то им придется прийти к тому что у меня самый идеальный вариант операционной системы и находится он тут  https://github.com/Griggorii/Linux_OS20.04_V4_X64_By_Griggorii.iso_ubuntu_focal_fossa-linux-image-kernel-5.9.3 на данныйц момент совпало много интересов разных фирм и все хотят заэсешеичится и сделать бустраповый билд обходя настоящего издателя самой системы и то что люди разбросаны по гуглу , яндексу и другим домаинам уже не ново залезть через жс ссх по этому инклюды скинуты может перестанут так делать и скажут где они оставили себе места для лаза по сговору или не сговору пусть покажут и закроем эти уязвимости вычеркнув их из листа или внеся в блок лист. В старых версиях была такая уязвимость https://www.youtube.com/watch?v=CLwqGce6AGo и еще по моему можно было взломать набрав три четыре раза рандомный пароль щас же рековери защищен и сделать такое может быть и возможно через chroot физически да , а удаленно не известно , но может быть для этого и нужен эсэсаш что бы вбить баш чрут текст и получить уязвимость , так же ранее efi вида либами не было , но тем не менее он ставился в версии 19.10 без либ так что это за библиотеки порождение генерации или специальные тоже не известно по скольку в раздел efi стали падать всякие shm.

Те кто понимает на сколько это огромная работа касаемо инклюдов и в корпорациях получают за такую сборку миллионы долларов , но нету денег можно отблагодарить звездочкой в избранное.

Griggorii@gmail.com




