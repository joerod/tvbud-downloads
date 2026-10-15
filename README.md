# TVBud APK downloads

This repository hosts Android TV and Fire TV APK downloads for TVBud. The app does not include any channels or playlists.

Create one reusable Downloader code for each URL at [go.aftvnews.com](https://go.aftvnews.com/):

| Channel | Current version | APK URL |
| --- | --- | --- |
| Production | 0.3.59 | https://github.com/joerod/tvbud-downloads/releases/download/fire-tv-prod/TVBud-FireTV.apk |
| Development | 0.3.60 | https://github.com/joerod/tvbud-downloads/releases/download/fire-tv-current-test/TVBud-FireTV.apk |

The two asset URLs stay the same when their APKs are updated. Production 0.3.59 includes the JoeRod skin, custom skin images, guide refresh controls, and the Browser Manager over HTTPS. Development 0.3.60 adds “Made by JoeRod” to About, improves guide snapshot caching and timeline alignment, and makes multiview Menu and full-screen controls easier to use. The Sony BRAVIA Android TV has one imported playlist with 48,382 channels; the development build is being checked there. Hardware stream capacity varies, so multiview warns when a new stream exceeds the device estimate. A 1920×1080 [Fire TV background image](assets/fire-tv-background.jpg) and 1280×720 [Appstore icon](assets/fire-tv-app-icon.png) are ready for an Amazon Appstore listing. TVBud starts in single view unless you enable **Reopen my multiview screens each time**. TiviMate `.tmb` backup import is not supported.

See the [releases](https://github.com/joerod/tvbud-downloads/releases) for downloads.

## User guide

Read the [TVBud user guide](USER_GUIDE.md) for installation, playlist setup, remote controls, Browser Manager, guide data, skins, and troubleshooting.

## Plugins

TVBud does not currently support executable plugins or offer a plugin API. Skins are JSON appearance presets, not plugins. Add playlist and XMLTV sources through the app or Browser Manager.
