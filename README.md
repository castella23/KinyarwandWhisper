
  🗣️ KinyaWhisper Voice Assistant

KinyaWhisper is a lightweight Kinyarwanda voice assistant that demonstrates how humanoid robots can interact with people in local languages. It uses a fine-tuned Whisper model for speech recognition, simple NLP for understanding, and text-to-speech for spoken replies. Built as part of an academic project, this assistant showcases the power of AI in culturally relevant applications.

---

  🎯 Project Goals

- Build a mini Kinyarwanda voice assistant from scratch.
- Enable full interaction in Kinyarwanda: speech-in, speech-out.
- Support real-time and batch transcription.
- Demonstrate how ASR, NLP, and TTS can power voice-enabled robots.

---

  🧠 Features

- 🎙️  Automatic Speech Recognition (ASR)  using the `kinyawhisper` model.
- 🧠  Natural Language Processing (NLP)  using rule-based and fuzzy matching.
- 🔊  Text-to-Speech (TTS)  replies using `pyttsx3` (offline).
- 🖥️ CLI and optional Streamlit GUI interface.
- 🗃️ Transcribes `.wav` files and matches them to answers in Kinyarwanda.

---

  🗂️ Folder Structure

```
.
├── audio/                   # 6 custom audio samples (Kinyarwanda)
├── dataset.jsonl           # Metadata: audio path + transcription
├── kinya-whisper-model/    # Fine-tuned Whisper model output
├── train.py                # Whisper training script
├── inference.py            # Batch transcription script
├── main.py                 # Voice assistant (batch mode)
├── bach_main.py            # Live voice input (CLI)
├── transcriptions.txt      # Transcription results
├── README.md               # Project documentation
```

---

  🚀 Quickstart

 # 1. Install Requirements

```bash
git clone https://github.com/your-username/KinyaWhisper.git
cd KinyaWhisper
pip install -r requirements.txt
```

 # 2. Run Voice Assistant (Batch Mode)

```bash
python main.py
```

 # 3. Run CLI (Live Audio)

```bash
python bach_main.py
```

 # 4. Transcribe Audio Only

```bash
python inference.py
```

 # 5. Train a New Model (Optional)

```bash
python train.py
```

---

  🧪 Sample Questions & Answers

| Question (Kinyarwanda) | Assistant Response                   |
|------------------------|--------------------------------------|
| amakuru yawe           | Ni meza, urakoze!                    |
| witwa nde              | Nitwa Mudasa AI.                     |
| uzi ikinyarwanda       | Nkunda gufasha abantu mu rurimi rwacu. |
| umupira                | Umupira ukinwa n’amakipe abiri.     |
| amafaranga             | Amafaranga akoreshwa mu kugura ibikoresho. |

> Fuzzy matching improves recognition even if the transcription isn't exact.

---

  📊 Training Summary

-  Model Used : `kinyawhisper`
-  Dataset: 6 Kinyarwanda audio samples
-  Fine-tuning Tool : Hugging Face Transformers

---

  ⚠️ Limitations

- Model may misrecognize if speech is too fast or unclear.
- Best results on short, clear Kinyarwanda phrases.
- Dictionary-based NLP may not scale to complex queries.

---

  📬 Contact

 Author : Ineza Cinta Castella (@castella23)  
📧 castellaine23@gmail.com  
🔗 GitHub: https://github.com/castella23

---

  📚 Acknowledgements

This project was developed for the  Intelligent Robotics  course at  Rwanda Coding Academy , under the guidance of  Gabriel Baziramwabo .
