# Value Stream Mapping (VSM)

---

El Value Stream Mapping mapea el flujo de valor end-to-end del proceso de cobro de tarifas, identificando los tiempos de valor agregado (VA), los tiempos de no valor agregado (NVA) y los tiempos de espera, con el fin de visualizar desperdicios y oportunidades de mejora. Se construyó en una sesión con el equipo y el personal operativo.

## Estado Actual (AS-IS) — Proceso Manual

| #   | Actividad                                     | Tipo   | Tiempo (h) |
| --- | --------------------------------------------- | ------ | ---------- |
| 1   | Recorrer puestos para registrar pagos en hoja | VA     | 16         |
| 2   | Trasladar planillas a la oficina central      | NVA    | 4          |
| 3   | Esperar consolidación de planillas            | Espera | 24         |
| 4   | Digitar datos en hoja de cálculo              | NVA    | 12         |
| 5   | Validar y corregir inconsistencias            | NVA    | 8          |
| 6   | Generar informe mensual manualmente           | NVA    | 6          |
| 7   | Esperar revisión del director                 | Espera | 48         |
| 8   | Aprobar y archivar el informe                 | VA     | 2          |

Tiempo total de ciclo AS-IS: 120 horas. Tiempo de valor agregado: 18 horas (15 %). Tiempo de espera y desperdicio: 102 horas (85 %). El ratio de eficiencia del proceso es muy bajo.

## Estado Futuro (TO-BE) — Proceso Digitalizado con SGMM

| #   | Actividad                                     | Tipo        | Tiempo (h) |
| --- | --------------------------------------------- | ----------- | ---------- |
| 1   | Registrar cobro en el sistema con comprobante | VA          | 2          |
| 2   | El sistema consolida automáticamente          | VA (autom.) | 0,1        |
| 3   | Sistema valida y emite alertas de deuda       | VA (autom.) | 0,1        |
| 4   | Generar informe mensual con un clic           | VA          | 0,2        |
| 5   | Revisión del director en panel                | VA          | 1          |
| 6   | Aprobar y archivar digitalmente               | VA          | 0,2        |

Tiempo total de ciclo TO-BE: 3,6 horas. Tiempo de valor agregado: 3,6 horas (100 % del tiempo activo). Reducción del tiempo de ciclo: 97 %. Eliminación completa de los tiempos de espera y de las actividades de no valor agregado manuales.

# Desperdicios Identificados y Eliminados

| Desperdicio (muda)        | Evidencia AS-IS                  | Solución TO-BE                 |
| ------------------------- | -------------------------------- | ------------------------------ |
| Sobreproducción           | Planillas duplicadas             | Registro único en sistema      |
| Espera                    | 48 h esperando revisión          | Acceso en tiempo real al panel |
| Transporte                | Traslado físico de planillas     | Operación digital              |
| Procesamiento innecesario | Digitación y redigitación        | Captura única en origen        |
| Inventario                | Planillas sin procesar           | Sin inventario de papel        |
| Movimiento                | Búsqueda de planillas archivadas | Búsqueda en el sistema         |
| Defectos                  | Errores de transcripción         | Validaciones automáticas       |

## Conclusión del VSM

La digitalización transforma un proceso con un 15 % de eficiencia en uno con un 100 % de actividades de valor agregado, reduciendo el tiempo de ciclo de 120 a 3,6 horas. Esto se traduce en el incremento de la recaudación, la reducción de evasión y la disponibilidad de información en tiempo real, alineado con los beneficios esperados del proyecto.
