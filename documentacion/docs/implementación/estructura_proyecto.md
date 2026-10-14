---

### 4. `docs/implementación/estructura_proyecto.md`
```markdown
---
sidebar_position: 4
title: Estructura del Proyecto
---

# Estructura del Proyecto 📁

La arquitectura de **MindPulse AI** está basada en una estructura monorepo modular utilizando TypeScript, Node.js y React (Docusaurus para la documentación).

```text
mindpulse-ai/
├── apps/
│   ├── client-desktop/      # Aplicación Electron/Tauri de monitoreo local
│   ├── web-dashboard/       # Dashboard web en React/Next.js
│   └── documentation/       # Sitio estático con Docusaurus (este proyecto)
├── packages/
│   ├── nlp-engine/          # Módulo de procesamiento de lenguaje natural
│   ├── biometric-core/      # Algoritmos de análisis de frecuencia e interacción
│   └── security-e2ee/       # Módulo de cifrado AES-256 y anonimización
├── docs/                    # Archivos Markdown de documentación
│   ├── intro.md
│   ├── análisis/
│   ├── diseño/
│   ├── implementación/
│   ├── pruebas/
│   └── despliegue/
├── .github/
│   └── workflows/
│       └── deploy-pages.yml # CI/CD para GitHub Pages
├── docusaurus.config.ts     # Configuración global de Docusaurus
└── package.json
