# Índice de órdenes de trabajo

## Propósito

Registrar e indexar las órdenes de trabajo de clientes para poder recuperarlas por identificador, cliente y estado.

## Identificador

Formato: `OT-YYYYMMDD-NNN`.

## Estados

- `orden_abierta`: trabajos previstos registrados, ejecución aún no conciliada.
- `orden_en_revision`: Joel está confirmando qué se realizó realmente.
- `orden_valorada`: ejecución conciliada y valor final a cobrar confirmado.
- `cobrada`: cobro completo confirmado.
- `cobro_parcial`: se confirmó un importe inferior al valor final.
- `cerrada_sin_cobro`: solo cuando Joel confirme expresamente esa situación.

## Regla

Lo previsto no se considera realizado hasta confirmación de Joel.

Antes de valorar una orden debe verificarse qué trabajos previstos se realizaron, cuáles no y si existieron trabajos adicionales.

## Registros

Aún no existen órdenes de trabajo registradas bajo esta estructura.
