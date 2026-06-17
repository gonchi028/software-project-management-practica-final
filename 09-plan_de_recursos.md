# Plan de Recursos Humanos

---

El plan de recursos describe la composición del equipo, los roles y responsabilidades, y la estrategia frente a la rotación. Especialmente relevante por la materialización del riesgo de renuncia de dos desarrolladores clave a mitad del proyecto.

## Estructura Organizacional del Proyecto

| Rol                             | Asignación                      | Responsabilidades clave                                                 |
| ------------------------------- | ------------------------------- | ----------------------------------------------------------------------- |
| Jefe de proyecto / Scrum Master | 20 % dedicación                 | Planificación, control, comunicación con sponsor, facilitación de Scrum |
| Product Owner                   | Parcial (Dirección de Ingresos) | Priorización del backlog, aceptación de incrementos                     |
| Arquitecto de software          | Parcial (30 %)                  | Decisiones técnicas, revisiones de arquitectura                         |
| Desarrollador backend (2)       | 100 %                           | API, lógica de negocio, base de datos                                   |
| Desarrollador frontend (1)      | 100 %                           | Interfaz web React                                                      |
| Ingeniero QA / Pruebas          | 100 %                           | Casos de prueba, automatización, UAT                                    |

## Distribución del Esfuerzo por Fase

| Rol              | Inicio | Ejecución | Cierre |
| ---------------- | ------ | --------- | ------ |
| Jefe de proyecto | Alta   | Media     | Alta   |
| Product Owner    | Alta   | Media     | Alta   |
| Arquitecto       | Alta   | Media     | Baja   |
| Desarrolladores  | Baja   | Alta      | Media  |
| QA               | Baja   | Alta      | Alta   |

## Gestión de la Rotación — Caso de las Renuncias

Aproximadamente en la semana 10 renunciaron dos desarrolladores clave: un desarrollador backend senior y el único desarrollador frontend. Este evento estaba previsto en el [registro de riesgos](10-registro_de_riesgos.md) (probabilidad media, impacto alto). Las acciones de contingencia ejecutadas fueron:

- Activación inmediata del plan de reemplazo: contratación de un desarrollador backend intermedio y reubicación interna de un desarrollador frontend desde otro proyecto.
- Redistribución temporal de tareas: el arquitecto asumió temporalmente tareas backend críticas durante dos semanas.
- Aceleración del onboarding mediante pair programming con los desarrolladores restantes y uso de la documentación técnica actualizada.
- Re-estimación del backlog: historias de menor prioridad (categoría Should) se movieron al backlog posterior para proteger el alcance Must.
- Reforzar la documentación y el emparejamiento (pairing) para reducir el riesgo de concentración de conocimiento.

## Matriz RACI (extracto de procesos clave)

| Actividad                      | JP  | PO  | Arq. | Dev | QA  |
| ------------------------------ | --- | --- | ---- | --- | --- |
| Definir y priorizar el backlog | C   | R/A | C    | I   | I   |
| Diseño técnico de un módulo    | C   | I   | R/A  | C   | I   |
| Desarrollo de historias        | I   | I   | C    | R/A | C   |
| Pruebas y aceptación           | I   | C   | I    | C   | R/A |
| Aprobación de cambios          | R   | C   | C    | I   | I   |
| Aprobación formal final        | C   | R/A | I    | I   | C   |

R = Responsable, A = Aprobador, C = Consultado, I = Informado.
