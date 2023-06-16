# Legacy-LWJGL3
Patched version of LWJGL3 to work alongside a LWJGL2 project. This means that you can use features from LWJGL3 in a LWJGL2 project such as NanoVG and other LWJGL3 modules. All modules have been built for Legacy-LWJGL3 but not all of them have been tested to work correctly with LWJGL2. Feel free to open an issue if you find a module that doesn't!

## Usage
```groovy
// Add the Jitpack repository
repositories {
    maven {
        name = 'Jitpack'
        url = 'https://jitpack.io'
    }
}

// Define LWJGL and Legacy-LWJGL versions
// Update this to use the latest version/patch
def lwjglVersion = '3.3.2' // LWJGL3 version, see the GitHub releases page for versions patched
def legacyLwjglPatch = '5' // Legacy-LWJGL3 patch, you should always use the latest patch

// Add Legacy-LWJGL3 to your dependencies
dependencies {
    implementation "io.waterwave.Legacy-LWJGL3:lwjgl:${lwjglVersion}-${legacyLwjglPatch}" // core (required, what did you expect?)
    implementation "io.waterwave.Legacy-LWJGL3:lwjgl-stb:${lwjglVersion}-${legacyLwjglPatch}" // stb (required for nanovg)
    implementation "io.waterwave.Legacy-LWJGL3:lwjgl-nanovg:${lwjglVersion}-${legacyLwjglPatch}" // nanovg
}
```

## Notes
I ([yolocat](https://github.com/yolocat-dev)) have not created the code used nor am I seeing this as mine, but only modified parts of the code to make it compatible with [LWJGL2](https://github.com/LWJGL/lwjgl). Full credits for [LWJGL](https://github.com/LWJGL) (both [2](https://github.com/LWJGL/lwjgl) and [3](https://github.com/LWJGL/lwjgl3)) goes to the over 40 collaborators who have spent their time on such an awesome open-source project.

## Licenses
All licenses for LWJGL and its modules can be found in the [licenses](https://github.com/WaterwaveMC/Legacy-LWJGL3/tree/master/licenses) folder, with `LICENSE` being the LWJGL license and all other licenses coming from its respecting modules (`*_license.txt`).
