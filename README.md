# SWN-OTOM

Automation for generating narrated videos using n8n.

## Workflow Overview

```mermaid
graph TD
    A[Telegram Trigger] --> B[Set API Keys]
    B --> C[Extract Script]
    C --> D[Split Sentences]
    D --> E[Combine Script]
    E --> F[ElevenLabs TTS]
    F --> G[OpenAI Whisper]
    G --> H[Build Timing Map]
    H --> I[Prompt Builder]
```

Each node in the workflow includes an in-flow note describing its purpose and any important behaviors, helping future contributors navigate the automation. Related nodes can be further modularized into sub-workflows as the project grows.

