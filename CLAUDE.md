# Video Editing — proxxy.sa

@~/.claude/skills/video-use/SKILL.md

## Project

This is the **Video Editing** project. All raw footage lives in this directory or a subdirectory. All session outputs go into `edit/` next to the sources.

## Default vlog prompt

When the user asks to edit footage without additional instruction, apply this intent:

> go ahead. make this vlog good. create a nice visual story with the footage you have. make sure it looks natural, chill, but not boring. don't cut me off if i'm talking. if there are clear mistakes in the recording of course don't include it. the goal is to view the final video and get a great sense of the time and experiences from the asset.

Translate this into editing decisions:
- **Preserve full speech.** Never cut mid-sentence or mid-thought. Only trim dead silence, obvious mic bumps, or clear recording errors (camera covered, hard clipping, "let me restart" retakes).
- **Natural pacing.** Keep breathing room — don't over-compress. 400–600ms between thoughts is fine. Let moments breathe.
- **Visual story structure.** Order beats chronologically but shape for arc: arrival/opening energy → experiences/highlights → quiet/reflective moments → close.
- **Chill but not flat.** Warm cinematic grade (`warm_cinematic`) unless the material calls for something else. Subtle motion — no jarring cuts.
- **Full sensory record.** The viewer should finish and feel like they were there.

## Helper invocation

Always invoke helpers via `uv run` inside the video-use repo:

```bash
uv run --project /home/user/video-use python /home/user/video-use/helpers/<script>.py [args]
```

Or activate the venv:

```bash
source /home/user/video-use/.venv/bin/activate
```

## ElevenLabs API key

Required for transcription. Check in this order:
1. `$ELEVENLABS_API_KEY` env var
2. `/home/user/video-use/.env`

If missing, ask the user once to paste their key from https://elevenlabs.io/app/settings/api-keys — then write it to `/home/user/video-use/.env` with `chmod 600`.
