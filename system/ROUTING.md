# Routing del organizador

## Objetivo

Resolver qué contexto leer y qué tipo de cambio puede ejecutar el organizador.

## Disparadores

### "Soy Franklin"

Modo: `governance`

Orden mínimo de lectura:

1. `README.md`
2. `BACKLOG.md`
3. `governance/RULES.md`
4. documento de gobernanza relacionado con la solicitud
5. fuentes operativas relacionadas, si aplica

Puede trabajar sobre gobernanza y operación.

### "Soy Joel"

Modo: `business_operation`

Orden mínimo de lectura:

1. `README.md`
2. `BACKLOG.md`
3. `governance/RULES.md`
4. fuentes operativas relacionadas
5. histórico pertinente, si la solicitud depende del tiempo

No modifica reglas duras.

## Solicitud de Joel sobre algo nuevo

Ruta de decisión:

```
Joel explica algo nuevo
        ↓
¿es información del negocio?
   ├─ sí → ¿existe fuente canónica?
   │          ├─ sí → ampliar/actualizar
   │          └─ no → crear estructura operativa mínima
   │
   └─ no → ¿afecta gobernanza?
              ├─ sí → registrar pendiente para Franklin
              └─ no → documentar según corresponda
```

## Consultas sin actor declarado

Si el actor no cambia el resultado, el organizador puede responder con las fuentes vigentes.

Si la solicitud pretende modificar gobernanza o existe riesgo de mezclar modos, debe requerirse contexto de actor antes de aplicar el cambio.

## Frases del proyecto

Referencias como:

- "Vulcanizadora"
- "Vulcanizadora Naranjal"
- "VN"

deben hacer que el organizador trate este repositorio como la fuente canónica cuando el contexto indique que se habla de este negocio.

## Routing de proformas y cobros

Ante expresiones como:

- "hazme la proforma";
- "cuánto cobro";
- "este fue el trabajo";
- "ya está correcto";
- "ya lo cobré";
- "ya fue cobrado";

el organizador debe:

1. leer `governance/PROFORMAS_Y_COBROS.md`;
2. leer las fuentes operativas de precios y reglas del trabajo;
3. resolver cualquier ambigüedad material con Joel antes de cerrar la proforma;
4. persistir la proforma solo después de confirmación;
5. registrar e indexar el cobro solo después de confirmación explícita de cobro.

## Routing de órdenes de trabajo

Ante expresiones como:

- "orden de trabajo";
- "a este cliente le voy a hacer";
- "qué tenía la orden de [cliente]";
- "qué se hizo en esa orden";
- "cuánto debo cobrar esta orden";

el organizador debe consultar `operacion/ordenes_trabajo/` y la política de `governance/PROFORMAS_Y_COBROS.md`.

Si se trata de cerrar una orden, primero debe conciliar lo previsto contra lo realmente ejecutado y preguntar por adicionales o trabajos no realizados antes de calcular el total.

## Routing de tarifas por horario

Ante consultas de precio, valoración de órdenes o cobro, el organizador debe consultar `operacion/tarifas/TARIFAS_POR_FRANJA.md` antes de usar un valor.

### Resolución

1. identificar la hora del servicio o la franja indicada por Joel;
2. si los límites horarios están definidos, clasificar automáticamente en la franja correspondiente;
3. si los límites todavía están pendientes y Joel no indicó la franja, preguntar;
4. aplicar únicamente una tarifa confirmada para esa franja;
5. si la tarifa de la franja está pendiente, detener el cálculo y pedir definición.

Para consultas del tipo "precio ahora", una vez definidos los rangos se utilizará la hora local `America/Guayaquil`.
