# auralis

a clean, bloat-free alternative to spotify

---

## x01 - The Problem and Idea

It's no secret that Spotify tracks you. They have a "Spotify Wrapped", which shows you statistics they collected on your listening habits and what songs you enjoy.

One of my friends who is an absolute music addict hates the idea of Spotify and other major music apps jotting down personal information on you. That's where I got the idea for this app from, all the way back in September.

## x02 - A Roadblock and Rabbithole

The first issue that came up was, of course, music licensing. I couldn't just have the app scrape stream URLs from big providers, as that would violate their ToS. I spent weeks trying to find something that would provide music for my app. I turned to YouTube's Player API, which uses YouTube's music but gives my code control over the player, such as seeking.

The setup was a invisible video frame that held the video, and a Google Cloud project with the YouTube Search API to search YouTube's library.

## x03 - What about the mess of results?

As I started building the central frame of the app, I ran into a major issue. Simply searching YouTube would cause results such as song reviews, music videos that don't match timestamps, and more. To solve this issue, I leveraged [Groq](https://groq.com)'s lightning-fast inference to place a small AI model in-between the search results and my app. It would sift through the results and return just the result with the actual track.

## x04 - Personal Issues

Halfway into development, end-of-quarter testing and fall-testing kicked in full-force. This diverted my focus from building Auralis and other apps onto more academics. This heavily slowed down development, and often caused confusion looking at my code after a month of not touching the project.

To solve this issue, I built a small, basic tracker app that tracked the development of the app and encouraged me to work on it whenever I had the free time. It motivated me to do productive activities rather than do other useless things like scroll on TikTok.

## x05 - Lyrics

One of the most popular Spotify features is, of course, word-synced lyrics. I figured I could do better. After a lot of digging, I found that Musixmatch offered richsynced (letter-by-letter) lyrics. After obtaining a API key from Musixmatch, I built a richsync parser for my app and made a beatiful richsync display.

<img width="600" height="364.63195691203" alt="Richsync Display on Auralis" src="https://github.com/user-attachments/assets/d7449f73-2377-4835-950b-c4a57611e75f" />

## x06 - Polishing up Auralis

As December approached, I aimed to get Auralis ready to release by Christmas. I began to add final touches, such as importing playlists from Spotify, uploading custom MP3 songs, and color theme selection. By the release date, Auralis looked immaculate.

<img width="1895" height="896" alt="image" src="https://github.com/user-attachments/assets/87218813-fd87-47da-86d2-98e049f79772" />

## x07 - The Future of Auralis (as of 3/6/26)

Auralis is the first ever real long-term project for me. While most projects I leave mostly untouched after release, I wanted this one to last on.

Auralis will continue to get constant updates to its web version on the [Aeos Website](https://aeosntw.web.app/music/app/). The desktop and Android builds might lag behind a few updates due to difficulties in packaging.

## x08 - What about my device?

Auralis, unfortunately, will likely never be available for iPhone. Packaging a iOS app requires owning Mac hardware, which I simply don't have the money to afford. I'm working on a Linux version, but I'm still dealing with installation issues on some Linux distros.

===

Take care, 

`SuperUltraDude | Aeosdev`
