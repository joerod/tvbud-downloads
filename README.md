# TVBud APK downloads

This repository hosts Android TV and Fire TV APK downloads for TVBud. The app does not include any channels or playlists.

Create one reusable Downloader code for each URL at [go.aftvnews.com](https://go.aftvnews.com/):

| Channel | Current version | APK URL |
| --- | --- | --- |
| Production baseline | 0.3.2 | https://github.com/joerod/tvbud-downloads/releases/download/fire-tv-prod/TVBud-FireTV.apk |
| Development | 0.3.15 | https://github.com/joerod/tvbud-downloads/releases/download/fire-tv-current-test/TVBud-FireTV.apk |

The two asset URLs stay the same when their APKs are updated. The user confirmed Browser Manager HTTPS works. Version 0.3.15 starts in single view and clears extra screens unless the user enables **Reopen my multiview screens each time**. Clear extra screens is available in Settings, the watch menu, and Screens. A failed prior multiview session triggers a single-view recovery launch. The flexible layout is capped at four screens; explicit templates can use up to six. Provider playback and the new TV layout still need Fire Stick testing. The production baseline still needs full Fire Stick testing. TiviMate `.tmb` backup import is not yet supported.

See the [releases](https://github.com/joerod/tvbud-downloads/releases) for downloads.
