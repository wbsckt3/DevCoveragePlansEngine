# Esquemas de arquitectura RPA IndiGO (draw.io)

Abrir en [diagrams.net](https://app.diagrams.net) o con la extensión Draw.io de VS Code/Cursor.

| Archivo | Contenido |
|---------|-----------|
| `01_comparativa_fase1_fase2.drawio` | Comparativa Fase 1 vs Fase 2 |
| `02_fase1_front_contrato.drawio` | Fase 1: front-herinco + mock STOMP + hooks RPA |
| `03_fase2_spring_9rpa.drawio` | Fase 2: Spring Boot + 9 RPA + broker STOMP |

Arquitectura: HTTP saliente desde cada PC; tiempo real (STOMP/SockJS) solo en el back central; PDFs locales; sin Socket.IO en cada equipo.
