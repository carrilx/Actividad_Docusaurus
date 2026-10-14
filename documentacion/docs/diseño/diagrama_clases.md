---
sidebar_position: 3
title: Diagrama de Clases
---

# Diagrama de Clases de la Arquitectura 📐

El core del sistema se compone de gestores de análisis biométrico, evaluadores de sentimiento y el motor de privacidad.

```mermaid
classDiagram
    class Usuario {
        +String idUsuario
        +String email
        +String tokenCifrado
        +iniciarSesion()
        +consultarEstadisticas()
    }

    class EvaluadorSentimiento {
        +float scoreEgresado
        +analizarTexto(String texto) float
        +detectarFrustracion(List~String~ mensajes) AlertLevel
    }

    class BiometricMonitor {
        +float nivelTension
        +capturarRitmoTipeo(KeystrokeData data)
        +evaluarVFC(SensorData sensor)
    }

    class MotorPrivacidad {
        +String anonimizarUID(String id)
        +boolean cifrarRegistro(HealthRecord record)
    }

    class DashboardService {
        +renderizarGraficaPersonal()
        +generarReporteAnonimoEquipo()
    }

    Usuario "1" -- "1" DashboardService : consulta
    BiometricMonitor "1" --> "1" MotorPrivacidad : envía métricas crudas
    EvaluadorSentimiento "1" --> "1" MotorPrivacidad : envía análisis NLP
    MotorPrivacidad "1" --> "1" DashboardService : entrega datos seguros

