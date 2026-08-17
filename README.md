# slowed

A slowed + reverb editor for Apple Silicon Macs. Everything runs on your own
Mac: nothing is uploaded, and it works offline after the one-time first-run
downloads.

Slow a track down, pitch it, add reverb and delay, play it back, and export a
WAV. It can also split a track into stems — vocals on their own, or vocals,
drums, bass, and everything else — so you can mute or drown any one of them.

## Install

1. Download `slowed-<version>.zip` from the [latest release](https://github.com/camclarke11/slowed-releases/releases/latest).
2. Unzip it and drag **slowed.app** into your **Applications** folder.
3. The first time only: right-click the app and choose **Open**, then **Open**
   again. macOS asks because the app is not registered with Apple, which costs
   a yearly fee.
4. Leave slowed open and online while it prepares stem splitting in the
   background. Progress appears in the app; no Terminal, Homebrew, Apple
   developer tools, password, or manual setup is needed.

It opens in your browser at `http://127.0.0.1:3000`.

## Stems and media links

Slowing, pitch, reverb, delay, and export work straight away.

On the first open, slowed automatically downloads its private copies of Python,
FFmpeg, the separator, and its models. They use about 3.3 GB in total. You can
keep using the normal editor while that runs; stem controls become available
when the progress banner finishes. The downloads are cached and reused on every
later launch.

Splitting a three minute track takes a minute or two on an Apple Silicon Mac.

## Updates

The app checks for a new version when it starts. When there is one, a bar
appears at the top of the page: press **Update** and it installs itself and
reloads. There is no need to download anything again by hand.

If stem setup failed in version 0.1.2, install the offered 0.1.3 update and
press **Try again**. Version 0.1.3 removes the accidental Apple developer-tools
requirement and reuses any downloads that already completed.
