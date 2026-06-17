# Plan de Mejora Continua

---

La mejora continua se sustenta en el ciclo PHVA (Planificar–Hacer–Verificar–Actuar) aplicado en cada retrospectiva de sprint y en las revisiones mensuales. El objetivo es que cada iteración sea mejor que la anterior y que las lecciones aprendidas se incorporen al proceso.

## Ciclo PHVA en el SGMM

| Fase           | Actividad                                      | Frecuencia         |
| -------------- | ---------------------------------------------- | ------------------ |
| Planificar (P) | Definir objetivo del sprint y métricas         | Cada sprint        |
| Hacer (H)      | Ejecutar historias y registrar datos           | Diaria             |
| Verificar (V)  | Comparar resultados con métricas y revisar KPI | Sprint Review      |
| Actuar (A)     | Definir acciones de mejora en la retrospectiva | Cada retrospectiva |

## Acciones de Mejora Identificadas en Retrospectivas

| Sprint | Problema detectado                    | Acción de mejora                                               | Estado       |
| ------ | ------------------------------------- | -------------------------------------------------------------- | ------------ |
| S2     | Demora en revisiones de código        | Establecer SLA de 24 h para PRs                                | Implementado |
| S4     | Defectos que llegan a QA              | Añadir pruebas unitarias obligatorias antes de PR              | Implementado |
| S6     | Requisitos ambiguos                   | Plantilla de historia con criterios de aceptación obligatorios | Implementado |
| S8     | Conocimiento concentrado en 1 persona | Pair programming en módulos críticos                           | En curso     |
| S10    | Pérdida de velocidad por bajas        | Plan de reemplazo y onboarding estructurado                    | En curso     |

## Métricas de Mejora

- Tasa de defectos escapados a producción: objetivo < 5 %.
- Tiempo medio de resolución de defectos: objetivo ≤ 2 días para severidad alta.
- Satisfacción del equipo (eNPS): objetivo ≥ 30.
- Cobertura de pruebas automatizadas: objetivo ≥ 80 %.
