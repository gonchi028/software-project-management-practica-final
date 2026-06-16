# Documento de Inception

---

La fase de Inception busca alinear la visión del producto, validar la viabilidad técnica y de negocio, y producir el Product Backlog inicial priorizado. Tuvo una duración de dos semanas (semanas 3 y 4 del proyecto) y contó con la participación conjunta del equipo de desarrollo y del personal operativo de la Alcaldía.

## Visión del Producto

"En 2026, la Alcaldía de Sucre contará con un sistema web único que administre en tiempo real los mercados municipales Campesino, Central y Entre Ríos, incrementando la recaudación, garantizando el cumplimiento sanitario y entregando información confiable para la gestión pública."

## Objetivos de la Inception

- Validar la comprensión compartida del problema con los usuarios operativos.
- Identificar y priorizar el backlog inicial mediante historias de usuario.
- Definir la arquitectura técnica de referencia y validar su viabilidad.
- Acordar el plan de entregas por sprints y los criterios de aceptación.
- Identificar los principales riesgos y supuestos del producto.

## Sesiones Realizadas

| Sesión | Técnica                  | Participantes                         | Producto                          |
| ------ | ------------------------ | ------------------------------------- | --------------------------------- |
| S1     | Mapeo de procesos AS-IS  | Administradores de mercado + analista | Diagrama de proceso actual        |
| S2     | Mapeo de procesos TO-BE  | Mismo grupo + arquitecto              | Diagrama del proceso digitalizado |
| S3     | User Story Mapping       | Equipo completo + Product Owner       | Backlog inicial priorizado        |
| S4     | Workshop de arquitectura | Arquitecto + líderes técnicos         | Documento de arquitectura         |
| S5     | Definición de MVP        | Product Owner + jefe de proyecto      | Alcance MVP y plan de sprints     |

## Arquitectura Técnica de Referencia

El sistema se implementa como una aplicación web de tres capas. La capa de presentación usa React con TypeScript. La capa de servicios es una API REST construida en Node.js con Express, y la capa de datos usa PostgreSQL. El despliegue se realiza sobre los servidores on-premise de la Alcaldía, en contenedores Docker. Se adopta autenticación con JWT y control de acceso basado en roles.

## Alcance del MVP (definido en Inception)

- Registro de puestos y comerciantes con carnet QR (RF-01 a RF-05).
- Cobro de tarifas con comprobante correlativo y conciliación (RF-06 a RF-10).
- Licencias sanitarias con alertas de vencimiento (RF-11 a RF-15).
- Panel de indicadores e informe mensual exportable (RF-16 a RF-18).
- Gestión de usuarios y roles con bitácora de auditoría (RF-19 a RF-21).

**Quedan fuera del MVP:** aplicación móvil, geolocalización de puestos (posteriormente solicitada vía control de cambios), integración con pasarela de pago y migración histórica.

## Riesgos y Supuestos Detectados en Inception

| Riesgo/Supuesto                                       | Impacto | Estrategia                                 |
| ----------------------------------------------------- | ------- | ------------------------------------------ |
| Cambios en la normativa sanitaria durante el proyecto | Medio   | Diseño flexible del módulo de licencias    |
| Rotación de personal técnico clave                    | Alto    | Documentación, pairing y plan de reemplazo |
| Calidad insuficiente de datos maestros actuales       | Medio   | Proceso de depuración previo a migración   |
| Supuesto: disponibilidad de servidores de la Alcaldía | —       | Validado con la unidad de TI               |

## Criterios para dar por terminada la Inception

- Backlog inicial priorizado y aceptado por el Product Owner.
- Arquitectura técnica documentada y validada.
- Plan de sprints con el alcance del MVP.
- Registro de riesgos inicial cargado.
