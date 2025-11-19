# 📘 LectureNotes.AI  
### Multimodal LLM Pipeline for Automated Lecture Note Generation  
_Built with ❤️ by **Anvitha Anand**_

---

## 🚀 Overview
LectureNotes.AI is a **multimodal note-generation system** that converts **educational videos + lecture slides** into high-quality, structured notes using a fully automated LLM pipeline.

The system integrates:
- Speech-to-Text transcription  
- Slide parsing + layout extraction  
- Multimodal alignment  
- LLM summarization + topic segmentation  
- Output formatting with emphasis & structured sections  

🎯 **Goal:** Reduce manual note-taking by **85%** while maintaining a **92%+** summarization accuracy across multiple academic domains.

---

## 🧠 Features
- 🎤 **Video → Text Pipeline** using Groq/HF STT  
- 🖼️ **Slide Parsing** using python-pptx  
- 🔗 **Multimodal Alignment** (slides + transcript merged automatically)  
- ✍️ **LLM Summaries** using structured prompts  
- 🧩 **Topic-Based Chunking** for clear notes  
- 📘 **Final Note Export** as Markdown / PDF / DOCX  
- ⚡ **Fast Processing** using Groq/LangChain optimizations  

---

## 🏗️ System Architecture

```mermaid
flowchart TD
    A[Video Input] --> B[Speech-to-Text Engine]
    C[Lecture Slides] --> D[Slide Parser]

    B --> E[Transcript Cleaning]
    D --> F[Slide Content Extractor]

    E --> G[Multimodal Alignment Layer]
    F --> G

    G --> H[LLM Summarizer]
    H --> I[Structured Note Formatter]
    I --> J[Final Notes (PDF/MD/DOCX)]
