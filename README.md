# ExoPlayer Readme #

## Description ##

ExoPlayer is an application level media player for Android. It provides an
alternative to Android’s MediaPlayer API for playing audio and video both
locally and over the Internet. ExoPlayer supports features not currently
supported by Android’s MediaPlayer API, including DASH and SmoothStreaming
adaptive playbacks. Unlike the MediaPlayer API, ExoPlayer is easy to
customize and extend, and can be updated through Play Store application
updates.

## castLabs ExoPlayer Fork ##

This a fork of the original ExoPlayer project maintained by castLabs GmbH.

For the original project please visit [google/ExoPlayer](https://github.com/google/ExoPlayer).

This README.md is a modified version of the original.

## Project branches ##

  * The [master][] branch is always synchronized with the original google/ExoPlayer branch.
  * The [dev][] branch is always synchronized with the original google/ExoPlayer branch.
  * Most development work happens on the [castlabs/dev][] branch.
  * The [castlabs/production][] branch is the stable release of ExoPlayer by castLabs GmbH.
  * Additional development branches may be established for major features.

[master]: https://github.com/castlabs/ExoPlayer/tree/master
[dev]: https://github.com/castlabs/ExoPlayer/tree/dev
[castlabs/dev]: https://github.com/castlabs/ExoPlayer/tree/dev
[castlabs/production]: https://github.com/castlabs/ExoPlayer/tree/dev

## Using Gradle ##

ExoPlayer can also be built using Gradle. You can include it as a dependent project and build from source:

```
// settings.gradle
include ':app', ':..:ExoPlayer:library'

// app/build.gradle
dependencies {
    compile project(':..:ExoPlayer:library')
}
```

If you want to use ExoPlayer as a jar, run:

```
./gradlew jarRelease
```

and copy library.jar to the libs-folder of your new project.
