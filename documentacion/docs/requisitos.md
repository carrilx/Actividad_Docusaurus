---
sidebar_position: 2
title: Análisis de Requisitos
---

# Análisis de Requisitos - MindPulse AI 📊

A continuación se detallan los requisitos funcionales y no funcionales del sistema.

---

## ⚙️ Requisitos Funcionales (RF)

| ID | Nombre | Descripción |
| :--- | :--- | :--- |
| **RF-01** | Análisis de Sentimiento en Commits | El sistema analizará los mensajes de Git para detectar patrones de frustración o fatiga mediante NLP. |
| **RF-02** | Detección de Patrones de Tipeo | Medición del ritmo y presión de tecleo para detectar tensión fisiológica. |
| **RF-03** | Recomendación de Micro-pausas | Notificación inteligente que sugiere ejercicios de respiración guiada cuando el nivel de estrés supera el 75%. |
| **RF-04** | Dashboard Personal de Salud | Panel individual e inalterable accesible solo por el usuario para consultar su estado emocional histórico. |
| **RF-05** | Métrica Global de Equipo | Visión agregada y anonimizada para líderes de equipo sobre el nivel de agotamiento del departamento. |

---

## 🛡️ Requisitos No Funcionales (RNF)

* **RNF-01 (Privacidad y Cifrado):** Todos los datos emocionales y métricas biométricas deben cifrarse de extremo a extremo (E2EE) con AES-256. Ningún gestor o empresa podrá acceder a registros individuales.
* **RNF-02 (Rendimiento):** El análisis en segundo plano de patrones de tipeo debe consumir menos del 1.5% de la CPU del usuario.
* **RNF-03 (Cumplimiento Regulatorio):** Cumplimiento estricto con la RGPD (Europa) y la HIPAA (Estados Unidos) respecto al manejo de datos sensibles de salud.
* **RNF-04 (Tiempo de Respuesta):** El motor de IA debe retornar el indicador de bienestar en menos de 200 ms tras procesar un evento.
