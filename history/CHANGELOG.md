# Changelog documental

## 2026-09-20 — Gobernanza 0.1.0

Se inicializa el repositorio canónico de Vulcanizadora Naranjal.

### Añadido

- modelo Franklin / Joel;
- separación gobernanza / operación;
- reglas contra invenciones;
- política de cambios;
- ciclo de vida del conocimiento;
- arquitectura documental inicial;
- routing del organizador;
- histórico de decisiones;
- política de auditoría;
- política de fuente de verdad;
- roadmap de madurez.

### Pendiente

- levantamiento real de la operación con Joel;
- definición del modelo canónico del negocio;
- definición de registros operativos;
- definición de indicadores;
- estructura de pilotos, escenarios y proyecciones a partir de datos reales.


## 2026-09-20 — Inicio de levantamiento operativo VN-01

### Añadido

- área `operacion/insumos/`;
- catálogo canónico inicial de parches informados por Joel;
- numeraciones confirmadas de parches, parches estrellados y parches pequeños;
- uso informado del parche pequeño 01 para motos o carros de llanta baja.

### Sin registrar todavía

No se agregaron precios, costos, stock, proveedores, marcas ni criterios técnicos no informados.


## 2026-09-20 — Precios cobrados por parches

### Añadido

Se registran como precios cobrados al cliente, informados directamente por Joel:

- parche 110: $10.00;
- parche 112: $10.00;
- parche 120: $18.00;
- parche 135: $25.00;
- parche 142: $30.00;
- parche estrellado 02: $10.00;
- parche estrellado 05: $18.00;
- parche pequeño 01: $3.00.

### Aclaración

Los valores registrados son precios de venta/cobro al cliente. El costo de compra de cada insumo continúa pendiente de levantamiento.


## 2026-09-20 — Regla comercial de parches

### Añadido

Joel confirma que:

- los precios registrados de los parches ya incluyen la mano de obra cuando se realiza la instalación;
- si el cliente compra únicamente el parche, sin instalación, se cobra el mismo valor;
- actualmente no existe diferencia de precio entre parche instalado y parche vendido sin instalación.

### Impacto

Los precios registrados continúan siendo el precio final cobrado al cliente para cada numeración. La mano de obra no se registra como cargo adicional separado en estos casos.


## 2026-09-20 — Catálogo inicial de servicios

### Añadido

Joel confirma que Vulcanizadora Naranjal ofrece:

- cambio de llantas;
- rotación de llantas;
- cambio de aro;
- apretada de tuercas;
- inflar llantas;
- dar aire;
- arreglo de llantas de moto.

### Pendiente

No se registran todavía precios, procedimientos, tiempos, materiales ni condiciones específicas para estos servicios.

### Nota

`Inflar llantas` y `Dar aire` se conservan como conceptos separados hasta que Joel confirme si son equivalentes o diferentes.


## 2026-09-20 — Tarifas de cambio de llantas para carro pequeño

### Añadido

Joel informa los siguientes servicios y precios:

- armar y desarmar la llanta: $2.00;
- cambio de posición de llanta: $1.00 por llanta;
- desarmar llantas fuera del vehículo: $1.00;
- armar y desarmar para virarla en el mismo aro: $2.00;
- cambio de llanta por la llanta de emergencia: $2.00;
- cambio por llantas nuevas: $2.00 por aro.

### Pendiente de precisión

No se infiere la unidad de cobro de los servicios donde Joel todavía no indicó expresamente si el valor corresponde a cada llanta, cada aro o a la operación.

## 2026-09-20 — Flujo gobernado de proformas y cobros

### Añadido

- política canónica `governance/PROFORMAS_Y_COBROS.md`;
- regla dura R-016;
- routing específico para proformas y cobros;
- índice de proformas confirmadas;
- índice de cobros confirmados;
- índice operativo para futuros indicadores de cobro.

### Regla principal

Una proforma se registra solo tras confirmación de Joel. Un cobro se registra e indexa únicamente cuando Joel confirme expresamente que el trabajo ya fue cobrado.

## 2026-09-20 — Aclaración de cambio de posición de llantas

### Confirmado

- la tarifa de cambio de posición para carro pequeño es $1.00 por llanta;
- cuando el cambio de posición implica intercambiar ubicaciones, se mueven dos llantas;
- en ese caso se cobran 2 llantas, para un total de $2.00 por el cambio de posición.

Esta regla queda incorporada en `operacion/servicios/CAMBIO_LLANTAS_CARRO_PEQUENO.md`.
