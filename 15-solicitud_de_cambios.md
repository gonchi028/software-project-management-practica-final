# Solicitud de Cambios — Módulo de Geolocalización

---

A las 10 semanas de iniciado el proyecto, la Alcaldía solicitó formalmente agregar un módulo de geolocalización de puestos que no estaba en el alcance original. Esta sección describe el proceso formal de gestión del cambio, los documentos generados y los roles involucrados, conforme al plan de gestión del cambio del proyecto.

## Proceso Formal de Gestión del Cambio

El proceso de control de cambios del SGMM sigue el flujo estándar del PMBOK con adaptaciones ágiles. Está diseñado para asegurar que todo cambio se evalúe de forma objetiva antes de aprobarse, protegiendo la línea base del proyecto.

| #   | Etapa                                                           | Responsable                             | Documento generado                      |
| --- | --------------------------------------------------------------- | --------------------------------------- | --------------------------------------- |
| 1   | Identificación y registro de la solicitud                       | Cualquier interesado → JP               | Formulario de Solicitud de Cambio (FSC) |
| 2   | Evaluación de impacto (alcance, tiempo, costo, riesgo, calidad) | JP + arquitecto + PO                    | Análisis de Impacto del Cambio          |
| 3   | Revisión y recomendación                                        | Comité de Control de Cambios (CCB)      | Acta de reunión del CCB                 |
| 4   | Decisión (aprobar / rechazar / diferir)                         | CCB con aprobación del sponsor si > 5 % | Resolución del cambio                   |
| 5   | Actualización de las líneas base y comunicación                 | JP                                      | Plan de proyecto actualizado            |
| 6   | Ejecución y verificación del cambio                             | Equipo de desarrollo + QA               | Historia de usuario en el backlog       |
| 7   | Cierre formal del cambio                                        | JP                                      | Registro de cambios actualizado         |

## Roles Involucrados en el Control de Cambios

| Rol                                | Composición                                                                           | Responsabilidad                                |
| ---------------------------------- | ------------------------------------------------------------------------------------- | ---------------------------------------------- |
| Solicitante                        | Dirección de Ingresos (en este caso)                                                  | Presenta la necesidad y su justificación       |
| Jefe de proyecto                   | JP del SGMM                                                                           | Registra, evalúa impacto y recomienda          |
| Comité de Control de Cambios (CCB) | Director de Ingresos (sponsor), JP, Product Owner, Arquitecto, representante jurídico | Analiza y aprueba/rechaza cambios              |
| Product Owner                      | Analista funcional de la Alcaldía                                                     | Re-prioriza el backlog si el cambio se aprueba |
| Equipo de desarrollo               | Backend, frontend, QA                                                                 | Estima esfuerzo y ejecuta el cambio            |
| Unidad jurídica                    | Asesor legal de la Alcaldía                                                           | Valida implicaciones normativas                |

## Formulario de Solicitud de Cambio (FSC-001)

| Campo                | Contenido                                                                                                                                                              |
| -------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ID del cambio        | FSC-001                                                                                                                                                                |
| Fecha de solicitud   | 11/03/2026 (semana 10)                                                                                                                                                 |
| Solicitante          | Dirección de Ingresos — Alcaldía de Sucre                                                                                                                              |
| Título               | Módulo de geolocalización de puestos de mercado                                                                                                                        |
| Descripción          | Capturar y mostrar en un mapa la ubicación geográfica (latitud/longitud) de cada puesto, asociada al registro del puesto, con visualización por mercado y sector.      |
| Justificación        | Permitir a la administración y a la fiscalización ubicar físicamente cada puesto, planificar inspecciones y verificar la correspondencia entre el padrón y el terreno. |
| Origen               | Requerimiento derivado de una inspección de la Dirección de Ingresos en el mercado Central                                                                             |
| Prioridad percibida  | Alta para el cliente                                                                                                                                                   |
| Documentos afectados | ERS (nuevas historias), Cronograma, Presupuesto, Plan de pruebas, Registro de riesgos                                                                                  |

## Análisis de Impacto del Cambio

| Dimensión    | Impacto estimado                      | Detalle                                                                       |
| ------------ | ------------------------------------- | ----------------------------------------------------------------------------- |
| Alcance      | Medio                                 | +4 historias de usuario nuevas; +1 módulo                                     |
| Tiempo       | +2 sprints de capacidad (3–4 semanas) | Reasignando alcance Should de menor prioridad                                 |
| Costo        | +4.500 Bs (6,4 %)                     | Cubierto por la reserva de gestión                                            |
| Calidad      | Bajo                                  | Nuevas pruebas de integración con mapas                                       |
| Riesgo       | Bajo-Medio                            | Nuevo riesgo R-09: precisión del GPS y calidad de los datos de ubicación      |
| Recursos     | Medio                                 | Requiere 1 desarrollador adicional con conocimiento de mapas (Leaflet/Mapbox) |
| Stakeholders | Bajo                                  | Beneficio percibido alto por la administración                                |

## Alternativas Evaluadas

- Alternativa A — Aprobar e incluir en el MVP: incrementa valor, pero exige absorber costo y reasignar alcance Should. Riesgo de presión sobre el cronograma.
- Alternativa B — Aprobar y entregar como incremento posterior al MVP: preserva el MVP original, entrega la funcionalidad 4 semanas después del cierre. Recomendada por el JP.
- Alternativa C — Rechazar: no satisface una necesidad explícita del cliente y genera insatisfacción.
- Alternativa D — Versión simplificada (solo registro de coordenadas, sin mapa): entrega valor mínimo sin mapa interactivo, posterga el mapa para una siguiente versión.

## Decisión del CCB

El Comité de Control de Cambios se reunió el 18/03/2026. Considerando que el proyecto tiene riesgos activos materializados (renuncias) y que la solicitud aporta valor claro pero no es bloqueante para el MVP, el CCB resolvió:

**RESOLUCIÓN:** Aprobar la solicitud bajo la Alternativa B. El módulo de geolocalización se entrega como incremento posterior al MVP, financiado con 4.500 Bs de la reserva de gestión, con un alcance limitado a: captura de coordenadas en el registro del puesto, visualización en mapa por mercado y exportación de ubicaciones. Se actualizan las líneas base de alcance, cronograma y presupuesto; se incorpora el riesgo R-09 al [registro actualizado](16-registro_de_riesgos_actualizado.md).

## Documentos Generados en el Proceso

- Formulario de Solicitud de Cambio (FSC-001).
- Análisis de Impacto del Cambio (alcance, tiempo, costo, calidad, riesgo).
- Acta de la reunión del CCB del 18/03/2026.
- Resolución formal del cambio y comunicación al equipo.
- Actualización del ERS, cronograma, presupuesto y registro de riesgos.
- Historias de usuario (RF-22 a RF-25) incorporadas al backlog priorizado.
