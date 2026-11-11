# GD Rewind Shorts

Turns [@GDRewind](https://x.com/GDRewind) posts into 9:16 shorts and posts them to TikTok, Instagram Reels and YouTube Shorts.

This repo runs the app on a timer. Every 10 minutes it looks for new posts with a video, makes the short and posts it.

## What is in here

- `app/` is the Windows app. It also runs by hand on a PC, with a window for editing.
- `seen.txt` is the list of posts already dealt with. A post in this list is never made or posted again.
- `.github/workflows/shorts.yml` is the timer.

## How to

- **Pause it:** Actions, Shorts, the three dots, Disable workflow.
- **Test a video without posting:** Actions, Shorts, Run workflow, type a post id (the number at the end of the post's link). The video shows up under Artifacts on that run.
- **Check the key still works:** same as the test, but type `accounts` instead of a post id.
- **Update the app:** replace `app/GD Rewind Shorts.exe` and push.

Posting goes through Zernio. The key is stored as the `ZERNIO_KEY` secret.
