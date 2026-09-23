# SLIX AI

**SLIX** is a local AI assistant designed to combine conversational AI, web research, file analysis, memory, coding, project creation, and AI-powered development tools into one modular application. SLIX runs AI models locally while optionally using the internet for research.

---

## Vision
SLIX aims to unify the best features of modern AI assistants into a single, modular system:
- ChatGPT-style conversational AI
- Gemini-style modern user interface
- Perplexity-style web research
- Claude-style coding-agent workflow

The architecture is designed to be modular, allowing models and features to be replaced or upgraded as needed.

---

## SLIX: The AI Assistant
SLIX supports a wide range of capabilities, including:
- General conversation and question answering
- Reasoning and mathematical problem-solving
- Web research and internet search
- Source-based research with citations
- Long conversations with history
- Persistent, user-controlled memory (SQLite)
- File uploads and document analysis (TXT, PDF, DOCX, code files, etc.)
- Image understanding (if a vision-capable model is used)
- Code generation, explanation, and debugging
- Markdown and code block support
- Project creation and management

---

## Memory System
SLIX uses **SQLite** for persistent memory, allowing users to:
- Add, view, delete, or clear memories
- Ask SLIX to remember specific information
- Control what is saved (not all conversations are stored as permanent memory)

---

## Web Research
When research mode is enabled, SLIX:
1. Searches relevant sources
2. Collects and analyzes information
3. Generates a response with source links/citations
4. Never pretends to have searched the web if it hasn’t

---

## File Analysis
SLIX supports file types like:
- Text: TXT, PDF, DOCX
- Code: Python, C, C++, Java, JavaScript, TypeScript, HTML, CSS, JSON, CSV
- Users can upload files and ask questions about them

---

## Image Understanding
- Compatible with vision-capable models (if available)
- Architecture allows vision models to be added without redesigning the entire app
- If the selected model doesn’t support vision, SLIX will clearly indicate this

---

## NEO: SLIX Coding Agent
**NEO** is the coding-agent component of SLIX, designed for software development tasks:
- Create/manage projects, folders, and files
- Read, edit, explain, and debug code
- Find errors, run programs, and test builds
- Analyze terminal output
- Show changes and help develop complete applications

**Supported Languages:**
Python, C, C++, Java, JavaScript, TypeScript, HTML, CSS, React, Node.js, SQL

**Safety:**
- Uses a safe project workspace
- Avoids destructive operations without confirmation

---

## Local AI Architecture
SLIX is built around local AI models (e.g., GGUF) and supports:
- Python backend (FastAPI)
- SQLite for conversation history, memory, and app data
- llama.cpp / llama-cpp-python for local inference
- Frontend: HTML, CSS, JavaScript (modern, dark-themed UI)

**Planned Model Architecture:**
- SLIX: Llama-family model for general conversation
- NEO: Qwen-family model for coding tasks
- Model files may be distributed separately based on their licenses

**Note:** SLIX does not claim ownership of third-party models or libraries. Their licenses are separate.

---

## Project Structure
