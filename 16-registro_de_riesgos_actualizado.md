# Registro de Riesgos Actualizado

---

Tras la materialización de los riesgos R-01 y R-02 y la aprobación del cambio FSC-001, el registro de riesgos se actualizó. Se incorporan los riesgos derivados del cambio, se reevalúan los riesgos materializados y se documentan las lecciones.

## Estado de los Riesgos Iniciales

| ID   | Riesgo                             | Estado        | Acción ejecutada                                                                     |
| ---- | ---------------------------------- | ------------- | ------------------------------------------------------------------------------------ |
| R-01 | Cambio normativo sobre licencias   | MATERIALIZADO | Diseño flexible permitió adaptar reglas sin reescritura; gasto de 30 h de la reserva |
| R-02 | Renuncia de personal técnico clave | MATERIALIZADO | Plan de reemplazo activado; onboarding acelerado con pairing                         |
| R-03 | Datos maestros incompletos         | Mitigado      | Depuración completada                                                                |
| R-04 | Indisponibilidad de servidores     | Aceptado      | Sin recurrencia significativa                                                        |
| R-05 | Resistencia al cambio              | Mitigado      | Capacitación iniciada                                                                |
| R-06 | Cambios de alcance                 | MATERIALIZADO | FSC-001 gestionado y resuelto                                                        |
| R-07 | Demora del PO                      | Mitigado      | SLA acordado y cumplido                                                              |
| R-08 | Vulnerabilidades de seguridad      | Monitoreo     | Sin hallazgos críticos                                                               |

## Nuevos Riesgos Derivados del Cambio y la Situación

| ID   | Riesgo                                                             | P     | I     | Sev. | Estrategia                                                            | Responsable |
| ---- | ------------------------------------------------------------------ | ----- | ----- | ---- | --------------------------------------------------------------------- | ----------- |
| R-09 | Precisión insuficiente del GPS y calidad de coordenadas capturadas | Media | Medio | 4    | Mitigar: validación en captura y depuración periódica                 | Arq.        |
| R-10 | Sobrecarga del equipo durante el onboarding de los reemplazos      | Alta  | Medio | 6    | Mitigar: priorizar alcance Must, horas extraordinarias acotadas       | JP          |
| R-11 | Pérdida de conocimiento tácito por las renuncias                   | Media | Alto  | 8    | Mitigar: pairing, documentación obligatoria, revisiones cruzadas      | Arq.        |
| R-12 | Sobrecosto al cierre (EAC > BAC)                                   | Media | Alto  | 8    | Mitigar: control estricto, repriorización del backlog, uso de reserva | JP          |

## Lecciones de los Riesgos Materializados

**Caso R-02 — Renuncia de personal clave**

El riesgo fue correctamente identificado con probabilidad media e impacto alto. La existencia de un plan de contingencia preacordado con recursos humanos permitió activar el reemplazo en menos de una semana. Sin embargo, la pérdida de conocimiento tácito del frontend no pudo compensarse totalmente y generó una caída de velocidad del 21 % durante dos sprints. Lección: reforzar la rotación de conocimiento (pairing, documentación viva) de forma preventiva, no solo cuando ocurre el riesgo.

**Caso R-06 — Cambio de alcance**

El proceso formal de control de cambios permitió procesar la solicitud sin desordenar el proyecto. La clave fue no responder de inmediato con un "sí" o un "no", sino canalizar la solicitud por el CCB y sustentar la decisión en un análisis de impacto. Lección: mantener un proceso de cambios explícito y conocido por todos los stakeholders evita negociaciones informales que erosionan la línea base.
