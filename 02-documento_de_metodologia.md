# Documento de metodología

---

El SGMM adopta una metodología híbrida, que combina las fortalezas del enfoque ágil (Scrum) para el desarrollo del producto, con prácticas tradicionales del PMBOK para el control de la triple restricción (alcance, tiempo, costo) que la naturaleza contractual pública exige. Esta combinación permite entregar valor de forma incremental y, al mismo tiempo, mantener la gobernanza documental y presupuestaria que demanda la Alcaldía.

## Justificación de la Selección Metodológica

La selección se sustenta en tres factores:

1. Los requerimientos del sistema son susceptibles de cambiar (como efectivamente ocurrió con la normativa de licencias), lo que favorece un enfoque iterativo.
2. El cliente es una entidad pública que requiere entregables formales, hitos aprobados y trazabilidad presupuestaria, lo que exige un enfoque tradicional.
3. El equipo es pequeño (cinco a seis personas), condición ideal para Scrum.

## Componente Ágil - Scrum

| Elemento                   | Adaptación en el SGMM                                                                            |
| -------------------------- | ------------------------------------------------------------------------------------------------ |
| Rol: Product Owner         | Un analista funcional de la Dirección de Ingresos, con poder de decisión sobre el backlog.       |
| Rol: Scrum Master          | El jefe de proyecto asume además este rol, facilitando las ceremonias y eliminando impedimentos. |
| Rol: Equipo de desarrollo  | 3 a 4 desarrolladores + 1 QA. Tras las renuncias se ajustó la carga (ver Plan de Recursos).      |
| Artefacto: Product Backlog | Lista priorizada de historias de usuario en la herramienta Jira.                                 |
| Artefacto: Sprint Backlog  | Historias comprometidas por sprint.                                                              |
| Artefacto: Incremento      | Funcionalidad desplegable al final de cada sprint.                                               |
| Ceremonia: Sprint Planning | Cada 2 semanas, lunes. Duración 2 horas.                                                         |
| Ceremonia: Daily Scrum     | Diaria, 15 minutos, formato impedimentos.                                                        |
| Ceremonia: Sprint Review   | Cada 2 semanas, viernes. Demo con el Product Owner.                                              |
| Ceremonia: Retrospectiva   | Tras cada Review. Genera acciones de mejora continua.                                            |

## Componente Tradicional — Cascada para Gobernanza

Sobre la capa ágil se aplican los procesos tradicionales del PMBOK para las áreas de Integración, Alcance (línea base formal), Tiempo (cronograma con hitos), Costos (presupuesto y línea base), Riesgos (registro formal) y Comunicaciones (informes de estado). Los entregables contractuales (plan, requerimientos firmados, actas) siguen el ciclo cascada, mientras que la construcción del software sigue Scrum.

## Ciclo de Vida del Proyecto

El proyecto se organiza en cinco fases de gobernanza sobre las que se ejecutan trece sprints de desarrollo:

| Fase                    | Semanas  | Sprints | Producto principal                                |
| ----------------------- | -------- | ------- | ------------------------------------------------- |
| Inicio                  | 1–4      | —       | Acta, plan de proyecto, requerimientos            |
| Planificación detallada | 3–6      | S1–S2   | Backlog priorizado, arquitectura, cronograma base |
| Ejecución               | 5–23     | S3–S11  | Incrementos funcionales de los módulos            |
| Monitoreo y control     | Continuo | —       | Informes, KPI, registro de cambios y riesgos      |
| Cierre                  | 24–26    | S12–S13 | Validación, despliegue, lecciones aprendidas      |

## Definición de Hecho (Definition of Done)

- Código revisado por pares (peer review) y fusionado en la rama principal.
- Pruebas unitarias con cobertura ≥ 80 % y todas en verde.
- Pruebas de integración y de aceptación de la historia pasadas.
- Documentación técnica y de usuario actualizada.
- Despliegue en entorno de preproducción exitoso.
- Aceptación del Product Owner en la Sprint Review.

## Herramientas

- Gestión del proyecto y backlog: Jira + Confluence.
- Control de versiones e integración continua: Git + GitLab CI.
- Comunicación: correo institucional, reuniones virtuales y un panel físico Kanban en la oficina del proyecto.
- Gestión de calidad: SonarQube para análisis estático.
