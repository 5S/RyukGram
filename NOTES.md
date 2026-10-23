# [release] RyukGram v1.5.0

### ✨ Highlights

- **Save all**: download every post, reel, story, highlight and profile picture from any profile, paced and resumable
- **Watchlist media**: new stories, posts and profile pictures from watched accounts saved in HD, with deletion alerts
- **Custom tabs**: add RyukGram screens, Saved and Activity as real tab bar tabs, with Instagram's own badges
- **Reels limits by weekday**: pick the days limits apply and set reels-free days
- **Shortcuts automation**: block reels, pause limits or toggle Messages-only from iOS Shortcuts, even without opening Instagram
- **Smarter search**: typo-tolerant search with highlighted matches in Settings, MobileConfig and every list
- **Safer API use**: far fewer requests, better pacing, hourly and daily limits, and full backoff on rate limits

### 🆕 New features

#### Gallery & media

- Save all from any profile menu by post count or date range, with a resumable queue, daily limit and optional HD videos
- Save all and Watchlist media can get their own Gallery folder, mix in, or stay hidden
- Upgrade saved posts, photos and videos to HD from the item menu
- New video player with pinch zoom, PiP, frame accurate scrubbing and double tap seeking
- Spot saved posts and stories deleted on Instagram, with a Deleted filter, off by default
- Save a whole folder to Photos, and delete Save all or Watchlist files by folder
- Pick several items from the gallery picker and send or post them together
- Hold any sticker to expand, save, share or copy its link, animated ones stay animated
- Cutout stickers can come from the Gallery, stay uncut, and be edited first
- Audio categories: hold a song in any music picker to file it, then pick it from a row or a manager

#### Profiles & tracking

- Watchlist saves new stories, posts, reels and profile pictures in HD, with per account choices
- Watchlist carousels save as one album, and each account's stories gather into one updating item
- Watchlist tracks bio links, pronouns, category, account type and public email and phone
- Approve or decline follow requests with a swipe or in bulk, with repeat requesters marked
- Following someone who declined you before asks first, showing how many times and when
- Follow requests get a home shortcut badge for new requests and answers
- Clone a profile: search or paste a link, pick what to copy, and optionally keep it synced
- Bio spoofing, story view count spoofing, and multipliers like 5x that follow the real count
- Spoofed posts and stories get a View button, and Boost all takes a custom amount

#### Reels & stories

- Reels limits by weekday, with reels-free days and a simpler Off, Time or Reels picker
- Extra reels time can be capped per day, with a custom amount and a wait before it unlocks
- Story playback panel adds PiP for video stories and next or previous person buttons
- Playback settings with a live preview, skip step picker and per control toggles
- Reel buttons can hide or move Instagram's new Shop similar button
- Instants eye button gets a Toggle mode, or hold it in Button mode to toggle read receipts
- Overlay layout editor can resize buttons and hide their circle backgrounds

#### Interface & shortcuts

- Tab bar editor adds real tabs with Instagram's red count badge, applied live and kept in Messages-only
- Launch tab, swiping and hold shortcuts share one Tab bar page, and launch can reopen the last tab
- Shortcuts page lists every link for iOS automations, with example shortcuts and a Siri prompt
- Messages-only page reworked with schedule days, timed sessions and undo
- Hide Meta AI per surface, including the About this post summary
- Hide some Instagram Plus upsells, and in-app banners for messages, activity or other accounts
- Hide the full screen button over feed videos
- Hide hidden chats from the share sheet
- Grid feed shading, spacing and rounded corners, and an option to turn off its cache
- Compact save sheet when you have no collections
- Safari extension opens any Instagram page in the app, and its banner swipes away
- Update prompt can be snoozed, skipped for a version or turned off
- Custom emoji fonts can be imported from Android emoji fonts
- Set the score you send in the DM emoji game
- Stacked notification pills share one width
- Slovak translation, thanks to @dddaaadddooo

#### MobileConfig & advanced

- MobileConfig marks configs and params new in the current Instagram version, with New filters
- Instagram API page shows live usage and cache hits, with an hourly background limit and a daily analyzer cap

### 🛠 Fixes

#### Instagram compatibility

- Works on Instagram 450, 451 and 452
- Reels download, expand and repost, DM inbox buttons, Messages-only, lock, story seen and notes work again on 452
- Send to group hide and confirm, story screenshot blocking and note actions work again on 451
- Force audio and the story menu hold work again on 450
- Like confirm, Hide Meta AI, story midcards and notes tray cover Instagram's newest variants
- Custom GIF in comments works with the new GIF button, and sticker slider counts update
- Note audio downloads and Plus story peek work again
- Hiding both call buttons also hides the group chat call button
- Full follower and post counts work again on the newer profile header
- Sideloaded iOS 15 and 16 builds run newer Instagram, and the share sheet no longer crashes on iOS 15.0 to 15.3

#### API & performance

- Far fewer and better paced API requests, which should cut Instagram warnings and rate limits
- Checkpoint and challenge replies count as rate limits, and the cooldown survives a relaunch
- Follow status in follower lists is correct and no longer slows scrolling
- Reels no longer stutter while downloads or background checks run
- Reel scrubber seeks respond faster and no longer stall playback
- Profile Analyzer and follow request batches keep running in the background

#### Media & playback

- Instants videos save as videos again
- Call recordings no longer sound sped up
- Voice messages sent as replies can be downloaded
- OGG voice messages play in the deleted messages log and Gallery
- HD previews start right away instead of downloading first
- Standard quality is greyed out when unavailable, and downloads no longer save broken files
- Spoofed post previews no longer go blank, and expired thumbnails reload properly
- PiP plays more videos, gives up on stuck playback and can retry
- Long links to a private account's post open the original post
- Muting from the reels playback panel sticks
- Disabling auto-unmute works again with the volume buttons

#### Interface & stability

- Message peek no longer marks chats as seen
- Grid feed respects the suggested posts and reels filters, and keeps loading after You're all caught up
- Hide suggested users also removes the suggested accounts carousel in reels
- Hide story highlights also skips them after stories end
- Story overlay buttons sit on the story on every screen size
- Reel sidebar buttons keep even spacing and no longer overlap when reordered
- Reels hold controls no longer crash Instagram
- Custom emoji fonts apply everywhere
- Profile picture in the story tray hold menu opens again
- Tab, shortcut, action bar and lock names follow the app language
- Settings icons share one size and color
- Settings search no longer shows a grey box on iOS 26
- Restoring a backup brings back the stories archive, and export ticks everything by default

### ⚠️ Known issues

- Unfollow confirmation is missing on profiles in Instagram 446 and later
