# TVBud APK downloads

This repository hosts Android TV and Fire TV APK downloads for TVBud. The app does not include any channels or playlists.

Create one reusable Downloader code for each URL at [go.aftvnews.com](https://go.aftvnews.com/):

| Channel | Current version | APK URL |
| --- | --- | --- |
| Production baseline | 0.3.2 | https://github.com/joerod/tvbud-downloads/releases/download/fire-tv-prod/TVBud-FireTV.apk |
| Development | 0.3.37 | https://github.com/joerod/tvbud-downloads/releases/download/fire-tv-current-test/TVBud-FireTV.apk |

The two asset URLs stay the same when their APKs are updated. The user confirmed Browser Manager HTTPS works. Version 0.3.37 makes guide channel focus wrap from bottom to top and top to bottom, including timeline focus, and uses fresh launcher icon and banner resource names to help Fire TV refresh cached branding. Version 0.3.36 unifies TVBud branding with a new original monogram on the launcher, Fire TV banner, app sidebar, browser header, and browser tab icon. Version 0.3.35 opens Browser Manager's Groups & Channels section on Favorites, with tabs ordered Favorites, Groups, Channels. Version 0.3.34 fixes the blocked cursor when dragging Groups and Favorites in Browser Manager by using pointer gestures for mouse and touch. Version 0.3.33 adds explicit Up/Down/Left/Right focus navigation across multiview screens and empty slots. Version 0.3.32 replaced the full multiview focus outline with a slim blue bottom line and adds direct audio switching by selecting a different screen, plus an Audio source picker in the watch Menu. Version 0.3.31 makes Groups and Favorites directly draggable in separate organizer views, adds precise above/below drop indicators and touch scrolling, and simplifies group cards. Version 0.3.30 fixed browser channel search. Version 0.3.29 added the guide opening preference and playback Up/Down switching within the active group. The Groups drill-down and Skins alignment fixes from 0.3.26 remain. The app starts in single view and clears extra screens unless the user enables **Reopen my multiview screens each time**. Provider playback and the updated remote navigation still need Fire Stick testing. The production baseline still needs full Fire Stick testing. TiviMate `.tmb` backup import is not yet supported.

See the [releases](https://github.com/joerod/tvbud-downloads/releases) for downloads.
