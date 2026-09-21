# Matriz canónica de tarifas por franja horaria

## Propósito

Resolver qué tarifa corresponde aplicar según la franja horaria, el concepto y la modalidad de atención de Vulcanizadora Naranjal.

El negocio opera 24/7 y las tarifas pueden cambiar según la franja. Esta matriz es la fuente canónica para seleccionar el valor aplicable antes de valorar una orden de trabajo, elaborar una cotización o responder una consulta de precios.

## Franjas definidas

| Franja | Estado | Hora inicio | Hora fin | Observación |
|---|---|---|---|---|
| Día | Confirmada como categoría | Pendiente | Pendiente | Los valores confirmados hasta el 2026-09-21 corresponden a esta franja. |
| Noche | Confirmada como categoría | Pendiente | Pendiente | Tarifas y límites horarios pendientes de definición. |

> Los horarios 08:30–17:30 mencionados como ejemplo **no están confirmados** y no se registran como límites oficiales.

## Método de resolución de tarifa

Para seleccionar una tarifa:

1. identificar la fecha y hora aplicable al servicio;
2. identificar el concepto exacto;
3. para parches, identificar obligatoriamente la modalidad: con mano de obra o solo parche;
4. si se indicó explícitamente la franja (Día o Noche), usar esa franja;
5. cuando existan límites horarios confirmados, clasificar automáticamente la hora;
6. aplicar únicamente una tarifa cuyo estado esté confirmado;
7. si falta franja, modalidad o tarifa, no inventar el precio: preguntar antes de valorar.

### Hora que gobierna

- Para una orden ya ejecutada: usar la hora de ejecución del trabajo cuando esté confirmada.
- Para una orden futura: usar la hora prevista del servicio si fue informada.
- Para una consulta de precio inmediato del tipo “¿cuánto cuesta ahora?”: cuando los rangos estén definidos, usar la hora local de Ecuador (America/Guayaquil).
- La hora en que se hace la consulta no reemplaza la hora real del servicio cuando ambas son diferentes.

## Tarifas vigentes — parches con mano de obra incluida

| Vehículo | Categoría | Servicio / insumo | Modalidad | Día | Estado día | Noche | Estado noche | Fuente |
|---|---|---|---|---:|---|---:|---|---|
| Carro pequeño | Parche | 110 | con mano de obra | $10.00 | confirmado | — | pendiente | operacion/insumos/PARCHES.md |
| Carro pequeño | Parche | 112 | con mano de obra | $13.00 | confirmado | — | pendiente | operacion/insumos/PARCHES.md |
| Carro pequeño | Parche | 114 | con mano de obra | $15.00 | confirmado | — | pendiente | operacion/insumos/PARCHES.md |
| Carro pequeño | Estrellado | 04 | con mano de obra | $18.00 | confirmado | — | pendiente | operacion/insumos/PARCHES.md |
| Carro pequeño | Estrellado | 05 | con mano de obra | $22.00 | confirmado | — | pendiente | operacion/insumos/PARCHES.md |
| Carro pequeño | Estrellado | 02 | con mano de obra | $12.00 | confirmado | — | pendiente | operacion/insumos/PARCHES.md |
| Carro pequeño | Estrellado | 01 | con mano de obra | $10.00 | confirmado | — | pendiente | operacion/insumos/PARCHES.md |
| Carro pequeño | Estrellado | 08 | con mano de obra | $10.00 | confirmado | — | pendiente | operacion/insumos/PARCHES.md |
| Carro pequeño | Grande | 140 | con mano de obra | $18.00 | confirmado | — | pendiente | operacion/insumos/PARCHES.md |
| Carro pequeño | Grande | 135 | con mano de obra | $25.00 | confirmado | — | pendiente | operacion/insumos/PARCHES.md |
| Carro pequeño | Grande | 142 | con mano de obra | $30.00 | confirmado | — | pendiente | operacion/insumos/PARCHES.md |
| Carro pequeño | Grande | 145 | con mano de obra | $40.00 | confirmado | — | pendiente | operacion/insumos/PARCHES.md |
| Carro | Especial | Pequeño Pulcaflex | con mano de obra | $3.00 | confirmado | — | pendiente | operacion/insumos/PARCHES.md |
| Carro | Especial | Cuadrado | con mano de obra | $4.00 | confirmado | — | pendiente | operacion/insumos/PARCHES.md |
| Carro | Especial | Mediano / redondo | con mano de obra | $5.00 | confirmado | — | pendiente | operacion/insumos/PARCHES.md |
| Moto | Especial | Pequeño Pulcaflex | con mano de obra | $3.00 | confirmado | — | pendiente | operacion/insumos/PARCHES.md |

## Tarifas vigentes — solo parche, sin mano de obra

| Vehículo | Categoría | Servicio / insumo | Modalidad | Día | Estado día | Noche | Estado noche | Fuente |
|---|---|---|---|---:|---|---:|---|---|
| Carro pequeño | Parche | 110 | solo parche | $10.00 | confirmado | — | pendiente | operacion/insumos/PARCHES.md |
| Carro pequeño | Parche | 112 | solo parche | $13.00 | confirmado | — | pendiente | operacion/insumos/PARCHES.md |
| Carro pequeño | Parche | 114 | solo parche | $15.00 | confirmado | — | pendiente | operacion/insumos/PARCHES.md |
| Carro pequeño | Estrellado | 04 | solo parche | $15.00 | confirmado | — | pendiente | operacion/insumos/PARCHES.md |
| Carro pequeño | Estrellado | 05 | solo parche | $18.00 | confirmado | — | pendiente | operacion/insumos/PARCHES.md |
| Carro pequeño | Estrellado | 02 | solo parche | $10.00 | confirmado | — | pendiente | operacion/insumos/PARCHES.md |
| Carro pequeño | Estrellado | 01 | solo parche | $8.00 | confirmado | — | pendiente | operacion/insumos/PARCHES.md |
| Carro pequeño | Estrellado | 08 | solo parche | $8.00 | confirmado | — | pendiente | operacion/insumos/PARCHES.md |
| Carro pequeño | Grande | 140 | solo parche | $18.00 | confirmado | — | pendiente | operacion/insumos/PARCHES.md |
| Carro pequeño | Grande | 135 | solo parche | $25.00 | confirmado | — | pendiente | operacion/insumos/PARCHES.md |
| Carro pequeño | Grande | 142 | solo parche | $30.00 | confirmado | — | pendiente | operacion/insumos/PARCHES.md |
| Carro pequeño | Grande | 145 | solo parche | $40.00 | confirmado | — | pendiente | operacion/insumos/PARCHES.md |
| Carro | Especial | Pequeño Pulcaflex | solo parche | $0.25 | confirmado | — | pendiente | operacion/insumos/PARCHES.md |
| Carro | Especial | Cuadrado | solo parche | $0.50 | confirmado | — | pendiente | operacion/insumos/PARCHES.md |
| Carro | Especial | Mediano / redondo | solo parche | $0.50 | confirmado | — | pendiente | operacion/insumos/PARCHES.md |
| Moto | Especial | Pequeño Pulcaflex | solo parche | $0.25 | confirmado | — | pendiente | operacion/insumos/PARCHES.md |

## Otros servicios vigentes — carro pequeño

| Tipo | Servicio | Unidad de cobro | Día | Estado día | Noche | Estado noche | Fuente operativa |
|---|---|---|---:|---|---:|---|---|
| Servicio carro pequeño | Armar y desarmar la llanta | unidad pendiente de precisar | $2.00 | confirmado | — | pendiente | operacion/servicios/CAMBIO_LLANTAS_CARRO_PEQUENO.md |
| Servicio carro pequeño | Cambio de posición de llanta | por llanta | $1.00 | confirmado | — | pendiente | operacion/servicios/CAMBIO_LLANTAS_CARRO_PEQUENO.md |
| Servicio carro pequeño | Desarmar llantas fuera del vehículo | unidad pendiente de precisar | $1.00 | confirmado | — | pendiente | operacion/servicios/CAMBIO_LLANTAS_CARRO_PEQUENO.md |
| Servicio carro pequeño | Armar y desarmar para virarla en el mismo aro | unidad pendiente de precisar | $2.00 | confirmado | — | pendiente | operacion/servicios/CAMBIO_LLANTAS_CARRO_PEQUENO.md |
| Servicio carro pequeño | Cambio de llanta por la llanta de emergencia | unidad pendiente de precisar | $2.00 | confirmado | — | pendiente | operacion/servicios/CAMBIO_LLANTAS_CARRO_PEQUENO.md |
| Servicio carro pequeño | Cambio por llantas nuevas | por aro | $2.00 | confirmado | — | pendiente | operacion/servicios/CAMBIO_LLANTAS_CARRO_PEQUENO.md |

## Regla especial de cambio de posición

La tarifa diurna es $1.00 por llanta. Cuando la operación implica intercambiar dos posiciones, se contabilizan dos llantas y el total diurno de ese movimiento es $2.00.

## Regla especial para parches

Antes de valorar cualquier parche se deben resolver cuatro datos:

1. tipo de vehículo;
2. tipo/código de parche;
3. modalidad: con mano de obra o solo parche;
4. franja horaria aplicable.

Si la modalidad no fue informada, se pregunta antes de cotizar. No se presume instalación ni venta directa.

Para moto, dentro del catálogo especial actual, únicamente está confirmado el parche pequeño Pulcaflex. No se aplican automáticamente los precios de parche cuadrado o mediano/redondo de carro a una moto.

## Pendientes obligatorios

Se debe definir posteriormente:

- hora de inicio y fin de la franja Día;
- hora de inicio y fin de la franja Noche;
- tarifas nocturnas por cada servicio e insumo;
- cualquier excepción por día de semana, feriado u otra condición, solo si realmente existe;
- cualquier unidad de cobro que aún figure pendiente.

## Regla de actualización

Cuando se confirmen límites horarios o nuevas tarifas, se actualiza esta matriz conservando trazabilidad cuando cambie una tarifa o se corrija un dato material.
