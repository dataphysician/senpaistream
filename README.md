## Senpai Stream
Overview

Senpai Stream transforms graphic novels into immersive, narrated audiobooks. Leveraging cutting-edge technologies, Senpai Stream converts manga into a compelling audio narrative with dynamic, character-specific voices. Whether you're a manga enthusiast or someone looking for accessible storytelling, Senpai Stream brings the vibrant world of manga to life through sound.

[![Vimeo link to Senpai Stream Demo](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/003/293/375/datas/original.png)](https://vimeo.com/manage/videos/1059640936)

## Motivation

Manga tells stories through a unique blend of detailed artwork and minimalistic text. However, many fans and visually impaired users often miss out on the full experience. Senpai Stream was created to:

- Enhance Accessibility: Convert manga visuals and dialogues into rich audio narratives.
- Deliver Immersive Narration: Generate detailed, emotionally engaging descriptions that complement character dialogues.
- Fuse Technologies: Combine advanced OCR, NLP, and TTS technologies to offer an end-to-end multimedia experience.

## Technology Stack

**Transcript Handling:**
        Users provide a PDF manga that is separated out into individual images. The images are then annotated by the [Magi v2 model from HuggingFace](https://huggingface.co/ragavsachdeva/magiv2), which captures all character dialogues and scene descriptions. The image panels are also visually annotated to provide proper guidance to a visual language model.
 
**Narrative Generation:**
        A VLM processes the transcript alongside the panel images to generate a vivid narrative script in a style reminiscent of Japanese manga storytelling.

**Text-to-Speech (TTS):**
        ElevenLabs’ TTS engine converts each dialogue segment into high-quality audio, mapping character identities to unique, expressive voices.

**User Interface:**
        A notebook-based web interface provides a simple and interactive experience, displaying detailed processing logs and enabling immediate audio playback.

**Manga Example:**
        [Regards to Black Jack Volume 1](https://densho810.com/free/) (Royalty Free)
