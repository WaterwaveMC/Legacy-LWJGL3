# Legacy-LWJGL3
Patched version of LWJGL for NanoVG to work with LWJGL2.

## Usage
```groovy
# Add the Jitpack repository
repositories {
    maven {
        name = 'Jitpack'
        url = 'https://jitpack.io'
    }
}

# Add Legacy-LWJGL3 to your dependencies
dependencies {
    implementation 'io.waterwave:Legacy-LWJGL3:3.1.1'
}
```

## Notes
I ([yolocat](https://github.com/yolocat-dev)) have not modified nor created the code used but only moved/removed code to make it compatible with [LWJGL2](https://github.com/LWJGL/lwjgl). Full credits for [LWJGL](https://github.com/LWJGL) (both [2](https://github.com/LWJGL/lwjgl) and [3](https://github.com/LWJGL/lwjgl3)) goes to the over 40 collaborators.
