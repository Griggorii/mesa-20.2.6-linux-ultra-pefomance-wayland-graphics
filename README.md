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

 griggorii@GriggoriiX64:~/\u0420\u0430\u0431\u043e\u0447\u0438\u0439 \u0441\u0442\u043e\u043b
$ glxinfo -v
name of display: :0
display: :0  screen: 0
direct rendering: Yes
server glx vendor string: SGI
server glx version string: 1.4
server glx extensions:
    GLX_ARB_context_flush_control, GLX_ARB_create_context, 
    GLX_ARB_create_context_no_error, GLX_ARB_create_context_profile, 
    GLX_ARB_fbconfig_float, GLX_ARB_framebuffer_sRGB, GLX_ARB_multisample, 
    GLX_EXT_create_context_es2_profile, GLX_EXT_create_context_es_profile, 
    GLX_EXT_fbconfig_packed_float, GLX_EXT_framebuffer_sRGB, 
    GLX_EXT_import_context, GLX_EXT_libglvnd, GLX_EXT_no_config_context, 
    GLX_EXT_texture_from_pixmap, GLX_EXT_visual_info, GLX_EXT_visual_rating, 
    GLX_MESA_copy_sub_buffer, GLX_OML_swap_method, GLX_SGIS_multisample, 
    GLX_SGIX_fbconfig, GLX_SGIX_pbuffer, GLX_SGIX_visual_select_group, 
    GLX_SGI_make_current_read
client glx vendor string: Mesa Project and SGI
client glx version string: 1.4
client glx extensions:
    GLX_ARB_context_flush_control, GLX_ARB_create_context, 
    GLX_ARB_create_context_no_error, GLX_ARB_create_context_profile, 
    GLX_ARB_create_context_robustness, GLX_ARB_fbconfig_float, 
    GLX_ARB_framebuffer_sRGB, GLX_ARB_get_proc_address, GLX_ARB_multisample, 
    GLX_EXT_buffer_age, GLX_EXT_create_context_es2_profile, 
    GLX_EXT_create_context_es_profile, GLX_EXT_fbconfig_packed_float, 
    GLX_EXT_framebuffer_sRGB, GLX_EXT_import_context, 
    GLX_EXT_texture_from_pixmap, GLX_EXT_visual_info, GLX_EXT_visual_rating, 
    GLX_INTEL_swap_event, GLX_MESA_copy_sub_buffer, 
    GLX_MESA_multithread_makecurrent, GLX_MESA_query_renderer, 
    GLX_MESA_swap_control, GLX_OML_swap_method, GLX_OML_sync_control, 
    GLX_SGIS_multisample, GLX_SGIX_fbconfig, GLX_SGIX_pbuffer, 
    GLX_SGIX_visual_select_group, GLX_SGI_make_current_read, 
    GLX_SGI_swap_control, GLX_SGI_video_sync
GLX version: 1.4
GLX extensions:
    GLX_ARB_create_context, GLX_ARB_create_context_no_error, 
    GLX_ARB_create_context_profile, GLX_ARB_fbconfig_float, 
    GLX_ARB_framebuffer_sRGB, GLX_ARB_get_proc_address, GLX_ARB_multisample, 
    GLX_EXT_buffer_age, GLX_EXT_create_context_es2_profile, 
    GLX_EXT_create_context_es_profile, GLX_EXT_fbconfig_packed_float, 
    GLX_EXT_framebuffer_sRGB, GLX_EXT_import_context, 
    GLX_EXT_texture_from_pixmap, GLX_EXT_visual_info, GLX_EXT_visual_rating, 
    GLX_MESA_copy_sub_buffer, GLX_MESA_query_renderer, GLX_MESA_swap_control, 
    GLX_OML_swap_method, GLX_OML_sync_control, GLX_SGIS_multisample, 
    GLX_SGIX_fbconfig, GLX_SGIX_pbuffer, GLX_SGIX_visual_select_group, 
    GLX_SGI_make_current_read, GLX_SGI_video_sync
Extended renderer info (GLX_MESA_query_renderer):
    Vendor: Intel Open Source Technology Center (0x8086)
    Device: Mesa DRI Intel(R) HD Graphics 3000 (SNB GT2) (0x116)
    Version: 20.2.6
    Accelerated: yes
    Video memory: 1536MB
    Unified memory: yes
    Preferred profile: core (0x1)
    Max core profile version: 3.3
    Max compat profile version: 3.0
    Max GLES1 profile version: 1.1
    Max GLES[23] profile version: 3.0
OpenGL vendor string: Intel Open Source Technology Center
OpenGL renderer string: Mesa DRI Intel(R) HD Graphics 3000 (SNB GT2)
OpenGL core profile version string: 3.3 (Core Profile) Mesa 20.2.6
OpenGL core profile shading language version string: 3.30
OpenGL core profile context flags: (none)
OpenGL core profile profile mask: core profile
OpenGL core profile extensions:
    GL_3DFX_texture_compression_FXT1, GL_AMD_draw_buffers_blend, 
    GL_AMD_seamless_cubemap_per_texture, GL_AMD_shader_trinary_minmax, 
    GL_AMD_texture_texture4, GL_AMD_vertex_shader_layer, 
    GL_AMD_vertex_shader_viewport_index, GL_ANGLE_texture_compression_dxt3, 
    GL_ANGLE_texture_compression_dxt5, GL_APPLE_object_purgeable, 
    GL_ARB_ES2_compatibility, GL_ARB_ES3_compatibility, 
    GL_ARB_arrays_of_arrays, GL_ARB_base_instance, GL_ARB_blend_func_extended, 
    GL_ARB_buffer_storage, GL_ARB_clear_buffer_object, GL_ARB_clear_texture, 
    GL_ARB_clip_control, GL_ARB_compressed_texture_pixel_storage, 
    GL_ARB_conditional_render_inverted, GL_ARB_copy_buffer, GL_ARB_copy_image, 
    GL_ARB_cull_distance, GL_ARB_debug_output, GL_ARB_depth_buffer_float, 
    GL_ARB_depth_clamp, GL_ARB_direct_state_access, GL_ARB_draw_buffers, 
    GL_ARB_draw_buffers_blend, GL_ARB_draw_elements_base_vertex, 
    GL_ARB_draw_instanced, GL_ARB_enhanced_layouts, 
    GL_ARB_explicit_attrib_location, GL_ARB_explicit_uniform_location, 
    GL_ARB_fragment_coord_conventions, GL_ARB_fragment_layer_viewport, 
    GL_ARB_fragment_shader, GL_ARB_framebuffer_object, 
    GL_ARB_framebuffer_sRGB, GL_ARB_get_program_binary, 
    GL_ARB_get_texture_sub_image, GL_ARB_half_float_pixel, 
    GL_ARB_half_float_vertex, GL_ARB_instanced_arrays, 
    GL_ARB_internalformat_query, GL_ARB_internalformat_query2, 
    GL_ARB_invalidate_subdata, GL_ARB_map_buffer_alignment, 
    GL_ARB_map_buffer_range, GL_ARB_multi_bind, GL_ARB_occlusion_query2, 
    GL_ARB_parallel_shader_compile, GL_ARB_pipeline_statistics_query, 
    GL_ARB_pixel_buffer_object, GL_ARB_point_sprite, 
    GL_ARB_polygon_offset_clamp, GL_ARB_program_interface_query, 
    GL_ARB_provoking_vertex, GL_ARB_robustness, GL_ARB_sample_shading, 
    GL_ARB_sampler_objects, GL_ARB_seamless_cube_map, 
    GL_ARB_seamless_cubemap_per_texture, GL_ARB_separate_shader_objects, 
    GL_ARB_shader_bit_encoding, GL_ARB_shader_draw_parameters, 
    GL_ARB_shader_group_vote, GL_ARB_shader_objects, GL_ARB_shader_subroutine, 
    GL_ARB_shader_texture_lod, GL_ARB_shader_viewport_layer_array, 
    GL_ARB_shading_language_420pack, GL_ARB_shading_language_include, 
    GL_ARB_shading_language_packing, GL_ARB_sync, GL_ARB_texture_barrier, 
    GL_ARB_texture_buffer_object, GL_ARB_texture_buffer_object_rgb32, 
    GL_ARB_texture_buffer_range, GL_ARB_texture_compression_rgtc, 
    GL_ARB_texture_cube_map_array, GL_ARB_texture_filter_anisotropic, 
    GL_ARB_texture_float, GL_ARB_texture_gather, 
    GL_ARB_texture_mirror_clamp_to_edge, GL_ARB_texture_multisample, 
    GL_ARB_texture_non_power_of_two, GL_ARB_texture_query_levels, 
    GL_ARB_texture_query_lod, GL_ARB_texture_rectangle, GL_ARB_texture_rg, 
    GL_ARB_texture_rgb10_a2ui, GL_ARB_texture_storage, 
    GL_ARB_texture_storage_multisample, GL_ARB_texture_swizzle, 
    GL_ARB_timer_query, GL_ARB_transform_feedback2, 
    GL_ARB_transform_feedback_overflow_query, GL_ARB_uniform_buffer_object, 
    GL_ARB_vertex_array_bgra, GL_ARB_vertex_array_object, 
    GL_ARB_vertex_attrib_binding, GL_ARB_vertex_buffer_object, 
    GL_ARB_vertex_shader, GL_ARB_vertex_type_10f_11f_11f_rev, 
    GL_ARB_vertex_type_2_10_10_10_rev, GL_ARB_viewport_array, 
    GL_ATI_blend_equation_separate, GL_ATI_texture_float, 
    GL_EXT_EGL_image_storage, GL_EXT_EGL_sync, GL_EXT_abgr, 
    GL_EXT_blend_equation_separate, GL_EXT_demote_to_helper_invocation, 
    GL_EXT_draw_buffers2, GL_EXT_draw_instanced, GL_EXT_framebuffer_blit, 
    GL_EXT_framebuffer_multisample, GL_EXT_framebuffer_multisample_blit_scaled, 
    GL_EXT_framebuffer_object, GL_EXT_framebuffer_sRGB, 
    GL_EXT_packed_depth_stencil, GL_EXT_packed_float, 
    GL_EXT_pixel_buffer_object, GL_EXT_polygon_offset_clamp, 
    GL_EXT_provoking_vertex, GL_EXT_shader_framebuffer_fetch_non_coherent, 
    GL_EXT_shader_integer_mix, GL_EXT_texture_array, 
    GL_EXT_texture_compression_dxt1, GL_EXT_texture_compression_rgtc, 
    GL_EXT_texture_compression_s3tc, GL_EXT_texture_filter_anisotropic, 
    GL_EXT_texture_integer, GL_EXT_texture_sRGB, GL_EXT_texture_sRGB_R8, 
    GL_EXT_texture_sRGB_decode, GL_EXT_texture_shadow_lod, 
    GL_EXT_texture_shared_exponent, GL_EXT_texture_snorm, 
    GL_EXT_texture_swizzle, GL_EXT_timer_query, GL_EXT_transform_feedback, 
    GL_EXT_vertex_array_bgra, GL_IBM_multimode_draw_arrays, 
    GL_INTEL_blackhole_render, GL_INTEL_performance_query, 
    GL_KHR_blend_equation_advanced, GL_KHR_context_flush_control, 
    GL_KHR_debug, GL_KHR_no_error, GL_KHR_parallel_shader_compile, 
    GL_KHR_robustness, GL_MESA_pack_invert, GL_MESA_shader_integer_functions, 
    GL_MESA_texture_signed_rgba, GL_NV_conditional_render, GL_NV_depth_clamp, 
    GL_NV_packed_depth_stencil, GL_NV_texture_barrier, GL_OES_EGL_image, 
    GL_S3_s3tc

OpenGL version string: 3.0 Mesa 20.2.6
OpenGL shading language version string: 1.30
OpenGL context flags: (none)
OpenGL extensions:
    GL_3DFX_texture_compression_FXT1, GL_AMD_draw_buffers_blend, 
    GL_AMD_seamless_cubemap_per_texture, GL_AMD_shader_trinary_minmax, 
    GL_AMD_texture_texture4, GL_ANGLE_texture_compression_dxt3, 
    GL_ANGLE_texture_compression_dxt5, GL_APPLE_object_purgeable, 
    GL_APPLE_packed_pixels, GL_ARB_ES2_compatibility, 
    GL_ARB_ES3_compatibility, GL_ARB_arrays_of_arrays, 
    GL_ARB_blend_func_extended, GL_ARB_buffer_storage, 
    GL_ARB_clear_buffer_object, GL_ARB_clear_texture, GL_ARB_clip_control, 
    GL_ARB_color_buffer_float, GL_ARB_compressed_texture_pixel_storage, 
    GL_ARB_conditional_render_inverted, GL_ARB_copy_buffer, GL_ARB_copy_image, 
    GL_ARB_cull_distance, GL_ARB_debug_output, GL_ARB_depth_buffer_float, 
    GL_ARB_depth_clamp, GL_ARB_depth_texture, GL_ARB_draw_buffers, 
    GL_ARB_draw_buffers_blend, GL_ARB_draw_elements_base_vertex, 
    GL_ARB_draw_instanced, GL_ARB_explicit_attrib_location, 
    GL_ARB_explicit_uniform_location, GL_ARB_fragment_coord_conventions, 
    GL_ARB_fragment_layer_viewport, GL_ARB_fragment_program, 
    GL_ARB_fragment_program_shadow, GL_ARB_fragment_shader, 
    GL_ARB_framebuffer_object, GL_ARB_framebuffer_sRGB, 
    GL_ARB_get_program_binary, GL_ARB_get_texture_sub_image, 
    GL_ARB_half_float_pixel, GL_ARB_half_float_vertex, 
    GL_ARB_instanced_arrays, GL_ARB_internalformat_query, 
    GL_ARB_internalformat_query2, GL_ARB_invalidate_subdata, 
    GL_ARB_map_buffer_alignment, GL_ARB_map_buffer_range, GL_ARB_multi_bind, 
    GL_ARB_multisample, GL_ARB_multitexture, GL_ARB_occlusion_query, 
    GL_ARB_occlusion_query2, GL_ARB_parallel_shader_compile, 
    GL_ARB_pipeline_statistics_query, GL_ARB_pixel_buffer_object, 
    GL_ARB_point_parameters, GL_ARB_point_sprite, GL_ARB_polygon_offset_clamp, 
    GL_ARB_program_interface_query, GL_ARB_provoking_vertex, 
    GL_ARB_robustness, GL_ARB_sample_shading, GL_ARB_sampler_objects, 
    GL_ARB_seamless_cube_map, GL_ARB_seamless_cubemap_per_texture, 
    GL_ARB_separate_shader_objects, GL_ARB_shader_bit_encoding, 
    GL_ARB_shader_draw_parameters, GL_ARB_shader_group_vote, 
    GL_ARB_shader_objects, GL_ARB_shader_texture_lod, 
    GL_ARB_shading_language_100, GL_ARB_shading_language_420pack, 
    GL_ARB_shading_language_include, GL_ARB_shading_language_packing, 
    GL_ARB_shadow, GL_ARB_sync, GL_ARB_texture_barrier, 
    GL_ARB_texture_border_clamp, GL_ARB_texture_compression, 
    GL_ARB_texture_compression_rgtc, GL_ARB_texture_cube_map, 
    GL_ARB_texture_cube_map_array, GL_ARB_texture_env_add, 
    GL_ARB_texture_env_combine, GL_ARB_texture_env_crossbar, 
    GL_ARB_texture_env_dot3, GL_ARB_texture_filter_anisotropic, 
    GL_ARB_texture_float, GL_ARB_texture_gather, 
    GL_ARB_texture_mirror_clamp_to_edge, GL_ARB_texture_mirrored_repeat, 
    GL_ARB_texture_multisample, GL_ARB_texture_non_power_of_two, 
    GL_ARB_texture_query_levels, GL_ARB_texture_query_lod, 
    GL_ARB_texture_rectangle, GL_ARB_texture_rg, GL_ARB_texture_rgb10_a2ui, 
    GL_ARB_texture_storage, GL_ARB_texture_storage_multisample, 
    GL_ARB_texture_swizzle, GL_ARB_timer_query, GL_ARB_transform_feedback2, 
    GL_ARB_transform_feedback_overflow_query, GL_ARB_transpose_matrix, 
    GL_ARB_uniform_buffer_object, GL_ARB_vertex_array_bgra, 
    GL_ARB_vertex_array_object, GL_ARB_vertex_attrib_binding, 
    GL_ARB_vertex_buffer_object, GL_ARB_vertex_program, GL_ARB_vertex_shader, 
    GL_ARB_vertex_type_10f_11f_11f_rev, GL_ARB_vertex_type_2_10_10_10_rev, 
    GL_ARB_window_pos, GL_ATI_blend_equation_separate, GL_ATI_draw_buffers, 
    GL_ATI_separate_stencil, GL_ATI_texture_env_combine3, 
    GL_ATI_texture_float, GL_EXT_EGL_image_storage, GL_EXT_EGL_sync, 
    GL_EXT_abgr, GL_EXT_bgra, GL_EXT_blend_color, 
    GL_EXT_blend_equation_separate, GL_EXT_blend_func_separate, 
    GL_EXT_blend_minmax, GL_EXT_blend_subtract, GL_EXT_compiled_vertex_array, 
    GL_EXT_copy_texture, GL_EXT_demote_to_helper_invocation, 
    GL_EXT_direct_state_access, GL_EXT_draw_buffers2, GL_EXT_draw_instanced, 
    GL_EXT_draw_range_elements, GL_EXT_fog_coord, GL_EXT_framebuffer_blit, 
    GL_EXT_framebuffer_multisample, GL_EXT_framebuffer_multisample_blit_scaled, 
    GL_EXT_framebuffer_object, GL_EXT_framebuffer_sRGB, 
    GL_EXT_gpu_program_parameters, GL_EXT_gpu_shader4, 
    GL_EXT_multi_draw_arrays, GL_EXT_packed_depth_stencil, 
    GL_EXT_packed_float, GL_EXT_packed_pixels, GL_EXT_pixel_buffer_object, 
    GL_EXT_point_parameters, GL_EXT_polygon_offset_clamp, 
    GL_EXT_provoking_vertex, GL_EXT_rescale_normal, GL_EXT_secondary_color, 
    GL_EXT_separate_specular_color, 
    GL_EXT_shader_framebuffer_fetch_non_coherent, GL_EXT_shader_integer_mix, 
    GL_EXT_shadow_funcs, GL_EXT_stencil_two_side, GL_EXT_stencil_wrap, 
    GL_EXT_subtexture, GL_EXT_texture, GL_EXT_texture3D, 
    GL_EXT_texture_array, GL_EXT_texture_compression_dxt1, 
    GL_EXT_texture_compression_rgtc, GL_EXT_texture_compression_s3tc, 
    GL_EXT_texture_cube_map, GL_EXT_texture_edge_clamp, 
    GL_EXT_texture_env_add, GL_EXT_texture_env_combine, 
    GL_EXT_texture_env_dot3, GL_EXT_texture_filter_anisotropic, 
    GL_EXT_texture_integer, GL_EXT_texture_lod_bias, GL_EXT_texture_object, 
    GL_EXT_texture_rectangle, GL_EXT_texture_sRGB, GL_EXT_texture_sRGB_R8, 
    GL_EXT_texture_sRGB_decode, GL_EXT_texture_shadow_lod, 
    GL_EXT_texture_shared_exponent, GL_EXT_texture_snorm, 
    GL_EXT_texture_swizzle, GL_EXT_timer_query, GL_EXT_transform_feedback, 
    GL_EXT_vertex_array, GL_EXT_vertex_array_bgra, 
    GL_IBM_multimode_draw_arrays, GL_IBM_rasterpos_clip, 
    GL_IBM_texture_mirrored_repeat, GL_INGR_blend_func_separate, 
    GL_INTEL_blackhole_render, GL_INTEL_performance_query, 
    GL_KHR_blend_equation_advanced, GL_KHR_context_flush_control, 
    GL_KHR_debug, GL_KHR_no_error, GL_KHR_parallel_shader_compile, 
    GL_KHR_robustness, GL_MESA_pack_invert, GL_MESA_shader_integer_functions, 
    GL_MESA_texture_signed_rgba, GL_MESA_window_pos, GL_NV_blend_square, 
    GL_NV_conditional_render, GL_NV_depth_clamp, GL_NV_fog_distance, 
    GL_NV_light_max_exponent, GL_NV_packed_depth_stencil, 
    GL_NV_primitive_restart, GL_NV_texgen_reflection, GL_NV_texture_barrier, 
    GL_NV_texture_env_combine4, GL_NV_texture_rectangle, GL_OES_EGL_image, 
    GL_OES_read_format, GL_S3_s3tc, GL_SGIS_generate_mipmap, 
    GL_SGIS_texture_border_clamp, GL_SGIS_texture_edge_clamp, 
    GL_SGIS_texture_lod, GL_SUN_multi_draw_arrays

OpenGL ES profile version string: OpenGL ES 3.0 Mesa 20.2.6
OpenGL ES profile shading language version string: OpenGL ES GLSL ES 3.00
OpenGL ES profile extensions:
    GL_ANGLE_texture_compression_dxt3, GL_ANGLE_texture_compression_dxt5, 
    GL_APPLE_texture_max_level, GL_EXT_EGL_image_storage, 
    GL_EXT_base_instance, GL_EXT_blend_func_extended, GL_EXT_blend_minmax, 
    GL_EXT_clip_control, GL_EXT_clip_cull_distance, GL_EXT_color_buffer_float, 
    GL_EXT_compressed_ETC1_RGB8_sub_texture, 
    GL_EXT_demote_to_helper_invocation, GL_EXT_depth_clamp, 
    GL_EXT_discard_framebuffer, GL_EXT_disjoint_timer_query, 
    GL_EXT_draw_buffers, GL_EXT_draw_buffers_indexed, 
    GL_EXT_draw_elements_base_vertex, GL_EXT_draw_instanced, 
    GL_EXT_float_blend, GL_EXT_frag_depth, GL_EXT_map_buffer_range, 
    GL_EXT_multi_draw_arrays, GL_EXT_occlusion_query_boolean, 
    GL_EXT_polygon_offset_clamp, GL_EXT_read_format_bgra, GL_EXT_robustness, 
    GL_EXT_sRGB_write_control, GL_EXT_separate_shader_objects, 
    GL_EXT_shader_framebuffer_fetch_non_coherent, GL_EXT_shader_group_vote, 
    GL_EXT_shader_integer_mix, GL_EXT_texture_border_clamp, 
    GL_EXT_texture_compression_dxt1, GL_EXT_texture_compression_rgtc, 
    GL_EXT_texture_compression_s3tc, GL_EXT_texture_compression_s3tc_srgb, 
    GL_EXT_texture_filter_anisotropic, GL_EXT_texture_format_BGRA8888, 
    GL_EXT_texture_query_lod, GL_EXT_texture_rg, GL_EXT_texture_sRGB_R8, 
    GL_EXT_texture_sRGB_decode, GL_EXT_texture_shadow_lod, 
    GL_EXT_texture_type_2_10_10_10_REV, GL_EXT_unpack_subimage, 
    GL_INTEL_blackhole_render, GL_INTEL_performance_query, 
    GL_KHR_blend_equation_advanced, GL_KHR_context_flush_control, 
    GL_KHR_debug, GL_KHR_no_error, GL_KHR_parallel_shader_compile, 
    GL_KHR_robustness, GL_MESA_framebuffer_flip_y, 
    GL_MESA_shader_integer_functions, GL_NV_conditional_render, 
    GL_NV_draw_buffers, GL_NV_fbo_color_attachments, 
    GL_NV_pixel_buffer_object, GL_NV_read_buffer, GL_NV_read_depth, 
    GL_NV_read_depth_stencil, GL_NV_read_stencil, GL_OES_EGL_image, 
    GL_OES_EGL_image_external, GL_OES_EGL_image_external_essl3, 
    GL_OES_EGL_sync, GL_OES_compressed_ETC1_RGB8_texture, GL_OES_depth24, 
    GL_OES_depth_texture, GL_OES_depth_texture_cube_map, 
    GL_OES_draw_buffers_indexed, GL_OES_draw_elements_base_vertex, 
    GL_OES_element_index_uint, GL_OES_fbo_render_mipmap, 
    GL_OES_get_program_binary, GL_OES_mapbuffer, GL_OES_packed_depth_stencil, 
    GL_OES_required_internalformat, GL_OES_rgb8_rgba8, GL_OES_sample_shading, 
    GL_OES_sample_variables, GL_OES_shader_multisample_interpolation, 
    GL_OES_standard_derivatives, GL_OES_stencil8, GL_OES_surfaceless_context, 
    GL_OES_texture_3D, GL_OES_texture_border_clamp, GL_OES_texture_float, 
    GL_OES_texture_float_linear, GL_OES_texture_half_float, 
    GL_OES_texture_half_float_linear, GL_OES_texture_npot, 
    GL_OES_vertex_array_object, GL_OES_vertex_half_float

108 GLX Visuals
Visual ID: 24  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 25  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 39e  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 3a0  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 3a2  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 3b0  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 3b2  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=16 greenSize=16 blueSize=16 alphaSize=16
    multiSample=0  multiSampleBuffers=0
    visualCaveat=Slow
    Opaque.
Visual ID: 3b3  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 3b4  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=16 greenSize=16 blueSize=16 alphaSize=16
    multiSample=0  multiSampleBuffers=0
    visualCaveat=Slow
    Opaque.
Visual ID: 3bc  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
Visual ID: 3bd  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
Visual ID: 3c5  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
Visual ID: 3c6  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
Visual ID: 3ca  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 3cc  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 3ce  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 3dc  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 3de  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 3df  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=16 greenSize=16 blueSize=16 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=Slow
    Opaque.
Visual ID: 3e0  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 3e1  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=16 greenSize=16 blueSize=16 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=Slow
    Opaque.
Visual ID: 3e9  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
Visual ID: 3ea  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
Visual ID: 3f2  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
Visual ID: 3f3  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
Visual ID: 3f7  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 3f9  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 3fb  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 409  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 40b  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 40c  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=16 greenSize=16 blueSize=16 alphaSize=16
    multiSample=0  multiSampleBuffers=0
    visualCaveat=Slow
    Opaque.
Visual ID: 40d  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 40e  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=16 greenSize=16 blueSize=16 alphaSize=16
    multiSample=0  multiSampleBuffers=0
    visualCaveat=Slow
    Opaque.
Visual ID: 416  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
Visual ID: 417  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
Visual ID: 41f  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
Visual ID: 420  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
Visual ID: 424  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 426  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 428  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 436  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 438  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 439  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=16 greenSize=16 blueSize=16 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=Slow
    Opaque.
Visual ID: 43a  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 43b  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=16 greenSize=16 blueSize=16 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=Slow
    Opaque.
Visual ID: 443  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
Visual ID: 444  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
Visual ID: 44c  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
Visual ID: 44d  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
Visual ID: 451  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 453  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 455  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 463  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 465  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=16 greenSize=16 blueSize=16 alphaSize=16
    multiSample=0  multiSampleBuffers=0
    visualCaveat=Slow
    Opaque.
Visual ID: 466  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 467  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=16 greenSize=16 blueSize=16 alphaSize=16
    multiSample=0  multiSampleBuffers=0
    visualCaveat=Slow
    Opaque.
Visual ID: 46f  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
Visual ID: 470  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
Visual ID: 478  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
Visual ID: 479  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
Visual ID: 47d  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 47f  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 481  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 48f  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 491  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 492  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=16 greenSize=16 blueSize=16 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=Slow
    Opaque.
Visual ID: 493  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 494  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=16 greenSize=16 blueSize=16 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=Slow
    Opaque.
Visual ID: 49c  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
Visual ID: 49d  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
Visual ID: 4a5  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
Visual ID: 4a6  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
Visual ID: 4aa  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 4ac  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 4ae  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 4bc  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 4be  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 4bf  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=16 greenSize=16 blueSize=16 alphaSize=16
    multiSample=0  multiSampleBuffers=0
    visualCaveat=Slow
    Opaque.
Visual ID: 4c0  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 4c1  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=16 greenSize=16 blueSize=16 alphaSize=16
    multiSample=0  multiSampleBuffers=0
    visualCaveat=Slow
    Opaque.
Visual ID: 4c9  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
Visual ID: 4ca  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
Visual ID: 4d2  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
Visual ID: 4d3  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
Visual ID: 4d7  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 4d9  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 4db  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 4e9  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 4eb  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 4ec  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=16 greenSize=16 blueSize=16 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=Slow
    Opaque.
Visual ID: 4ed  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 4ee  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=16 greenSize=16 blueSize=16 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=Slow
    Opaque.
Visual ID: 4f6  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
Visual ID: 4f7  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
Visual ID: 4ff  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
Visual ID: 500  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
Visual ID: 55  depth=32  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 504  depth=32  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 505  depth=32  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 506  depth=32  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 50d  depth=32  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 50e  depth=32  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 512  depth=32  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 513  depth=32  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 514  depth=32  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 51b  depth=32  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 51c  depth=32  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
Visual ID: 51d  depth=32  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.

78 GLXFBConfigs:
FBConfig ID: 10a  Visual ID=39e  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 10c  Visual ID=3a0  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 11c  Visual ID=3b0  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 11e  Visual ID=24  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 11f  Visual ID=3b2  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=16 greenSize=16 blueSize=16 alphaSize=16
    multiSample=0  multiSampleBuffers=0
    visualCaveat=Slow
    Opaque.
FBConfig ID: 129  Visual ID=3bc  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
FBConfig ID: 132  Visual ID=3c5  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
FBConfig ID: 137  Visual ID=3ca  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 139  Visual ID=3cc  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 149  Visual ID=3dc  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 14b  Visual ID=3de  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 14c  Visual ID=3df  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=16 greenSize=16 blueSize=16 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=Slow
    Opaque.
FBConfig ID: 156  Visual ID=3e9  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
FBConfig ID: 15f  Visual ID=3f2  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
FBConfig ID: 164  Visual ID=3f7  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 166  Visual ID=3f9  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 176  Visual ID=409  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 178  Visual ID=40b  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 179  Visual ID=40c  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=16 greenSize=16 blueSize=16 alphaSize=16
    multiSample=0  multiSampleBuffers=0
    visualCaveat=Slow
    Opaque.
FBConfig ID: 183  Visual ID=416  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
FBConfig ID: 18c  Visual ID=41f  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
FBConfig ID: 191  Visual ID=424  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 193  Visual ID=426  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 1a3  Visual ID=436  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 1a5  Visual ID=438  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 1a6  Visual ID=439  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=16 greenSize=16 blueSize=16 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=Slow
    Opaque.
FBConfig ID: 1b0  Visual ID=443  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
FBConfig ID: 1b9  Visual ID=44c  depth=24  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
FBConfig ID: 1be  Visual ID=0  depth=0  class=TrueColor, type=pixmap,pbuffer
    bufferSize=16 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=5 greenSize=6 blueSize=5 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 1c0  Visual ID=0  depth=0  class=TrueColor, type=pixmap,pbuffer
    bufferSize=16 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=5 greenSize=6 blueSize=5 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 1d0  Visual ID=0  depth=0  class=TrueColor, type=pixmap,pbuffer
    bufferSize=16 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=5 greenSize=6 blueSize=5 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 1d2  Visual ID=0  depth=0  class=TrueColor, type=pixmap,pbuffer
    bufferSize=16 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=5 greenSize=6 blueSize=5 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 1d3  Visual ID=0  depth=0  class=TrueColor, type=pixmap,pbuffer
    bufferSize=16 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=5 greenSize=6 blueSize=5 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=16 greenSize=16 blueSize=16 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=Slow
    Opaque.
FBConfig ID: 1dd  Visual ID=0  depth=0  class=TrueColor, type=pixmap,pbuffer
    bufferSize=16 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=5 greenSize=6 blueSize=5 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
FBConfig ID: 1e6  Visual ID=0  depth=0  class=TrueColor, type=pixmap,pbuffer
    bufferSize=16 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=5 greenSize=6 blueSize=5 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
FBConfig ID: 29f  Visual ID=451  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 2a1  Visual ID=453  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 2b1  Visual ID=463  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 2b3  Visual ID=25  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 2b4  Visual ID=465  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=16 greenSize=16 blueSize=16 alphaSize=16
    multiSample=0  multiSampleBuffers=0
    visualCaveat=Slow
    Opaque.
FBConfig ID: 2be  Visual ID=46f  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
FBConfig ID: 2c7  Visual ID=478  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
FBConfig ID: 2cc  Visual ID=47d  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 2ce  Visual ID=47f  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 2de  Visual ID=48f  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 2e0  Visual ID=491  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 2e1  Visual ID=492  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=16 greenSize=16 blueSize=16 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=Slow
    Opaque.
FBConfig ID: 2eb  Visual ID=49c  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
FBConfig ID: 2f4  Visual ID=4a5  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
FBConfig ID: 2f9  Visual ID=4aa  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 2fb  Visual ID=4ac  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 30b  Visual ID=4bc  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 30d  Visual ID=4be  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 30e  Visual ID=4bf  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=16 greenSize=16 blueSize=16 alphaSize=16
    multiSample=0  multiSampleBuffers=0
    visualCaveat=Slow
    Opaque.
FBConfig ID: 318  Visual ID=4c9  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
FBConfig ID: 321  Visual ID=4d2  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
FBConfig ID: 326  Visual ID=4d7  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 328  Visual ID=4d9  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 338  Visual ID=4e9  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 33a  Visual ID=4eb  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 33b  Visual ID=4ec  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=16 greenSize=16 blueSize=16 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=Slow
    Opaque.
FBConfig ID: 345  Visual ID=4f6  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
FBConfig ID: 34e  Visual ID=4ff  depth=24  class=DirectColor, type=window,pixmap,pbuffer
    bufferSize=24 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=0 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
FBConfig ID: 353  Visual ID=0  depth=0  class=DirectColor, type=pixmap,pbuffer
    bufferSize=16 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=5 greenSize=6 blueSize=5 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 355  Visual ID=0  depth=0  class=DirectColor, type=pixmap,pbuffer
    bufferSize=16 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=5 greenSize=6 blueSize=5 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 365  Visual ID=0  depth=0  class=DirectColor, type=pixmap,pbuffer
    bufferSize=16 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=5 greenSize=6 blueSize=5 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 367  Visual ID=0  depth=0  class=DirectColor, type=pixmap,pbuffer
    bufferSize=16 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=5 greenSize=6 blueSize=5 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 368  Visual ID=0  depth=0  class=DirectColor, type=pixmap,pbuffer
    bufferSize=16 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=5 greenSize=6 blueSize=5 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=16 greenSize=16 blueSize=16 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=Slow
    Opaque.
FBConfig ID: 372  Visual ID=0  depth=0  class=DirectColor, type=pixmap,pbuffer
    bufferSize=16 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=5 greenSize=6 blueSize=5 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
FBConfig ID: 37b  Visual ID=0  depth=0  class=DirectColor, type=pixmap,pbuffer
    bufferSize=16 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=5 greenSize=6 blueSize=5 alphaSize=0 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=4  multiSampleBuffers=1
    visualCaveat=None
    Opaque.
FBConfig ID: 380  Visual ID=504  depth=32  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 381  Visual ID=505  depth=32  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 389  Visual ID=50d  depth=32  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 38a  Visual ID=55  depth=32  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=N
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 38f  Visual ID=512  depth=32  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 390  Visual ID=513  depth=32  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=0 stencilSize=0
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 398  Visual ID=51b  depth=32  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=0 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.
FBConfig ID: 399  Visual ID=51c  depth=32  class=TrueColor, type=window,pixmap,pbuffer
    bufferSize=32 level=0 renderType=rgba doubleBuffer=1 stereo=0
    rgba: redSize=8 greenSize=8 blueSize=8 alphaSize=8 float=N sRGB=Y
    auxBuffers=0 depthSize=24 stencilSize=8
    accum: redSize=0 greenSize=0 blueSize=0 alphaSize=0
    multiSample=0  multiSampleBuffers=0
    visualCaveat=None
    Opaque.


[HKEY_LOCAL_MACHINE\System\CurrentControlSet\Enum\PCI\VEN_0000&DEV_0000&SUBSYS_00000000&REV_00\00000000]
"Class"="Display"
"ClassGUID"="{4D36E968-E325-11CE-BFC1-08002BE10318}"
"DeviceDesc"="Griggorii_mesa_modification"
"Driver"="{4D36E968-E325-11CE-BFC1-08002BE10318}\\0000"
"HardwareID"=hex(7):50,00,43,00,49,00,5c,00,56,00,45,00,4e,00,5f,00,30,00,30,\
  00,30,00,30,00,26,00,44,00,45,00,56,00,5f,00,30,00,30,00,30,00,30,00,26,00,\
  53,00,55,00,42,00,53,00,59,00,53,00,5f,00,30,00,30,00,30,00,30,00,30,00,30,\
  00,30,00,30,00,26,00,52,00,45,00,56,00,5f,00,30,00,30,00,00,00,00,00

Griggorii@gmail.com




