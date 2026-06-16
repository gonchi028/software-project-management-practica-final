# Registro de Riesgos (versión inicial)

---

El registro de riesgos inicial se elaboró durante la Inception y se mantiene actualizado a lo largo del proyecto. Cada riesgo se evalúa en probabilidad e impacto (Bajo, Medio, Alto), se le asigna un responsable y se definen acciones de prevención y de contingencia.

## Escala de Valoración

| Nivel | Probabilidad | Impacto                              | Severidad (P×I) |
| ----- | ------------ | ------------------------------------ | --------------- |
| Bajo  | ≤ 25 %       | Mínimo efecto en alcance/costo/plazo | 1–4             |
| Medio | 26–60 %      | Efecto moderado, recuperable         | 5–9             |
| Alto  | > 60 %       | Efecto severo en objetivos           | 10–16           |

## Matriz de Probabilidad vs. Impacto

La severidad se obtiene del producto de la probabilidad por el impacto, ambos en escala 1–4. Los riesgos con severidad ≥ 9 se consideran prioritarios.

## Riesgos Iniciales

| ID   | Riesgo                                                            | P     | I     | Sev. | Estrategia                                                 | Responsable |
| ---- | ----------------------------------------------------------------- | ----- | ----- | ---- | ---------------------------------------------------------- | ----------- |
| R-01 | Cambios normativos sobre licencias sanitarias durante el proyecto | Media | Alto  | 8    | Mitigar: diseño flexible del módulo de licencias           | P           |
| R-02 | Renuncia de personal técnico clave                                | Media | Alto  | 8    | Mitigar: documentación, plan de reemplazo, pairing         | JP          |
| R-03 | Datos maestros de puestos incompletos o erróneos                  | Alta  | Medio | 6    | Mitigar: depuración previa y validación con administración | PO          |
| R-04 | Indisponibilidad de servidores de la Alcaldía                     | Baja  | Alto  | 4    | Aceptar: entorno de respaldo y plan de despliegue          | Arq.        |
| R-05 | Resistencia al cambio del personal operativo                      | Media | Medio | 4    | Mitigar: capacitación temprana y participación             | JP          |
| R-06 | Cambios de alcance por nuevas solicitudes del cliente             | Media | Medio | 4    | Mitigar: proceso formal de control de cambios              | JP          |
| R-07 | Retraso en decisiones del Product Owner                           | Media | Medio | 4    | Mitigar: reuniones semanales y SLA de respuesta            | PO          |
| R-08 | Vulnerabilidades de seguridad detectadas tardíamente              | Baja  | Alto  | 4    | Mitigar: análisis estático continuo y pentest              | Arq.        |

## Top Riesgos y Plan de Acción

**R-01 — Cambios normativos sobre licencias sanitarias**

Severidad 8. Se mitiga con un diseño paramétrico del módulo de licencias (categorías, plazos y reglas configurables), de modo que un cambio normativo no implique reescritura del código. Plan de contingencia: reservar 80 horas dentro de la reserva de gestión para adaptaciones.

**R-02 — Renuncia de personal técnico clave**

Severidad 8. Se mitiga con documentación técnica obligatoria por módulo, pair programming en tareas críticas y un plan de reemplazo preacordado con el área de recursos humanos. Plan de contingencia: activar reemplazo en menos de una semana y redistribuir temporalmente tareas. Este riesgo se materializó en la semana 10 (ver sección 16, registro actualizado).
