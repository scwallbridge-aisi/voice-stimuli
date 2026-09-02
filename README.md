# Voice stimuli

Short voice clips for first-impressions stimuli, hosted for url access through pages.

Each clip is the agent side of an ElevenLabs conversation: silence-trimmed, padded with 0.5 s of silence at each end, and loudness-normalised to -23 LUFS (EBU R128) with a -1 dBFS ceiling. 16 kHz mono, MP3 and WAV.

Rounds 1 and 2 sit at the top level; every round after that has its own directory (`ELround3/`, ...), because voice names and utterance slugs repeat across rounds and would otherwise collide. Each directory carries its own `manifest.csv` and `index.html`.

`manifest.csv` carries provenance (source conversation id, recording time, transcript, measured loudness before and after).

Browse and listen: <https://scwallbridge-aisi.github.io/voice-stimuli/>

Built by `build_voice_stimuli.py` / `publish_stimuli.sh` in the conversation-modalities project.
