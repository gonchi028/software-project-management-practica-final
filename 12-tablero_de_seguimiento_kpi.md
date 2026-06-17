# Tablero de Seguimiento KPI

---

El tablero de seguimiento consolida los indicadores clave de desempeño del proyecto en sus cuatro dimensiones: alcance, tiempo, costo y calidad. Se actualiza semanalmente y se revisa en el informe de estado con la Dirección de Ingresos. El método de referencia es el Análisis del Valor Ganado (EVA, Earned Value Analysis).

## Indicadores de Desempeño

| KPI                        | Definición                         | Objetivo              | Valor sem. 10 | Estado |
| -------------------------- | ---------------------------------- | --------------------- | ------------- | ------ |
| SPI                        | Schedule Performance Index = EV/PV | ≥ 0,95                | 0,89          | Ámbar  |
| CPI                        | Cost Performance Index = EV/AC     | ≥ 0,95                | 1,02          | Verde  |
| % avance real              | EV / BAC                           | Acumulado planificado | 34 %          | Ámbar  |
| Velocidad de sprint        | Story points cerrados por sprint   | 28 SP                 | 22 SP         | Ámbar  |
| Tasa de aceptación         | Historias aceptadas / entregadas   | ≥ 90 %                | 92 %          | Verde  |
| Defectos críticos abiertos | Defectos de severidad alta/crítica | 0                     | 1             | Rojo   |
| Cobertura de pruebas       | Cobertura de código automatizada   | ≥ 80 %                | 76 %          | Ámbar  |
| Satisfacción del PO        | Encuesta rápida semanal (1–5)      | ≥ 4                   | 3,8           | Ámbar  |

## Análisis del Valor Ganado (semana 10)

Considerando el BAC (Budget at Completion) de 70.000 Bs y un avance planificado del 38 % a la semana 10:

| Variable | Valor                         | Cálculo / Interpretación                          |
| -------- | ----------------------------- | ------------------------------------------------- |
| PV       | (Planned Value) 26.600 Bs     | 70.000 × 0,38                                     |
| EV       | (Earned Value) 23.800 Bs      | 70.000 × 0,34                                     |
| AC       | (Actual Cost) 23.300 Bs       | Gasto real acumulado                              |
| SV       | (Schedule Variance) -2.800 Bs | EV − PV (atraso)                                  |
| CV       | (Cost Variance) +500 Bs       | EV − AC (ligero ahorro)                           |
| SPI      | 0,89                          | EV / PV (atrasado)                                |
| CPI      | 1,02                          | EV / AC (en costo)                                |
| EAC      | 68.627 Bs                     | BAC / CPI (estimado al cierre)                    |
| VAC      | +1.373 Bs                     | BAC − EAC (ahorro proyectado al cierre)           |

La proyección EAC se sitúa por debajo del BAC, lo que indica que de mantenerse la tendencia de costo el proyecto cerraría con un ligero ahorro. Sin embargo, el indicador crítico es el SPI: el atraso se relaciona con la pérdida temporal de personal, cuya mitigación está en curso. Si las acciones de recuperación funcionan, el SPI debería volver a la zona verde en 3–4 semanas; en caso contrario, el atraso podría presionar al alza el costo por la necesidad de horas extraordinarias, deteriorando el CPI actual.

## Semáforo de Salud del Proyecto

| Dimensión | Estado | Comentario                                                 |
| --------- | ------ | ---------------------------------------------------------- |
| Alcance   | Verde  | Alcance Must protegido; Should en revisión                 |
| Tiempo    | Ámbar  | Desviación del 4 %; plan de recuperación en marcha         |
| Costo     | Verde  | CPI > 1; reserva intacta                                   |
| Calidad   | Ámbar  | 1 defecto crítico abierto; cobertura por debajo del umbral |
| Riesgos   | Ámbar  | Dos riesgos materializados; mitigación activa              |
| Recursos  | Rojo   | Equipo con 2 bajas; reemplazo en proceso                   |
