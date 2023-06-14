# Comparing `tmp/photobooth_app-0.1.0rc5.tar.gz` & `tmp/photobooth_app-0.1.0rc6.tar.gz`

## Comparing `photobooth_app-0.1.0rc5.tar` & `photobooth_app-0.1.0rc6.tar`

### file list

```diff
@@ -1,138 +1,139 @@
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/__init__.py
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/__main__.py
--rw-r--r--   0        0        0    17072 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/appconfig.py
--rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/application.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/containers.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/routers/__init__.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/routers/aquisition.py
--rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/routers/config.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/routers/home.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/routers/log.py
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/routers/mediacollection.py
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/routers/mediaprocessing.py
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/routers/processing.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/routers/sse.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/routers/system.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/__init__.py
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/aquisitionservice.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/baseservice.py
--rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/containers.py
--rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/informationservice.py
--rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/keyboardservice.py
--rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/loggingservice.py
--rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/mediacollectionservice.py
--rw-r--r--   0        0        0    10102 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/mediaprocessingservice.py
--rw-r--r--   0        0        0     8999 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/processingservice.py
--rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/systemservice.py
--rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/wledservice.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/assets/systemservice/boothupload.service
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/assets/systemservice/boothupload.sh
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/assets/systemservice/photobooth-app.service
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/__init__.py
--rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/abstractbackend.py
--rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/containers.py
--rw-r--r--   0        0        0    11212 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/gphoto2.py
--rw-r--r--   0        0        0    16283 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/picamera2.py
--rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/picamera2_libcamafcontinuous.py
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/picamera2_libcamafinterval.py
--rw-r--r--   0        0        0     6965 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/simulated.py
--rw-r--r--   0        0        0    10084 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/webcamcv2.py
--rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/webcamv4l.py
--rw-r--r--   0        0        0    43739 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg
--rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt
--rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf
--rw-r--r--   0        0        0   710982 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg
--rw-r--r--   0        0        0   585221 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg
--rw-r--r--   0        0        0   865667 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg
--rw-r--r--   0        0        0  2314332 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg
--rw-r--r--   0        0        0  2126411 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/mediacollection/__init__.py
--rw-r--r--   0        0        0     6853 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/mediacollection/mediaitem.py
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/mediaprocessing/image_pipelinestages.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/utils/exceptions.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/utils/fastapi_get_openapi.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/utils/helper.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/utils/repeatedtimer.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/utils/stoppablethread.py
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/LICENSE.txt
--rw-r--r--   0        0        0   168060 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf
--rw-r--r--   0        0        0   174108 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf
--rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf
--rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf
--rw-r--r--   0        0        0   170504 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf
--rw-r--r--   0        0        0   167000 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf
--rw-r--r--   0        0        0   173172 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf
--rw-r--r--   0        0        0   168644 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf
--rw-r--r--   0        0        0   173416 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf
--rw-r--r--   0        0        0   168260 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf
--rw-r--r--   0        0        0   168488 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf
--rw-r--r--   0        0        0   172860 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/.gitattributes
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/.gitignore
--rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/CHANGES.md
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/LICENSE.txt
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/MANIFEST.in
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/Makefile
--rw-r--r--   0        0        0    29447 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/README.md
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/make_release.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/setup.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/examples/10_second_macro.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/examples/customizable_hotkey.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/examples/pressed_keys.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/examples/push_to_talk_ubuntu.py
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/examples/segmented_macro.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/examples/simulate_held_down.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/examples/stdin_stdout_events.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/examples/write.py
--rw-r--r--   0        0        0    46771 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/__init__.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/__main__.py
--rw-r--r--   0        0        0    29387 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_canonical_names.py
--rw-r--r--   0        0        0    19352 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_darwinkeyboard.py
--rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_darwinmouse.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_generic.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_keyboard_event.py
--rw-r--r--   0        0        0    36792 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_keyboard_tests.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_mouse_event.py
--rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_mouse_tests.py
--rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_nixcommon.py
--rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_nixkeyboard.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_nixmouse.py
--rw-r--r--   0        0        0    20549 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_winkeyboard.py
--rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_winmouse.py
--rw-r--r--   0        0        0     7608 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/mouse.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/index.html
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/css/272.0be6c807.css
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/css/706.28b224d0.css
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/css/835.eb55e979.css
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/css/app.f5a22106.css
--rw-r--r--   0        0        0   208939 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/css/vendor.46e03c42.css
--rw-r--r--   0        0        0    20436 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
--rw-r--r--   0        0        0    20544 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-r--r--   0        0        0    20416 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-r--r--   0        0        0    20408 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-r--r--   0        0        0    20424 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-r--r--   0        0        0    20344 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-r--r--   0        0        0   164912 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-r--r--   0        0        0   128616 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
--rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/icons/favicon-128x128.png
--rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/icons/logo-notext-black-transparent.png
--rw-r--r--   0        0        0    10435 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/icons/logo-text-black-transparent.png
--rw-r--r--   0        0        0     8328 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/icons/logo-text-white-transparent.png
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/js/247.74c0e45d.js
--rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/js/272.a73245eb.js
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/js/391.70a80bd8.js
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/js/429.76096bfa.js
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/js/546.92b02def.js
--rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/js/705.fc48b137.js
--rw-r--r--   0        0        0     9146 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/js/706.1c5cc1da.js
--rw-r--r--   0        0        0     9742 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/js/835.70f6a199.js
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/js/862.525f2f13.js
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/js/863.e0c5ac02.js
--rw-r--r--   0        0        0     7393 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/js/954.7419ae78.js
--rw-r--r--   0        0        0    12636 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/js/app.64608eed.js
--rw-r--r--   0        0        0  1417500 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/js/vendor.c9e02ba9.js
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/LICENSE.md
--rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/README.md
--rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/pyproject.toml
--rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/PKG-INFO
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/__init__.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/__main__.py
+-rw-r--r--   0        0        0    17627 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/appconfig.py
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/application.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/containers.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/routers/__init__.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/routers/aquisition.py
+-rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/routers/config.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/routers/home.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/routers/log.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/routers/mediacollection.py
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/routers/mediaprocessing.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/routers/processing.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/routers/sse.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/routers/system.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/__init__.py
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/aquisitionservice.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/baseservice.py
+-rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/containers.py
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/gpioservice.py
+-rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/informationservice.py
+-rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/keyboardservice.py
+-rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/loggingservice.py
+-rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/mediacollectionservice.py
+-rw-r--r--   0        0        0    10102 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/mediaprocessingservice.py
+-rw-r--r--   0        0        0     8999 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/processingservice.py
+-rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/systemservice.py
+-rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/wledservice.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/assets/systemservice/boothupload.service
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/assets/systemservice/boothupload.sh
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/assets/systemservice/photobooth-app.service
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/__init__.py
+-rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/abstractbackend.py
+-rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/containers.py
+-rw-r--r--   0        0        0    11212 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/gphoto2.py
+-rw-r--r--   0        0        0    16283 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/picamera2.py
+-rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/picamera2_libcamafcontinuous.py
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/picamera2_libcamafinterval.py
+-rw-r--r--   0        0        0     6965 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/simulated.py
+-rw-r--r--   0        0        0    10084 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/webcamcv2.py
+-rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/webcamv4l.py
+-rw-r--r--   0        0        0    43739 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg
+-rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt
+-rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   710982 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg
+-rw-r--r--   0        0        0   585221 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg
+-rw-r--r--   0        0        0   865667 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg
+-rw-r--r--   0        0        0  2314332 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg
+-rw-r--r--   0        0        0  2126411 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/mediacollection/__init__.py
+-rw-r--r--   0        0        0     6853 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/mediacollection/mediaitem.py
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/mediaprocessing/image_pipelinestages.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/utils/exceptions.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/utils/fastapi_get_openapi.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/utils/helper.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/utils/repeatedtimer.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/utils/stoppablethread.py
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/LICENSE.txt
+-rw-r--r--   0        0        0   168060 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf
+-rw-r--r--   0        0        0   174108 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf
+-rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf
+-rw-r--r--   0        0        0   170504 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf
+-rw-r--r--   0        0        0   167000 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf
+-rw-r--r--   0        0        0   173172 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf
+-rw-r--r--   0        0        0   168644 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf
+-rw-r--r--   0        0        0   173416 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf
+-rw-r--r--   0        0        0   168260 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf
+-rw-r--r--   0        0        0   168488 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf
+-rw-r--r--   0        0        0   172860 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/.gitattributes
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/.gitignore
+-rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/CHANGES.md
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/LICENSE.txt
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/MANIFEST.in
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/Makefile
+-rw-r--r--   0        0        0    29447 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/README.md
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/make_release.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/setup.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/examples/10_second_macro.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/examples/customizable_hotkey.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/examples/pressed_keys.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/examples/push_to_talk_ubuntu.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/examples/segmented_macro.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/examples/simulate_held_down.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/examples/stdin_stdout_events.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/examples/write.py
+-rw-r--r--   0        0        0    46771 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/__init__.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/__main__.py
+-rw-r--r--   0        0        0    29387 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_canonical_names.py
+-rw-r--r--   0        0        0    19352 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_darwinkeyboard.py
+-rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_darwinmouse.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_generic.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_keyboard_event.py
+-rw-r--r--   0        0        0    36792 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_keyboard_tests.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_mouse_event.py
+-rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_mouse_tests.py
+-rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_nixcommon.py
+-rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_nixkeyboard.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_nixmouse.py
+-rw-r--r--   0        0        0    20549 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_winkeyboard.py
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_winmouse.py
+-rw-r--r--   0        0        0     7608 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/mouse.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/index.html
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/css/272.0be6c807.css
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/css/706.28b224d0.css
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/css/835.eb55e979.css
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/css/app.f5a22106.css
+-rw-r--r--   0        0        0   208939 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/css/vendor.46e03c42.css
+-rw-r--r--   0        0        0    20436 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+-rw-r--r--   0        0        0    20544 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-r--r--   0        0        0    20416 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-r--r--   0        0        0    20408 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-r--r--   0        0        0    20424 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-r--r--   0        0        0    20344 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-r--r--   0        0        0   164912 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-r--r--   0        0        0   128616 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
+-rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/icons/favicon-128x128.png
+-rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/icons/logo-notext-black-transparent.png
+-rw-r--r--   0        0        0    10435 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/icons/logo-text-black-transparent.png
+-rw-r--r--   0        0        0     8328 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/icons/logo-text-white-transparent.png
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/js/247.74c0e45d.js
+-rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/js/272.a73245eb.js
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/js/391.70a80bd8.js
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/js/429.76096bfa.js
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/js/546.92b02def.js
+-rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/js/705.fc48b137.js
+-rw-r--r--   0        0        0     9146 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/js/706.1c5cc1da.js
+-rw-r--r--   0        0        0     9742 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/js/835.70f6a199.js
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/js/862.525f2f13.js
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/js/863.e0c5ac02.js
+-rw-r--r--   0        0        0     7393 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/js/954.7419ae78.js
+-rw-r--r--   0        0        0    12636 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/js/app.64608eed.js
+-rw-r--r--   0        0        0  1417500 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/js/vendor.c9e02ba9.js
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/LICENSE.md
+-rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/README.md
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/pyproject.toml
+-rw-r--r--   0        0        0     5119 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/PKG-INFO
```

### Comparing `photobooth_app-0.1.0rc5/photobooth/__main__.py` & `photobooth_app-0.1.0rc6/photobooth/__main__.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/appconfig.py` & `photobooth_app-0.1.0rc6/photobooth/appconfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,14 +350,31 @@
         description="Enable WLED integration for user feedback during countdown and capture by LEDs.",
     )
     wled_serial_port: str = Field(
         default="",
         description="Serial port the WLED device is connected to.",
     )
 
+    # GpioService Config
+    gpio_enabled: bool = Field(
+        default=False,
+        description="Enable Raspberry Pi GPIOzero integration.",
+    )
+    gpio_pin_shutdown: int = Field(
+        default=17,
+        description="GPIO pin to shutdown after holding it for 2 seconds.",
+    )
+    gpio_pin_reboot: int = Field(
+        default=18,
+        description="GPIO pin to reboot after holding it for 2 seconds.",
+    )
+    gpio_pin_take1pic: int = Field(
+        default=27,
+        description="GPIO pin to take one picture.",
+    )
 
 
 class GroupUiSettings(BaseModel):
     """Personalize the booth's UI."""
 
     class Config:
         title = "Personalize the User Interface"
```

### Comparing `photobooth_app-0.1.0rc5/photobooth/application.py` & `photobooth_app-0.1.0rc6/photobooth/application.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/containers.py` & `photobooth_app-0.1.0rc6/photobooth/containers.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/routers/aquisition.py` & `photobooth_app-0.1.0rc6/photobooth/routers/aquisition.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/routers/config.py` & `photobooth_app-0.1.0rc6/photobooth/routers/config.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/routers/home.py` & `photobooth_app-0.1.0rc6/photobooth/routers/home.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/routers/log.py` & `photobooth_app-0.1.0rc6/photobooth/routers/log.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/routers/mediacollection.py` & `photobooth_app-0.1.0rc6/photobooth/routers/mediacollection.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/routers/mediaprocessing.py` & `photobooth_app-0.1.0rc6/photobooth/routers/mediaprocessing.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/routers/processing.py` & `photobooth_app-0.1.0rc6/photobooth/routers/processing.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/routers/sse.py` & `photobooth_app-0.1.0rc6/photobooth/routers/sse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/routers/system.py` & `photobooth_app-0.1.0rc6/photobooth/routers/system.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/services/aquisitionservice.py` & `photobooth_app-0.1.0rc6/photobooth/services/aquisitionservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/services/containers.py` & `photobooth_app-0.1.0rc6/photobooth/services/containers.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import logging
 
 from dependency_injector import containers, providers
 from pymitter import EventEmitter
 
 from ..appconfig import AppConfig
 from .aquisitionservice import AquisitionService
+from .gpioservice import GpioService
 from .informationservice import InformationService
 from .keyboardservice import KeyboardService
 from .mediacollectionservice import MediacollectionService
 from .mediaprocessingservice import MediaprocessingService
 from .processingservice import ProcessingService
 from .systemservice import SystemService
 from .wledservice import WledService
@@ -56,14 +57,21 @@
     else:
         yield resource
         resource.stop()
     finally:
         pass
 
 
+def init_gpio_resource(evtbus, config, processing_service):
+    resource = GpioService(evtbus=evtbus, config=config, processing_service=processing_service)
+    resource.start()
+    yield resource
+    resource.stop()
+
+
 class ServicesContainer(containers.DeclarativeContainer):
     evtbus = providers.Dependency(instance_of=EventEmitter)
     config = providers.Dependency(instance_of=AppConfig)
     backends = providers.DependenciesContainer()
 
     # Services: Core
 
@@ -107,7 +115,14 @@
     system_service = providers.Factory(SystemService, evtbus=evtbus, config=config)
 
     wled_service = providers.Resource(
         init_wled_resource,
         evtbus=evtbus,
         config=config,
     )
+
+    gpio_service = providers.Resource(
+        init_gpio_resource,
+        evtbus=evtbus,
+        config=config,
+        processing_service=processing_service,
+    )
```

### Comparing `photobooth_app-0.1.0rc5/photobooth/services/informationservice.py` & `photobooth_app-0.1.0rc6/photobooth/services/informationservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/services/keyboardservice.py` & `photobooth_app-0.1.0rc6/photobooth/services/keyboardservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/services/loggingservice.py` & `photobooth_app-0.1.0rc6/photobooth/services/loggingservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/services/mediacollectionservice.py` & `photobooth_app-0.1.0rc6/photobooth/services/mediacollectionservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/services/mediaprocessingservice.py` & `photobooth_app-0.1.0rc6/photobooth/services/mediaprocessingservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/services/processingservice.py` & `photobooth_app-0.1.0rc6/photobooth/services/processingservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/services/systemservice.py` & `photobooth_app-0.1.0rc6/photobooth/services/systemservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/services/wledservice.py` & `photobooth_app-0.1.0rc6/photobooth/services/wledservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/services/assets/systemservice/photobooth-app.service` & `photobooth_app-0.1.0rc6/photobooth/services/assets/systemservice/photobooth-app.service`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/services/backends/abstractbackend.py` & `photobooth_app-0.1.0rc6/photobooth/services/backends/abstractbackend.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/services/backends/containers.py` & `photobooth_app-0.1.0rc6/photobooth/services/backends/containers.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/services/backends/gphoto2.py` & `photobooth_app-0.1.0rc6/photobooth/services/backends/gphoto2.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/services/backends/picamera2.py` & `photobooth_app-0.1.0rc6/photobooth/services/backends/picamera2.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/services/backends/picamera2_libcamafcontinuous.py` & `photobooth_app-0.1.0rc6/photobooth/services/backends/picamera2_libcamafcontinuous.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/services/backends/picamera2_libcamafinterval.py` & `photobooth_app-0.1.0rc6/photobooth/services/backends/picamera2_libcamafinterval.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/services/backends/simulated.py` & `photobooth_app-0.1.0rc6/photobooth/services/backends/simulated.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/services/backends/webcamcv2.py` & `photobooth_app-0.1.0rc6/photobooth/services/backends/webcamcv2.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/services/backends/webcamv4l.py` & `photobooth_app-0.1.0rc6/photobooth/services/backends/webcamv4l.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg` & `photobooth_app-0.1.0rc6/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt` & `photobooth_app-0.1.0rc6/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf` & `photobooth_app-0.1.0rc6/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg` & `photobooth_app-0.1.0rc6/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg` & `photobooth_app-0.1.0rc6/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg` & `photobooth_app-0.1.0rc6/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg` & `photobooth_app-0.1.0rc6/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg` & `photobooth_app-0.1.0rc6/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/services/mediacollection/mediaitem.py` & `photobooth_app-0.1.0rc6/photobooth/services/mediacollection/mediaitem.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/services/mediaprocessing/image_pipelinestages.py` & `photobooth_app-0.1.0rc6/photobooth/services/mediaprocessing/image_pipelinestages.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/utils/repeatedtimer.py` & `photobooth_app-0.1.0rc6/photobooth/utils/repeatedtimer.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/utils/stoppablethread.py` & `photobooth_app-0.1.0rc6/photobooth/utils/stoppablethread.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/LICENSE.txt` & `photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf` & `photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf` & `photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf` & `photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf` & `photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf` & `photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf` & `photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf` & `photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf` & `photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf` & `photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf` & `photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf` & `photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf` & `photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/.gitignore` & `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/.gitignore`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/CHANGES.md` & `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/CHANGES.md`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/LICENSE.txt` & `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/Makefile` & `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/Makefile`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/README.md` & `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/README.md`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/make_release.py` & `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/make_release.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/setup.py` & `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/setup.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/examples/push_to_talk_ubuntu.py` & `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/examples/push_to_talk_ubuntu.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/examples/segmented_macro.py` & `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/examples/segmented_macro.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/examples/stdin_stdout_events.py` & `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/examples/stdin_stdout_events.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/__init__.py` & `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/__init__.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_canonical_names.py` & `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_canonical_names.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_darwinkeyboard.py` & `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_darwinkeyboard.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_darwinmouse.py` & `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_darwinmouse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_generic.py` & `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_generic.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_keyboard_event.py` & `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_keyboard_event.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_keyboard_tests.py` & `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_keyboard_tests.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_mouse_tests.py` & `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_mouse_tests.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_nixcommon.py` & `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_nixcommon.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_nixkeyboard.py` & `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_nixkeyboard.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_nixmouse.py` & `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_nixmouse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_winkeyboard.py` & `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_winkeyboard.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_winmouse.py` & `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_winmouse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/mouse.py` & `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/mouse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/web_spa/index.html` & `photobooth_app-0.1.0rc6/photobooth/web_spa/index.html`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/web_spa/css/vendor.46e03c42.css` & `photobooth_app-0.1.0rc6/photobooth/web_spa/css/vendor.46e03c42.css`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `photobooth_app-0.1.0rc6/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `photobooth_app-0.1.0rc6/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `photobooth_app-0.1.0rc6/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `photobooth_app-0.1.0rc6/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `photobooth_app-0.1.0rc6/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `photobooth_app-0.1.0rc6/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `photobooth_app-0.1.0rc6/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2` & `photobooth_app-0.1.0rc6/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/web_spa/icons/favicon-128x128.png` & `photobooth_app-0.1.0rc6/photobooth/web_spa/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/web_spa/icons/logo-notext-black-transparent.png` & `photobooth_app-0.1.0rc6/photobooth/web_spa/icons/logo-notext-black-transparent.png`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/web_spa/icons/logo-text-black-transparent.png` & `photobooth_app-0.1.0rc6/photobooth/web_spa/icons/logo-text-black-transparent.png`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/web_spa/icons/logo-text-white-transparent.png` & `photobooth_app-0.1.0rc6/photobooth/web_spa/icons/logo-text-white-transparent.png`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/web_spa/js/247.74c0e45d.js` & `photobooth_app-0.1.0rc6/photobooth/web_spa/js/247.74c0e45d.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/web_spa/js/272.a73245eb.js` & `photobooth_app-0.1.0rc6/photobooth/web_spa/js/272.a73245eb.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/web_spa/js/391.70a80bd8.js` & `photobooth_app-0.1.0rc6/photobooth/web_spa/js/391.70a80bd8.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/web_spa/js/429.76096bfa.js` & `photobooth_app-0.1.0rc6/photobooth/web_spa/js/429.76096bfa.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/web_spa/js/546.92b02def.js` & `photobooth_app-0.1.0rc6/photobooth/web_spa/js/546.92b02def.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/web_spa/js/705.fc48b137.js` & `photobooth_app-0.1.0rc6/photobooth/web_spa/js/705.fc48b137.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/web_spa/js/706.1c5cc1da.js` & `photobooth_app-0.1.0rc6/photobooth/web_spa/js/706.1c5cc1da.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/web_spa/js/835.70f6a199.js` & `photobooth_app-0.1.0rc6/photobooth/web_spa/js/835.70f6a199.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/web_spa/js/862.525f2f13.js` & `photobooth_app-0.1.0rc6/photobooth/web_spa/js/862.525f2f13.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/web_spa/js/863.e0c5ac02.js` & `photobooth_app-0.1.0rc6/photobooth/web_spa/js/863.e0c5ac02.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/web_spa/js/954.7419ae78.js` & `photobooth_app-0.1.0rc6/photobooth/web_spa/js/954.7419ae78.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/web_spa/js/app.64608eed.js` & `photobooth_app-0.1.0rc6/photobooth/web_spa/js/app.64608eed.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/photobooth/web_spa/js/vendor.c9e02ba9.js` & `photobooth_app-0.1.0rc6/photobooth/web_spa/js/vendor.c9e02ba9.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/LICENSE.md` & `photobooth_app-0.1.0rc6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/README.md` & `photobooth_app-0.1.0rc6/README.md`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc5/pyproject.toml` & `photobooth_app-0.1.0rc6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b70 726f 6a65 6374 5d0d 0a6e 616d 6520  [project]..name 
 00000010: 3d20 2270 686f 746f 626f 6f74 682d 6170  = "photobooth-ap
 00000020: 7022 0d0a 7265 7175 6972 6573 2d70 7974  p"..requires-pyt
 00000030: 686f 6e20 3d20 223e 3d33 2e39 2c3c 332e  hon = ">=3.9,<3.
 00000040: 3132 220d 0a76 6572 7369 6f6e 203d 2022  12"..version = "
-00000050: 302e 312e 3072 6335 220d 0a64 6573 6372  0.1.0rc5"..descr
+00000050: 302e 312e 3072 6336 220d 0a64 6573 6372  0.1.0rc6"..descr
 00000060: 6970 7469 6f6e 203d 2022 5068 6f74 6f62  iption = "Photob
 00000070: 6f6f 7468 2061 7070 2077 7269 7474 656e  ooth app written
 00000080: 2069 6e20 5079 7468 6f6e 2073 7570 706f   in Python suppo
 00000090: 7274 696e 6720 4453 4c52 2c20 7069 6361  rting DSLR, pica
 000000a0: 6d65 7261 322c 2077 6562 6361 6d65 7261  mera2, webcamera
 000000b0: 7322 0d0a 6175 7468 6f72 7320 3d20 5b7b  s"..authors = [{
 000000c0: 206e 616d 6520 3d20 224d 6963 6861 656c   name = "Michael
@@ -81,129 +81,127 @@
 00000500: 2c0d 0a20 2264 6570 656e 6465 6e63 792d  ,.. "dependency-
 00000510: 696e 6a65 6374 6f72 7e3d 342e 3431 2e30  injector~=4.41.0
 00000520: 222c 0d0a 2022 7069 6c67 7261 6d32 7e3d  ",.. "pilgram2~=
 00000530: 322e 302e 3222 2c0d 0a20 2276 346c 3270  2.0.2",.. "v4l2p
 00000540: 797e 3d30 2e36 2e32 3b20 706c 6174 666f  y~=0.6.2; platfo
 00000550: 726d 5f73 7973 7465 6d20 3d3d 2027 4c69  rm_system == 'Li
 00000560: 6e75 7827 222c 0d0a 2022 6770 696f 7a65  nux'",.. "gpioze
-00000570: 726f 7e3d 312e 362e 323b 2070 6c61 7466  ro~=1.6.2; platf
-00000580: 6f72 6d5f 7379 7374 656d 203d 3d20 274c  orm_system == 'L
-00000590: 696e 7578 2722 2c0d 0a20 2267 7068 6f74  inux'",.. "gphot
-000005a0: 6f32 7e3d 322e 332e 343b 2070 6c61 7466  o2~=2.3.4; platf
-000005b0: 6f72 6d5f 7379 7374 656d 203d 3d20 274c  orm_system == 'L
-000005c0: 696e 7578 2722 2c0d 0a20 2270 7974 686f  inux'",.. "pytho
-000005d0: 6e2d 7374 6174 656d 6163 6869 6e65 7e3d  n-statemachine~=
-000005e0: 322e 302e 3022 0d0a 5d0d 0a0d 0a5b 746f  2.0.0"..]....[to
-000005f0: 6f6c 2e68 6174 6368 2e65 6e76 732e 7465  ol.hatch.envs.te
-00000600: 7374 5d0d 0a64 6570 656e 6465 6e63 6965  st]..dependencie
-00000610: 7320 3d20 5b0d 0a20 2022 7079 7465 7374  s = [..  "pytest
-00000620: 7e3d 372e 322e 3022 2c0d 0a20 2022 7079  ~=7.2.0",..  "py
-00000630: 7465 7374 2d62 656e 6368 6d61 726b 7e3d  test-benchmark~=
-00000640: 342e 302e 3022 2c0d 0a20 2022 7079 7465  4.0.0",..  "pyte
-00000650: 7374 2d63 6f76 7e3d 342e 302e 3022 2c0d  st-cov~=4.0.0",.
-00000660: 0a20 2022 7275 6666 7e3d 302e 302e 3237  .  "ruff~=0.0.27
-00000670: 3022 2c0d 0a20 2022 6874 7470 782d 7373  0",..  "httpx-ss
-00000680: 657e 3d30 2e33 2e31 222c 0d0a 2020 2268  e~=0.3.1",..  "h
-00000690: 7474 7078 7e3d 302e 3234 2e31 222c 0d0a  ttpx~=0.24.1",..
-000006a0: 2020 2273 696d 706c 656a 7065 677e 3d31    "simplejpeg~=1
-000006b0: 2e36 2e36 222c 0d0a 2020 2263 6f76 6572  .6.6",..  "cover
-000006c0: 6167 655b 746f 6d6c 5d7e 3d37 2e32 2e37  age[toml]~=7.2.7
-000006d0: 222c 0d0a 2020 2262 6c61 636b 220d 0a5d  ",..  "black"..]
-000006e0: 0d0a 2320 6c69 6263 616d 6572 612f 7069  ..# libcamera/pi
-000006f0: 6361 6d65 7261 3220 6172 6520 6176 6169  camera2 are avai
-00000700: 6c20 666f 7220 6e6f 7720 6f6e 6c79 2061  l for now only a
-00000710: 7320 7379 7374 656d 2070 7974 686f 6e20  s system python 
-00000720: 7061 636b 6167 6520 2d20 6973 6f6c 6174  package - isolat
-00000730: 6564 2065 6e76 2063 616e 6e6f 7420 7573  ed env cannot us
-00000740: 6520 7468 656d 2077 6974 686f 7574 2067  e them without g
-00000750: 6c6f 6261 6c20 6163 6365 7373 0d0a 7379  lobal access..sy
-00000760: 7374 656d 2d70 6163 6b61 6765 7320 3d20  stem-packages = 
-00000770: 7472 7565 0d0a 0d0a 5b74 6f6f 6c2e 6861  true....[tool.ha
-00000780: 7463 682e 656e 7673 2e74 6573 742e 7363  tch.envs.test.sc
-00000790: 7269 7074 735d 0d0a 7465 7374 203d 2022  ripts]..test = "
-000007a0: 7079 7465 7374 202d 7620 2d2d 636f 762d  pytest -v --cov-
-000007b0: 7265 706f 7274 3d74 6572 6d20 2d2d 636f  report=term --co
-000007c0: 762d 7265 706f 7274 3d78 6d6c 3a63 6f76  v-report=xml:cov
-000007d0: 6572 6167 652e 786d 6c20 2d2d 636f 7620  erage.xml --cov 
-000007e0: 2e2f 220d 0a0d 0a0d 0a0d 0a5b 7072 6f6a  ./"........[proj
-000007f0: 6563 742e 7572 6c73 5d0d 0a68 6f6d 6570  ect.urls]..homep
-00000800: 6167 6520 3d20 2268 7474 7073 3a2f 2f67  age = "https://g
-00000810: 6974 6875 622e 636f 6d2f 6d67 726c 2f70  ithub.com/mgrl/p
-00000820: 686f 746f 626f 6f74 682d 6170 7022 0d0a  hotobooth-app"..
-00000830: 7265 706f 7369 746f 7279 203d 2022 6874  repository = "ht
-00000840: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000850: 2f6d 6772 6c2f 7068 6f74 6f62 6f6f 7468  /mgrl/photobooth
-00000860: 2d61 7070 220d 0a64 6f63 756d 656e 7461  -app"..documenta
-00000870: 7469 6f6e 203d 2022 6874 7470 733a 2f2f  tion = "https://
-00000880: 6d67 726c 2e67 6974 6875 622e 696f 2f70  mgrl.github.io/p
-00000890: 686f 746f 626f 6f74 682d 646f 6373 220d  hotobooth-docs".
-000008a0: 0a0d 0a5b 7072 6f6a 6563 742e 7363 7269  ...[project.scri
-000008b0: 7074 735d 0d0a 7068 6f74 6f62 6f6f 7468  pts]..photobooth
-000008c0: 203d 2022 7068 6f74 6f62 6f6f 7468 2e5f   = "photobooth._
-000008d0: 5f6d 6169 6e5f 5f3a 6d61 696e 220d 0a0d  _main__:main"...
-000008e0: 0a5b 746f 6f6c 2e68 6174 6368 2e62 7569  .[tool.hatch.bui
-000008f0: 6c64 5d0d 0a69 6e63 6c75 6465 203d 205b  ld]..include = [
-00000900: 0d0a 2020 222f 7068 6f74 6f62 6f6f 7468  ..  "/photobooth
-00000910: 222c 0d0a 5d0d 0a0d 0a5b 6275 696c 642d  ",..]....[build-
-00000920: 7379 7374 656d 5d0d 0a72 6571 7569 7265  system]..require
-00000930: 7320 3d20 5b22 6861 7463 686c 696e 6722  s = ["hatchling"
-00000940: 5d0d 0a62 7569 6c64 2d62 6163 6b65 6e64  ]..build-backend
-00000950: 203d 2022 6861 7463 686c 696e 672e 6275   = "hatchling.bu
-00000960: 696c 6422 0d0a 0d0a 5b74 6f6f 6c2e 7079  ild"....[tool.py
-00000970: 7465 7374 2e69 6e69 5f6f 7074 696f 6e73  test.ini_options
-00000980: 5d0d 0a6c 6f67 5f63 6c69 203d 2074 7275  ]..log_cli = tru
-00000990: 650d 0a6c 6f67 5f63 6c69 5f6c 6576 656c  e..log_cli_level
-000009a0: 203d 2022 4445 4255 4722 0d0a 6c6f 675f   = "DEBUG"..log_
-000009b0: 636c 695f 666f 726d 6174 203d 2022 2528  cli_format = "%(
-000009c0: 6173 6374 696d 6529 7320 5b25 286c 6576  asctime)s [%(lev
-000009d0: 656c 6e61 6d65 2938 735d 2025 286d 6573  elname)8s] %(mes
-000009e0: 7361 6765 2973 2028 2528 6669 6c65 6e61  sage)s (%(filena
-000009f0: 6d65 2973 3a25 286c 696e 656e 6f29 7329  me)s:%(lineno)s)
-00000a00: 220d 0a6c 6f67 5f63 6c69 5f64 6174 655f  "..log_cli_date_
-00000a10: 666f 726d 6174 203d 2022 2559 2d25 6d2d  format = "%Y-%m-
-00000a20: 2564 2025 483a 254d 3a25 5322 0d0a 0d0a  %d %H:%M:%S"....
-00000a30: 5b74 6f6f 6c2e 636f 7665 7261 6765 2e72  [tool.coverage.r
-00000a40: 756e 5d0d 0a23 2064 6973 6162 6c65 2063  un]..# disable c
-00000a50: 6f75 6c64 6e74 2d70 6172 7365 3a20 6874  ouldnt-parse: ht
-00000a60: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000a70: 2f6e 6564 6261 742f 636f 7665 7261 6765  /nedbat/coverage
-00000a80: 7079 2f69 7373 7565 732f 3133 3932 0d0a  py/issues/1392..
-00000a90: 6469 7361 626c 655f 7761 726e 696e 6773  disable_warnings
-00000aa0: 203d 205b 2263 6f75 6c64 6e74 2d70 6172   = ["couldnt-par
-00000ab0: 7365 225d 0d0a 6f6d 6974 203d 205b 0d0a  se"]..omit = [..
-00000ac0: 2020 2020 2274 6573 745f 2a2e 7079 222c      "test_*.py",
-00000ad0: 0d0a 2020 2020 222e 2f74 6573 7473 2f2a  ..    "./tests/*
-00000ae0: 222c 0d0a 2020 2020 222e 2f70 686f 746f  ",..    "./photo
-00000af0: 626f 6f74 682f 7665 6e64 6f72 2f2a 220d  booth/vendor/*".
-00000b00: 0a20 2020 205d 0d0a 7061 7261 6c6c 656c  .    ]..parallel
-00000b10: 203d 2074 7275 650d 0a63 6f6e 6375 7272   = true..concurr
-00000b20: 656e 6379 203d 205b 2274 6872 6561 6422  ency = ["thread"
-00000b30: 2c22 6d75 6c74 6970 726f 6365 7373 696e  ,"multiprocessin
-00000b40: 6722 5d0d 0a0d 0a5b 746f 6f6c 2e62 6c61  g"]....[tool.bla
-00000b50: 636b 5d0d 0a6c 696e 652d 6c65 6e67 7468  ck]..line-length
-00000b60: 203d 2031 3230 0d0a 0d0a 5b74 6f6f 6c2e   = 120....[tool.
-00000b70: 7275 6666 5d0d 0a6c 696e 652d 6c65 6e67  ruff]..line-leng
-00000b80: 7468 203d 2031 3230 0d0a 7365 6c65 6374  th = 120..select
-00000b90: 203d 205b 0d0a 2020 2245 222c 2020 2023   = [..  "E",   #
-00000ba0: 2070 7963 6f64 6573 7479 6c65 0d0a 2020   pycodestyle..  
-00000bb0: 2257 222c 2020 2023 2070 7963 6f64 6573  "W",   # pycodes
-00000bc0: 7479 6c65 0d0a 2020 2246 222c 2020 2023  tyle..  "F",   #
-00000bd0: 2070 7966 6c61 6b65 730d 0a20 2022 4222   pyflakes..  "B"
-00000be0: 2c20 2020 2320 6275 6762 6561 720d 0a20  ,   # bugbear.. 
-00000bf0: 2022 5550 222c 2020 2320 7079 7570 6772   "UP",  # pyupgr
-00000c00: 6164 650d 0a20 2022 4922 2c20 2020 2320  ade..  "I",   # 
-00000c10: 6973 6f72 740d 0a20 2023 2244 222c 2020  isort..  #"D",  
-00000c20: 2023 2070 7964 6f63 7374 796c 6520 2020   # pydocstyle   
-00000c30: 2320 6164 6420 6c61 7465 720d 0a5d 0d0a  # add later..]..
-00000c40: 6967 6e6f 7265 203d 205b 0d0a 2020 2242  ignore = [..  "B
-00000c50: 3030 3822 2023 7573 6564 2066 6f72 2044  008" #used for D
-00000c60: 4920 696e 6a65 6374 696f 6e0d 0a20 205d  I injection..  ]
-00000c70: 0d0a 6578 7465 6e64 2d65 7863 6c75 6465  ..extend-exclude
-00000c80: 203d 205b 2276 656e 646f 7222 5d0d 0a0d   = ["vendor"]...
-00000c90: 0a5b 746f 6f6c 2e72 7566 662e 7065 722d  .[tool.ruff.per-
-00000ca0: 6669 6c65 2d69 676e 6f72 6573 5d0d 0a22  file-ignores].."
-00000cb0: 7068 6f74 6f62 6f6f 7468 2f61 7070 636f  photobooth/appco
-00000cc0: 6e66 6967 2e70 7922 203d 205b 2245 3530  nfig.py" = ["E50
-00000cd0: 3122 5d0d 0a0d 0a5b 746f 6f6c 2e72 7566  1"]....[tool.ruf
-00000ce0: 662e 7079 646f 6373 7479 6c65 5d0d 0a63  f.pydocstyle]..c
-00000cf0: 6f6e 7665 6e74 696f 6e20 3d20 2267 6f6f  onvention = "goo
-00000d00: 676c 6522                                gle"
+00000570: 726f 7e3d 312e 362e 3222 2c0d 0a20 2267  ro~=1.6.2",.. "g
+00000580: 7068 6f74 6f32 7e3d 322e 332e 343b 2070  photo2~=2.3.4; p
+00000590: 6c61 7466 6f72 6d5f 7379 7374 656d 203d  latform_system =
+000005a0: 3d20 274c 696e 7578 2722 2c0d 0a20 2270  = 'Linux'",.. "p
+000005b0: 7974 686f 6e2d 7374 6174 656d 6163 6869  ython-statemachi
+000005c0: 6e65 7e3d 322e 302e 3022 0d0a 5d0d 0a0d  ne~=2.0.0"..]...
+000005d0: 0a5b 746f 6f6c 2e68 6174 6368 2e65 6e76  .[tool.hatch.env
+000005e0: 732e 7465 7374 5d0d 0a64 6570 656e 6465  s.test]..depende
+000005f0: 6e63 6965 7320 3d20 5b0d 0a20 2022 7079  ncies = [..  "py
+00000600: 7465 7374 7e3d 372e 322e 3022 2c0d 0a20  test~=7.2.0",.. 
+00000610: 2022 7079 7465 7374 2d62 656e 6368 6d61   "pytest-benchma
+00000620: 726b 7e3d 342e 302e 3022 2c0d 0a20 2022  rk~=4.0.0",..  "
+00000630: 7079 7465 7374 2d63 6f76 7e3d 342e 302e  pytest-cov~=4.0.
+00000640: 3022 2c0d 0a20 2022 7275 6666 7e3d 302e  0",..  "ruff~=0.
+00000650: 302e 3237 3022 2c0d 0a20 2022 6874 7470  0.270",..  "http
+00000660: 782d 7373 657e 3d30 2e33 2e31 222c 0d0a  x-sse~=0.3.1",..
+00000670: 2020 2268 7474 7078 7e3d 302e 3234 2e31    "httpx~=0.24.1
+00000680: 222c 0d0a 2020 2273 696d 706c 656a 7065  ",..  "simplejpe
+00000690: 677e 3d31 2e36 2e36 222c 0d0a 2020 2263  g~=1.6.6",..  "c
+000006a0: 6f76 6572 6167 655b 746f 6d6c 5d7e 3d37  overage[toml]~=7
+000006b0: 2e32 2e37 222c 0d0a 2020 2262 6c61 636b  .2.7",..  "black
+000006c0: 220d 0a5d 0d0a 2320 6c69 6263 616d 6572  "..]..# libcamer
+000006d0: 612f 7069 6361 6d65 7261 3220 6172 6520  a/picamera2 are 
+000006e0: 6176 6169 6c20 666f 7220 6e6f 7720 6f6e  avail for now on
+000006f0: 6c79 2061 7320 7379 7374 656d 2070 7974  ly as system pyt
+00000700: 686f 6e20 7061 636b 6167 6520 2d20 6973  hon package - is
+00000710: 6f6c 6174 6564 2065 6e76 2063 616e 6e6f  olated env canno
+00000720: 7420 7573 6520 7468 656d 2077 6974 686f  t use them witho
+00000730: 7574 2067 6c6f 6261 6c20 6163 6365 7373  ut global access
+00000740: 0d0a 7379 7374 656d 2d70 6163 6b61 6765  ..system-package
+00000750: 7320 3d20 7472 7565 0d0a 0d0a 5b74 6f6f  s = true....[too
+00000760: 6c2e 6861 7463 682e 656e 7673 2e74 6573  l.hatch.envs.tes
+00000770: 742e 7363 7269 7074 735d 0d0a 7465 7374  t.scripts]..test
+00000780: 203d 2022 7079 7465 7374 202d 7620 2d2d   = "pytest -v --
+00000790: 636f 762d 7265 706f 7274 3d74 6572 6d20  cov-report=term 
+000007a0: 2d2d 636f 762d 7265 706f 7274 3d78 6d6c  --cov-report=xml
+000007b0: 3a63 6f76 6572 6167 652e 786d 6c20 2d2d  :coverage.xml --
+000007c0: 636f 7620 2e2f 220d 0a0d 0a0d 0a0d 0a5b  cov ./"........[
+000007d0: 7072 6f6a 6563 742e 7572 6c73 5d0d 0a68  project.urls]..h
+000007e0: 6f6d 6570 6167 6520 3d20 2268 7474 7073  omepage = "https
+000007f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d67  ://github.com/mg
+00000800: 726c 2f70 686f 746f 626f 6f74 682d 6170  rl/photobooth-ap
+00000810: 7022 0d0a 7265 706f 7369 746f 7279 203d  p"..repository =
+00000820: 2022 6874 7470 733a 2f2f 6769 7468 7562   "https://github
+00000830: 2e63 6f6d 2f6d 6772 6c2f 7068 6f74 6f62  .com/mgrl/photob
+00000840: 6f6f 7468 2d61 7070 220d 0a64 6f63 756d  ooth-app"..docum
+00000850: 656e 7461 7469 6f6e 203d 2022 6874 7470  entation = "http
+00000860: 733a 2f2f 6d67 726c 2e67 6974 6875 622e  s://mgrl.github.
+00000870: 696f 2f70 686f 746f 626f 6f74 682d 646f  io/photobooth-do
+00000880: 6373 220d 0a0d 0a5b 7072 6f6a 6563 742e  cs"....[project.
+00000890: 7363 7269 7074 735d 0d0a 7068 6f74 6f62  scripts]..photob
+000008a0: 6f6f 7468 203d 2022 7068 6f74 6f62 6f6f  ooth = "photoboo
+000008b0: 7468 2e5f 5f6d 6169 6e5f 5f3a 6d61 696e  th.__main__:main
+000008c0: 220d 0a0d 0a5b 746f 6f6c 2e68 6174 6368  "....[tool.hatch
+000008d0: 2e62 7569 6c64 5d0d 0a69 6e63 6c75 6465  .build]..include
+000008e0: 203d 205b 0d0a 2020 222f 7068 6f74 6f62   = [..  "/photob
+000008f0: 6f6f 7468 222c 0d0a 5d0d 0a0d 0a5b 6275  ooth",..]....[bu
+00000900: 696c 642d 7379 7374 656d 5d0d 0a72 6571  ild-system]..req
+00000910: 7569 7265 7320 3d20 5b22 6861 7463 686c  uires = ["hatchl
+00000920: 696e 6722 5d0d 0a62 7569 6c64 2d62 6163  ing"]..build-bac
+00000930: 6b65 6e64 203d 2022 6861 7463 686c 696e  kend = "hatchlin
+00000940: 672e 6275 696c 6422 0d0a 0d0a 5b74 6f6f  g.build"....[too
+00000950: 6c2e 7079 7465 7374 2e69 6e69 5f6f 7074  l.pytest.ini_opt
+00000960: 696f 6e73 5d0d 0a6c 6f67 5f63 6c69 203d  ions]..log_cli =
+00000970: 2074 7275 650d 0a6c 6f67 5f63 6c69 5f6c   true..log_cli_l
+00000980: 6576 656c 203d 2022 4445 4255 4722 0d0a  evel = "DEBUG"..
+00000990: 6c6f 675f 636c 695f 666f 726d 6174 203d  log_cli_format =
+000009a0: 2022 2528 6173 6374 696d 6529 7320 5b25   "%(asctime)s [%
+000009b0: 286c 6576 656c 6e61 6d65 2938 735d 2025  (levelname)8s] %
+000009c0: 286d 6573 7361 6765 2973 2028 2528 6669  (message)s (%(fi
+000009d0: 6c65 6e61 6d65 2973 3a25 286c 696e 656e  lename)s:%(linen
+000009e0: 6f29 7329 220d 0a6c 6f67 5f63 6c69 5f64  o)s)"..log_cli_d
+000009f0: 6174 655f 666f 726d 6174 203d 2022 2559  ate_format = "%Y
+00000a00: 2d25 6d2d 2564 2025 483a 254d 3a25 5322  -%m-%d %H:%M:%S"
+00000a10: 0d0a 0d0a 5b74 6f6f 6c2e 636f 7665 7261  ....[tool.covera
+00000a20: 6765 2e72 756e 5d0d 0a23 2064 6973 6162  ge.run]..# disab
+00000a30: 6c65 2063 6f75 6c64 6e74 2d70 6172 7365  le couldnt-parse
+00000a40: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+00000a50: 2e63 6f6d 2f6e 6564 6261 742f 636f 7665  .com/nedbat/cove
+00000a60: 7261 6765 7079 2f69 7373 7565 732f 3133  ragepy/issues/13
+00000a70: 3932 0d0a 6469 7361 626c 655f 7761 726e  92..disable_warn
+00000a80: 696e 6773 203d 205b 2263 6f75 6c64 6e74  ings = ["couldnt
+00000a90: 2d70 6172 7365 225d 0d0a 6f6d 6974 203d  -parse"]..omit =
+00000aa0: 205b 0d0a 2020 2020 2274 6573 745f 2a2e   [..    "test_*.
+00000ab0: 7079 222c 0d0a 2020 2020 222e 2f74 6573  py",..    "./tes
+00000ac0: 7473 2f2a 222c 0d0a 2020 2020 222e 2f70  ts/*",..    "./p
+00000ad0: 686f 746f 626f 6f74 682f 7665 6e64 6f72  hotobooth/vendor
+00000ae0: 2f2a 220d 0a20 2020 205d 0d0a 7061 7261  /*"..    ]..para
+00000af0: 6c6c 656c 203d 2074 7275 650d 0a63 6f6e  llel = true..con
+00000b00: 6375 7272 656e 6379 203d 205b 2274 6872  currency = ["thr
+00000b10: 6561 6422 2c22 6d75 6c74 6970 726f 6365  ead","multiproce
+00000b20: 7373 696e 6722 5d0d 0a0d 0a5b 746f 6f6c  ssing"]....[tool
+00000b30: 2e62 6c61 636b 5d0d 0a6c 696e 652d 6c65  .black]..line-le
+00000b40: 6e67 7468 203d 2031 3230 0d0a 0d0a 5b74  ngth = 120....[t
+00000b50: 6f6f 6c2e 7275 6666 5d0d 0a6c 696e 652d  ool.ruff]..line-
+00000b60: 6c65 6e67 7468 203d 2031 3230 0d0a 7365  length = 120..se
+00000b70: 6c65 6374 203d 205b 0d0a 2020 2245 222c  lect = [..  "E",
+00000b80: 2020 2023 2070 7963 6f64 6573 7479 6c65     # pycodestyle
+00000b90: 0d0a 2020 2257 222c 2020 2023 2070 7963  ..  "W",   # pyc
+00000ba0: 6f64 6573 7479 6c65 0d0a 2020 2246 222c  odestyle..  "F",
+00000bb0: 2020 2023 2070 7966 6c61 6b65 730d 0a20     # pyflakes.. 
+00000bc0: 2022 4222 2c20 2020 2320 6275 6762 6561   "B",   # bugbea
+00000bd0: 720d 0a20 2022 5550 222c 2020 2320 7079  r..  "UP",  # py
+00000be0: 7570 6772 6164 650d 0a20 2022 4922 2c20  upgrade..  "I", 
+00000bf0: 2020 2320 6973 6f72 740d 0a20 2023 2244    # isort..  #"D
+00000c00: 222c 2020 2023 2070 7964 6f63 7374 796c  ",   # pydocstyl
+00000c10: 6520 2020 2320 6164 6420 6c61 7465 720d  e   # add later.
+00000c20: 0a5d 0d0a 6967 6e6f 7265 203d 205b 0d0a  .]..ignore = [..
+00000c30: 2020 2242 3030 3822 2023 7573 6564 2066    "B008" #used f
+00000c40: 6f72 2044 4920 696e 6a65 6374 696f 6e0d  or DI injection.
+00000c50: 0a20 205d 0d0a 6578 7465 6e64 2d65 7863  .  ]..extend-exc
+00000c60: 6c75 6465 203d 205b 2276 656e 646f 7222  lude = ["vendor"
+00000c70: 5d0d 0a0d 0a5b 746f 6f6c 2e72 7566 662e  ]....[tool.ruff.
+00000c80: 7065 722d 6669 6c65 2d69 676e 6f72 6573  per-file-ignores
+00000c90: 5d0d 0a22 7068 6f74 6f62 6f6f 7468 2f61  ].."photobooth/a
+00000ca0: 7070 636f 6e66 6967 2e70 7922 203d 205b  ppconfig.py" = [
+00000cb0: 2245 3530 3122 5d0d 0a0d 0a5b 746f 6f6c  "E501"]....[tool
+00000cc0: 2e72 7566 662e 7079 646f 6373 7479 6c65  .ruff.pydocstyle
+00000cd0: 5d0d 0a63 6f6e 7665 6e74 696f 6e20 3d20  ]..convention = 
+00000ce0: 2267 6f6f 676c 6522                      "google"
```

### Comparing `photobooth_app-0.1.0rc5/PKG-INFO` & `photobooth_app-0.1.0rc6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photobooth-app
-Version: 0.1.0rc5
+Version: 0.1.0rc6
 Summary: Photobooth app written in Python supporting DSLR, picamera2, webcameras
 Project-URL: homepage, https://github.com/mgrl/photobooth-app
 Project-URL: repository, https://github.com/mgrl/photobooth-app
 Project-URL: documentation, https://mgrl.github.io/photobooth-docs
 Author-email: Michael G <me@mgrl.de>
 Maintainer-email: Michael G <me@mgrl.de>
 License-File: LICENSE.md
@@ -18,15 +18,15 @@
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Graphics :: Capture :: Digital Camera
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: <3.12,>=3.9
 Requires-Dist: dependency-injector~=4.41.0
 Requires-Dist: fastapi<0.97.0,>=0.95.2
 Requires-Dist: gphoto2~=2.3.4; platform_system == 'Linux'
-Requires-Dist: gpiozero~=1.6.2; platform_system == 'Linux'
+Requires-Dist: gpiozero~=1.6.2
 Requires-Dist: jsonref~=1.1.0
 Requires-Dist: opencv-python~=4.7.0
 Requires-Dist: piexif~=1.1.3
 Requires-Dist: pilgram2~=2.0.2
 Requires-Dist: pillow~=9.5.0
 Requires-Dist: psutil~=5.9.5
 Requires-Dist: pydantic~=1.10.8
```

