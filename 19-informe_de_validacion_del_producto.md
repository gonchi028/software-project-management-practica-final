# Informe de Validación del Producto

El informe de validación del producto documenta la verificación formal por parte del cliente de que el MVP cumple con los criterios de aceptación acordados. Es la base del acta de aceptación firmada.

## Alcance de la Validación

La validación se realizó entre las semanas 24 y 25 mediante pruebas de aceptación del usuario (UAT) con administradores de los tres mercados, el cajero, el inspector sanitario y un representante de la Dirección de Ingresos. Se ejecutaron 86 casos de prueba que cubren el 100 % de los requerimientos del MVP.

## Resultados de las Pruebas de Aceptación

| Módulo                             | Casos ejecutados | Aprobados | Defectos | % aprobación |
| ---------------------------------- | ---------------- | --------- | -------- | ------------ |
| Registro de puestos y comerciantes | 18               | 17        | 1 medio  | 94 %         |
| Cobros de tarifas                  | 16               | 15        | 1 medio  | 94 %         |
| Licencias sanitarias               | 15               | 15        | 0        | 100 %        |
| Informes y panel                   | 12               | 11        | 1 bajo   | 92 %         |
| Seguridad y roles                  | 13               | 13        | 0        | 100 %        |
| Integración y rendimiento          | 12               | 11        | 1 bajo   | 92 %         |
| TOTAL                              | 86               | 82        | 4        | 95 %         |

## Validación de Requerimientos No Funcionales

| Atributo                     | Objetivo    | Medición              | Cumple |
| ---------------------------- | ----------- | --------------------- | ------ |
| Rendimiento p95              | ≤ 2 s       | 1,4 s                 | Sí     |
| Disponibilidad (sem. de UAT) | ≥ 99,5 %    | 99,8 %                | Sí     |
| Cobertura de pruebas         | ≥ 80 %      | 82 %                  | Sí     |
| Clics por tarea frecuente    | ≤ 3         | ≤ 3                   | Sí     |
| Cumplimiento normativo       | Obligatorio | Validado por jurídica | Sí     |

## Defectos Pendientes y su Gestión

Al cierre de la validación quedaron 4 defectos no críticos: 2 medios (una validación de pantalla y un borde en el reporte) y 2 bajos (cosméticos). Ninguno impide la operación del sistema. Se acordó su corrección durante los primeros 30 días de operación dentro del soporte acordado.

## Veredicto de Validación

Con base en los resultados, el producto cumple los criterios de aceptación del MVP. El cliente valida formalmente el producto mediante acta firmada el 02/07/2026, con la condición de resolver los defectos no críticos en el período de soporte inicial.
