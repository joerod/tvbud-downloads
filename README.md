# TVBud APK downloads

This repository hosts Android TV and Fire TV APK downloads for TVBud. The app does not include any channels or playlists.

Create one reusable Downloader code for each URL at [go.aftvnews.com](https://go.aftvnews.com/):

| Channel | Current version | APK URL |
| --- | --- | --- |
| Production | 0.3.64 | https://github.com/joerod/tvbud-downloads/releases/download/prod/TVBud.apk |
| Development | 0.3.64 | https://github.com/joerod/tvbud-downloads/releases/download/fire-tv-current-test/TVBud.apk |

The two asset URLs stay the same when their APKs are updated. Version 0.3.64 starts faster with an optimized release build and keeps buffering behind a splash that says **Loading**. Search finds live TV, movies, and shows, with a microphone button for voice input on supported devices. Movies and Shows reuse saved catalogs and show progress while loading or refreshing them. The app includes GitHub update checks, the JoeRod skin, custom skin images, guide refresh controls, and Browser Manager over HTTPS. Startup restores saved guide data and reads a compact visible-channel index; hidden groups load when management opens. Left from playback opens channels, another Left reveals categories, and a third Left opens the section menu. Guide size is configured in Settings, and the guide header marks the exact current minute. Hardware stream capacity varies, so multiview warns when a new stream exceeds the device estimate. A 1920×1080 [Fire TV background image](assets/fire-tv-background.jpg) and 1280×720 [Appstore icon](assets/fire-tv-app-icon.png) are ready for an Amazon Appstore listing. TVBud starts in single view unless you enable **Reopen my multiview screens each time**. TiviMate `.tmb` backup import is not supported.

See the [releases](https://github.com/joerod/tvbud-downloads/releases) for downloads.

## User guide

Read the [TVBud user guide](USER_GUIDE.md) for installation, playlist setup, remote controls, Browser Manager, guide data, skins, and troubleshooting.

## Plugins

TVBud does not currently support executable plugins or offer a plugin API. Skins are JSON appearance presets, not plugins. Add playlist and XMLTV sources through the app or Browser Manager.
