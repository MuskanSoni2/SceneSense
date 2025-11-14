# SceneSense: A Multimodal Vision-Language Consistency Analyzer


# SceneSense  
### *Multimodal Scene–Dialogue Consistency Analyzer*

“Where vision meets language — and truth is verified.”

- 🎬 Multimodal Scene–Dialogue Consistency Analyzer
- 🔍 Check whether what is said matches what is seen.
- 🧠 Combines NLP, Computer Vision, and Multimodal Reasoning.

SceneSense is an AI system that checks whether **what is said in a video matches what is happening on screen**.  
It analyzes video frames + audio transcript, extracts events, and detects inconsistencies using a multimodal reasoning pipeline.

---

## 🔥 Key Features

- 🎥 **Visual Event Extraction**  
  Detects objects, actions, attributes, and spatial relations from video frames.

- 🎙️ **Dialogue Semantic Parsing**  
  Converts spoken text into structured event representations.

- 🔗 **Cross-Modal Alignment**  
  Compares visual events with spoken events to detect mismatches.

- 🧠 **Multimodal LLM Reasoning**  
  Uses an LLM to provide natural-language explanations of inconsistencies.

- 📊 **Scoring System**  
  Generates a consistency score based on subject/action/object/attribute alignment.

- 🧾 **Explainable Output**  
  Understand *why* a scene contradicts the dialogue.

---

## 🧩 Architecture Overview
       ┌───────────────┐                 ┌───────────────────┐
       │     Video     │                 │       Audio       │
       └───────┬───────┘                 └─────────┬─────────┘
               │                                     │
               ▼                                     ▼
       ┌──────────────┐                    ┌───────────────────┐
       │ Frame Sampler│                    │   Speech-to-Text  │
       └───────┬──────┘                    │     (ASR/Whisper) │
               │                           └─────────┬─────────┘
               ▼                                     │
     ┌────────────────────┐                 ┌──────────────────────┐
     │ Visual Event       │                 │ Dialogue Semantic    │
     │ Extraction (YOLO,  │                 │ Parsing (LLMs,       │
     │ DETR, SAM, etc.)   │                 │ Event Extraction)    │
     └─────────┬──────────┘                 └──────────┬───────────┘
               │                                       │
               └────────────────────┬──────────────────┘
                                    ▼
                  ┌──────────────────────────────────┐
                  │   Multimodal Alignment Engine    │
                  │  (Visual ↔ Dialogue Comparison)  │
                  └────────────────┬─────────────────┘
                                   ▼
                ┌─────────────────────────────────────────┐
                │ Consistency Score + Explanation (LLM)   │
                └─────────────────────────────────────────┘

       
## 🧪 Example Use Cases

- 🎬 Film/TV continuity checking

- 🔍 Video fact-checking

- 📚 Educational video verification

- 🛡️ Safety compliance monitoring

- 📰 Fake/misinformation video detection

🤝 Contributing

Pull requests are welcome!
Please open an issue first to discuss your ideas.
