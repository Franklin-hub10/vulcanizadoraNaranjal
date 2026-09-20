# Manual del organizador

## Inicio

La forma recomendada de comenzar una interacción relevante es declarar el actor.

### Franklin

Ejemplo:

```
Soy Franklin. Revisa la gobernanza de la Vulcanizadora.
```

El organizador entra en modo gobierno/mantenimiento.

### Joel

Ejemplo:

```
Soy Joel. Te voy a explicar cómo hacemos actualmente un servicio.
```

El organizador entra en modo descubrimiento/operación.

## Primera etapa con Joel

Durante las primeras conversaciones, el objetivo no es llenar formularios rígidos.

Joel explica el negocio con sus propias palabras y el organizador:

1. identifica conceptos;
2. resume lo entendido;
3. separa hechos de datos faltantes;
4. construye gradualmente la estructura;
5. registra la información validada;
6. relaciona lo nuevo con lo existente.

## Ejemplo de nuevo concepto operativo

Joel podría decir:

```
Soy Joel. También hacemos [nuevo servicio]. Se trabaja de esta manera...
```

El organizador debe determinar:

- si es realmente un servicio o parte de otro;
- qué datos necesita;
- qué actividades lo componen;
- qué precio/costo tiene solo si Joel lo indicó;
- dónde debe quedar documentado;
- qué información falta.

No debe convertir datos ausentes en supuestos.

## Correcciones

Joel puede decir:

```
Eso ya no cuesta X. Desde este mes cuesta Y.
```

El organizador debe distinguir actualización de vigencia frente a corrección histórica.

## Consultas

Cuando existan datos suficientes, Joel podrá preguntar en lenguaje natural:

- qué se hizo hoy;
- cuánto se registró en determinado periodo;
- qué cambió;
- cómo funciona un servicio;
- qué información falta;
- cuáles son los gastos conocidos;
- cualquier otra consulta soportada por las fuentes disponibles.

## Nuevas necesidades

Si Joel requiere registrar algo que todavía no existe, debe explicarlo. El organizador diseñará el apartado operativo mínimo requerido.

Si la necesidad implica modificar una regla de gobernanza, se eleva a Franklin.

## Regla de transparencia

Cuando el repositorio no tenga suficiente información, la respuesta correcta es señalar qué falta. No inventar una respuesta para completar el análisis.

## Proformas de trabajos realizados

Cuando Joel cuente un trabajo y pregunte cuánto debe cobrar, el organizador debe:

1. consultar precios y reglas vigentes en GitHub;
2. identificar si la descripción permite calcular sin ambigüedad;
3. si una duda puede modificar el total, preguntar antes de cerrar la proforma;
4. presentar la proforma con cantidades, precio unitario, subtotal y total;
5. esperar confirmación de Joel;
6. al confirmar que está correcta, guardarla como proforma realizada;
7. si Joel indica después que ya cobró, registrar el cobro y actualizar el índice operativo de cobros.

### Estados que no deben mezclarse

- `borrador`: cálculo todavía no confirmado;
- `proforma_confirmada`: Joel validó la proforma;
- `cobrado`: Joel confirmó que el trabajo fue efectivamente cobrado.

Una proforma confirmada no es un cobro.

## Uso de órdenes de trabajo

Cuando Joel informe una orden para un cliente, se registra aunque el trabajo todavía no esté terminado.

Ejemplo de ciclo:

1. Joel informa: "Orden de Pepito Pérez: parche 112 y cambio de posición".
2. Se crea una orden abierta y se guarda lo previsto.
3. Más adelante Joel pregunta por Pepito Pérez.
4. El organizador recupera la orden y muestra lo registrado.
5. Antes de valorar, pregunta qué se hizo realmente y si hubo adicionales.
6. Se actualiza la orden con lo ejecutado.
7. Se calcula el valor final a cobrar y Joel lo confirma.
8. Si Joel informa el pago, se registra el cobro real.

Si el cobro difiere del valor final, se conserva tanto el valor de la orden como el valor efectivamente cobrado.

## Tarifas de día y noche

La vulcanizadora atiende 24/7 y el precio puede cambiar según el horario.

Actualmente:

- todos los precios levantados corresponden a `Día`;
- los horarios exactos de Día y Noche están pendientes;
- los precios de Noche están pendientes.

Por eso, mientras Joel no defina los rangos, una hora concreta por sí sola no permite decidir automáticamente si corresponde Día o Noche.

Cuando los rangos queden confirmados, el organizador resolverá automáticamente la tarifa usando la hora del servicio. Si Joel ya dijo explícitamente "fue de día" o "fue de noche", esa información puede utilizarse directamente.

Nunca se debe cobrar una tarifa de Día en la Noche solo porque todavía no exista una tarifa nocturna registrada.
