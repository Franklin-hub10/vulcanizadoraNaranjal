# Matriz canónica de tarifas por franja horaria

## Propósito

Resolver qué tarifa corresponde aplicar según la franja horaria de atención de Vulcanizadora Naranjal.

El negocio opera 24/7 y las tarifas pueden cambiar según la franja. Esta matriz es la fuente canónica para seleccionar el valor aplicable antes de valorar una orden de trabajo, elaborar una cotización o responder una consulta de precios.

## Franjas definidas

| Franja | Estado | Hora inicio | Hora fin | Observación |
|---|---|---|---|---|
| Día | Confirmada como categoría | Pendiente | Pendiente | Todos los valores levantados hasta el 2026-09-20 corresponden a esta franja. |
| Noche | Confirmada como categoría | Pendiente | Pendiente | Tarifas y límites horarios pendientes de definición por Joel. |

> Los horarios 08:30–17:30 mencionados como ejemplo **no están confirmados** y no se registran como límites oficiales.

## Método de resolución de tarifa

Para seleccionar una tarifa:

1. identificar la fecha y hora aplicable al servicio;
2. si Joel indicó explícitamente la franja (`día` o `noche`), usar esa franja;
3. cuando existan límites horarios confirmados, clasificar automáticamente la hora en la franja correspondiente;
4. consultar esta matriz y aplicar únicamente una tarifa cuyo estado esté confirmado;
5. si la franja puede identificarse pero su tarifa está pendiente, no inventar el precio: preguntar a Joel;
6. si los límites horarios aún no permiten clasificar la hora y Joel no indicó la franja, preguntar antes de valorar.

### Hora que gobierna

- Para una orden ya ejecutada: usar la hora de ejecución del trabajo cuando esté confirmada.
- Para una orden futura: usar la hora prevista del servicio si fue informada.
- Para una consulta de precio inmediato del tipo "¿cuánto cuesta ahora?": cuando los rangos estén definidos, usar la hora local de Ecuador (`America/Guayaquil`).
- La hora en que se hace la consulta no reemplaza la hora real del servicio cuando ambas son diferentes.

## Tarifas vigentes

| Tipo | Servicio / insumo | Unidad de cobro | Día | Estado día | Noche | Estado noche | Fuente operativa |
|---|---|---|---:|---|---:|---|---|
| Parche | 110 | unidad / instalación incluida | $10.00 | confirmado | — | pendiente | `operacion/insumos/PARCHES.md` |
| Parche | 112 | unidad / instalación incluida | $10.00 | confirmado | — | pendiente | `operacion/insumos/PARCHES.md` |
| Parche | 120 | unidad / instalación incluida | $18.00 | confirmado | — | pendiente | `operacion/insumos/PARCHES.md` |
| Parche | 135 | unidad / instalación incluida | $25.00 | confirmado | — | pendiente | `operacion/insumos/PARCHES.md` |
| Parche | 142 | unidad / instalación incluida | $30.00 | confirmado | — | pendiente | `operacion/insumos/PARCHES.md` |
| Parche estrellado | 02 | unidad / instalación incluida | $10.00 | confirmado | — | pendiente | `operacion/insumos/PARCHES.md` |
| Parche estrellado | 05 | unidad / instalación incluida | $18.00 | confirmado | — | pendiente | `operacion/insumos/PARCHES.md` |
| Parche pequeño | 01 | unidad / instalación incluida | $3.00 | confirmado | — | pendiente | `operacion/insumos/PARCHES.md` |
| Servicio carro pequeño | Armar y desarmar la llanta | unidad pendiente de precisar | $2.00 | confirmado | — | pendiente | `operacion/servicios/CAMBIO_LLANTAS_CARRO_PEQUENO.md` |
| Servicio carro pequeño | Cambio de posición de llanta | por llanta | $1.00 | confirmado | — | pendiente | `operacion/servicios/CAMBIO_LLANTAS_CARRO_PEQUENO.md` |
| Servicio carro pequeño | Desarmar llantas fuera del vehículo | unidad pendiente de precisar | $1.00 | confirmado | — | pendiente | `operacion/servicios/CAMBIO_LLANTAS_CARRO_PEQUENO.md` |
| Servicio carro pequeño | Armar y desarmar para virarla en el mismo aro | unidad pendiente de precisar | $2.00 | confirmado | — | pendiente | `operacion/servicios/CAMBIO_LLANTAS_CARRO_PEQUENO.md` |
| Servicio carro pequeño | Cambio de llanta por la llanta de emergencia | unidad pendiente de precisar | $2.00 | confirmado | — | pendiente | `operacion/servicios/CAMBIO_LLANTAS_CARRO_PEQUENO.md` |
| Servicio carro pequeño | Cambio por llantas nuevas | por aro | $2.00 | confirmado | — | pendiente | `operacion/servicios/CAMBIO_LLANTAS_CARRO_PEQUENO.md` |

## Regla especial de cambio de posición

La tarifa diurna es $1.00 por llanta. Cuando la operación implica intercambiar dos posiciones, se contabilizan dos llantas y el total diurno de ese movimiento es $2.00.

## Pendientes obligatorios

Joel debe definir posteriormente:

- hora de inicio y fin de la franja Día;
- hora de inicio y fin de la franja Noche;
- tarifas nocturnas por cada servicio e insumo;
- cualquier excepción por día de semana, feriado u otra condición, solo si realmente existe;
- cualquier unidad de cobro que aún figure pendiente.

## Regla de actualización

Cuando Joel confirme límites horarios o nuevas tarifas, se actualiza esta matriz conservando histórico cuando cambie una tarifa previamente vigente.
