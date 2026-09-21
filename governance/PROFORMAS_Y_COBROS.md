# Política de órdenes de trabajo, proformas y cobros

## Propósito

Definir el flujo obligatorio para órdenes de trabajo, proformas/cotizaciones previas, valoración final de trabajos ejecutados y cobros.

Esta política evita que una duda operativa se convierta en un valor inventado y separa claramente lo planificado, lo realizado, lo valorado y lo efectivamente cobrado.

## Flujo obligatorio

### Etapa 1 — Aclaración antes de la proforma

Antes de construir la proforma, el organizador debe revisar las fuentes canónicas de precios, servicios, insumos y reglas aplicables.

Si existe cualquier duda material sobre lo que Joel hizo, la cantidad, la unidad de cobro, el servicio aplicado, el precio vigente o una regla necesaria para calcular el valor:

1. no cerrar la proforma;
2. preguntar a Joel;
3. esperar su definición;
4. registrar la aclaración operativa si corresponde;
5. recién entonces calcular la proforma.

No se debe completar un vacío mediante suposición.

Si toda la información necesaria ya está confirmada y es inequívoca, se puede construir la proforma directamente.

### Etapa 2 — Proforma confirmada

La primera proforma presentada es un borrador conversacional hasta que Joel confirme explícitamente que está correcta.

Ejemplos válidos de confirmación:

- "está correcto";
- "está bien";
- "ok";
- "esa es";
- otra expresión inequívoca de aprobación.

Una vez confirmada:

1. registrar la proforma en `operacion/proformas/`;
2. asignar un identificador único;
3. incluir el detalle de conceptos, cantidades, precios unitarios, subtotales y total;
4. indicar las fuentes canónicas utilizadas;
5. registrar la fecha de confirmación;
6. añadirla a `operacion/proformas/INDEX.md`.

Estado canónico: `proforma_confirmada`.

Una proforma confirmada **no se considera cobrada** por el solo hecho de haber sido aprobada.

### Etapa 3 — Cobro confirmado

Solo cuando Joel indique explícitamente que la proforma o trabajo **ya fue cobrado**, se registra como cobro.

Al recibir esa confirmación:

1. crear el registro correspondiente en `operacion/cobros/`;
2. relacionarlo con la proforma de origen;
3. registrar el importe efectivamente cobrado;
4. si el importe cobrado difiere de la proforma, aclarar la diferencia antes de cerrar el registro;
5. añadir el cobro a `operacion/cobros/INDEX.md`;
6. indexarlo en `operacion/indicadores/COBROS.md`.

Estado canónico: `cobrado`.

Si Joel no confirma que fue cobrado, no se registra como ingreso ni como cobro realizado.

## Regla de ambigüedad

Cuando una ambigüedad pueda cambiar el valor final, el organizador debe preguntar antes de emitir la proforma.

Ejemplos:

- no está claro cuántas llantas se movieron;
- no está claro si una tarifa es por llanta, por aro o por operación;
- no está claro qué parche se utilizó;
- el trabajo informado no coincide con un servicio documentado;
- existe más de una interpretación razonable que produce totales distintos.

### Regla específica para parches

Cuando una proforma, orden o consulta incluya un parche, antes de seleccionar el precio debe quedar resuelta la modalidad comercial:

- **con mano de obra**: usar la tarifa de parche instalado; esa tarifa ya incluye la mano de obra;
- **solo parche / sin mano de obra**: usar la tarifa de venta del insumo sin instalación.

Si la persona no especifica la modalidad, el organizador debe preguntar antes de calcular, aunque ambas tarifas coincidan para una numeración determinada.

La fuente operativa de esta distinción es operacion/insumos/PARCHES.md y la tarifa aplicable por franja se resuelve en operacion/tarifas/TARIFAS_POR_FRANJA.md.

## Identificadores

Las proformas usarán: `PF-YYYYMMDD-NNN`.

Los cobros usarán: `CB-YYYYMMDD-NNN`.

La secuencia se determina revisando los registros existentes para la fecha. No se reutilizan identificadores.

## Campos mínimos de una proforma

- identificador;
- fecha de trabajo, si está confirmada;
- fecha de confirmación;
- detalle de trabajos e insumos;
- cantidad;
- precio unitario;
- subtotal;
- total;
- fuentes de precios/reglas;
- aclaraciones relevantes;
- estado.

No se inventan cliente, placa, forma de pago u otros campos no informados.

## Campos mínimos de un cobro

- identificador de cobro;
- proforma relacionada;
- fecha de confirmación del cobro;
- fecha efectiva de cobro, únicamente si está confirmada;
- total cobrado;
- diferencias frente a la proforma, si existen;
- estado `cobrado`.

## Indicadores

`operacion/indicadores/COBROS.md` es un índice operativo de cobros confirmados. Su existencia no implica que todos los KPI financieros de VN-04 estén definidos.

Solo se alimenta con registros cuyo estado sea `cobrado`.

## Autoridad

Esta política fue definida por Franklin como regla de gobernanza el 2026-09-20.

## Órdenes de trabajo — flujo previo a la valoración

Cuando Joel informe una orden de trabajo para un cliente, el organizador debe registrarla antes del cobro en `operacion/ordenes_trabajo/` con un identificador `OT-YYYYMMDD-NNN`.

La orden debe separar siempre:

- trabajos previstos;
- trabajos confirmados como realizados;
- trabajos confirmados como no realizados;
- trabajos adicionales realizados;
- observaciones relevantes;
- estado de la orden.

El nombre del cliente puede utilizarse para localizar la orden, pero no es un identificador único. Si existen varias órdenes razonablemente coincidentes, se debe aclarar cuál corresponde antes de modificarla.

### Recuperación posterior

Cuando Joel pregunte por una orden anterior, el organizador debe consultar el repositorio y responder con lo que quedó registrado. Debe distinguir lo previsto de lo ya confirmado como realizado.

Antes de calcular el valor final, debe preguntarse o verificarse con Joel:

1. si se hicieron todos los trabajos previstos;
2. si alguno no se realizó;
3. si se realizó algo adicional;
4. si cambió alguna cantidad, pieza, parche, servicio o condición que afecte el cobro.

Lo previsto nunca se considera realizado por defecto.

### Valor final de la orden

Una vez conciliado lo realmente ejecutado, se calcula el **valor final a cobrar de la orden de trabajo**. Para trabajo ya ejecutado, este valor no se trata como una proforma previa.

Solo los ítems confirmados como realizados o adicionales realizados forman parte del total a cobrar.

La orden pasa a `orden_valorada` únicamente después de que Joel confirme que el detalle y el total son correctos.

### Cobro y desfases

Una orden valorada no equivale a un cobro. Solo se registra como cobrada cuando Joel confirme el pago.

Si Joel informa que cobró un valor distinto al valor final de la orden, se registra el importe realmente cobrado y el desfase. No se inventa la causa; se registra únicamente la explicación que Joel proporcione.

### Órdenes informadas después de ejecutar el trabajo

Si Joel informa por primera vez un trabajo cuando ya fue realizado, se puede crear una orden retrospectiva y marcar como realizados únicamente los ítems que Joel confirme.

## Resolución horaria antes de valorar

Antes de calcular el valor final de una orden, una cotización o cualquier importe a cobrar, el organizador debe resolver la franja horaria aplicable usando `operacion/tarifas/TARIFAS_POR_FRANJA.md`.

La hora relevante es la hora del servicio, no necesariamente la hora en que Joel hace la consulta.

Si el trabajo incluye actividades realizadas en franjas diferentes, cada ítem deberá valorarse con la franja que corresponda a su ejecución cuando esa información esté disponible.

Si la franja o su tarifa no están definidas, el valor no se cierra hasta que Joel aclare el dato necesario.
