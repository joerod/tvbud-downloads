# TVBud user guide

TVBud is an Android TV and Fire TV IPTV player. It does not include channels. You need your own M3U playlist, Xtream Codes account, or Stalker portal from a provider you are authorized to use.

## Install and update

Use the permanent APK URL for the channel you want:

| Channel | APK URL |
| --- | --- |
| Production | https://github.com/joerod/tvbud-downloads/releases/download/fire-tv-prod/TVBud-FireTV.apk |
| Development | https://github.com/joerod/tvbud-downloads/releases/download/fire-tv-current-test/TVBud-FireTV.apk |

On Fire TV, enter a URL in Downloader, or create a reusable numeric Downloader code at https://go.aftvnews.com/. On Android TV, open the APK URL in a browser or sideload the APK. Install updates over the existing app to keep local settings. Check the installed version in **Settings → About TVBud**. Development receives features first; production is the more tested release.

## Add playlists

Open **Settings → Playlists** or **Manage from browser** and select a source type:

1. **M3U:** enter the playlist URL or import a local M3U file. Add its XMLTV guide URL if your provider supplies one.
2. **Xtream Codes:** enter the provider server URL, username, and password. TVBud imports live channels and uses the same account for Movies and Shows when the provider supports those catalogs.
3. **Stalker/Ministra:** enter the portal URL and account MAC address. Live streams and provider guide data depend on the portal.

You can add several playlists. They remain separate sources, and each can be removed individually. Large imports show progress and may take time on slower TVs.

## Watch TV with the remote

- Select a channel and press **OK/Select** to play it full screen.
- While watching, press **Up/Down** to change channels within the current group or Favorites. The list wraps at either end.
- Press **OK/Select** while watching to open the guide. The half-screen guide leaves video visible; use **Expand guide** for the full guide. Press **Left** from categories to open the app section flyout.
- Use **Left/Right** to move among the section flyout, categories, channels, and EPG timeline. Use **Up/Down** within a list. **Back** moves to the previous panel or closes the overlay.
- Open the watch **Menu** or use the remote **Info** key for playback options. Controls fade during idle playback.
- Long-press a channel when supported to open its channel options.

The guide opens on Favorites by default when any exist. Change this under **Settings → Guide opens to**. In **Settings → Guide size**, choose half or full screen. The guide time header stays visible while channel rows scroll.

## Favorites, groups, and search

The TV guide groups channels by playlist category. Use **Search** in the left flyout to find a channel. Browser Manager offers a faster way to organize large lists: its **Groups & Channels** tab has **Favorites**, **Groups**, and **Channels** views. Expand a group to see its channels and mark specific ones as Favorites. Drag group or Favorite handles to reorder them; Up/Down controls are also available. Hiding a group hides its channels from ordinary group browsing, while saved Favorites can still appear in Favorites and My List. Hidden groups stay visible in Browser Manager so you can show them again.

## Connect Browser Manager

On the TV, choose **Manage from browser**. Scan its QR code with a phone or computer on the same private network. The QR link carries a short-lived PIN and pairs automatically. If it expires, refresh the QR code or reopen the dialog. You can also type the HTTPS address and PIN shown on the TV. Because TVBud makes its own certificate, your browser may warn about it; compare the certificate SHA-256 fingerprint with the TV display before continuing. Do not expose the manager port to the internet.

Browser Manager has **Config**, **Groups & Channels**, and **Skins** tabs. Config adds sources, changes guide options, and exports/imports a JSON backup. The backup contains provider credentials; keep it private. A skin JSON file contains appearance settings and images, not channel streams.

## Guide data

TVBud uses the provider guide first, then a custom XMLTV URL if configured, then enabled public fallback feeds for missing listings. It matches channel IDs and cleaned channel names. **No guide data** means none of those sources had a usable match for that channel and time; the app cannot invent a listing.

Successful guide listings are saved locally and restored on restart. Set **Guide refresh** in TV Settings or Browser Manager Config to every **1, 3, 6, 12, or 24 hours**; six hours is the default. You can also refresh guide data manually from **Settings → Guide data**. If a favorite has no listings, add your provider's XMLTV URL to its playlist, then refresh the guide. Online fallback needs an internet connection.

## Movies, Shows, and multiview

**Movies** and **Shows** use saved Xtream account details when the provider supplies on-demand catalogs. They can take time to load and may be unavailable for M3U-only or Stalker sources. In the watch Menu, choose **Multiview** to select a layout and add channels to empty screens. Use direction keys to focus a tile and **OK** to switch its audio. The active tile has a blue line at its bottom. Left from the leftmost tile or Up from the topmost tile focuses the watch Menu, where **Screens** can remove streams. Long-press **OK** on a playing tile to view it full screen; one **Back** returns to the same running multiview. The flexible layout has no fixed screen limit, but the app warns when a new stream exceeds its estimate of device capacity. The app starts in single view by default; **Settings → Multiview startup** can restore extra screens.

## Appearance and settings

Open **Settings → Appearance & skins** to choose TVBud Classic or JoeRod. JoeRod uses the custom headshot TV logo and TV Guide art. In Browser Manager **Skins**, create or import a JSON skin, change colors, and upload separate images for the TV frame logo and TV Guide heading. The selected TV frame logo also appears on the loading screen.

Other TV Settings include video buffer size, clock location, weather location and units, guide opening behavior, guide refresh, and About. **About TVBud** shows the installed version and the “Made by JoeRod” credit. Weather uses an approximate IP location unless you enter a five-digit US ZIP code. The clock and weather can appear in the top right or bottom channel information bar.

## Troubleshooting

- **No channels:** check the source type, provider URL, credentials, and whether the import completed. An app install does not include playlists.
- **No guide data:** add or correct the provider XMLTV URL, refresh guide data, and check a known channel. Some channels are absent from public feeds.
- **Browser Manager will not connect:** keep phone and TV on the same local network, reopen Manage from browser for a fresh QR/PIN, and compare the certificate fingerprint if warned.
- **Large backup import seems slow:** leave TVBud open while progress advances. The TV may need time to index tens of thousands of channels.
- **Multiview becomes unstable:** clear extra screens and use fewer simultaneous streams; decoder limits differ by device.
- **Need to move settings to another TV:** export Config JSON in Browser Manager, keep it private, then import it on the second TV. Importing replaces the local setup.

## Plugins

TVBud currently has no plugin loader or plugin API. Skin JSON imports change appearance only. Configure playlist and XMLTV sources through the app or Browser Manager.
