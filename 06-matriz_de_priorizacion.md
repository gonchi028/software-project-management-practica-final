# Matriz de Priorización

---

Para priorizar las historias de usuario y los módulos del backlog se aplicó el método MoSCoW complementado con una matriz de Valor vs. Esfuerzo. La priorización se realizó con el Product Owner en la sesión S3 de la Inception y se reajustó tras el control de cambios de la semana 10.

## Priorización MoSCoW

| Categoría              | Funcionalidades                                                                      | Justificación                                                     |
| ---------------------- | ------------------------------------------------------------------------------------ | ----------------------------------------------------------------- |
| Must (debe tener)      | RF-01 a RF-03, RF-06, RF-07, RF-11, RF-13, RF-16, RF-19, RF-20                       | Núcleo del sistema; sin ellas no hay MVP                          |
| Should (debería tener) | RF-04, RF-08, RF-09, RF-12, RF-14, RF-17, RF-18, RF-21                               | Alto valor, pero el MVP puede operar sin ellas en primera versión |
| Could (podría tener)   | RF-05 (carnet QR), RF-10 (conciliación diaria), RF-15 (categoría sanitaria)          | Mejoras deseables si el cronograma lo permite                     |
| Won't (no en este MVP) | App móvil, pasarela de pago, geolocalización (posteriormente replanteada por cambio) | Fuera de alcance inicial                                          |

## Matriz Valor vs. Esfuerzo

Cada historia se ubicó en un cuadrante según su valor de negocio y el esfuerzo estimado, expresado en puntos de historia (story points) sobre la escala de Fibonacci.

| Cuadrante                  | Característica                                                | Decisión                                  |
| -------------------------- | ------------------------------------------------------------- | ----------------------------------------- |
| Alto valor / Bajo esfuerzo | Quick wins. Ej.: RF-13 (alerta de vencimiento), RF-20 (login) | Priorizar primero                         |
| Alto valor / Alto esfuerzo | Pilares del producto. Ej.: RF-06 (cobro), RF-11 (licencias)   | Planificar con cuidado, sprints tempranos |
| Bajo valor / Bajo esfuerzo | Rellenos. Ej.: RF-05 (carnet QR)                              | Si sobra capacidad                        |
| Bajo valor / Alto esfuerzo | Evitar. Ej.: integración con pasarela de pago                 | Excluir del MVP                           |
