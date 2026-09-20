# Actores y alcance

## Objetivo

Separar con claridad las funciones de **Franklin** y **Joel** dentro del organizador sin confundir contexto conversacional con autenticación técnica.

## Franklin

**Modo principal:** gobernanza / mantenimiento.

Puede solicitar:

- creación, modificación o retiro de reglas de gobernanza;
- reestructuración de carpetas y documentos;
- cambios de metodología;
- cambios de taxonomía;
- definición de indicadores y criterios;
- revisión de consistencia;
- auditoría del repositorio;
- cambios de routing;
- decisiones sobre qué se considera fuente canónica.

También puede operar sobre información del negocio.

## Joel

**Modo principal:** descubrimiento / operación.

Puede:

- contar cómo funciona el negocio;
- describir servicios;
- explicar actividades;
- informar precios;
- informar costos y gastos;
- explicar recursos y materiales;
- informar movimientos y resultados;
- corregir datos de operación;
- agregar nuevas necesidades;
- introducir un servicio, actividad, gasto, recurso o concepto no modelado todavía;
- solicitar consultas y análisis.

### Cuando Joel introduce algo nuevo

El organizador no debe responder "eso no existe en la estructura".

Debe:

1. escuchar la explicación;
2. identificar la naturaleza del nuevo concepto;
3. verificar relaciones con conceptos existentes;
4. crear o ampliar la documentación operativa necesaria;
5. registrar el nuevo concepto como confirmado, parcial o pendiente según la evidencia;
6. conservar trazabilidad.

### Límite de Joel

Joel no cambia directamente:

- reglas duras;
- autoridad de actores;
- política de histórico;
- arquitectura de gobernanza;
- política de cambios;
- definición de fuente de verdad.

Una solicitud de este tipo se registra como propuesta pendiente para Franklin.

## Cambio de actor durante una conversación

Si el usuario declara explícitamente un actor distinto, el organizador cambia de modo para las acciones siguientes.

La información registrada no cambia de dueño por ese motivo: pertenece al negocio.

## Seguridad

Este modelo es una **barrera operativa del organizador**.

No prueba identidad. Si en el futuro se requiere seguridad fuerte, deberá implementarse mediante autenticación y permisos fuera de esta declaración conversacional.
