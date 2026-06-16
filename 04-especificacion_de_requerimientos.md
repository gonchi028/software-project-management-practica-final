# Especificación de Requerimientos

---

La Especificación de Requerimientos de Software (ERS) describe las funcionalidades y restricciones del SGMM. Combina requerimientos funcionales (en formato de historias de usuario) y no funcionales (en formato de atributos de calidad), siguiendo el estándar IEEE 830 como marco de referencia.

## Requerimientos Funcionales por Módulo

**Módulo 1 — Registro de Puestos y Comerciantes**

| ID    | Historia de usuario                                                                                                                                     | Prioridad |
| ----- | ------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
| RF-01 | Como administrador, quiero registrar un nuevo comerciante con sus datos personales, foto y referencia catastral, para mantener un padrón actualizado.   | Alta      |
| RF-02 | Como administrador, quiero asignar un puesto físico a un comerciante, asociando mercado, sector, número y dimensión, para controlar el uso del espacio. | Alta      |
| RF-03 | Como administrador, quiero consultar y modificar los datos de un puesto o comerciante, para mantener la información correcta.                           | Alta      |
| RF-04 | Como administrador, quiero dar de baja temporal o definitiva un puesto, para reflejar la situación real del mercado.                                    | Media     |
| RF-05 | Como administrador, quiero generar un carnet impreso con el código QR del comerciante, para identificarlo físicamente.                                  | Media     |

**Módulo 2 — Cobros de Tarifas**

| ID    | Historia de usuario                                                                                                                                      | Prioridad |
| ----- | -------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
| RF-06 | Como cajero, quiero registrar el cobro mensual de la tarifa de un puesto, emitiendo comprobante con número correlativo, para garantizar la trazabilidad. | Alta      |
| RF-07 | Como administrador, quiero configurar el monto de tarifas por tipo de puesto y mercado, para reflejar la normativa vigente.                              | Alta      |
| RF-08 | Como administrador, quiero ver la deuda pendiente de cada comerciante, para gestionar la cobranza.                                                       | Alta      |
| RF-09 | Como cajero, quiero emitir notas de crédito y anular comprobantes con autorización, para corregir errores.                                               | Media     |
| RF-10 | Como administrador, quiero conciliar el total cobrado con el total depositado, para el cierre del día.                                                   | Media     |

**Módulo 3 — Licencias Sanitarias**

| ID    | Historia de usuario                                                                                                                                 | Prioridad |
| ----- | --------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
| RF-11 | Como inspector sanitario, quiero registrar la licencia sanitaria de un comerciante con fecha de emisión y vigencia, para controlar el cumplimiento. | Alta      |
| RF-12 | Como inspector, quiero registrar inspecciones y observaciones a un puesto, para el seguimiento sanitario.                                           | Alta      |
| RF-13 | Como comerciante, quiero recibir una alerta 15 días antes del vencimiento de mi licencia, para renovarla a tiempo.                                  | Alta      |
| RF-14 | Como administrador, quiero generar el reporte de puestos con licencia vencida o sin licencia, para las acciones de fiscalización.                   | Alta      |
| RF-15 | Como inspector, quiero registrar la categoría sanitaria del establecimiento según la normativa vigente, para clasificarlo correctamente.            | Media     |

**Módulo 4 — Informes Mensuales y Panel**

| ID    | Historia de usuario                                                                                                                               | Prioridad |
| ----- | ------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
| RF-16 | Como Director de Ingresos, quiero obtener el informe mensual de recaudación por mercado y por tipo de tarifa, para la rendición de cuentas.       | Alta      |
| RF-17 | Como Director, quiero ver un panel con indicadores de recaudación, cumplimiento sanitario y morosidad en tiempo real, para la toma de decisiones. | Alta      |
| RF-18 | Como administrador, quiero exportar los informes en formato PDF y Excel, para su uso institucional.                                               | Media     |

**Módulo 5 — Seguridad y Administración**

| ID    | Historia de usuario                                                                                                                                             | Prioridad |
| ----- | --------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
| RF-19 | Como administrador del sistema, quiero gestionar usuarios y asignar roles (administrador, cajero, inspector, director, solo lectura), para controlar el acceso. | Alta      |
| RF-20 | Como usuario, quiero autenticarme con usuario y contraseña, para acceder de forma segura.                                                                       | Alta      |
| RF-21 | Como auditor, quiero consultar el registro de acciones de cada usuario (bitácora), para la trazabilidad.                                                        | Alta      |

## Requerimientos No Funcionales

| Categoría      | Requerimiento                                                                                                                                        | Métrica/objetivo    |
| -------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------- |
| Rendimiento    | El sistema debe responder a cualquier transacción del usuario en menos de 2 segundos con la carga esperada de 200 usuarios concurrentes.             | ≤ 2 s p95           |
| Disponibilidad | El sistema debe estar disponible durante el horario administrativo (07:00–20:00) con un máximo de 1 hora de indisponibilidad mensual no planificada. | ≥ 99,5 %            |
| Seguridad      | Las contraseñas deben almacenarse con hash bcrypt y los datos sensibles cifrados en reposo. Acceso por roles.                                        | Cumplimiento        |
| Usabilidad     | La interfaz debe ser usable por personas con formación básica, con un máximo de 3 clics para las tareas frecuentes.                                  | Tarea ≤ 3 clics     |
| Mantenibilidad | Cobertura de pruebas unitarias ≥ 80 % y análisis estático sin vulnerabilidades críticas.                                                             | ≥ 80 %              |
| Compatibilidad | Operación en los navegadores Chrome y Edge en sus versiones recientes.                                                                               | Últimas 2 versiones |
| Cumplimiento   | Ajuste a la Ley de Gobierno Electrónico, Ley de Protección de Datos y normativa municipal vigente.                                                   | Obligatorio         |

## Requisitos de Interfaz Externa

El sistema es una aplicación web responsiva operada desde los puntos de atención de cada mercado y desde las oficinas centrales de la Dirección de Ingresos. No se prevén integraciones externas en el MVP; en una fase posterior podría integrarse con la pasarela de pago y con el sistema de catastro municipal.

## Matriz de Trazabilidad

Cada requerimiento se traza hacia los objetivos del negocio y hacia los casos de prueba que lo verifican. La matriz completa se mantiene en Confluence.

| Requerimiento    | Objertivo de negocio                   | Caso de prueba                           |
| ---------------- | -------------------------------------- | ---------------------------------------- |
| RF-06 (cobro)    | Incrementar recaudación y trazabilidad | CT-06: registro de cobro con comprobante |
| RF-11 (licencia) | Cumplimiento sanitario normativo       | CT-11: registro de licencia y alerta     |
| RF-16 (informe)  | Información oportuna para decisiones   | CT-16: generación de informe mensual     |
| RF-19 (roles)    | Seguridad y control de acceso          | CT-19: permisos por rol                  |
