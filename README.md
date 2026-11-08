# Description

This is an Android camera application that uses a rolling buffer to provide a delayed live playback of the camera feed. The app also allows the user to easily save a clip of the past x seconds of the camera feed, view it in an in-app mediaplayer and save it as an mp4 file if they deem it interesting.

Features include:

- Custom configurations including the ability to choose resolution, frame rate, front/back camera, delay and mediaplayer clip lengths.
- In-app mediaplayer allows fine controls over the playback, also allows user to easily save the clip as an mp4 file or save an individual frame as an image.
- Quickly switch between realtime and delayed modes for easy camera positioning.
- Disk-backed rolling buffer to allow for longer clips without running out of memory.

## Requirements and installation

- The app requires an Android device running **Android 10 (API 29) or newer**. Performance may vary between devices, especially at higher resolutions or frame rates.

### Permissions

#### Android 10–12 (API 29–32)

- Camera access
- Read external storage
- Write external storage

#### Android 13 and newer (API 33+)

- Camera access
- Read videos from shared storage

### Installation

1. Open the project's [latest GitHub release](https://github.com/V-Lind/ONT-ReplayViewer/releases/latest) on your Android device.
2. Under **Assets**, download the `.apk` file.
3. Open the downloaded APK from your browser or **Downloads** folder.
4. If prompted, allow the installation of unknown apps.

> Only install APKs downloaded from a trusted release source. You can disable the **Install unknown apps** permission again after installation.

## Libraries and Frameworks Used

- **Kotlin**: The primary language used for development.
- **Gradle**: Used for dependency management and build automation.
- **Android Jetpack Compose**: Primary UI toolkit used to build the interfaces for the application.
- **Kotlin Coroutines**: Used for managing background threads, critical for processing frames with the limited performance of mobile devices.
- **Android MediaMuxer & MediaCodec**: Used for video processing, encoding mp4 files out of saved video clips.
- **Android CameraX**: Highly automated camera library that allows fast/easy use-cases for camera.
- **Android Camera2**: Low-level camera library that allows higher degree of control over cameras and more complex use-cases than CameraX alone.
- **Material3**: Material Design library for easy components.

## Images

![image](https://github.com/user-attachments/assets/469b9038-104a-427f-af18-63a364e43fa0)
![image](https://github.com/user-attachments/assets/cb21d9d0-2168-4a99-9d96-0002a0f1d47d)
![image](https://github.com/user-attachments/assets/6548315f-9c4e-4848-b799-9864c62785ab)
![image](https://github.com/user-attachments/assets/a1f50e4c-4ee3-4bae-891d-4e171c893373)
![image](https://github.com/user-attachments/assets/5836d98d-e5ed-487e-8146-f7358bf53740)
