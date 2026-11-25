# AirWindow

Sistema de ventilación natural con apertura automática de ventana. Proyecto TFG, Media_Lab 2025.

El firmware del ESP32 controla el motor paso a paso y publica su estado por MQTT. La app móvil lee ese estado y envía órdenes y configuración por los mismos topics.

| Carpeta | Contenido | Stack |
|---|---|---|
| [firmware/](firmware/README.md) | Lectura de sensores, motor, finales de carrera, MQTT | ESP32, PlatformIO |
| [app/](app/README.md) | Control manual, modo automático, horarios y parámetros | React Native, Expo |

Los comandos de PlatformIO se ejecutan dentro de `firmware/` y los de Expo dentro de `app/`.
