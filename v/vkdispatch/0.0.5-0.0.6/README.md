# Comparing `tmp/vkdispatch-0.0.5.tar.gz` & `tmp/vkdispatch-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vkdispatch-0.0.5.tar", last modified: Sat May  4 16:17:47 2024, max compression
+gzip compressed data, was "vkdispatch-0.0.6.tar", last modified: Tue May  7 06:43:37 2024, max compression
```

## Comparing `vkdispatch-0.0.5.tar` & `vkdispatch-0.0.6.tar`

### file list

```diff
@@ -1,373 +1,376 @@
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.306294 vkdispatch-0.0.5/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    11357 2024-05-04 03:04:33.000000 vkdispatch-0.0.5/LICENSE
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      764 2024-05-04 05:34:22.000000 vkdispatch-0.0.5/MANIFEST.in
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      809 2024-05-04 16:17:47.306048 vkdispatch-0.0.5/PKG-INFO
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      121 2024-05-04 03:04:33.000000 vkdispatch-0.0.5/README.md
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.197155 vkdispatch-0.0.5/deps/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.197002 vkdispatch-0.0.5/deps/VKL/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.196314 vkdispatch-0.0.5/deps/VKL/deps/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.202333 vkdispatch-0.0.5/deps/VKL/deps/VMA/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1099 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VKL/deps/VMA/LICENSE.txt
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.202621 vkdispatch-0.0.5/deps/VKL/deps/VMA/include/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)   711190 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VKL/deps/VMA/include/vk_mem_alloc.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.204478 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      458 2024-05-04 05:19:24.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/LICENSE.md
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.189254 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.206770 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vk_video/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    16507 2024-05-04 05:19:24.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_av1std.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4250 2024-05-04 05:19:24.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_av1std_decode.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    13853 2024-05-04 05:19:24.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_h264std.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2722 2024-05-04 05:19:24.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_h264std_decode.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6878 2024-05-04 05:19:24.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_h264std_encode.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    23416 2024-05-04 05:19:24.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_h265std.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2428 2024-05-04 05:19:24.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_h265std_decode.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7462 2024-05-04 05:19:24.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_h265std_encode.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      660 2024-05-04 05:19:24.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codecs_common.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.211777 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     8164 2024-05-04 05:19:24.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vk_icd.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7073 2024-05-04 05:19:24.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vk_layer.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2828 2024-05-04 05:19:24.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vk_platform.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1555 2024-05-04 05:19:24.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6201 2024-05-04 05:19:24.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_android.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    10381 2024-05-04 05:19:24.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_beta.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)  1000714 2024-05-04 05:19:24.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_core.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1866 2024-05-04 05:19:24.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_directfb.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12470 2024-05-04 05:19:24.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_fuchsia.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1896 2024-05-04 05:19:24.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_ggp.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1309 2024-05-04 05:19:24.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_ios.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1341 2024-05-04 05:19:24.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_macos.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5907 2024-05-04 05:19:24.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_metal.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4064 2024-05-04 05:19:24.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_screen.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1282 2024-05-04 05:19:24.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_vi.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1866 2024-05-04 05:19:24.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_wayland.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    15112 2024-05-04 05:19:24.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_win32.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1880 2024-05-04 05:19:24.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_xcb.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1861 2024-05-04 05:19:24.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_xlib.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1411 2024-05-04 05:19:24.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_xlib_xrandr.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.211887 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Utility-Libraries/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      304 2024-05-04 05:33:49.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Utility-Libraries/LICENSE.md
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.189414 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Utility-Libraries/include/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.211996 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Utility-Libraries/include/vulkan/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.212780 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Utility-Libraries/include/vulkan/layer/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3565 2024-05-04 05:33:49.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Utility-Libraries/include/vulkan/layer/vk_layer_settings.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.213196 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Utility-Libraries/include/vulkan/utility/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)   129114 2024-05-04 05:33:49.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Utility-Libraries/include/vulkan/utility/vk_dispatch_table.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)   144058 2024-05-04 05:33:49.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Utility-Libraries/include/vulkan/utility/vk_format_utils.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)   495518 2024-05-04 05:33:49.000000 vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Utility-Libraries/include/vulkan/vk_enum_string_helper.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.213491 vkdispatch-0.0.5/deps/VKL/deps/glslang/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    54705 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/LICENSE.txt
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.220521 vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.220696 vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/CInterface/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4254 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/CInterface/spirv_c_interface.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3616 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/GLSL.ext.AMD.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1598 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/GLSL.ext.ARM.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2585 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/GLSL.ext.EXT.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4486 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/GLSL.ext.KHR.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3781 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/GLSL.ext.NV.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1808 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/GLSL.ext.QCOM.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4126 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/GLSL.std.450.h
--rwxr-xr-x   0 shaharsandhaus   (501) staff       (20)   461067 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/GlslangToSpv.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2666 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/GlslangToSpv.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5747 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/InReadableOrder.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2731 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/Logger.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2685 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/Logger.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1858 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/NonSemanticDebugPrintf.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7908 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/NonSemanticShaderDebugInfo100.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    11638 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/SPVRemapper.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)   152756 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/SpvBuilder.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    45577 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/SpvBuilder.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    21678 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/SpvPostProcess.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12426 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/SpvTools.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4677 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/SpvTools.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3316 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/bitutils.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    35712 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/disassemble.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1926 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/disassemble.h
--rwxr-xr-x   0 shaharsandhaus   (501) staff       (20)   195172 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/doc.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     8080 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/doc.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    39345 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/hex_float.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)   140795 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/spirv.hpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    19791 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/spvIR.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.220997 vkdispatch-0.0.5/deps/VKL/deps/glslang/StandAlone/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5782 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/StandAlone/DirStackFileIncluder.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2821 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/StandAlone/Worklist.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.221564 vkdispatch-0.0.5/deps/VKL/deps/glslang/Test/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       11 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/Test/bar.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       30 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/Test/foo.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       24 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/Test/i1.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.221997 vkdispatch-0.0.5/deps/VKL/deps/glslang/Test/inc1/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       21 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/Test/inc1/badInc.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       29 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/Test/inc1/bar.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       32 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/Test/inc1/foo.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.222497 vkdispatch-0.0.5/deps/VKL/deps/glslang/Test/inc1/path1/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       14 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/Test/inc1/path1/bar.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       11 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/Test/inc1/path1/local.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       51 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/Test/inc1/path1/notHere.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.222943 vkdispatch-0.0.5/deps/VKL/deps/glslang/Test/inc1/path2/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       14 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/Test/inc1/path2/bar.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       15 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/Test/inc1/path2/notHere.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       11 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/Test/inc1/path2/remote.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.223235 vkdispatch-0.0.5/deps/VKL/deps/glslang/Test/inc2/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       28 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/Test/inc2/bar.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       11 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/Test/inc2/foo.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       11 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/Test/parent.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.195999 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.223389 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/CInterface/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    16918 2024-05-04 04:47:39.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/CInterface/glslang_c_interface.cpp
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.223754 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/GenericCodeGen/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2607 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/GenericCodeGen/CodeGen.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2750 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/GenericCodeGen/Link.cpp
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.231466 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/HLSL/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2132 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/HLSL/hlslAttributes.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6781 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/HLSL/hlslGrammar.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2327 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/HLSL/hlslOpMap.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    28652 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/HLSL/hlslParseHelper.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2622 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/HLSL/hlslParseables.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3560 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/HLSL/hlslScanContext.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3856 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/HLSL/hlslTokenStream.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     9628 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/HLSL/hlslTokens.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1996 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/HLSL/pch.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.236317 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Include/
--rwxr-xr-x   0 shaharsandhaus   (501) staff       (20)    21618 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Include/BaseTypes.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     9241 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Include/Common.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    35998 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Include/ConstantUnion.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5927 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Include/InfoSink.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1854 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Include/InitializeGlobals.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    11856 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Include/PoolAlloc.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5664 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Include/ResourceLimits.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6312 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Include/ShHandle.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4413 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Include/SpirvIntrinsics.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)   109017 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Include/Types.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12025 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Include/arrays.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    11752 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Include/glslang_c_interface.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     9017 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Include/glslang_c_shader_types.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    61736 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Include/intermediate.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.260033 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    61113 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/Constant.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3142 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/InfoSink.cpp
--rwxr-xr-x   0 shaharsandhaus   (501) staff       (20)   562823 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/Initialize.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5491 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/Initialize.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     8084 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/IntermTraverse.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)   139980 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/Intermediate.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6435 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/LiveTraverser.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    27638 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/ParseContextBase.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)   481062 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/ParseHelper.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    33022 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/ParseHelper.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     9110 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/PoolAlloc.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3121 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/RemoveTree.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1704 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/RemoveTree.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    76508 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/Scan.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     9697 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/Scan.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3206 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/ScanContext.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    83435 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/ShaderLang.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12826 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/SpirvIntrinsics.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    17198 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/SymbolTable.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    36832 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/SymbolTable.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    69599 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/Versions.cpp
--rwxr-xr-x   0 shaharsandhaus   (501) staff       (20)    25529 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/Versions.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12678 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/attribute.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4554 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/attribute.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    10171 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/gl_types.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)   654870 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/glslang_tab.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    28552 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/glslang_tab.cpp.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    94894 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/intermOut.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    76316 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/iomapper.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    14491 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/iomapper.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6408 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/limits.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)   109336 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/linkValidate.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    53321 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/localintermediate.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7568 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/parseConst.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    10098 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/parseVersions.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1896 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/pch.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.268781 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    50129 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/Pp.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6672 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/PpAtom.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5211 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/PpContext.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    27894 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/PpContext.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    57222 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/PpScanner.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7488 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/PpTokens.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5791 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/PpTokens.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    40778 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/propagateNoContraction.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2417 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/propagateNoContraction.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    56404 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/reflection.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     8171 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/reflection.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3346 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/span.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.268941 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/OSDependent/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1751 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/OSDependent/osinclude.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.269419 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Public/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2438 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Public/ResourceLimits.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    43942 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Public/ShaderLang.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2295 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Public/resource_limits_c.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.269702 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/ResourceLimits/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    34391 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/ResourceLimits/ResourceLimits.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2145 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/ResourceLimits/resource_limits_c.cpp
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.272782 vkdispatch-0.0.5/deps/VKL/deps/glslang/gtests/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2130 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/gtests/Initializer.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2142 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/gtests/Settings.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    32978 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/gtests/TestFixture.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1678 2024-05-04 04:29:15.000000 vkdispatch-0.0.5/deps/VKL/deps/glslang/gtests/pch.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.196421 vkdispatch-0.0.5/deps/VKL/deps/volk/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.274946 vkdispatch-0.0.5/deps/VKL/deps/volk/volk/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1066 2024-05-04 03:43:54.000000 vkdispatch-0.0.5/deps/VKL/deps/volk/volk/LICENSE.md
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)   252357 2024-05-04 03:43:54.000000 vkdispatch-0.0.5/deps/VKL/deps/volk/volk/volk.c
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)   127213 2024-05-04 03:43:54.000000 vkdispatch-0.0.5/deps/VKL/deps/volk/volk/volk.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.196852 vkdispatch-0.0.5/deps/VKL/include/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.277932 vkdispatch-0.0.5/deps/VKL/include/VKL/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      553 2024-05-04 03:04:57.000000 vkdispatch-0.0.5/deps/VKL/include/VKL/VKL.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1937 2024-05-04 03:04:57.000000 vkdispatch-0.0.5/deps/VKL/include/VKL/VKLBuffer.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2741 2024-05-04 03:04:57.000000 vkdispatch-0.0.5/deps/VKL/include/VKL/VKLCommandBuffer.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      829 2024-05-04 03:04:57.000000 vkdispatch-0.0.5/deps/VKL/include/VKL/VKLDescriptorSet.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     8377 2024-05-04 03:04:57.000000 vkdispatch-0.0.5/deps/VKL/include/VKL/VKLDevice.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1384 2024-05-04 03:04:57.000000 vkdispatch-0.0.5/deps/VKL/include/VKL/VKLFramebuffer.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2938 2024-05-04 03:04:57.000000 vkdispatch-0.0.5/deps/VKL/include/VKL/VKLImage.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      834 2024-05-04 03:04:57.000000 vkdispatch-0.0.5/deps/VKL/include/VKL/VKLImageView.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4176 2024-05-04 03:41:07.000000 vkdispatch-0.0.5/deps/VKL/include/VKL/VKLInstance.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1859 2024-05-04 03:04:57.000000 vkdispatch-0.0.5/deps/VKL/include/VKL/VKLPhysicalDevice.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2240 2024-05-04 03:04:57.000000 vkdispatch-0.0.5/deps/VKL/include/VKL/VKLPipeline.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2984 2024-05-04 03:04:57.000000 vkdispatch-0.0.5/deps/VKL/include/VKL/VKLPipelineLayout.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1077 2024-05-04 03:04:57.000000 vkdispatch-0.0.5/deps/VKL/include/VKL/VKLQueue.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3570 2024-05-04 03:04:57.000000 vkdispatch-0.0.5/deps/VKL/include/VKL/VKLRenderPass.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      671 2024-05-04 03:04:57.000000 vkdispatch-0.0.5/deps/VKL/include/VKL/VKLStaticAllocator.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1790 2024-05-04 03:04:57.000000 vkdispatch-0.0.5/deps/VKL/include/VKL/VKLSurface.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1628 2024-05-04 03:04:57.000000 vkdispatch-0.0.5/deps/VKL/include/VKL/VKLSwapChain.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4305 2024-05-04 04:04:13.000000 vkdispatch-0.0.5/deps/VKL/include/VKL/VKL_base.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.278105 vkdispatch-0.0.5/deps/VKL/include/glslang/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2895 2024-05-04 05:27:42.000000 vkdispatch-0.0.5/deps/VKL/include/glslang/build_info.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.285851 vkdispatch-0.0.5/deps/VKL/src/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7536 2024-05-04 03:04:57.000000 vkdispatch-0.0.5/deps/VKL/src/VKLBuffer.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7748 2024-05-04 03:04:57.000000 vkdispatch-0.0.5/deps/VKL/src/VKLCommandBuffer.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3646 2024-05-04 03:04:57.000000 vkdispatch-0.0.5/deps/VKL/src/VKLDescriptorSet.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    25947 2024-05-04 04:01:54.000000 vkdispatch-0.0.5/deps/VKL/src/VKLDevice.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3322 2024-05-04 03:04:57.000000 vkdispatch-0.0.5/deps/VKL/src/VKLFramebuffer.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    16236 2024-05-04 03:04:57.000000 vkdispatch-0.0.5/deps/VKL/src/VKLImage.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2433 2024-05-04 03:04:57.000000 vkdispatch-0.0.5/deps/VKL/src/VKLImageView.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    14379 2024-05-04 03:41:46.000000 vkdispatch-0.0.5/deps/VKL/src/VKLInstance.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4502 2024-05-04 03:29:09.000000 vkdispatch-0.0.5/deps/VKL/src/VKLPhysicalDevice.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12903 2024-05-04 03:04:57.000000 vkdispatch-0.0.5/deps/VKL/src/VKLPipeline.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12997 2024-05-04 03:04:57.000000 vkdispatch-0.0.5/deps/VKL/src/VKLPipelineLayout.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2167 2024-05-04 03:04:57.000000 vkdispatch-0.0.5/deps/VKL/src/VKLQueue.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6916 2024-05-04 03:04:57.000000 vkdispatch-0.0.5/deps/VKL/src/VKLRenderPass.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3383 2024-05-04 03:04:57.000000 vkdispatch-0.0.5/deps/VKL/src/VKLStaticAllocator.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5503 2024-05-04 03:31:09.000000 vkdispatch-0.0.5/deps/VKL/src/VKLSurface.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    10896 2024-05-04 03:04:57.000000 vkdispatch-0.0.5/deps/VKL/src/VKLSwapChain.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       52 2024-05-04 03:22:46.000000 vkdispatch-0.0.5/deps/VKL/src/VMAImpl.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       53 2024-05-04 03:22:41.000000 vkdispatch-0.0.5/deps/VKL/src/VolkImpl.cpp
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.286158 vkdispatch-0.0.5/deps/VkFFT/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1084 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/LICENSE
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.287142 vkdispatch-0.0.5/deps/VkFFT/vkFFT/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.199862 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.290652 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12556 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_DeleteApp.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    91082 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_InitializeApp.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    44680 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_RunApp.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.199144 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.291347 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    15591 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_KernelStartEnd.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12866 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_KernelUtils.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.198333 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.294491 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     9486 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_Constants.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    14546 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_InputOutput.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6762 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_InputOutputLayout.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4342 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_PushConstants.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    23925 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_Registers.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    15546 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_SharedMemory.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.294741 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryTransfers/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    23235 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryTransfers/vkFFT_Transfers.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7697 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_Zeropad.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.295723 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.296393 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5753 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_4step.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    11508 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_Bluestein.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    19521 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_Convolution.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    22937 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_R2C.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)   141736 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_R2R.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    91669 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RaderKernels.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)   102595 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixKernels.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    35985 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixShuffle.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    28166 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixStage.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    84118 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_ReadWrite.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6365 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RegisterBoost.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.296868 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel2/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12743 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel2/vkFFT_FFT.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     9610 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel2/vkFFT_R2C_even_decomposition.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.297061 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_MathUtils/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)   114660 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_MathUtils/vkFFT_MathUtils.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.297248 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_StringManagement/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1722 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_StringManagement/vkFFT_StringManager.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.199721 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.298102 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    33238 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_CompileKernel.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5016 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_DeletePlan.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    26535 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_DispatchPlan.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    27280 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_InitAPIParameters.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    16495 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_ManageMemory.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    80386 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_UpdateBuffers.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.298752 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    37848 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_AxisBlockSplitter.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)   102541 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_ManageLUT.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    73734 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_RecursiveFFTGenerators.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)   147838 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_Scheduler.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.299076 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    50505 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/vkFFT_Plan_FFT.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    17441 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/vkFFT_Plan_R2C.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.299204 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_Structs/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    58072 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_Structs/vkFFT_Structs.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3191 2024-05-04 03:06:00.000000 vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      851 2024-05-04 16:17:35.000000 vkdispatch-0.0.5/pyproject.toml
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       38 2024-05-04 16:17:47.306336 vkdispatch-0.0.5/setup.cfg
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3807 2024-05-04 16:17:31.000000 vkdispatch-0.0.5/setup.py
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.301139 vkdispatch-0.0.5/vkdispatch/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1057 2024-05-04 03:04:33.000000 vkdispatch-0.0.5/vkdispatch/__init__.py
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       88 2024-05-04 03:04:33.000000 vkdispatch-0.0.5/vkdispatch/__main__.py
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1355 2024-05-04 16:00:59.000000 vkdispatch-0.0.5/vkdispatch/buffer.py
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2060 2024-05-04 03:04:33.000000 vkdispatch-0.0.5/vkdispatch/command_list.py
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1653 2024-05-04 16:00:33.000000 vkdispatch-0.0.5/vkdispatch/context.py
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      374 2024-05-04 03:04:33.000000 vkdispatch-0.0.5/vkdispatch/descriptor_set.py
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4176 2024-05-04 03:04:33.000000 vkdispatch-0.0.5/vkdispatch/dtype.py
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7489 2024-05-04 16:02:21.000000 vkdispatch-0.0.5/vkdispatch/image.py
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4494 2024-05-04 15:59:49.000000 vkdispatch-0.0.5/vkdispatch/init.py
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     9802 2024-05-04 16:09:47.000000 vkdispatch-0.0.5/vkdispatch/shader_builder.py
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4315 2024-05-04 16:06:25.000000 vkdispatch-0.0.5/vkdispatch/shader_decorator.py
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     8410 2024-05-04 16:03:58.000000 vkdispatch-0.0.5/vkdispatch/shader_variable.py
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      826 2024-05-04 16:04:34.000000 vkdispatch-0.0.5/vkdispatch/stage_compute.py
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2054 2024-05-04 16:04:59.000000 vkdispatch-0.0.5/vkdispatch/stage_fft.py
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     8538 2024-05-04 16:05:34.000000 vkdispatch-0.0.5/vkdispatch/stage_transfer.py
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.305629 vkdispatch-0.0.5/vkdispatch.egg-info/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      809 2024-05-04 16:17:47.000000 vkdispatch-0.0.5/vkdispatch.egg-info/PKG-INFO
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    15881 2024-05-04 16:17:47.000000 vkdispatch-0.0.5/vkdispatch.egg-info/SOURCES.txt
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)        1 2024-05-04 16:17:47.000000 vkdispatch-0.0.5/vkdispatch.egg-info/dependency_links.txt
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       52 2024-05-04 16:17:47.000000 vkdispatch-0.0.5/vkdispatch.egg-info/entry_points.txt
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)        1 2024-05-04 03:06:34.000000 vkdispatch-0.0.5/vkdispatch.egg-info/not-zip-safe
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       23 2024-05-04 16:17:47.000000 vkdispatch-0.0.5/vkdispatch.egg-info/requires.txt
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       29 2024-05-04 16:17:47.000000 vkdispatch-0.0.5/vkdispatch.egg-info/top_level.txt
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 16:17:47.305468 vkdispatch-0.0.5/vkdispatch_native/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      222 2024-05-04 03:04:33.000000 vkdispatch-0.0.5/vkdispatch_native/base.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3664 2024-05-04 03:12:26.000000 vkdispatch-0.0.5/vkdispatch_native/buffer.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      661 2024-05-04 03:04:33.000000 vkdispatch-0.0.5/vkdispatch_native/buffer.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1740 2024-05-04 03:04:33.000000 vkdispatch-0.0.5/vkdispatch_native/buffer.pxd
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3138 2024-05-04 05:22:58.000000 vkdispatch-0.0.5/vkdispatch_native/command_list.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      605 2024-05-04 03:04:33.000000 vkdispatch-0.0.5/vkdispatch_native/command_list.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1642 2024-05-04 03:04:33.000000 vkdispatch-0.0.5/vkdispatch_native/command_list.pxd
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1729 2024-05-04 03:04:33.000000 vkdispatch-0.0.5/vkdispatch_native/context.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      276 2024-05-04 03:04:33.000000 vkdispatch-0.0.5/vkdispatch_native/context.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1239 2024-05-04 03:04:33.000000 vkdispatch-0.0.5/vkdispatch_native/context.pxd
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1141 2024-05-04 03:04:33.000000 vkdispatch-0.0.5/vkdispatch_native/descriptor_set.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      378 2024-05-04 03:04:33.000000 vkdispatch-0.0.5/vkdispatch_native/descriptor_set.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1040 2024-05-04 03:04:33.000000 vkdispatch-0.0.5/vkdispatch_native/descriptor_set.pxd
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     8683 2024-05-04 05:33:00.000000 vkdispatch-0.0.5/vkdispatch_native/image.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1017 2024-05-04 03:04:33.000000 vkdispatch-0.0.5/vkdispatch_native/image.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4124 2024-05-04 03:04:33.000000 vkdispatch-0.0.5/vkdispatch_native/image.pxd
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4108 2024-05-04 03:40:31.000000 vkdispatch-0.0.5/vkdispatch_native/init.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1133 2024-05-04 03:04:33.000000 vkdispatch-0.0.5/vkdispatch_native/init.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2864 2024-05-04 03:04:33.000000 vkdispatch-0.0.5/vkdispatch_native/init.pxd
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1703 2024-05-04 03:04:33.000000 vkdispatch-0.0.5/vkdispatch_native/internal.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3574 2024-05-04 03:04:33.000000 vkdispatch-0.0.5/vkdispatch_native/stage_compute.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      797 2024-05-04 03:04:33.000000 vkdispatch-0.0.5/vkdispatch_native/stage_compute.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2108 2024-05-04 03:04:33.000000 vkdispatch-0.0.5/vkdispatch_native/stage_compute.pxd
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2803 2024-05-04 03:04:33.000000 vkdispatch-0.0.5/vkdispatch_native/stage_fft.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      410 2024-05-04 03:04:33.000000 vkdispatch-0.0.5/vkdispatch_native/stage_fft.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1519 2024-05-04 03:04:33.000000 vkdispatch-0.0.5/vkdispatch_native/stage_fft.pxd
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7021 2024-05-04 03:04:33.000000 vkdispatch-0.0.5/vkdispatch_native/stage_transfer.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1383 2024-05-04 03:04:33.000000 vkdispatch-0.0.5/vkdispatch_native/stage_transfer.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5522 2024-05-04 03:04:33.000000 vkdispatch-0.0.5/vkdispatch_native/stage_transfer.pxd
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      308 2024-05-04 03:04:33.000000 vkdispatch-0.0.5/vkdispatch_native/wrapper.pyx
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.689172 vkdispatch-0.0.6/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    11357 2024-05-04 03:04:33.000000 vkdispatch-0.0.6/LICENSE
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      817 2024-05-07 03:49:41.000000 vkdispatch-0.0.6/MANIFEST.in
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      809 2024-05-07 06:43:37.688945 vkdispatch-0.0.6/PKG-INFO
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      121 2024-05-04 03:04:33.000000 vkdispatch-0.0.6/README.md
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.539242 vkdispatch-0.0.6/deps/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.539173 vkdispatch-0.0.6/deps/VKL/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.538821 vkdispatch-0.0.6/deps/VKL/deps/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.551349 vkdispatch-0.0.6/deps/VKL/deps/VMA/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1099 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VKL/deps/VMA/LICENSE.txt
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.551730 vkdispatch-0.0.6/deps/VKL/deps/VMA/include/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   711190 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VKL/deps/VMA/include/vk_mem_alloc.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.553036 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      458 2024-05-04 05:19:24.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/LICENSE.md
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.531863 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.558452 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vk_video/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    16507 2024-05-04 05:19:24.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_av1std.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4250 2024-05-04 05:19:24.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_av1std_decode.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    13853 2024-05-04 05:19:24.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_h264std.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2722 2024-05-04 05:19:24.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_h264std_decode.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6878 2024-05-04 05:19:24.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_h264std_encode.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    23416 2024-05-04 05:19:24.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_h265std.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2428 2024-05-04 05:19:24.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_h265std_decode.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7462 2024-05-04 05:19:24.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_h265std_encode.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      660 2024-05-04 05:19:24.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codecs_common.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.581393 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     8164 2024-05-04 05:19:24.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vk_icd.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7073 2024-05-04 05:19:24.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vk_layer.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2828 2024-05-04 05:19:24.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vk_platform.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1555 2024-05-04 05:19:24.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6201 2024-05-04 05:19:24.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_android.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    10381 2024-05-04 05:19:24.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_beta.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)  1000714 2024-05-04 05:19:24.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_core.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1866 2024-05-04 05:19:24.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_directfb.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12470 2024-05-04 05:19:24.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_fuchsia.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1896 2024-05-04 05:19:24.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_ggp.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1309 2024-05-04 05:19:24.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_ios.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1341 2024-05-04 05:19:24.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_macos.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5907 2024-05-04 05:19:24.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_metal.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4064 2024-05-04 05:19:24.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_screen.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1282 2024-05-04 05:19:24.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_vi.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1866 2024-05-04 05:19:24.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_wayland.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    15112 2024-05-04 05:19:24.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_win32.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1880 2024-05-04 05:19:24.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_xcb.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1861 2024-05-04 05:19:24.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_xlib.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1411 2024-05-04 05:19:24.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_xlib_xrandr.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.581802 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Utility-Libraries/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      304 2024-05-04 05:33:49.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Utility-Libraries/LICENSE.md
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.532065 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Utility-Libraries/include/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.582187 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Utility-Libraries/include/vulkan/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.582946 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Utility-Libraries/include/vulkan/layer/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3565 2024-05-04 05:33:49.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Utility-Libraries/include/vulkan/layer/vk_layer_settings.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.586546 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Utility-Libraries/include/vulkan/utility/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   129114 2024-05-04 05:33:49.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Utility-Libraries/include/vulkan/utility/vk_dispatch_table.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   144058 2024-05-04 05:33:49.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Utility-Libraries/include/vulkan/utility/vk_format_utils.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   495518 2024-05-04 05:33:49.000000 vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Utility-Libraries/include/vulkan/vk_enum_string_helper.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.586928 vkdispatch-0.0.6/deps/VKL/deps/glslang/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    54705 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/LICENSE.txt
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.600584 vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.602521 vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/CInterface/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4254 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/CInterface/spirv_c_interface.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3616 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/GLSL.ext.AMD.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1598 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/GLSL.ext.ARM.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2585 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/GLSL.ext.EXT.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4486 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/GLSL.ext.KHR.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3781 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/GLSL.ext.NV.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1808 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/GLSL.ext.QCOM.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4126 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/GLSL.std.450.h
+-rwxr-xr-x   0 shaharsandhaus   (501) staff       (20)   461067 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/GlslangToSpv.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2666 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/GlslangToSpv.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5747 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/InReadableOrder.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2731 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/Logger.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2685 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/Logger.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1858 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/NonSemanticDebugPrintf.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7908 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/NonSemanticShaderDebugInfo100.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    11638 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/SPVRemapper.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   152756 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/SpvBuilder.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    45577 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/SpvBuilder.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    21678 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/SpvPostProcess.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12426 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/SpvTools.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4677 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/SpvTools.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3316 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/bitutils.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    35712 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/disassemble.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1926 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/disassemble.h
+-rwxr-xr-x   0 shaharsandhaus   (501) staff       (20)   195172 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/doc.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     8080 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/doc.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    39345 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/hex_float.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   140795 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/spirv.hpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    19791 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/spvIR.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.603300 vkdispatch-0.0.6/deps/VKL/deps/glslang/StandAlone/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5782 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/StandAlone/DirStackFileIncluder.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2821 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/StandAlone/Worklist.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.607450 vkdispatch-0.0.6/deps/VKL/deps/glslang/Test/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       11 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/Test/bar.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       30 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/Test/foo.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       24 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/Test/i1.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.609226 vkdispatch-0.0.6/deps/VKL/deps/glslang/Test/inc1/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       21 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/Test/inc1/badInc.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       29 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/Test/inc1/bar.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       32 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/Test/inc1/foo.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.611492 vkdispatch-0.0.6/deps/VKL/deps/glslang/Test/inc1/path1/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       14 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/Test/inc1/path1/bar.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       11 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/Test/inc1/path1/local.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       51 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/Test/inc1/path1/notHere.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.613221 vkdispatch-0.0.6/deps/VKL/deps/glslang/Test/inc1/path2/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       14 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/Test/inc1/path2/bar.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       15 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/Test/inc1/path2/notHere.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       11 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/Test/inc1/path2/remote.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.613510 vkdispatch-0.0.6/deps/VKL/deps/glslang/Test/inc2/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       28 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/Test/inc2/bar.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       11 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/Test/inc2/foo.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       11 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/Test/parent.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.538625 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.613652 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/CInterface/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    16918 2024-05-04 04:47:39.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/CInterface/glslang_c_interface.cpp
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.613969 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/GenericCodeGen/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2607 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/GenericCodeGen/CodeGen.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2750 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/GenericCodeGen/Link.cpp
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.619648 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/HLSL/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2132 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/HLSL/hlslAttributes.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6781 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/HLSL/hlslGrammar.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2327 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/HLSL/hlslOpMap.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    28652 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/HLSL/hlslParseHelper.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2622 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/HLSL/hlslParseables.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3560 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/HLSL/hlslScanContext.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3856 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/HLSL/hlslTokenStream.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     9628 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/HLSL/hlslTokens.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1996 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/HLSL/pch.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.626121 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Include/
+-rwxr-xr-x   0 shaharsandhaus   (501) staff       (20)    21618 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Include/BaseTypes.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     9241 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Include/Common.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    35998 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Include/ConstantUnion.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5927 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Include/InfoSink.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1854 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Include/InitializeGlobals.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    11856 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Include/PoolAlloc.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5664 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Include/ResourceLimits.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6312 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Include/ShHandle.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4413 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Include/SpirvIntrinsics.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   109017 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Include/Types.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12025 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Include/arrays.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    11752 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Include/glslang_c_interface.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     9017 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Include/glslang_c_shader_types.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    61736 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Include/intermediate.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.640404 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    61113 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/Constant.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3142 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/InfoSink.cpp
+-rwxr-xr-x   0 shaharsandhaus   (501) staff       (20)   562823 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/Initialize.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5491 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/Initialize.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     8084 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/IntermTraverse.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   139980 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/Intermediate.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6435 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/LiveTraverser.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    27638 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/ParseContextBase.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   481062 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/ParseHelper.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    33022 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/ParseHelper.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     9110 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/PoolAlloc.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3121 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/RemoveTree.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1704 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/RemoveTree.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    76508 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/Scan.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     9697 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/Scan.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3206 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/ScanContext.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    83435 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/ShaderLang.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12826 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/SpirvIntrinsics.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    17198 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/SymbolTable.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    36832 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/SymbolTable.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    69599 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/Versions.cpp
+-rwxr-xr-x   0 shaharsandhaus   (501) staff       (20)    25529 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/Versions.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12678 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/attribute.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4554 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/attribute.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    10171 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/gl_types.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   654870 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/glslang_tab.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    28552 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/glslang_tab.cpp.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    94894 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/intermOut.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    76316 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/iomapper.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    14491 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/iomapper.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6408 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/limits.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   109336 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/linkValidate.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    53321 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/localintermediate.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7568 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/parseConst.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    10098 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/parseVersions.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1896 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/pch.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.641703 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    50129 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/Pp.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6672 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/PpAtom.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5211 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/PpContext.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    27894 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/PpContext.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    57222 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/PpScanner.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7488 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/PpTokens.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5791 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/PpTokens.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    40778 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/propagateNoContraction.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2417 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/propagateNoContraction.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    56404 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/reflection.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     8171 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/reflection.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3346 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/span.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.642073 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/OSDependent/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1751 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/OSDependent/osinclude.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.644179 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Public/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2438 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Public/ResourceLimits.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    43942 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Public/ShaderLang.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2295 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Public/resource_limits_c.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.644912 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/ResourceLimits/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    34391 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/ResourceLimits/ResourceLimits.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2145 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/ResourceLimits/resource_limits_c.cpp
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.646501 vkdispatch-0.0.6/deps/VKL/deps/glslang/gtests/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2130 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/gtests/Initializer.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2142 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/gtests/Settings.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    32978 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/gtests/TestFixture.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1678 2024-05-04 04:29:15.000000 vkdispatch-0.0.6/deps/VKL/deps/glslang/gtests/pch.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.538888 vkdispatch-0.0.6/deps/VKL/deps/volk/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.647343 vkdispatch-0.0.6/deps/VKL/deps/volk/volk/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1066 2024-05-04 03:43:54.000000 vkdispatch-0.0.6/deps/VKL/deps/volk/volk/LICENSE.md
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   252357 2024-05-04 03:43:54.000000 vkdispatch-0.0.6/deps/VKL/deps/volk/volk/volk.c
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   127213 2024-05-04 03:43:54.000000 vkdispatch-0.0.6/deps/VKL/deps/volk/volk/volk.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.539105 vkdispatch-0.0.6/deps/VKL/include/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.650044 vkdispatch-0.0.6/deps/VKL/include/VKL/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      553 2024-05-04 03:04:57.000000 vkdispatch-0.0.6/deps/VKL/include/VKL/VKL.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1937 2024-05-04 03:04:57.000000 vkdispatch-0.0.6/deps/VKL/include/VKL/VKLBuffer.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2741 2024-05-04 03:04:57.000000 vkdispatch-0.0.6/deps/VKL/include/VKL/VKLCommandBuffer.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      829 2024-05-04 03:04:57.000000 vkdispatch-0.0.6/deps/VKL/include/VKL/VKLDescriptorSet.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     8377 2024-05-04 03:04:57.000000 vkdispatch-0.0.6/deps/VKL/include/VKL/VKLDevice.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1384 2024-05-04 03:04:57.000000 vkdispatch-0.0.6/deps/VKL/include/VKL/VKLFramebuffer.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2938 2024-05-04 03:04:57.000000 vkdispatch-0.0.6/deps/VKL/include/VKL/VKLImage.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      834 2024-05-04 03:04:57.000000 vkdispatch-0.0.6/deps/VKL/include/VKL/VKLImageView.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4176 2024-05-04 03:41:07.000000 vkdispatch-0.0.6/deps/VKL/include/VKL/VKLInstance.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1859 2024-05-04 03:04:57.000000 vkdispatch-0.0.6/deps/VKL/include/VKL/VKLPhysicalDevice.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2240 2024-05-04 03:04:57.000000 vkdispatch-0.0.6/deps/VKL/include/VKL/VKLPipeline.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2984 2024-05-04 03:04:57.000000 vkdispatch-0.0.6/deps/VKL/include/VKL/VKLPipelineLayout.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1077 2024-05-04 03:04:57.000000 vkdispatch-0.0.6/deps/VKL/include/VKL/VKLQueue.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3570 2024-05-04 03:04:57.000000 vkdispatch-0.0.6/deps/VKL/include/VKL/VKLRenderPass.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      671 2024-05-04 03:04:57.000000 vkdispatch-0.0.6/deps/VKL/include/VKL/VKLStaticAllocator.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1790 2024-05-04 03:04:57.000000 vkdispatch-0.0.6/deps/VKL/include/VKL/VKLSurface.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1628 2024-05-04 03:04:57.000000 vkdispatch-0.0.6/deps/VKL/include/VKL/VKLSwapChain.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4375 2024-05-07 06:39:14.000000 vkdispatch-0.0.6/deps/VKL/include/VKL/VKL_base.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.655732 vkdispatch-0.0.6/deps/VKL/include/glslang/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2895 2024-05-04 05:27:42.000000 vkdispatch-0.0.6/deps/VKL/include/glslang/build_info.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.665763 vkdispatch-0.0.6/deps/VKL/src/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7536 2024-05-04 03:04:57.000000 vkdispatch-0.0.6/deps/VKL/src/VKLBuffer.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7748 2024-05-04 03:04:57.000000 vkdispatch-0.0.6/deps/VKL/src/VKLCommandBuffer.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3646 2024-05-04 03:04:57.000000 vkdispatch-0.0.6/deps/VKL/src/VKLDescriptorSet.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    25947 2024-05-04 04:01:54.000000 vkdispatch-0.0.6/deps/VKL/src/VKLDevice.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3322 2024-05-04 03:04:57.000000 vkdispatch-0.0.6/deps/VKL/src/VKLFramebuffer.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    16236 2024-05-04 03:04:57.000000 vkdispatch-0.0.6/deps/VKL/src/VKLImage.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2433 2024-05-04 03:04:57.000000 vkdispatch-0.0.6/deps/VKL/src/VKLImageView.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    14415 2024-05-07 06:37:16.000000 vkdispatch-0.0.6/deps/VKL/src/VKLInstance.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4502 2024-05-04 03:29:09.000000 vkdispatch-0.0.6/deps/VKL/src/VKLPhysicalDevice.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12903 2024-05-04 03:04:57.000000 vkdispatch-0.0.6/deps/VKL/src/VKLPipeline.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12997 2024-05-04 03:04:57.000000 vkdispatch-0.0.6/deps/VKL/src/VKLPipelineLayout.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2167 2024-05-04 03:04:57.000000 vkdispatch-0.0.6/deps/VKL/src/VKLQueue.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6916 2024-05-04 03:04:57.000000 vkdispatch-0.0.6/deps/VKL/src/VKLRenderPass.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3383 2024-05-04 03:04:57.000000 vkdispatch-0.0.6/deps/VKL/src/VKLStaticAllocator.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5503 2024-05-04 03:31:09.000000 vkdispatch-0.0.6/deps/VKL/src/VKLSurface.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    10896 2024-05-04 03:04:57.000000 vkdispatch-0.0.6/deps/VKL/src/VKLSwapChain.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       52 2024-05-04 03:22:46.000000 vkdispatch-0.0.6/deps/VKL/src/VMAImpl.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       53 2024-05-04 03:22:41.000000 vkdispatch-0.0.6/deps/VKL/src/VolkImpl.cpp
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.665874 vkdispatch-0.0.6/deps/VkFFT/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1084 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/LICENSE
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.665979 vkdispatch-0.0.6/deps/VkFFT/vkFFT/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.545971 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.666480 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12556 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_DeleteApp.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    91082 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_InitializeApp.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    44680 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_RunApp.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.545074 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.666926 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    15591 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_KernelStartEnd.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12866 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_KernelUtils.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.543958 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.667873 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     9486 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_Constants.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    14546 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_InputOutput.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6762 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_InputOutputLayout.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4342 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_PushConstants.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    23925 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_Registers.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    15546 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_SharedMemory.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.668032 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryTransfers/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    23235 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryTransfers/vkFFT_Transfers.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7697 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_Zeropad.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.668986 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.669778 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5753 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_4step.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    11508 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_Bluestein.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    19521 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_Convolution.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    22937 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_R2C.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   141736 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_R2R.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    91669 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RaderKernels.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   102595 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixKernels.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    35985 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixShuffle.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    28166 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixStage.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    84118 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_ReadWrite.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6365 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RegisterBoost.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.670139 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel2/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12743 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel2/vkFFT_FFT.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     9610 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel2/vkFFT_R2C_even_decomposition.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.670287 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_MathUtils/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   114660 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_MathUtils/vkFFT_MathUtils.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.670460 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_StringManagement/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1722 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_StringManagement/vkFFT_StringManager.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.545809 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.671305 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    33238 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_CompileKernel.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5016 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_DeletePlan.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    26535 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_DispatchPlan.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    27280 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_InitAPIParameters.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    16495 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_ManageMemory.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    80386 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_UpdateBuffers.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.672053 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    37848 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_AxisBlockSplitter.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   102541 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_ManageLUT.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    73734 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_RecursiveFFTGenerators.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   147838 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_Scheduler.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.672431 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    50505 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/vkFFT_Plan_FFT.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    17441 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/vkFFT_Plan_R2C.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.672573 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_Structs/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    58072 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_Structs/vkFFT_Structs.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3191 2024-05-04 03:06:00.000000 vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.672871 vkdispatch-0.0.6/libs/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    11358 2024-05-07 03:49:28.000000 vkdispatch-0.0.6/libs/LICENSE.txt
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20) 20105552 2024-03-13 20:09:53.000000 vkdispatch-0.0.6/libs/libMoltenVK.a
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      851 2024-05-07 06:43:17.000000 vkdispatch-0.0.6/pyproject.toml
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       38 2024-05-07 06:43:37.689214 vkdispatch-0.0.6/setup.cfg
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4488 2024-05-07 06:43:13.000000 vkdispatch-0.0.6/setup.py
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.683945 vkdispatch-0.0.6/vkdispatch/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1057 2024-05-04 03:04:33.000000 vkdispatch-0.0.6/vkdispatch/__init__.py
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       88 2024-05-04 03:04:33.000000 vkdispatch-0.0.6/vkdispatch/__main__.py
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1355 2024-05-04 16:00:59.000000 vkdispatch-0.0.6/vkdispatch/buffer.py
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2060 2024-05-04 03:04:33.000000 vkdispatch-0.0.6/vkdispatch/command_list.py
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1653 2024-05-04 16:00:33.000000 vkdispatch-0.0.6/vkdispatch/context.py
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      374 2024-05-04 03:04:33.000000 vkdispatch-0.0.6/vkdispatch/descriptor_set.py
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4176 2024-05-04 03:04:33.000000 vkdispatch-0.0.6/vkdispatch/dtype.py
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7489 2024-05-04 16:02:21.000000 vkdispatch-0.0.6/vkdispatch/image.py
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4494 2024-05-04 15:59:49.000000 vkdispatch-0.0.6/vkdispatch/init.py
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     9802 2024-05-04 16:09:47.000000 vkdispatch-0.0.6/vkdispatch/shader_builder.py
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4315 2024-05-04 16:06:25.000000 vkdispatch-0.0.6/vkdispatch/shader_decorator.py
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     8410 2024-05-04 16:03:58.000000 vkdispatch-0.0.6/vkdispatch/shader_variable.py
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      826 2024-05-04 16:04:34.000000 vkdispatch-0.0.6/vkdispatch/stage_compute.py
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2054 2024-05-04 16:04:59.000000 vkdispatch-0.0.6/vkdispatch/stage_fft.py
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     8538 2024-05-04 16:05:34.000000 vkdispatch-0.0.6/vkdispatch/stage_transfer.py
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.688655 vkdispatch-0.0.6/vkdispatch.egg-info/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      809 2024-05-07 06:43:37.000000 vkdispatch-0.0.6/vkdispatch.egg-info/PKG-INFO
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    15917 2024-05-07 06:43:37.000000 vkdispatch-0.0.6/vkdispatch.egg-info/SOURCES.txt
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)        1 2024-05-07 06:43:37.000000 vkdispatch-0.0.6/vkdispatch.egg-info/dependency_links.txt
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       52 2024-05-07 06:43:37.000000 vkdispatch-0.0.6/vkdispatch.egg-info/entry_points.txt
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)        1 2024-05-04 03:06:34.000000 vkdispatch-0.0.6/vkdispatch.egg-info/not-zip-safe
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       23 2024-05-07 06:43:37.000000 vkdispatch-0.0.6/vkdispatch.egg-info/requires.txt
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       29 2024-05-07 06:43:37.000000 vkdispatch-0.0.6/vkdispatch.egg-info/top_level.txt
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-07 06:43:37.688493 vkdispatch-0.0.6/vkdispatch_native/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      222 2024-05-04 03:04:33.000000 vkdispatch-0.0.6/vkdispatch_native/base.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3664 2024-05-04 03:12:26.000000 vkdispatch-0.0.6/vkdispatch_native/buffer.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      661 2024-05-04 03:04:33.000000 vkdispatch-0.0.6/vkdispatch_native/buffer.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1740 2024-05-04 03:04:33.000000 vkdispatch-0.0.6/vkdispatch_native/buffer.pxd
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3138 2024-05-04 05:22:58.000000 vkdispatch-0.0.6/vkdispatch_native/command_list.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      605 2024-05-04 03:04:33.000000 vkdispatch-0.0.6/vkdispatch_native/command_list.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1642 2024-05-04 03:04:33.000000 vkdispatch-0.0.6/vkdispatch_native/command_list.pxd
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1729 2024-05-04 03:04:33.000000 vkdispatch-0.0.6/vkdispatch_native/context.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      276 2024-05-04 03:04:33.000000 vkdispatch-0.0.6/vkdispatch_native/context.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1239 2024-05-04 03:04:33.000000 vkdispatch-0.0.6/vkdispatch_native/context.pxd
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1141 2024-05-04 03:04:33.000000 vkdispatch-0.0.6/vkdispatch_native/descriptor_set.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      378 2024-05-04 03:04:33.000000 vkdispatch-0.0.6/vkdispatch_native/descriptor_set.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1040 2024-05-04 03:04:33.000000 vkdispatch-0.0.6/vkdispatch_native/descriptor_set.pxd
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     8683 2024-05-04 05:33:00.000000 vkdispatch-0.0.6/vkdispatch_native/image.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1017 2024-05-04 03:04:33.000000 vkdispatch-0.0.6/vkdispatch_native/image.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4124 2024-05-04 03:04:33.000000 vkdispatch-0.0.6/vkdispatch_native/image.pxd
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4256 2024-05-07 06:41:04.000000 vkdispatch-0.0.6/vkdispatch_native/init.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1133 2024-05-04 03:04:33.000000 vkdispatch-0.0.6/vkdispatch_native/init.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2864 2024-05-04 03:04:33.000000 vkdispatch-0.0.6/vkdispatch_native/init.pxd
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1703 2024-05-04 03:04:33.000000 vkdispatch-0.0.6/vkdispatch_native/internal.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3574 2024-05-04 03:04:33.000000 vkdispatch-0.0.6/vkdispatch_native/stage_compute.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      797 2024-05-04 03:04:33.000000 vkdispatch-0.0.6/vkdispatch_native/stage_compute.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2108 2024-05-04 03:04:33.000000 vkdispatch-0.0.6/vkdispatch_native/stage_compute.pxd
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2803 2024-05-04 03:04:33.000000 vkdispatch-0.0.6/vkdispatch_native/stage_fft.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      410 2024-05-04 03:04:33.000000 vkdispatch-0.0.6/vkdispatch_native/stage_fft.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1519 2024-05-04 03:04:33.000000 vkdispatch-0.0.6/vkdispatch_native/stage_fft.pxd
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7021 2024-05-04 03:04:33.000000 vkdispatch-0.0.6/vkdispatch_native/stage_transfer.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1383 2024-05-04 03:04:33.000000 vkdispatch-0.0.6/vkdispatch_native/stage_transfer.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5522 2024-05-04 03:04:33.000000 vkdispatch-0.0.6/vkdispatch_native/stage_transfer.pxd
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      308 2024-05-04 03:04:33.000000 vkdispatch-0.0.6/vkdispatch_native/wrapper.pyx
```

### Comparing `vkdispatch-0.0.5/LICENSE` & `vkdispatch-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/MANIFEST.in` & `vkdispatch-0.0.6/MANIFEST.in`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 include deps/VKL/include/glslang/*.h
 include deps/VKL/deps/VMA/include/*.h
 include deps/VKL/deps/VMA/LICENSE.txt
 include deps/VKL/deps/volk/volk/volk.h
 include deps/VKL/deps/volk/volk/volk.c
 include deps/VKL/deps/volk/volk/LICENSE.md
 
+include libs/libMoltenVK.a
+include libs/LICENSE.txt
+
 recursive-include deps/VKL/deps/Vulkan-Headers/include *.h
 include deps/VKL/deps/Vulkan-Headers/LICENSE.md
 
 recursive-include deps/VKL/deps/Vulkan-Utility-Libraries/include *.h
 include deps/VKL/deps/Vulkan-Utility-Libraries/LICENSE.md
 
 recursive-include deps/VkFFT/vkFFT *.h
```

### Comparing `vkdispatch-0.0.5/PKG-INFO` & `vkdispatch-0.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vkdispatch
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python module for orchestrating and dispatching large computations across multi-GPU systems using Vulkan.
 Author-email: Shahar Sandhaus <shahar.sandhaus@gmail.com>
 Project-URL: Homepage, https://github.com/sharhar/vkdispatch
 Project-URL: Issues, https://github.com/sharhar/vkdispatch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/VMA/LICENSE.txt` & `vkdispatch-0.0.6/deps/VKL/deps/VMA/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/VMA/include/vk_mem_alloc.h` & `vkdispatch-0.0.6/deps/VKL/deps/VMA/include/vk_mem_alloc.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_av1std.h` & `vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_av1std.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_av1std_decode.h` & `vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_av1std_decode.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_h264std.h` & `vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_h264std.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_h264std_decode.h` & `vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_h264std_decode.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_h264std_encode.h` & `vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_h264std_encode.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_h265std.h` & `vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_h265std.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_h265std_decode.h` & `vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_h265std_decode.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_h265std_encode.h` & `vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_h265std_encode.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codecs_common.h` & `vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codecs_common.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vk_icd.h` & `vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vk_icd.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vk_layer.h` & `vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vk_layer.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vk_platform.h` & `vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vk_platform.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan.h` & `vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_android.h` & `vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_android.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_beta.h` & `vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_beta.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_core.h` & `vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_core.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_directfb.h` & `vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_directfb.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_fuchsia.h` & `vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_fuchsia.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_ggp.h` & `vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_ggp.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_ios.h` & `vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_ios.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_macos.h` & `vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_macos.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_metal.h` & `vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_metal.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_screen.h` & `vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_screen.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_vi.h` & `vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_vi.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_wayland.h` & `vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_wayland.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_win32.h` & `vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_win32.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_xcb.h` & `vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_xcb.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_xlib.h` & `vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_xlib.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_xlib_xrandr.h` & `vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_xlib_xrandr.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Utility-Libraries/include/vulkan/layer/vk_layer_settings.h` & `vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Utility-Libraries/include/vulkan/layer/vk_layer_settings.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Utility-Libraries/include/vulkan/utility/vk_dispatch_table.h` & `vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Utility-Libraries/include/vulkan/utility/vk_dispatch_table.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Utility-Libraries/include/vulkan/utility/vk_format_utils.h` & `vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Utility-Libraries/include/vulkan/utility/vk_format_utils.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/Vulkan-Utility-Libraries/include/vulkan/vk_enum_string_helper.h` & `vkdispatch-0.0.6/deps/VKL/deps/Vulkan-Utility-Libraries/include/vulkan/vk_enum_string_helper.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/LICENSE.txt` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/CInterface/spirv_c_interface.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/CInterface/spirv_c_interface.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/GLSL.ext.AMD.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/GLSL.ext.AMD.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/GLSL.ext.ARM.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/GLSL.ext.ARM.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/GLSL.ext.EXT.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/GLSL.ext.EXT.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/GLSL.ext.KHR.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/GLSL.ext.KHR.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/GLSL.ext.NV.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/GLSL.ext.NV.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/GLSL.ext.QCOM.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/GLSL.ext.QCOM.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/GLSL.std.450.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/GLSL.std.450.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/GlslangToSpv.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/GlslangToSpv.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/GlslangToSpv.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/GlslangToSpv.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/InReadableOrder.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/InReadableOrder.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/Logger.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/Logger.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/Logger.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/Logger.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/NonSemanticDebugPrintf.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/NonSemanticDebugPrintf.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/NonSemanticShaderDebugInfo100.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/NonSemanticShaderDebugInfo100.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/SPVRemapper.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/SPVRemapper.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/SpvBuilder.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/SpvBuilder.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/SpvBuilder.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/SpvBuilder.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/SpvPostProcess.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/SpvPostProcess.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/SpvTools.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/SpvTools.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/SpvTools.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/SpvTools.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/bitutils.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/bitutils.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/disassemble.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/disassemble.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/disassemble.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/disassemble.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/doc.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/doc.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/doc.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/doc.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/hex_float.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/hex_float.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/spirv.hpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/spirv.hpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/SPIRV/spvIR.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/SPIRV/spvIR.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/StandAlone/DirStackFileIncluder.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/StandAlone/DirStackFileIncluder.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/StandAlone/Worklist.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/StandAlone/Worklist.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/CInterface/glslang_c_interface.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/CInterface/glslang_c_interface.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/GenericCodeGen/CodeGen.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/GenericCodeGen/CodeGen.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/GenericCodeGen/Link.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/GenericCodeGen/Link.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/HLSL/hlslAttributes.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/HLSL/hlslAttributes.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/HLSL/hlslGrammar.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/HLSL/hlslGrammar.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/HLSL/hlslOpMap.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/HLSL/hlslOpMap.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/HLSL/hlslParseHelper.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/HLSL/hlslParseHelper.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/HLSL/hlslParseables.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/HLSL/hlslParseables.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/HLSL/hlslScanContext.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/HLSL/hlslScanContext.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/HLSL/hlslTokenStream.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/HLSL/hlslTokenStream.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/HLSL/hlslTokens.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/HLSL/hlslTokens.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/HLSL/pch.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/HLSL/pch.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Include/BaseTypes.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Include/BaseTypes.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Include/Common.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Include/Common.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Include/ConstantUnion.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Include/ConstantUnion.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Include/InfoSink.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Include/InfoSink.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Include/InitializeGlobals.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Include/InitializeGlobals.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Include/PoolAlloc.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Include/PoolAlloc.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Include/ResourceLimits.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Include/ResourceLimits.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Include/ShHandle.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Include/ShHandle.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Include/SpirvIntrinsics.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Include/SpirvIntrinsics.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Include/Types.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Include/Types.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Include/arrays.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Include/arrays.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Include/glslang_c_interface.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Include/glslang_c_interface.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Include/glslang_c_shader_types.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Include/glslang_c_shader_types.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Include/intermediate.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Include/intermediate.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/Constant.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/Constant.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/InfoSink.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/InfoSink.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/Initialize.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/Initialize.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/Initialize.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/Initialize.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/IntermTraverse.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/IntermTraverse.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/Intermediate.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/Intermediate.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/LiveTraverser.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/LiveTraverser.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/ParseContextBase.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/ParseContextBase.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/ParseHelper.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/ParseHelper.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/ParseHelper.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/ParseHelper.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/PoolAlloc.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/PoolAlloc.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/RemoveTree.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/RemoveTree.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/RemoveTree.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/RemoveTree.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/Scan.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/Scan.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/Scan.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/Scan.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/ScanContext.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/ScanContext.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/ShaderLang.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/ShaderLang.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/SpirvIntrinsics.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/SpirvIntrinsics.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/SymbolTable.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/SymbolTable.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/SymbolTable.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/SymbolTable.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/Versions.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/Versions.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/Versions.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/Versions.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/attribute.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/attribute.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/attribute.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/attribute.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/gl_types.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/gl_types.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/glslang_tab.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/glslang_tab.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/glslang_tab.cpp.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/glslang_tab.cpp.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/intermOut.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/intermOut.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/iomapper.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/iomapper.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/iomapper.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/iomapper.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/limits.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/limits.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/linkValidate.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/linkValidate.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/localintermediate.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/localintermediate.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/parseConst.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/parseConst.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/parseVersions.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/parseVersions.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/pch.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/pch.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/Pp.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/Pp.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/PpAtom.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/PpAtom.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/PpContext.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/PpContext.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/PpContext.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/PpContext.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/PpScanner.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/PpScanner.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/PpTokens.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/PpTokens.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/PpTokens.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/PpTokens.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/propagateNoContraction.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/propagateNoContraction.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/propagateNoContraction.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/propagateNoContraction.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/reflection.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/reflection.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/reflection.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/reflection.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/MachineIndependent/span.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/MachineIndependent/span.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/OSDependent/osinclude.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/OSDependent/osinclude.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Public/ResourceLimits.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Public/ResourceLimits.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Public/ShaderLang.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Public/ShaderLang.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/Public/resource_limits_c.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/Public/resource_limits_c.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/ResourceLimits/ResourceLimits.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/ResourceLimits/ResourceLimits.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/glslang/ResourceLimits/resource_limits_c.cpp` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/glslang/ResourceLimits/resource_limits_c.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/gtests/Initializer.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/gtests/Initializer.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/gtests/Settings.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/gtests/Settings.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/gtests/TestFixture.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/gtests/TestFixture.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/glslang/gtests/pch.h` & `vkdispatch-0.0.6/deps/VKL/deps/glslang/gtests/pch.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/volk/volk/LICENSE.md` & `vkdispatch-0.0.6/deps/VKL/deps/volk/volk/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/volk/volk/volk.c` & `vkdispatch-0.0.6/deps/VKL/deps/volk/volk/volk.c`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/deps/volk/volk/volk.h` & `vkdispatch-0.0.6/deps/VKL/deps/volk/volk/volk.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/include/VKL/VKL.h` & `vkdispatch-0.0.6/deps/VKL/include/VKL/VKL.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/include/VKL/VKLBuffer.h` & `vkdispatch-0.0.6/deps/VKL/include/VKL/VKLBuffer.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/include/VKL/VKLCommandBuffer.h` & `vkdispatch-0.0.6/deps/VKL/include/VKL/VKLCommandBuffer.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/include/VKL/VKLDescriptorSet.h` & `vkdispatch-0.0.6/deps/VKL/include/VKL/VKLDescriptorSet.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/include/VKL/VKLDevice.h` & `vkdispatch-0.0.6/deps/VKL/include/VKL/VKLDevice.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/include/VKL/VKLFramebuffer.h` & `vkdispatch-0.0.6/deps/VKL/include/VKL/VKLFramebuffer.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/include/VKL/VKLImage.h` & `vkdispatch-0.0.6/deps/VKL/include/VKL/VKLImage.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/include/VKL/VKLImageView.h` & `vkdispatch-0.0.6/deps/VKL/include/VKL/VKLImageView.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/include/VKL/VKLInstance.h` & `vkdispatch-0.0.6/deps/VKL/include/VKL/VKLInstance.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/include/VKL/VKLPhysicalDevice.h` & `vkdispatch-0.0.6/deps/VKL/include/VKL/VKLPhysicalDevice.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/include/VKL/VKLPipeline.h` & `vkdispatch-0.0.6/deps/VKL/include/VKL/VKLPipeline.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/include/VKL/VKLPipelineLayout.h` & `vkdispatch-0.0.6/deps/VKL/include/VKL/VKLPipelineLayout.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/include/VKL/VKLQueue.h` & `vkdispatch-0.0.6/deps/VKL/include/VKL/VKLQueue.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/include/VKL/VKLRenderPass.h` & `vkdispatch-0.0.6/deps/VKL/include/VKL/VKLRenderPass.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/include/VKL/VKLStaticAllocator.h` & `vkdispatch-0.0.6/deps/VKL/include/VKL/VKLStaticAllocator.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/include/VKL/VKLSurface.h` & `vkdispatch-0.0.6/deps/VKL/include/VKL/VKLSurface.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/include/VKL/VKLSwapChain.h` & `vkdispatch-0.0.6/deps/VKL/include/VKL/VKLSwapChain.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/include/VKL/VKL_base.h` & `vkdispatch-0.0.6/deps/VKL/include/VKL/VKL_base.h`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,27 @@
 
 //#ifndef _DEBUG
 //#define VK_CALL(result) result;
 //#endif
 
 #define VKL_VALIDATION
 
+
+#ifdef VKDISPATCH_USE_MVK
+#include <vulkan/vulkan.h>
+#else
+
 #define VK_NO_PROTOTYPES
-#define VMA_STATIC_VULKAN_FUNCTIONS 0
-#define VMA_DYNAMIC_VULKAN_FUNCTIONS 1
 #include <vulkan/vulkan.h>
 #include <volk/volk.h>
+
+#endif
+
+#define VMA_STATIC_VULKAN_FUNCTIONS 0
+#define VMA_DYNAMIC_VULKAN_FUNCTIONS 1
 #include <vk_mem_alloc.h>
 
 #include <assert.h>
 #include <stdio.h>
 #include <string.h>
 #include <stdlib.h>
```

### Comparing `vkdispatch-0.0.5/deps/VKL/include/glslang/build_info.h` & `vkdispatch-0.0.6/deps/VKL/include/glslang/build_info.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/src/VKLBuffer.cpp` & `vkdispatch-0.0.6/deps/VKL/src/VKLBuffer.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/src/VKLCommandBuffer.cpp` & `vkdispatch-0.0.6/deps/VKL/src/VKLCommandBuffer.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/src/VKLDescriptorSet.cpp` & `vkdispatch-0.0.6/deps/VKL/src/VKLDescriptorSet.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/src/VKLDevice.cpp` & `vkdispatch-0.0.6/deps/VKL/src/VKLDevice.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/src/VKLFramebuffer.cpp` & `vkdispatch-0.0.6/deps/VKL/src/VKLFramebuffer.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/src/VKLImage.cpp` & `vkdispatch-0.0.6/deps/VKL/src/VKLImage.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/src/VKLImageView.cpp` & `vkdispatch-0.0.6/deps/VKL/src/VKLImageView.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/src/VKLInstance.cpp` & `vkdispatch-0.0.6/deps/VKL/src/VKLInstance.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,17 @@
 	VkValidationFeatureEnableEXT enabledValidationFeatures[] = {VK_VALIDATION_FEATURE_ENABLE_DEBUG_PRINTF_EXT};
 	validationFeatures.pEnabledValidationFeatures = enabledValidationFeatures;
 
 	((VkInstanceCreateInfo*)&createInfo.m_createInfo)->pNext = &validationFeatures;
 
 	VK_CALL(vkCreateInstance(&createInfo.m_createInfo, m_allocationCallbacks, &m_handle));
 
+	#ifndef VKDISPATCH_USE_MVK
 	volkLoadInstance(m_handle);
+	#endif
 
 	VkDebugUtilsMessengerCreateInfoEXT debugCreateInfo = {};
 	debugCreateInfo.sType = VK_STRUCTURE_TYPE_DEBUG_UTILS_MESSENGER_CREATE_INFO_EXT;
 	debugCreateInfo.pNext = NULL;
     debugCreateInfo.flags = 0;
     debugCreateInfo.messageSeverity = VK_DEBUG_UTILS_MESSAGE_SEVERITY_VERBOSE_BIT_EXT |
 						VK_DEBUG_UTILS_MESSAGE_SEVERITY_INFO_BIT_EXT |
```

### Comparing `vkdispatch-0.0.5/deps/VKL/src/VKLPhysicalDevice.cpp` & `vkdispatch-0.0.6/deps/VKL/src/VKLPhysicalDevice.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/src/VKLPipeline.cpp` & `vkdispatch-0.0.6/deps/VKL/src/VKLPipeline.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/src/VKLPipelineLayout.cpp` & `vkdispatch-0.0.6/deps/VKL/src/VKLPipelineLayout.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/src/VKLQueue.cpp` & `vkdispatch-0.0.6/deps/VKL/src/VKLQueue.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/src/VKLRenderPass.cpp` & `vkdispatch-0.0.6/deps/VKL/src/VKLRenderPass.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/src/VKLStaticAllocator.cpp` & `vkdispatch-0.0.6/deps/VKL/src/VKLStaticAllocator.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/src/VKLSurface.cpp` & `vkdispatch-0.0.6/deps/VKL/src/VKLSurface.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VKL/src/VKLSwapChain.cpp` & `vkdispatch-0.0.6/deps/VKL/src/VKLSwapChain.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/LICENSE` & `vkdispatch-0.0.6/deps/VkFFT/LICENSE`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_DeleteApp.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_DeleteApp.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_InitializeApp.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_InitializeApp.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_RunApp.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_RunApp.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_KernelStartEnd.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_KernelStartEnd.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_KernelUtils.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_KernelUtils.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_Constants.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_Constants.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_InputOutput.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_InputOutput.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_InputOutputLayout.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_InputOutputLayout.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_PushConstants.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_PushConstants.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_Registers.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_Registers.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_SharedMemory.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_SharedMemory.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryTransfers/vkFFT_Transfers.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryTransfers/vkFFT_Transfers.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_Zeropad.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_Zeropad.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_4step.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_4step.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_Bluestein.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_Bluestein.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_Convolution.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_Convolution.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_R2C.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_R2C.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_R2R.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_R2R.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RaderKernels.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RaderKernels.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixKernels.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixKernels.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixShuffle.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixShuffle.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixStage.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixStage.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_ReadWrite.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_ReadWrite.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RegisterBoost.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RegisterBoost.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel2/vkFFT_FFT.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel2/vkFFT_FFT.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel2/vkFFT_R2C_even_decomposition.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel2/vkFFT_R2C_even_decomposition.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_MathUtils/vkFFT_MathUtils.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_MathUtils/vkFFT_MathUtils.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_StringManagement/vkFFT_StringManager.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_StringManagement/vkFFT_StringManager.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_CompileKernel.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_CompileKernel.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_DeletePlan.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_DeletePlan.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_DispatchPlan.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_DispatchPlan.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_InitAPIParameters.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_InitAPIParameters.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_ManageMemory.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_ManageMemory.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_UpdateBuffers.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_UpdateBuffers.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_AxisBlockSplitter.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_AxisBlockSplitter.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_ManageLUT.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_ManageLUT.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_RecursiveFFTGenerators.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_RecursiveFFTGenerators.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_Scheduler.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_Scheduler.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/vkFFT_Plan_FFT.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/vkFFT_Plan_FFT.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/vkFFT_Plan_R2C.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/vkFFT_Plan_R2C.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT/vkFFT_Structs/vkFFT_Structs.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT/vkFFT_Structs/vkFFT_Structs.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/deps/VkFFT/vkFFT/vkFFT.h` & `vkdispatch-0.0.6/deps/VkFFT/vkFFT/vkFFT.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/pyproject.toml` & `vkdispatch-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "Cython",
     "numpy"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vkdispatch"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Shahar Sandhaus", email="shahar.sandhaus@gmail.com" },
 ]
 description = "A Python module for orchestrating and dispatching large computations across multi-GPU systems using Vulkan."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `vkdispatch-0.0.5/vkdispatch/__init__.py` & `vkdispatch-0.0.6/vkdispatch/__init__.py`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch/buffer.py` & `vkdispatch-0.0.6/vkdispatch/buffer.py`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch/command_list.py` & `vkdispatch-0.0.6/vkdispatch/command_list.py`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch/context.py` & `vkdispatch-0.0.6/vkdispatch/context.py`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch/dtype.py` & `vkdispatch-0.0.6/vkdispatch/dtype.py`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch/image.py` & `vkdispatch-0.0.6/vkdispatch/image.py`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch/init.py` & `vkdispatch-0.0.6/vkdispatch/init.py`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch/shader_builder.py` & `vkdispatch-0.0.6/vkdispatch/shader_builder.py`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch/shader_decorator.py` & `vkdispatch-0.0.6/vkdispatch/shader_decorator.py`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch/shader_variable.py` & `vkdispatch-0.0.6/vkdispatch/shader_variable.py`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch/stage_compute.py` & `vkdispatch-0.0.6/vkdispatch/stage_compute.py`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch/stage_fft.py` & `vkdispatch-0.0.6/vkdispatch/stage_fft.py`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch/stage_transfer.py` & `vkdispatch-0.0.6/vkdispatch/stage_transfer.py`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch.egg-info/PKG-INFO` & `vkdispatch-0.0.6/vkdispatch.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vkdispatch
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python module for orchestrating and dispatching large computations across multi-GPU systems using Vulkan.
 Author-email: Shahar Sandhaus <shahar.sandhaus@gmail.com>
 Project-URL: Homepage, https://github.com/sharhar/vkdispatch
 Project-URL: Issues, https://github.com/sharhar/vkdispatch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vkdispatch-0.0.5/vkdispatch.egg-info/SOURCES.txt` & `vkdispatch-0.0.6/vkdispatch.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -250,14 +250,16 @@
 deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_AxisBlockSplitter.h
 deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_ManageLUT.h
 deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_RecursiveFFTGenerators.h
 deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_Scheduler.h
 deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/vkFFT_Plan_FFT.h
 deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/vkFFT_Plan_R2C.h
 deps/VkFFT/vkFFT/vkFFT/vkFFT_Structs/vkFFT_Structs.h
+libs/LICENSE.txt
+libs/libMoltenVK.a
 vkdispatch/__init__.py
 vkdispatch/__main__.py
 vkdispatch/buffer.py
 vkdispatch/command_list.py
 vkdispatch/context.py
 vkdispatch/descriptor_set.py
 vkdispatch/dtype.py
```

### Comparing `vkdispatch-0.0.5/vkdispatch_native/buffer.cpp` & `vkdispatch-0.0.6/vkdispatch_native/buffer.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch_native/buffer.h` & `vkdispatch-0.0.6/vkdispatch_native/buffer.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch_native/buffer.pxd` & `vkdispatch-0.0.6/vkdispatch_native/buffer.pxd`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch_native/command_list.cpp` & `vkdispatch-0.0.6/vkdispatch_native/command_list.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch_native/command_list.h` & `vkdispatch-0.0.6/vkdispatch_native/command_list.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch_native/command_list.pxd` & `vkdispatch-0.0.6/vkdispatch_native/command_list.pxd`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch_native/context.cpp` & `vkdispatch-0.0.6/vkdispatch_native/context.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch_native/context.pxd` & `vkdispatch-0.0.6/vkdispatch_native/context.pxd`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch_native/descriptor_set.cpp` & `vkdispatch-0.0.6/vkdispatch_native/descriptor_set.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch_native/descriptor_set.pxd` & `vkdispatch-0.0.6/vkdispatch_native/descriptor_set.pxd`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch_native/image.cpp` & `vkdispatch-0.0.6/vkdispatch_native/image.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch_native/image.h` & `vkdispatch-0.0.6/vkdispatch_native/image.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch_native/image.pxd` & `vkdispatch-0.0.6/vkdispatch_native/image.pxd`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch_native/init.cpp` & `vkdispatch-0.0.6/vkdispatch_native/init.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 #include "internal.h"
 
 #include <stdio.h>
 
 MyInstance _instance;
 
 void init_extern(bool debug) {
-
-	VK_CALL(volkInitialize());
+    #ifdef VKDISPATCH_USE_MVK
+    setenv("MVK_CONFIG_LOG_LEVEL", "2", 0);
+    #else
+    VK_CALL(volkInitialize());
+    #endif
+	
 
     LOG_INFO("Initializing glslang...");
 
     if(!glslang_initialize_process()) {
         LOG_ERROR("Failed to initialize glslang process");
         return;
     }
@@ -18,14 +22,16 @@
     LOG_INFO("Initializing Vulkan Instance...");
     
     _instance.instance.create(
         VKLInstanceCreateInfo()
         .debug(VK_TRUE)
     );
 
+    LOG_INFO("Initializing Vulkan Devices...");
+
     const std::vector<VKLPhysicalDevice*>& physicalDevices = _instance.instance.getPhysicalDevices();
 
     _instance.devices = new PhysicalDeviceProperties[physicalDevices.size()];
 
     for(int i = 0; i < physicalDevices.size(); i++) {
         VkPhysicalDeviceProperties properties = physicalDevices[i]->getProperties();
         VkPhysicalDeviceFeatures features = physicalDevices[i]->getFeatures();
```

### Comparing `vkdispatch-0.0.5/vkdispatch_native/init.h` & `vkdispatch-0.0.6/vkdispatch_native/init.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch_native/init.pxd` & `vkdispatch-0.0.6/vkdispatch_native/init.pxd`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch_native/internal.h` & `vkdispatch-0.0.6/vkdispatch_native/internal.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch_native/stage_compute.cpp` & `vkdispatch-0.0.6/vkdispatch_native/stage_compute.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch_native/stage_compute.h` & `vkdispatch-0.0.6/vkdispatch_native/stage_compute.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch_native/stage_compute.pxd` & `vkdispatch-0.0.6/vkdispatch_native/stage_compute.pxd`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch_native/stage_fft.cpp` & `vkdispatch-0.0.6/vkdispatch_native/stage_fft.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch_native/stage_fft.pxd` & `vkdispatch-0.0.6/vkdispatch_native/stage_fft.pxd`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch_native/stage_transfer.cpp` & `vkdispatch-0.0.6/vkdispatch_native/stage_transfer.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch_native/stage_transfer.h` & `vkdispatch-0.0.6/vkdispatch_native/stage_transfer.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.5/vkdispatch_native/stage_transfer.pxd` & `vkdispatch-0.0.6/vkdispatch_native/stage_transfer.pxd`

 * *Files identical despite different names*

