# Deep-Live-Cam — Side project face swap (referencia local)

## Identity (single source of truth)
- Canonical slug: deep-live-cam
- 🔐 Secretos: onboardéalos SOLO por el Rotation Vault `http://127.0.0.1:8799` (card por secreto → Keychain + Infisical + edge/host auto). NUNCA `security add-generic-password` a mano ni pegar valores en el chat. Ver skill `infra` §Secretos.
- GitHub: Catalizadora/Deep-Live-Cam (origin) · upstream: hacksider/Deep-Live-Cam (ajeno)
- Tipo: experimento personal / clon ML (NO cliente Catalizadora)
- Stack: Python + tkinter UI + ONNX/insightface models

> Real-time face swap y video deepfake (single click, una sola imagen). Side project de Pablo.

## Qué es

Clone local del proyecto open-source Deep-Live-Cam (v2.1). Stack Python + tkinter UI + modelos en `models/`. Entry points: `run.py`, `start.sh`, `run-cuda.bat`, `run-directml.bat`. Features: real-time face swap, mouth mask, face mapping, multiple subjects.

El README upstream declara explícitamente disclaimers éticos y checks built-in para evitar contenido inapropiado.

## REGLA OPERATIVA — Uso responsable

- NO usar para deepfakes maliciosos, suplantación de identidad, contenido no consentido ni desinformación.
- Solo testing autorizado con consentimiento explícito del sujeto.
- Cualquier output compartido públicamente debe estar etiquetado como deepfake.
- Side project personal de Pablo: NO incluir en deliverables de clientes Catalizadora/Beautonomous.
- Respetar las restricciones de contenido del proyecto upstream (no nudity, gore, war footage, etc.).

## Memoria (Mem0)

- **Namespace obligatorio**: cuando llames `memory_save` del MCP `mem0`, pasa SIEMPRE:
  - `scope: "project_team"`
  - `project: "deep-live-cam"`
- **Antes de `memory_search`**, considera filtrar por `scope: "project_team"` para evitar contaminación con otros proyectos.
