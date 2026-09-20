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
