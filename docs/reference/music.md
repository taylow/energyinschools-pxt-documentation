# Music

Generation of music tones through pin ``P0``.

```cards
music.playTone(0, 0);
music.ringTone(0);
music.rest(0);
music.beginMelody(music.builtInMelody(Melodies.Entertainer), MelodyOptions.Once);
music.stopMelody(MelodyStopOptions.All);
music.onEvent(MusicEvent.MelodyNotePlayed, () => {});
music.beat(BeatFraction.Whole);
music.tempo();
music.changeTempoBy(20);
music.setTempo(120);
```

## See Also

[playTone](/makecode-blockeditor/reference/music/play-tone), [ringTone](/makecode-blockeditor/reference/music/ring-tone), [rest](/makecode-blockeditor/reference/music/rest),
[beginMelody](/makecode-blockeditor/reference/music/begin-melody), 
[stopMelody](/makecode-blockeditor/reference/music/stop-melody),
[onEvent](/makecode-blockeditor/reference/music/on-event),
[beat](/makecode-blockeditor/reference/music/beat), [tempo](/makecode-blockeditor/reference/music/tempo), [changeTempoBy](/makecode-blockeditor/reference/music/change-tempo-by), [setTempo](/makecode-blockeditor/reference/music/set-tempo),
