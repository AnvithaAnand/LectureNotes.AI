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
    A[Video Input]:::input --> B[Speech to Text Engine]:::process
    C[Lecture Slides]:::input --> D[Slide Parser]:::process

    B --> E[Transcript Cleaning]:::process
    D --> F[Slide Content Extraction]:::process

    E --> G[Multimodal Alignment Layer]:::core
    F --> G

    G --> H[LLM Summarizer]:::core
    H --> I[Note Formatter]:::process
    I --> J[Final Notes Output]:::output

    classDef input fill:#d1ecf1,stroke:#0c5460,color:#0c5460;
    classDef process fill:#f8f9fa,stroke:#6c757d,color:#343a40;
    classDef core fill:#e2e3ff,stroke:#383d9a,color:#383d9a;
    classDef output fill:#d4edda,stroke:#155724,color:#155724;

