---

### 5. `docs/pruebas/analisis_caja_blanca.md`
```markdown
---
sidebar_position: 5
title: Análisis de Caja Blanca
---

# Pruebas de Caja Blanca 🧪

Las pruebas de caja blanca garantizan la cobertura de código y la solidez lógica de los módulos críticos, especialmente en el motor de análisis emocional y cifrado.

---

## 🔬 Caso de Prueba: Algoritmo de Evaluación de Estrés (`BiometricCore`)

El siguiente fragmento de código prueba la cobertura de caminos (*path coverage*) de la función que determina si se debe activar una alerta de pausa.

```typescript
// Módulo: biometric-core/stressCalculator.ts
export function calcularNivelEstrés(latenciaTipeoMs: number, vfc: number): string {
  if (latenciaTipeoMs < 0 || vfc < 0) {
    throw new Error("Métricas biométricas inválidas");
  }
  
  if (latenciaTipeoMs < 80 && vfc < 40) {
    return "ALTO_ESTRES";
  } else if (latenciaTipeoMs < 120 || vfc < 60) {
    return "ESTRES_MODERADO";
  }
  
  return "ESTADO_OPTIMO";
}
