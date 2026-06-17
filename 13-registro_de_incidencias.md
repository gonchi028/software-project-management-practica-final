# Registro de Incidencias

---

El registro de incidencias documenta los problemas operativos, defectos y eventos que afectan el día a día del proyecto y que no son riesgos formales. Cada incidencia tiene un responsable y un plazo de resolución.

## Clasificación de Incidencias

| Severidad | Definición                                          | SLA de resolución |
| --------- | --------------------------------------------------- | ----------------- |
| Crítica   | Bloquea el avance de un módulo o impide una entrega | 24 h              |
| Alta      | Afecta funcionalidad importante sin bloquear        | 3 días            |
| Media     | Funciona con limitaciones; workaround posible       | 1 semana          |
| Baja      | Cosmético o de menor impacto                        | Próximo sprint    |

## Incidencias Registradas (extracto, hasta semana 10)

| ID     | Fecha | Descripción                                                 | Severidad | Estado          |
| ------ | ----- | ----------------------------------------------------------- | --------- | --------------- |
| INC-01 | S3    | Entorno de CI sin permisos para desplegar a preproducción   | Alta      | Resuelta        |
| INC-02 | S4    | Datos maestros de comerciantes con duplicados               | Media     | Resuelta        |
| INC-03 | S6    | Demora del PO en validar la pantalla de cobro               | Media     | Resuelta        |
| INC-04 | S8    | Defecto crítico: el comprobante pierde numeración al anular | Crítica   | Abierta         |
| INC-05 | S9    | Servidor de la Alcaldía con caída de 3 h                    | Alta      | Resuelta        |
| INC-06 | S10   | Renuncia de desarrollador backend senior                    | Alta      | En seguimiento  |
| INC-07 | S10   | Renuncia de desarrollador frontend (único)                  | Alta      | En seguimiento  |
| INC-08 | S10   | Solicitud de cambio de alcance (geolocalización)            | Media     | En análisis CCB |

## Gestión de Incidencias

Las incidencias se registran en Jira con su responsable asignado. Las críticas y altas se revisan en el Daily Scrum; las medias y bajas, en la reunión semanal. Toda incidencia crítica genera una acción correctiva inmediata y, si corresponde, una entrada en el registro de riesgos o una solicitud de cambio.
