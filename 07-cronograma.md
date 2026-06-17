# Cronograma del Proyecto

---

El cronograma se construye sobre una línea base de 26 semanas, organizada en 13 sprints quincenales. Los hitos principales son las entregas de incrementos y las aprobaciones formales del cliente. La ruta crítica atraviesa los módulos de registro, cobro y licencias, ya que el módulo de informes depende de los datos que ellos generan.

## Hitos Principales

| Hito                                  | Semana | Fecha      | Criterio de cierre                     |
| ------------------------------------- | ------ | ---------- | -------------------------------------- |
| M0 — Acta aprobada                    | 2      | 16/01/2026 | Firmas del sponsor y JP                |
| M1 — Backlog y arquitectura aprobados | 4      | 30/01/2026 | ERS y arquitectura firmadas            |
| M2 — MVP funcional interno            | 22     | 11/06/2026 | Todos los módulos Must listos          |
| M3 — Validación del cliente           | 24     | 25/06/2026 | Acta de validación firmada             |
| M4 — Despliegue y cierre              | 26     | 03/07/2026 | Sistema en producción y acta de cierre |

## Plan de Sprints

| Sprint | Semanas | Objetivo                             | Entregable                  |
| ------ | ------- | ------------------------------------ | --------------------------- |
| S1     | 3–4     | Setup técnico, arquitectura, backlog | Entorno y backlog inicial   |
| S2     | 5–6     | Autenticación y roles                | Login y RBAC (RF-19, RF-20) |
| S3     | 7–8     | Registro de comerciantes             | RF-01, RF-02                |
| S4     | 9–10    | Registro de puestos + carnet QR      | RF-03, RF-04, RF-05         |
| S5     | 11–12   | Configuración de tarifas             | RF-07                       |
| S6     | 13–14   | Cobro y comprobantes                 | RF-06, RF-08                |
| S7     | 15–16   | Conciliación y notas de crédito      | RF-09, RF-10                |
| S8     | 17–18   | Licencias sanitarias e inspecciones  | RF-11, RF-12, RF-15         |
| S9     | 19–20   | Alertas y reportes sanitarios        | RF-13, RF-14                |
| S10    | 21–22   | Panel e informes                     | RF-16, RF-17, RF-18         |
| S11    | 23      | Bitácora y auditoría                 | RF-21                       |
| S12    | 24      | Pruebas de sistema y UAT             | Plan de pruebas ejecutado   |
| S13    | 25–26   | Despliegue y estabilización          | Sistema en producción       |

## Ruta Crítica

La ruta crítica del proyecto está compuesta por la cadena: autenticación (S2) → registro de comerciantes (S3) → registro de puestos (S4) → configuración de tarifas (S5) → cobro (S6) → licencias (S8) → panel e informes (S10) → pruebas y despliegue (S12–S13). Cualquier retraso en esta cadena impacta directamente la fecha de cierre. Los módulos de conciliación (S7) y alertas (S9) tienen holgura.

## Ajuste del Cronograma tras la Semana 10

Tras la solicitud de geolocalización (semana 10) y la renuncia de dos desarrolladores clave, el cronograma se reestimó. El módulo de geolocalización se reprogramó fuera del MVP original como incremento opcional de los sprints S11–S12, condicionado a la autorización del cambio. Las holguras de los sprints S7 y S9 se absorbieron parcialmente para mitigar el impacto de las renuncias. La línea base revisada mantiene el hito M4 del 03/07/2026 gracias a las acciones de mitigación de riesgos descritas en el [registro actualizado](16-registro_de_riesgos_actualizado.md).
