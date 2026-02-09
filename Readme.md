This is a 2026 refresh of https://github.com/sfalexrog/Imgui_Android/tree/master.
The principal product is an Android app that runs the default imgui demo using OpenGL3 as the renderer
backend and SDL3 as the platform backend.
app/src/main/cpp/main.cpp has been copied from cpp/deps/imgui/examples/example_sdl3_opengl3/main.cpp

### Local machine config:
    - installed sdk: Android 16 Baklava; API level 36
    - installed ndk: 28.2.13676358
    - output of `./gradlew --version`
    ```
    ------------------------------------------------------------
    Gradle 9.1.0
    ------------------------------------------------------------

    Build time:    2025-09-18 13:05:56 UTC
    Revision:      e45a8dbf2470c2e2474ccc25be9f49331406a07e

    Kotlin:        2.2.0
    Groovy:        4.0.28
    Ant:           Apache Ant(TM) version 1.10.15 compiled on August 25 2024
    Launcher JVM:  25.0.1 (Oracle Corporation 25.0.1+8-LTS-27)
    Daemon JVM:    /Library/Java/JavaVirtualMachines/jdk-25.jdk/Contents/Home (no JDK specified, using current Java home)
    OS:            Mac OS X 15.5 x86_64
    ```
    - Android Studio version: Otter 3 Feature Drop | 2025.2.3
        - conceivably, it is sufficient to just have the ndk, sdk, java, and gradle installed

### Setup:
    - change sdk.dir in local.properties to point to the Android sdk on your computer
    - possibly, run `chmod +700 gradlew` from the repo home directory to make gradlew executable
    - to minimize headaches, update java and the android ndk and sdk on your computer to the versions stated above

### Build and install:
    - connect your Android device to your computer
    - from the repo home directory, run `run ./gradlew -DANDROID installDebug`

