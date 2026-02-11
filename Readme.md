This is a 2026 refresh of https://github.com/sfalexrog/Imgui_Android/tree/master.
The principal product is an Android app that runs the default imgui demo using OpenGL3 as the renderer
backend and SDL3 as the platform backend.

### Local machine config:
- installed sdk: Android 16 Baklava; API level 36
- installed ndk: 28.2.13676358
- Tested build environment 1:
    - 2019 Intel Mac 
    - OS: Mac OS X 15.5
    - Java: Oracle corp. JDK 25.0.1
- Tested build environment 2:
    - OS: Debian Linux
    - Java: OpenJDK 17.0.18

### Setup:
- download this repo (and its dependencies: SDL3 and imgui) to your computer by running
`git clone --recursive https://github.com/brentfpage/android_imgui_sdl3_opengl3_template.git`
- change sdk.dir in local.properties to point to the Android sdk on your computer
- possibly, run `chmod +700 gradlew` from the repo home directory to make gradlew executable
- to minimize headaches, update java and the android ndk and sdk on your computer to the versions stated above

### Build and install:
- connect your Android device to your computer
- from the repo home directory, run `run ./gradlew -DANDROID installDebug`

