# clipper-upload

A **personal, single-user automation script** used by one individual creator to publish
their own short-form videos to their own YouTube channel.

This repository exists to document the application publicly. It is not the application
itself — the source code is kept in a private repository.

## What it does

1. Writes a script for a short educational video (topic: video "clipping" as a
   profession — how long-form content is cut into short clips, the editing skills
   involved, and the business side of it).
2. Generates a voice-over from that script.
3. Assembles a vertical 1080x1920 video with FFmpeg using licensed stock footage and
   burned-in subtitles.
4. Uploads the finished video to **the author's own YouTube channel** via the
   YouTube Data API (`videos.insert`).
5. Reads the performance of **the author's own videos** via the YouTube Analytics API
   so the author can evaluate retention and improve the next video.

Every video published is an original work created by the author.

## Scope of use

- **Users:** one — the author. There is no sign-up, no login page, no distribution.
- **Volume:** approximately one upload per day. Quota needs are minimal.
- **Channels touched:** only the author's own channel.

## What it does NOT do

- It does not download, copy, modify, or republish videos belonging to anyone else.
- It does not collect or store data about any other person.
- It does not display YouTube content anywhere outside of YouTube.
- It is not offered to, or usable by, any third party.

## YouTube API Services

This application uses YouTube API Services and is bound by the
[YouTube Terms of Service](https://www.youtube.com/t/terms). Data handling is
described in [PRIVACY.md](PRIVACY.md), and information obtained through YouTube API
Services is also governed by the
[Google Privacy Policy](https://policies.google.com/privacy).

OAuth scopes requested:

- `https://www.googleapis.com/auth/youtube.upload`
- `https://www.googleapis.com/auth/yt-analytics.readonly`

Access can be revoked at any time at https://myaccount.google.com/permissions.

## Contact

ikhlasbisnisdigital@gmail.com
