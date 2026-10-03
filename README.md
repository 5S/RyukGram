<div align="center">

# RyukGram

**The Instagram tweak for iOS power users.**

`v1.4.5` · Instagram 449.0.0 | Instagram 410.1.0

<sub>The Instagram 410 build is for older iOS versions and trails the main build on newer features.</sub>

<p>
  <a href="https://github.com/faroukbmiled/RyukGram/releases/latest"><img src="https://img.shields.io/badge/Download-Latest%20release-7C3AED?style=for-the-badge&labelColor=1F2430" alt="Latest release" height="32"></a>
  <a href="https://t.me/ryukgram"><img src="https://img.shields.io/badge/Telegram-Channel-2AABEE?style=for-the-badge&labelColor=1F2430" alt="Telegram" height="32"></a>
  <a href="https://buymeacoffee.com/axryuk"><img src="https://img.shields.io/badge/Donate-Support%20the%20project-E5484D?style=for-the-badge&labelColor=1F2430" alt="Donate" height="32"></a>
</p>

<p>
  <a href="https://github.com/faroukbmiled/RyukGram/issues">Issues</a>
  ·
  <a href="#translating">Translate</a>
  ·
  <a href="#features">Features</a>
</p>

</div>

---

> [!NOTE]
> RyukGram is [closed source](#credits) for now and will open up again later. Builds and translations stay current here.

## Install

### Add it in one tap

<div align="center">

<a href="https://store.ryuksign.com"><img src="https://img.shields.io/badge/Add%20RyukGram-store.ryuksign.com-7C3AED?style=for-the-badge&labelColor=1F2430" alt="Add RyukGram" height="36"></a>

</div>

Open it on your phone and everything is one tap away. Add it once and updates arrive on their own.

- **Sideload.** Adds the source to **Feather** or **RyukSign**, **SideStore**, or **AltStore**. Pick the **plugins** build normally, or **no plugins** if you sign with a free Apple account, since free accounts cannot sign the bundled extensions.
- **Jailbreak.** Adds the repo to **Sileo** or **Zebra**, then installs the build that matches your setup. To paste it by hand the repo is `https://source.ryuksign.com/apt/`.

### Build your own IPA

Instagram itself cannot be bundled here, so you bring the Instagram IPA and the build slots RyukGram into it.

**With GitHub Actions, no Mac needed.** Fork this repo, open the **Actions** tab, and run **Build sideloaded IPA from Release Assets**. Give it your Instagram IPA and it hands back a patched IPA ready to sign and install. Turn on the no-plugins option if you sign with a free account.

**Or by hand** with a tool like cyan, injecting into your own Instagram IPA:
- Regular build. Inject `zxPluginsInject.dylib` into the app and its plugins. The normal one, with the bundled extensions.
- No-plugins build. Inject `NoPluginsPatch.dylib` instead. For a plugin free sideload, or a free account where extensions cannot be signed.

### Download the .deb

Prefer the file? Both builds are on the [latest release](https://github.com/faroukbmiled/RyukGram/releases/latest).

<table>
  <tr>
    <th align="left">File</th>
    <th align="left">Build</th>
  </tr>
  <tr>
    <td><code>RyukGram_x.x.x_rootless.deb</code></td>
    <td>Rootless</td>
  </tr>
  <tr>
    <td><code>RyukGram_x.x.x_rootful.deb</code></td>
    <td>Rootful</td>
  </tr>
</table>

The rootless .deb also carries the dylib and bundle the sideload builds use.

### TrollStore

Download `RyukGram_trollfools.zip` from the [latest release](https://github.com/faroukbmiled/RyukGram/releases/latest) and inject it into Instagram with TrollFools.

---

Once it is running, open the settings by holding the button at the top of your profile, or the home button in the tab bar. Screenshots are [below](#opening-settings).

## Features

### General
- Hide ads and Meta AI
- Hide the TestFlight popup and turn off app haptics
- Always mute starts every surface silent until you tap a speaker or press volume
- Copy captions, comment text, and profile info
- Open copied text in a sheet to edit it or copy only the part you select
- Download, copy, or expand image and GIF comments
- Send any Giphy link as a comment GIF, and pin the ones you favorite
- Download audio from the reels audio page
- Hold a song in any music picker to download its audio
- Clean shared links for embeds and strip their tracking, with your own param list
- Open links in an external browser or straight from the clipboard
- Tap links, emails and phone numbers in captions, comments and bios, or hold one to copy or share
- Native color picker, teen app icons, and a picker for the bundled app icons
- Liquid glass controls, with a force off switch and tab bar behavior
- Instagram Plus turns on Instagram's own paid features
- Notes tweaks: hide the tray, hide the friends map, custom themes
- Drop suggested accounts and searches, trending, the explore grid, sensitive covers, and surveys
- Hide reels in explore, keeping only photos and carousels
- Stat pills on search and explore, with a page to pick and reorder them
- Anonymous live viewing and toggleable live comments
- Redact RyukGram's own buttons in screenshots and recordings
- Update checker with what changed, notes for every past release, and a link to Telegram
- Safari extension with an Open in RyukGram banner that also strips Instagram's app prompts and App Store jumps
- Crash logs you can read, search and share, off by default

### Feed
- Grid feed turns your home feed into thumbnails, each with its stats and author
- Pick which stats show and their order, tile shape, columns by pinch, and the date format
- Hold a tile to preview it, or to like, follow, expand, share, or copy the link
- Switch back to Instagram's feed from the header heart or a floating button you place
- Hide the stories tray, suggested stories, and highlights
- View a profile picture from a story tray long press
- Hide the whole feed, or just suggested posts, accounts, reels, threads, and Facebook cards
- Cap how many posts load in a row and filter posts by minimum likes, comments, views, or reposts
- Turn off video autoplay
- Tap a reel in the feed to play it in place, or play first and open Reels on a second tap
- Long press any media to open it full screen, muted if you want
- Custom date format with your own template and relative times
- Turn off background and home button refresh
- Status bar tap can scroll up only, or do nothing
- Stop the right swipe on the feed from opening the camera
- Confirm before a pull to refresh, or refresh only the stories tray
- Post buttons page to reorder, hide, or drop the counts on Instagram's own like, comment, share, repost and save buttons

### Reels
- Custom tap controls and auto scroll, Instagram's own or ours, which also skips sponsored and photo reels
- Hold controls to pause, open the options menu, or open it with picture in picture
- Playback menu for speed, seek, pause, sound, picture in picture, and auto scroll
- Always visible scrubber, no auto unmute, and refresh confirmation
- Expanded view that shows the whole reel instead of cropping the sides
- Unlock password locked reels
- Reel buttons page to reorder, hide, or drop the counts on the sidebar buttons
- Hide the header, friend avatars, promo pills, and the stuck comment bar
- Swipe left to open the author's profile
- Show the repost date
- Disable scrolling reels so one stays in place
- Reels limit per session, capping reels in a row, or per day with time or reel caps overall or per place, a week chart with day history, break nudges and a heads up before you hit one
- Once a limit hits, reels stay paused everywhere, previews included, and feed videos can hide until tomorrow
- Filter the reels feed by minimum likes, comments, views, or reposts
- Enhanced pause and play mode

### Action buttons
- Context aware menus on feed, reels, stories, DMs, and profiles
- Configurable default tap, and a searchable browser of Instagram and system icons
- Carousel and multi story bulk download
- Save a photo post with its music as a video, from feed or reels
- Save a photo story as just the image
- Repost through Instagram's own flow
- Full screen viewer with zoom and swipe
- Drag your overlay buttons into place on a live preview, with a spacing slider

### Profile
- Zoom or save the profile picture, and view every picture on the account
- View highlight covers from a long press
- Action button for info, the picture, and follower stats
- Follow indicator that shows who follows you back, in lists and on profiles
- Copy notes, reveal full counts, and spoof your picture, username, name, Threads handle, stats, badge and post metrics on your device
- Hide the Threads button in the header
- Sort and search follower and following lists by mutuals, verified, and more
- Follow request tracker that logs every request, even ones canceled before you answer

### Profile analyzer
- Follower and following scans, with mutuals and non followbacks
- New and lost trackers across scans
- Change history for name, username, bio, and picture
- Inline and batch follow, unfollow, and remove
- A private log of every profile you open, with notes, filters and CSV or JSON export
- Watchlist that checks accounts on a schedule, even ones you never opened, and backs off for a day if Instagram limits you
- Tracked changes feed for username, name, bio, link, picture, privacy, follow back and counts, with alerts per type
- Per-check toggles, with a badge for gains and losses since your last look

### Saving
- HD downloads up to 1080p, with a quality picker and preview
- Full-resolution photos at their original upload size, or picked per size
- Audio only and raw photo options
- Download manager with live speed, filters, swipe actions, and bulk select
- Download history that survives a restart, with redownload and a keep window
- Duplicate check before you save the same media twice, dropping the old gallery copy if you want
- Auto retry for downloads that drop offline
- Save into a dedicated RyukGram album
- Advanced encoding panel for codec, bitrate, and resolution
- One clean filename everywhere, stamped with the date the post went up
- Optional `ryuk_` prefix on saved filenames
- Optional download confirmation

### Gallery
- A private in-app library that every download can mirror into
- Images, video, audio, and animated GIFs
- Filter by type, source, uploader, date, and favorites, with folders
- Sort by date, name, or size, with images, videos, or favorites first
- Group by user into sections or folders, from 2 to 5 columns
- A downloaded post or story stays one swipeable item, and you can group or split albums yourself
- Long press a user section to select all their media
- In-app preview carousel
- Pull audio and GIFs straight from the gallery
- Import your own photos, videos and files into the gallery
- Pick from it inside Instagram: Send from gallery in the DM plus menu, hold the photo button in comments, or hold Recents in the story, post and reel galleries
- Repost any photo, video or GIF from it as a story, post or reel
- Edit in place: crop, rotate and resize photos, trim and crop videos, trim audio, pull or strip a video's sound, turn GIFs into videos
- Save an edit as a new file or replace the original, keeping its source info
- Info page with editable source details, camera and codec info, and one tap location removal
- Grid tiles show a date chip, and a long press gives date, source and size

### Stories and messages
- Keep deleted messages, including your own unsends
- Mark the ones you kept with a tag, a faded bubble, a tinted bubble, or nothing
- A full quality log of every unsent message, grouped by chat and searchable
- Jump from the log straight to where the message sat in the chat
- Catch view-once media that arrives while Instagram is closed
- Log view-once media the moment you open it, off by default
- Activity notifications for reads, online, offline, and typing, set per person or only for people in your list
- An activity log as a timeline, filterable and swipe to delete
- Accurate active status so the green dot turns off the moment someone leaves
- Playback menu for story speed, seek, pause, and sound, held from the story buttons or its menu
- Your own fonts in the story text tool, next to the built-in ones
- Manual and automatic mark as seen
- Hold the eye button to mark a whole story reel seen, or only up to where you are
- Mark chats seen on your device only, the eye button stays orange until you really send it
- Stories you already marked seen hide or tint the eye button for 48 hours
- Send audio as a file or a voice note, with a trim editor
- Send an image as your doodle in Draw, with a crop, rotate, flip and background remover
- Download voice messages
- Force the missing sound toggle in the DM camera
- Turn off typing status, the vanish swipe, and view once limits
- Hide shared reels in chats so they never show or open in a thread
- Toggle your activity status from a dot in the DMs inbox
- Custom chat backgrounds from an image, video, or GIF, with a built-in editor
- Filter, sort, search, and pin story viewers, and see who reacted with what
- Archive your own stories before they expire, viewer list included, per account
- Story stats over your archive
- View story mentions and reveal poll and quiz results
- Bypass Reveal stickers and pick custom sticker colors
- Custom story backgrounds in any color or gradient, in any direction
- Download disappearing DM media in full quality
- Hide the views toggle from the chat header and keep views blocked
- Send Instants from your album, with crop and trim editors
- Auto close the Instants viewer once you have seen them all
- Toggle the Instants switch confirmation from a button in the viewer
- Keep Instants unseen until you mark them seen with the eye button
- Record voice and video calls into an adaptive grid, browsed per person
- Each recording is tagged auto or manual in the list
- Select recordings to save, share, share as audio only, or delete together

### Interface
- Custom notification sounds for DMs and other alerts, imported from Files, Photos or the gallery and trimmed, or Instagram's own tones
- A universal notification pill you can place anywhere on screen
- Mirror toasts to the iOS notification center, in the background or while the app is open
- Reorder and hide tab bar icons on a live tab bar preview
- Hold any tab bar tab to open a RyukGram screen, picked per tab
- Messages-only mode, with a daily schedule that switches in place and inbox header shortcuts
- Force Instagram into any supported language
- Home shortcut button with new item badges
- Notification history with filters, search, and a choice of which features get saved
- Bring back the old Instagram logo in the feed header
- Experimental flags
- MobileConfig browser to read, change, export and import Instagram's own internal settings
- Switch MobileConfig overrides off without losing them, note any config, and filter or search the list
- Every config and field Instagram exposes on iOS is named, with a coverage count under the list

### Confirm actions
- Optional confirmations for likes, follows, reposts, calls, comments, and more
- Confirm DM reactions, either the double tap one only or every reaction

### Fake location
- Override your location across the app, with a map picker and saved presets

### Theme
- Off, light, dark, or OLED, applied to Instagram only
- OLED chat theme and a matching keyboard theme
- Custom fonts for Instagram, RyukGram, or both
- Import your own .ttf or .otf fonts, or download from thousands online
- Custom emoji fonts, converted once so they scroll as smooth as the stock ones
- Manage installed fonts in bulk, with multi select and swipe

### Security and privacy
- Mask the device identifiers Instagram reads, from settings or the login screen
- Passcode and biometric lock for settings, chats, logs, recordings, and the app itself
- Hidden chats and per account lists
- App switcher shroud and hidden previews for locked chats

### Backup and profiles
- Export your settings and feature data as JSON or an encrypted bundle
- Restore with replace or merge
- Scope any export, import, or reset to the accounts you pick
- Save your whole setup as a named profile and switch between setups in a tap
- Give a profile its own name, color and icon, duplicate it, or share it as a file
- Tie a profile to Instagram accounts so it switches when you do, and leave one untied to cover the rest
- Reset a profile to defaults or turn everything off in it, with a count of what is on
- Send an imported backup's settings to a new profile instead of the setup you use
- See what RyukGram keeps on your device, by section and account, and clear it

### Localization
- English, Spanish, French, Russian, Korean, Japanese, Arabic, Vietnamese, Chinese, Portuguese, Turkish, and Indonesian
- In app language picker, with English as the fallback

### Optimization
- Clear the Instagram cache on demand or on a timer
- Profile pictures kept on device, so they survive expired links and cache clears
- Smoother feed scrolling

## Translating

Want RyukGram in your language? Export the strings from **Settings, Debug, Localization**, translate the right side of each `"key" = "value";` line, and open a pull request with your file at `src/Localization/Resources/<code>.lproj/Localizable.strings`. Keep the format specifiers like `%@` and `%lu` exactly as they are. Missing lines fall back to English, so partial work is welcome. Anything you contribute is licensed to the project under the same terms as RyukGram.

## Opening settings

|                                             |                                             |
|:-------------------------------------------:|:-------------------------------------------:|
| <img src="https://i.imgur.com/OnjLpZK.png"> | <img src="https://i.imgur.com/pHIuYTm.jpeg"> |

## Credits

RyukGram got its start from [SCInsta](https://github.com/SoCuul/SCInsta) by [@SoCuul](https://github.com/SoCuul), and I'm grateful for the foundation it gave the project. That code has since been fully rewritten and none of it remains, so RyukGram is its own separate codebase. It went closed source because earlier releases were being lifted and resold as paid tweaks, which is something I can't keep feeding, and I know some of you valued it staying open. Thanks to @SoCuul and the wider iOS tweak scene for paving the way.

- [**@SoCuul**](https://github.com/SoCuul) for SCInsta, the spark for this project
- [**@BandarHL**](https://github.com/BandarHL) for BHInstagram
- [**@VAXMG**](https://t.me/ciesIPAs) for OLED theme inspiration
- [**@euoradan**](https://t.me/euoradan) for experiment flag research
- [**@n3d1117**](https://github.com/n3d1117) for the Following feed
- [**BillyCurtis**](https://github.com/BillyCurtis/OpenInstagramSafariExtension) for the Safari extension base
- [**@asdfzxcvbn**](https://github.com/asdfzxcvbn) for ipapatch and zxPluginsInject
- Furamako, [@ZomkaDEV](https://github.com/ZomkaDEV), [@ch1tmdgus](https://github.com/ch1tmdgus), [@hooray804](https://github.com/hooray804), [@bruuhim](https://github.com/bruuhim), [@jaydenjcpy](https://github.com/jaydenjcpy), [@brunorainha](https://github.com/brunorainha), [@yesnt10](https://github.com/yesnt10), [@tranbinh02](https://github.com/tranbinh02), [@yannouuuu](https://github.com/yannouuuu), [@willybilly981](https://github.com/willybilly981), and [@diemasmahendra](https://github.com/diemasmahendra) for translations

## Support

If RyukGram earns a spot on your phone, you can keep it going here.

<div align="center">

<a href="https://buymeacoffee.com/axryuk"><img src="https://img.shields.io/badge/Donate-Support%20the%20project-E5484D?style=for-the-badge&labelColor=1F2430" alt="Donate" height="32"></a>
<a href="https://github.com/faroukbmiled/RyukGram"><img src="https://img.shields.io/badge/Star-the%20repo-6B7280?style=for-the-badge&labelColor=1F2430" alt="Star the repo" height="32"></a>

</div>
