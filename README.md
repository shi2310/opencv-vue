# OpenCV-Vue

opencv 在 vue 中的简单使用.

opencv 信息

```
-----------------------------------------------------------------
General configuration for OpenCV 3.3.1-dev =====================================
  Version control:               3.3.1-1-g21c8e6d-dirty

  Platform:
    Timestamp:                   2017-11-01T08:05:43Z
    Host:                        Linux 4.4.0-97-generic x86_64
    Target:                      Emscripten 1 x86
    CMake:                       3.5.2
    CMake generator:             Unix Makefiles
    CMake build tool:            /usr/bin/make
    Configuration:               Release

  CPU/HW features:
    Baseline:

  C/C++:
    Built as dynamic libs?:      NO
    C++ Compiler:                /home/sajjad/emsdk-portable/emscripten/incoming/em++  (ver 4.0.0)
    C++ flags (Release):         -fPIC   -fsigned-char -W -Wall -Werror=return-type -Werror=non-virtual-dtor -Werror=address -Werror=sequence-point -Wformat -Werror=format-security -Wmissing-declarations -Wmissing-prototypes -Wstrict-prototypes -Wundef -Winit-self -Wpointer-arith -Wshadow -Wsign-promo -Wuninitialized -Winit-self -Wno-narrowing -Wno-delete-non-virtual-dtor -Wno-unnamed-type-template-args -Wno-comment -Wno-implicit-fallthrough -fdiagnostics-show-option -pthread -Qunused-arguments -march=i686 -fomit-frame-pointer -ffunction-sections  -fvisibility=hidden -fvisibility-inlines-hidden -DNDEBUG -O2  -DNDEBUG
    C++ flags (Debug):           -fPIC   -fsigned-char -W -Wall -Werror=return-type -Werror=non-virtual-dtor -Werror=address -Werror=sequence-point -Wformat -Werror=format-security -Wmissing-declarations -Wmissing-prototypes -Wstrict-prototypes -Wundef -Winit-self -Wpointer-arith -Wshadow -Wsign-promo -Wuninitialized -Winit-self -Wno-narrowing -Wno-delete-non-virtual-dtor -Wno-unnamed-type-template-args -Wno-comment -Wno-implicit-fallthrough -fdiagnostics-show-option -pthread -Qunused-arguments -march=i686 -fomit-frame-pointer -ffunction-sections  -fvisibility=hidden -fvisibility-inlines-hidden -g  -O0 -DDEBUG -D_DEBUG
    C Compiler:                  /home/sajjad/emsdk-portable/emscripten/incoming/emcc
    C flags (Release):           -fPIC   -fsigned-char -W -Wall -Werror=return-type -Werror=non-virtual-dtor -Werror=address -Werror=sequence-point -Wformat -Werror=format-security -Wmissing-declarations -Wmissing-prototypes -Wstrict-prototypes -Wundef -Winit-self -Wpointer-arith -Wshadow -Wsign-promo -Wuninitialized -Winit-self -Wno-narrowing -Wno-delete-non-virtual-dtor -Wno-unnamed-type-template-args -Wno-comment -Wno-implicit-fallthrough -fdiagnostics-show-option -pthread -Qunused-arguments -march=i686 -fomit-frame-pointer -ffunction-sections  -fvisibility=hidden -fvisibility-inlines-hidden -DNDEBUG -O2  -DNDEBUG
    C flags (Debug):             -fPIC   -fsigned-char -W -Wall -Werror=return-type -Werror=non-virtual-dtor -Werror=address -Werror=sequence-point -Wformat -Werror=format-security -Wmissing-declarations -Wmissing-prototypes -Wstrict-prototypes -Wundef -Winit-self -Wpointer-arith -Wshadow -Wsign-promo -Wuninitialized -Winit-self -Wno-narrowing -Wno-delete-non-virtual-dtor -Wno-unnamed-type-template-args -Wno-comment -Wno-implicit-fallthrough -fdiagnostics-show-option -pthread -Qunused-arguments -march=i686 -fomit-frame-pointer -ffunction-sections  -fvisibility=hidden -fvisibility-inlines-hidden -g  -O0 -DDEBUG -D_DEBUG
    Linker flags (Release):      -O2
    Linker flags (Debug):
    ccache:                      YES
    Precompiled headers:         NO
    Extra dependencies:          stdc++
    3rdparty dependencies:       zlib libjpeg

  OpenCV modules:
    To be built:                 core imgproc objdetect video imgcodecs highgui features2d js
    Disabled:                    calib3d flann ml photo shape stitching superres videoio videostab world
    Disabled by dependency:      -
    Unavailable:                 cudaarithm cudabgsegm cudacodec cudafeatures2d cudafilters cudaimgproc cudalegacy cudaobjdetect cudaoptflow cudastereo cudawarping cudev java python2 python3 ts viz

  GUI:
    QT:                          NO
    GTK+:                        NO
    GThread :                    NO
    GtkGlExt:                    NO
    OpenGL support:              NO
    VTK support:                 NO

  Media I/O:
    ZLib:                        build (ver 1.2.8)
    JPEG:                        build (ver 90)
    WEBP:                        NO
    PNG:                         NO
    TIFF:                        NO
    JPEG 2000:                   NO
    OpenEXR:                     NO
    GDAL:                        NO
    GDCM:                        NO

  Video I/O:
    DC1394 1.x:                  NO
    DC1394 2.x:                  NO
    FFMPEG:                      NO
      avcodec:                   NO
      avformat:                  NO
      avutil:                    NO
      swscale:                   NO
      avresample:                NO
    GStreamer:                   NO
    OpenNI:                      NO
    OpenNI PrimeSensor Modules:  NO
    OpenNI2:                     NO
    PvAPI:                       NO
    GigEVisionSDK:               NO
    Aravis SDK:                  NO
    UniCap:                      NO
    UniCap ucil:                 NO
    V4L/V4L2:                    NO/NO
    XIMEA:                       NO
    Xine:                        NO
    Intel Media SDK:             NO
    gPhoto2:                     NO

  Parallel framework:            none

  Other third-party libraries:
    Use Intel IPP:               NO
    Use Intel IPP IW:            NO
    Use VA:                      NO
    Use Intel VA-API/OpenCL:     NO
    Use Lapack:                  NO
    Use Eigen:                   NO
    Use Cuda:                    NO
    Use OpenCL:                  NO
    Use OpenVX:                  NO
    Use custom HAL:              NO

  Python 2:
    Interpreter:                 /usr/bin/python2.7 (ver 2.7.12)

  Python 3:
    Interpreter:                 /usr/bin/python3 (ver 3.5.2)

  Python (for build):            /usr/bin/python2.7

  Java:
    ant:                         /usr/bin/ant (ver 1.9.6)
    JNI:                         NO
    Java wrappers:               NO
    Java tests:                  NO

  Matlab:                        NO

  Tests and samples:
    Tests:                       NO
    Performance tests:           NO
    C/C++ Examples:              NO

  Install path:                  /home/sajjad/opencv/build_js/install

  cvconfig.h is in:              /home/sajjad/opencv/build_js
-----------------------------------------------------------------
```

- Tested with opencv.js version 4.0.0
