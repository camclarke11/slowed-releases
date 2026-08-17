# slowed

A slowed + reverb editor for macOS. Everything runs on your own Mac: nothing is
uploaded, and it works offline.

Slow a track down, pitch it, add reverb and delay, play it back, and export a
WAV. It can also split a track into stems — vocals on their own, or vocals,
drums, bass, and everything else — so you can mute or drown any one of them.

## Install

1. Download `slowed-<version>.zip` from the [latest release](https://github.com/camclarke11/slowed-releases/releases/latest).
2. Unzip it and drag **slowed.app** into your **Applications** folder.
3. The first time only: right-click the app and choose **Open**, then **Open**
   again. macOS asks because the app is not registered with Apple, which costs
   a yearly fee.

It opens in your browser at `http://127.0.0.1:3000`. Nothing else to install.

## Stems and media links

Slowing, pitch, reverb, delay, and export work straight away.

Splitting stems and opening media links need some extra tools that are too
large to ship inside the app. Load a track and press **Set up stem splitting**,
and the app opens a Terminal window that installs them. It takes a while and
downloads a few gigabytes. The first split then downloads the separation models
themselves, around 1.2 GB, once.

Splitting a three minute track takes a minute or two on an Apple Silicon Mac.

## Updates

The app checks for a new version when it starts. When there is one, a bar
appears at the top of the page: press **Update** and it installs itself and
reloads. There is no need to download anything again by hand.
