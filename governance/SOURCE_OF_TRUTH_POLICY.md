# Política de fuente de verdad

## Fuente principal

El repositorio `Franklin-hub10/vulcanizadoraNaranjal` es la fuente persistente de verdad para la información que haya sido incorporada formalmente al sistema.

## Prioridad

Cuando existan versiones distintas de una misma información, usar este orden:

1. fuente canónica vigente del repositorio;
2. actualización explícita más reciente con vigencia clara;
3. histórico para reconstruir periodos anteriores;
4. conversación actual aún no persistida;
5. memoria o contexto previo solo como pista para localizar la fuente, nunca para contradecirla.

## Datos nuevos durante una conversación

Un dato informado por Franklin o Joel puede utilizarse en la conversación actual, pero si debe formar parte del conocimiento reutilizable del negocio debe persistirse en GitHub.

## Conflictos

Si una conversación contradice el repositorio:

- determinar si es una corrección;
- determinar si es un cambio de vigencia;
- no sobrescribir silenciosamente;
- actualizar la fuente adecuada;
- conservar histórico cuando corresponda.

## Ausencia de datos

Que el repositorio no contenga un dato significa **dato no registrado**, no valor cero y no autorización para inferirlo.

## Fuentes externas futuras

Si se incorporan facturas, hojas de cálculo, documentos, APIs u otras fuentes, cada integración deberá definir:

- autoridad de la fuente;
- frecuencia;
- campos;
- fecha de corte;
- método de conciliación;
- tratamiento de inconsistencias.

## Proformas y cobros

Para trabajos realizados se distinguen tres niveles de evidencia:

1. **información conversacional / borrador:** puede usarse para aclarar y calcular, pero no representa una proforma confirmada;
2. **proforma confirmada:** existe cuando Joel valida expresamente el cálculo y debe persistirse en `operacion/proformas/`;
3. **cobro confirmado:** existe únicamente cuando Joel declara que el trabajo fue cobrado y debe persistirse en `operacion/cobros/` e indexarse para indicadores.

La confirmación de una proforma nunca sustituye la confirmación de cobro.

## Órdenes de trabajo como evidencia operativa

Las órdenes persistidas en `operacion/ordenes_trabajo/` son la fuente canónica para reconstruir trabajos previstos y su evolución.

Dentro de una orden, `previsto` y `realizado` son estados distintos. Un ítem previsto no prueba ejecución.

El valor final debe basarse en ítems confirmados como realizados. El cobro real debe basarse en confirmación explícita de Joel.
