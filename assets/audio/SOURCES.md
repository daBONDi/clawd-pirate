# Audio-Quellen

| Datei | Quelle | Lizenz |
|-------|--------|--------|
| `cannon_fire.ogg` | https://opengameart.org/content/cannon-fire | CC0 |
| `cannon_hit.ogg` | https://opengameart.org/content/cannon-hit-wall | CC0 |
| `feuer.wav`, `aua.wav`, `nachgeladen.wav`, `treffer.wav`, `arrr.wav` | selbst erzeugt mit Piper TTS (MIT), Stimme `de_DE-thorsten-high` (https://huggingface.co/rhasspy/piper-voices, Datensatz CC0) | – |

Neu erzeugen (Host, `uv` vorhanden):

    uv venv piper-venv --python 3.12 && uv pip install --python piper-venv/bin/python piper-tts
    curl -L -o de_DE-thorsten-high.onnx https://huggingface.co/rhasspy/piper-voices/resolve/v1.0.0/de/de_DE/thorsten/high/de_DE-thorsten-high.onnx
    curl -L -o de_DE-thorsten-high.onnx.json https://huggingface.co/rhasspy/piper-voices/resolve/v1.0.0/de/de_DE/thorsten/high/de_DE-thorsten-high.onnx.json
    echo "Feuer!" | piper-venv/bin/piper --model de_DE-thorsten-high.onnx --output_file feuer.wav --length_scale 0.9

| `coins.wav` | https://opengameart.org/content/purchasing-sound-effect (Spring Spring, „Purchasing Sound Effect“; auf 24 kHz mono reduziert) | CC0 |
| `delfine.wav`, `wal.wav`, `hai.wav`, `kraken.wav`, `schiff.wav`, `schatz.wav`, `warnschuss.wav`, `nachladen.wav` | Piper TTS wie oben | – |
