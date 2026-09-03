# Voice stimuli

Short voice clips for first-impressions stimuli, hosted for url access through pages.

Every clip is processed identically: resampled to 16 kHz mono, silence-trimmed, padded with 0.5 s of silence at each end, and loudness-normalised to -23 LUFS (EBU R128) with a -1 dBFS ceiling. MP3 and WAV.

Clips come from one of two sources, given per row by the `source` column of `manifest.csv`: `elevenlabs` (one side of an ElevenLabs conversation) or `file` (audio rendered or recorded elsewhere). `manifest.csv` also carries the provenance -- conversation id, recording time and transcript for EL clips, the source filename for the rest -- plus the measured loudness before and after.

The current flat build sits at the top level; every round published since then has its own directory (`ELround3/`, ...), because a voice can be re-recorded in a later round under the same name and would otherwise overwrite the published clip. Each directory carries its own `manifest.csv` and `index.html`.

Browse and listen: <https://scwallbridge-aisi.github.io/voice-stimuli/>

Built by `build_voice_stimuli.py` / `publish_stimuli.sh` in the conversation-modalities project.
