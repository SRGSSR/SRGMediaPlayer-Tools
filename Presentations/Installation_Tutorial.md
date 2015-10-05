# Android

## Requirements
- Android Studio (recommended 1.4)
- Android SDK 21
- A device (API 15, recommended > 16)
- An emulator (recommended: genymotion with the Device: Google Nexus 5 - 5.1.0 - API 22 - 1080x1920)

## Repositories
### Mandatory
- https://github.com/SRGSSR/SRGMediaPlayer-Android

### Optional
- https://github.com/rtsmb/ExoPlayer (just for information, binaries are already integrated in the library above)

## Setup
- Create a project in a folder along side SRGMediaPlayer-Android to have the following directory structure:

```
mediaplayerProjects/SRGMediaPlayer-Android
mediaplayerProjects/myProject
```
- Edit your settings.gradle:

```
include 'MY_PROJECT', ':srgmediaplayer', ':segmentOverlay', ':srgmediaplayer-extras', ':srgmediaplayer-service'

project(':srgmediaplayer').projectDir = new File(settingsDir, '../SRGMediaPlayer-Android/srgmediaplayer')
project(':segmentOverlay').projectDir = new File(settingsDir, '../SRGMediaPlayer-Android/segmentOverlay')
project(':srgmediaplayer-extras').projectDir = new File(settingsDir, '../SRGMediaPlayer-Android/srgmediaplayer-extras')
project(':srgmediaplayer-service').projectDir = new File(settingsDir, '../SRGMediaPlayer-Android/srgmediaplayer-service')
```

- Edit your build.gradle:

```groovy
dependencies {
// ...
  compile project(':srgmediaplayer')
  compile project(':srgmediaplayer-extras')
  compile project(':srgmediaplayer-service')
  compile project(':segmentOverlay')
// ...
}
```

# iOS

## Requirements

## Repositories
