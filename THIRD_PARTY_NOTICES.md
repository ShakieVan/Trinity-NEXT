# Third-Party Notices

This is a binary-distribution repository. Public availability does not grant
an open-source license to the original application or its artwork. Dependency
licenses remain in effect.

## Runtime Components

| Component | License |
| --- | --- |
| [AndroidX Core 1.18.0 and the AndroidX libraries it depends on](https://android.googlesource.com/platform/frameworks/support/) | [Apache 2.0](licenses/androidx-core.txt) |
| [Kotlin Standard Library 2.2.10](https://github.com/JetBrains/kotlin) | [Apache 2.0](licenses/kotlin-stdlib.txt) |
| [kotlinx.coroutines 1.9.0](https://github.com/Kotlin/kotlinx.coroutines) | [Apache 2.0](licenses/kotlin-stdlib.txt) |
| [Guava ListenableFuture 1.0](https://github.com/google/guava) | [Apache 2.0](licenses/androidx-core.txt) |
| [JetBrains Annotations 23.0.0](https://github.com/JetBrains/java-annotations) | [Apache 2.0](licenses/kotlin-stdlib.txt) |
| [JSpecify 1.0.0](https://github.com/jspecify/jspecify) | [Apache 2.0](licenses/androidx-core.txt) |

These libraries arrive through the Android build; the release build keeps only the
parts the app uses. The two license files hold the same Apache License 2.0 text and
also ship inside the app.

## The App's Own Content

The rules, the graphics and the app icon were made for Trinity-NEXT. Every stone is
drawn by the app itself; no image files, fonts or music are included, and text is drawn
with the fonts of your device.

The sounds are short recordings generated for Trinity-NEXT with the text-to-sound model
[MOSS-SoundEffect v2.0](https://huggingface.co/OpenMOSS-Team/MOSS-SoundEffect-v2.0)
(Apache 2.0), then cut and levelled. The model is a tool used in making them and is not
part of the app. No third-party recordings are included.
