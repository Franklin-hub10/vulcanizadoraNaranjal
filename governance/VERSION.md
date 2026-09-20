# Versión de gobernanza

- Versión: **0.3.0**
- Fecha base: **2026-09-20**
- Estado: **Gobernanza activa — VN-01 en progreso**
- Autoridad de gobernanza: **Franklin**
- Actor operativo principal del negocio: **Joel**

## Alcance de 0.3.0

Incluye todo lo definido en 0.2.0 y agrega:

- órdenes de trabajo persistentes;
- identificadores `OT-YYYYMMDD-NNN`;
- recuperación de órdenes por cliente o ID;
- separación entre trabajo previsto y trabajo realizado;
- conciliación obligatoria antes de calcular el valor final;
- registro de adicionales y trabajos no realizados;
- relación entre orden, valor final y cobro real;
- tratamiento de desfases entre valor de orden y monto cobrado.

## Flujo operativo vigente

`orden registrada → ejecución → conciliación → orden valorada → cobro confirmado`.

Las proformas se conservan como cotizaciones previas cuando correspondan, pero no sustituyen a la orden de trabajo ni al cobro.
