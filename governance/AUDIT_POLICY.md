# Política de auditoría

## Objetivo

Permitir reconstruir por qué existe una regla, de dónde provino un dato relevante y cuándo cambió la estructura del conocimiento.

## Debe dejar trazabilidad

- cambios de gobernanza;
- cambios de arquitectura;
- cambios de roles o alcance;
- altas o retiros de fuentes canónicas;
- correcciones materiales;
- cambios de vigencia que afecten análisis históricos;
- decisiones sobre nuevas categorías estructurales.

## No requiere log individual obligatorio

Una captura operativa rutinaria puede quedar trazada por el propio historial Git cuando su modificación ya contiene fecha, fuente y contexto suficientes.

## Datos mínimos para decisiones estructurales

- fecha;
- identificador;
- actor/origen;
- decisión;
- motivo;
- impacto;
- archivos afectados, cuando aplique.

## Principio

Git conserva el cambio técnico; los documentos de histórico conservan el **significado del cambio**.

No duplicar cada commit en un log manual. Registrar manualmente aquello que una revisión de diff no explicaría por sí sola.
