# /audio

MP3 files for Field Notes episodes live here.

## Naming convention

```
ep1-before-the-clock-punched-in.mp3
ep2-the-guild-and-the-gift.mp3
ep3-the-dark-satanic-mills.mp3
```

## Size limit

GitHub has a **100MB per file** hard limit. GitHub Pages repos have a **1GB total** soft limit.

At ~1MB/min for 128kbps mono, a 45-minute episode ≈ 45MB. You have room for ~20 episodes before needing to move audio to external hosting (Backblaze B2 is the cheapest — $6/TB/mo, with a free Cloudflare CDN layer).

## Getting the audio_size field

Run this in your terminal to get the byte count for the feed enclosure tag:

```bash
wc -c < audio/ep1-before-the-clock-punched-in.mp3
```

Paste that number into the episode's `audio_size:` front matter field.

## Encoding recommendation

- Format: MP3
- Bitrate: 128kbps mono (voice)
- Sample rate: 44.1kHz
- Tags: Set title, artist, album art in your editor (Hindenburg, Descript, Audacity)
