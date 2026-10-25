# Tilawah — spraakmodel

Het spraakmodel dat de Tilawah-app (iOS) gebruikt om Koranrecitatie te verstaan.
De app bevat het model niet zelf, maar haalt het hier op bij het eerste gebruik
van de opnameknop (±144 MB). Elke release bevat `manifest.json` met per bestand
de plek in de modelmap, de grootte en een SHA-256-controlegetal; de app
controleert ieder bestand na het ophalen.

The speech model used by the Tilawah iOS app to follow Quran recitation. The app
downloads it on first use of the record button (about 144 MB) and verifies every
file against `manifest.json` (path, size, SHA-256).

## Herkomst / origin

- Model: [tarteel-ai/whisper-base-ar-quran](https://huggingface.co/tarteel-ai/whisper-base-ar-quran)
  (Apache License 2.0), a Whisper base model fine-tuned on Quran recitation by Tarteel.
- Converted to Core ML with [whisperkittools](https://github.com/argmaxinc/whisperkittools) (Argmax).
- Tokenizer files from [openai/whisper-base](https://huggingface.co/openai/whisper-base).

Zie `NOTICE` voor de licentievermeldingen. Dit is geen eigen werk van Tilawah;
het is hier alleen gepubliceerd zodat de app het kan downloaden.
