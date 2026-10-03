# [release] RyukGram v1.4.5

### ✨ Highlights

- **RyukGram Gallery** — Pick and repost media directly inside Instagram, edit photos and videos, manage file details, and save everything to your gallery
- **Reels limits** — Set session or daily limits by time or reel count, track usage, get break reminders, and pause reels across the app when limits are reached
- **Watchlist & profile tracking** — Monitor accounts for username, bio, picture, privacy, verification and count changes, with configurable alerts and a private profile history
- **Playback controls** — A redesigned reels and stories panel with live seeking, frame-by-frame navigation, custom skip steps, playback speed memory and frame saving
- **Notification history** — Search and filter saved notifications, choose which features are recorded, and access them from a home shortcut
- **Custom notification sounds** — Import and trim your own sounds for DMs and other alerts, or use Instagram's built-in tones
- **Gallery media limits and feed controls** — Control how much content loads, filter posts by engagement, and hide feed videos when your reels limit is reached
- **MobileConfig Browser Update** — The browser now names all configs and fields Instagram exposes on iOS, with a coverage count at the bottom of the list

### 🆕 New features

#### Gallery & media

- Pick media from the RyukGram Gallery directly in Instagram: use the DM + menu, hold the comment photo button, or hold Recents in story, post and reel galleries
- Repost gallery photos, videos and GIFs as stories, posts or reels
- Edit gallery media: crop, rotate and resize photos, trim and crop videos, trim audio, extract or remove video audio, and convert GIFs to video. Save as a new file or replace the original
- Gallery info editor — Rename files, edit source details, view camera and codec information, and remove photo location data
- Redesigned crop editor for Draw and chat backgrounds, with more ratios, free crop, flip and zoom-to-fit
- Save photo posts with their music from the reels action button, disabled by default
- Open profile pictures to browse every available picture on the account
- Group chats without a picture now show member avatars in RyukGram lists

#### Reels & stories

- Reels and stories playback panel — Live progress, elapsed and remaining time, larger play/pause, custom skip intervals, frame-by-frame seeking, next/previous navigation and frame saving
- Playback speed can be remembered globally, for the current session or only for the current video
- Reel sidebar playback button shows the current speed and can switch between 1× and your last speed by holding it
- Move the reels action and playback buttons anywhere in the sidebar
- Access playback controls from the reels and stories action button, with auto-advance controls in the story panel
- Reels auto-scroll can skip sponsored and photo reels
- Keep Instants unseen after viewing, or mark an individual one seen with the viewer's eye button
- Hold the story background button to choose a solid color or gradient, with an adjustable direction

#### Profiles & tracking

- Watchlist — Add accounts from profiles, recent chats or search. Accounts are checked on a schedule and for free when opened, with a 24-hour pause if Instagram rate-limits requests
- Track watchlist changes to usernames, names, bios, links, pictures, privacy, verification, follow-back status and counts, with per-type alerts and a home shortcut
- Visited profiles — Keep a private history of opened profiles with notes, filters, multi-select and CSV or JSON export
- Activity notifications can now track only accounts in your list
- Fake profile picture — Use an image from Photos, Gallery, Files or a link, displayed throughout Instagram on your device only
- Spoofing editor redesigned around your profile header, including the Threads badge. Tap fields to edit, apply changes, or disable all spoofing with one switch. Edit Profile always shows your real information
- Post spoofing — Select your own posts and change displayed likes, comments, views, shares, reposts and saves locally

#### MobileConfig & advanced

- Active MobileConfig overrides show how many times Instagram has read them
- Identify unnamed MobileConfig entries by the code that reads them, and use that code as their label
- Toggle individual or all overrides off and on without losing their values
- Filter MobileConfig parameters by overridden status or platform
- Add searchable notes to configs, visible in the list and config details
- Search MobileConfig by notes, parameter names, IDs, names or numbers
- Every MobileConfig config and field Instagram exposes on iOS now has a name, up from under a third
- The MobileConfig list footer shows how many configs and fields are named out of the total
- Instagram API settings — Reuse recent replies for a chosen period, pace requests, and set daily follow and unfollow limits

#### Interface & customization

- Custom emoji fonts — Import color emoji fonts to replace emoji throughout Instagram
- Custom notification sounds for DMs and other alerts, with imports from Files, Photos or Gallery, trimming, and Instagram's built-in tones
- Safari extension — Add an Open in RyukGram banner at the top or bottom, remove Instagram app prompts, block App Store redirects, and optionally open links automatically
- Strip tracking menu — Manage tracking removal for shared and opened links, choose which parameters to remove, or strip unnecessary parameters from shared links
- Embed domains and tracking parameters now support multi-select deletion
- Hide search suggestions, including suggested accounts and searches in the Search tab
- Hide Facebook cards: removes the Facebook suggestion cards from the feed
- Hide Meta AI also removes AI-generated images from the gallery picker
- Force audio button restores the DM camera sound toggle in the ••• menu when Instagram does not show it
- Links, email addresses and phone numbers in captions, comments and profile bios are tappable, with long-press options to copy or share
- Option to hide the disappearing media views toggle from the chat header

#### Reels limits

- Choose per-session limits, the previous doom-scrolling cap, or daily limits based on time or reel count
- Set limits per location or across the app
- Usage dashboard with daily history, break reminders and warnings before reaching a limit
- Strict mode and a home shortcut
- When a limit is reached, reels pause across the app, with an option to hide feed videos

#### Diagnostics & notifications

- Crash logging under Debug → Logging — Automatically save reports when Instagram crashes, with search, sharing and an indicator when RyukGram appears in the trace
- Share log files can now include crash reports
- Notification history — Save notifications in one searchable place, filter by feature or type, choose which features are recorded, and use a home shortcut with unread counts

### 🛠 Fixes

#### Instagram compatibility

- Updated compatibility with Instagram 447, 448 and 449
- DM inbox header buttons, chat menus, hidden chats, locks, refresh warnings and Meta AI search hiding work again on the new Swift inbox
- Inbox and profile action buttons no longer overlap the back button or username on older layouts
- Voice message downloads, forced DM saving and Meta AI menu hiding work again on newer Instagram
- Feed autoplay controls, story midcard hiding and sticker-reply seen state work again on Instagram 448
- Hiding the reels long-press menu and reels surveys works again on Instagram 448
- Keep deleted messages, reels playback speed, tap-to-mute on photo reels and feed refresh interval overrides work again on Instagram 448
- Hiding Meta AI and suggested people on the new chat screen works again
- The chat message preview no longer displays a Try Instagram Plus label

#### Media & downloads

- Saved voice messages now use the sender's name
- Profile and group pictures remain cached after links expire or caches are cleared, and Refresh Names & Photos updates every screen
- Story image saving with music now saves the photo instead of the video
- Save with music works again on affected photo posts
- Reels action button downloads photo posts opened from DMs again
- Instants saves and expanded media now use the correct account name
- Feed action button no longer offers bulk download for single posts or downloads older posts
- Switching crop ratios no longer leaves photos stuck zoomed in
- Audio trimming now displays the actual waveform, supports long recordings with a draggable selection limit, and correctly handles silent clips

#### Feed, reels & stories

- Instagram's native reels auto-scroll works again and switches off immediately when changing modes
- Reels auto-scroll no longer skips the first reel or advances before playback finishes
- Reels opened from profiles no longer have a stuck comment bar covering the bottom, with a toggle to restore it
- Custom story timestamps appear again on stories nearing expiration
- Story peek no longer closes Instagram
- Links open in the external browser again when that option is enabled
- OLED theme turns search bar backgrounds black and keeps the field inside grey
- OLED theme now covers the story viewers list

#### Profiles & notifications

- Read notifications work for users with custom settings even when the default Read setting is disabled
- Profile Analyzer now displays every change without truncating usernames, and entries remain visible during refresh
- Follower and following lists show the correct follow status without slowing scrolling
- Following a private account now correctly displays Requested when the action becomes a follow request
- Fake follower, following and post counts work on non-English Instagram and the newer profile header
- Fake counts now apply immediately without restarting Instagram
- No Suggested Users also removes unrelated accounts from the new chat list while preserving contacts and groups

#### Stability & settings

- Fixed inbox loading crashes caused by Keep Deleted Messages writing from multiple threads
- Copying from the share sheet no longer closes Instagram
- Quickly restarting Instagram several times no longer triggers a false crash detection
- MobileConfig overrides are preserved after repeated crashes and disabled instead of being erased
- MobileConfig overrides now apply correctly using the identifier Instagram actually reads
- MobileConfig overrides carry over when updating Instagram versions
- Backup and Restore now lives under Profiles, bringing export, import, reset and storage together
- Follow and unfollow batches now run more slowly, pause automatically when Instagram rate-limits requests, and stop before exceeding safe daily limits
- The follower and following filter/sort button no longer hides behind the tab bar
- Custom story fonts display their correct names in the font picker
- Sideloaded builds no longer install on devices too old to run them

### ⚠️ Known issues

- Reopening the story text tool highlights your last custom font but starts typing in the default font until you select the custom font again
- Unfollow confirmation is missing on profiles in Instagram 446 and later
