# TVBud APK downloads

This repository hosts Android TV and Fire TV APK downloads for TVBud. The app does not include any channels or playlists.

Create one reusable Downloader code for each URL at [go.aftvnews.com](https://go.aftvnews.com/):

| Channel | Current version | APK URL |
| --- | --- | --- |
| Production baseline | 0.3.2 | https://github.com/joerod/tvbud-downloads/releases/download/fire-tv-prod/TVBud-FireTV.apk |
| Development | 0.3.23 | https://github.com/joerod/tvbud-downloads/releases/download/fire-tv-current-test/TVBud-FireTV.apk |

The two asset URLs stay the same when their APKs are updated. The user confirmed Browser Manager HTTPS works. Version 0.3.23 includes channel search and per-channel Favorites to the top of the browser page, adds Favorites-only filtering, and lets bulk unhide reply before rebuilding the TV guide. Browser Manager now puts groups first: hide a group, expand it to add individual channels to Favorites, and load more channels within large groups. The top clock sits just left of the far-right Menu button with a modest gap. The browser manager adopts the TV's active skin colors and spacing. The app starts in single view and clears extra screens unless the user enables **Reopen my multiview screens each time**. Provider playback and the updated remote navigation still need Fire Stick testing. The production baseline still needs full Fire Stick testing. TiviMate `.tmb` backup import is not yet supported.

See the [releases](https://github.com/joerod/tvbud-downloads/releases) for downloads.
