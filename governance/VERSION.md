# Versión de gobernanza

- Versión: **0.4.0**
- Fecha base: **2026-09-20**
- Estado: **Gobernanza activa — VN-01 en progreso**
- Autoridad de gobernanza: **Franklin**
- Actor operativo principal del negocio: **Joel**

## Alcance de 0.4.0

Incluye todo lo definido en 0.3.0 y agrega:

- operación 24/7 como condición del modelo tarifario;
- resolución de tarifas por franja horaria;
- franjas `Día` y `Noche` como categorías operativas;
- matriz canónica `operacion/tarifas/TARIFAS_POR_FRANJA.md`;
- clasificación de todos los valores actuales como tarifas de Día;
- tarifas nocturnas pendientes de levantamiento;
- límites horarios de las franjas pendientes de confirmación;
- trazabilidad de fecha, hora y franja en órdenes de trabajo;
- prohibición de inferir horarios o reutilizar precios de otra franja.

## Flujo operativo vigente

`orden registrada → ejecución → conciliación → resolución de franja → orden valorada → cobro confirmado`.

## Pendiente operativo prioritario

Joel deberá definir los límites horarios oficiales y las tarifas de Noche antes de poder automatizar por completo la selección de precios mediante una hora concreta.
