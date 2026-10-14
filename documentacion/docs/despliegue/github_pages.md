---

### 6. `docs/despliegue/github_pages.md`
```markdown
---
sidebar_position: 6
title: Despliegue en GitHub Pages
---

# Despliegue Continuo con GitHub Pages 🚀

Esta sección describe el proceso de compilación y publicación automática de la documentación de **MindPulse AI** utilizando GitHub Actions y GitHub Pages.

---

## ⚙️ Configuración del Proyecto (`docusaurus.config.ts`)

Para asegurar que los archivos estáticos y rutas funcionen correctamente en GitHub Pages, los campos principales se configuran como:

```typescript
const config: Config = {
  title: 'MindPulse AI - Documentación',
  url: 'https://<tu-usuario>.github.io',
  baseUrl: '/documentacion-daw/', // Nombre exacto del repositorio
  organizationName: '<tu-usuario>',
  projectName: 'documentacion-daw',
  deploymentBranch: 'gh-pages',
  // ...
};
