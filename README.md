# Voice stimuli

Short voice clips used as first-impressions stimuli in a speech study. Hosted
here so the study platform can reference them by URL.

Each clip is the agent side of an ElevenLabs conversation: silence-trimmed,
padded with 0.5 s of silence at each end, and loudness-normalised to -23 LUFS
(EBU R128) with a -1 dBFS ceiling. 16 kHz mono, MP3 and WAV.

`manifest.csv` carries the provenance (source conversation id, recording time,
transcript, measured loudness before and after).

Browse and listen: <https://scwallbridge-aisi.github.io/voice-stimuli/>

Built by `build_voice_stimuli.py` / `publish_stimuli.sh` in the
conversation-modalities project.
