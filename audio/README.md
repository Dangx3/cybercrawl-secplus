# Background music

CyberCrawl has a built-in music player (mute button, volume slider, skip button, track name — visible in the HUD on the map and combat screens), but it doesn't ship with any audio files, since redistributing licensed/commercial music through a public repo isn't something we can do.

To enable music, drop your own tracks into this folder using these exact filenames:

```
audio/track1.mp3
audio/track2.mp3
audio/track3.mp3
audio/track4.mp3
```

The player loops through all four in order and repeats. Any royalty-free or properly-licensed-for-your-use MP3 works — good sources include [Pixabay Music](https://pixabay.com/music/), [Free Music Archive](https://freemusicarchive.org/), or your own recordings.

## Using fewer or more tracks

The playlist is defined near the bottom of `index.html`, just above `const AUDIO = {`:

```js
const PLAYLIST = [
  { name: 'Track 1', src: 'audio/track1.mp3' },
  { name: 'Track 2', src: 'audio/track2.mp3' },
  { name: 'Track 3', src: 'audio/track3.mp3' },
  { name: 'Track 4', src: 'audio/track4.mp3' },
];
```

Add, remove, or rename entries freely — `name` is just the display label shown in the HUD, and `src` is the file path. The player works with any number of tracks (including just one).

## Note if you deploy this yourself

If you're running your own copy of this repo and add copyrighted music you don't have redistribution rights for, keep your repo **private** and don't enable a public GitHub Pages deployment for it — publishing licensed audio files (even indirectly, via `git push`) on a public page can violate the license and put your account at risk of a takedown.
