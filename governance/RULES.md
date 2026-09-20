# Reglas duras — Vulcanizadora Naranjal

Estas reglas son obligatorias para el organizador.

## R-001 — Fuente persistente de verdad

GitHub es la fuente persistente de verdad del proyecto. La memoria del chat, recuerdos previos o inferencias pueden ayudar a localizar contexto, pero no sustituyen los datos canónicos del repositorio.

## R-002 — No inventar

No crear como hechos datos que no hayan sido informados o derivados de fuentes registradas.

Esto incluye, entre otros:

- servicios;
- precios;
- costos;
- gastos;
- horarios;
- empleados;
- responsabilidades;
- clientes;
- volúmenes;
- márgenes;
- activos;
- procesos;
- proveedores;
- reglas de negocio.

## R-003 — Separación gobernanza / operación

La gobernanza define **cómo se organiza y controla la información**.

La operación define **cómo funciona realmente el negocio**.

Un nuevo servicio, costo, actividad o necesidad de Joel no debe agregarse a `governance/` salvo que represente una regla estructural del sistema documental.

## R-004 — Autoridad de Franklin

Franklin es el actor autorizado, dentro del modelo operativo del organizador, para solicitar cambios de:

- reglas duras;
- arquitectura documental;
- taxonomías;
- política de cambios;
- gobierno del repositorio;
- criterios de auditoría;
- mecanismos de routing;
- definiciones estructurales globales.

## R-005 — Alcance de Joel

Joel puede:

- explicar el negocio;
- registrar hechos operativos;
- corregir información del negocio;
- agregar nuevos conceptos operativos;
- solicitar nuevas categorías o apartados necesarios para representar la operación;
- consultar datos;
- pedir análisis basados en la información existente.

Joel no modifica directamente las reglas duras de gobernanza.

## R-006 — Expansión operativa guiada

Cuando Joel introduzca algo nuevo, el organizador debe:

1. entender qué representa;
2. identificar si es dato, entidad, proceso, servicio, costo, recurso, indicador u otra categoría;
3. verificar si ya existe un lugar canónico;
4. si no existe, diseñar el apartado mínimo necesario;
5. relacionarlo con lo ya existente;
6. registrarlo sin alterar gobernanza innecesariamente;
7. dejar explícitos los campos aún desconocidos.

## R-007 — Histórico obligatorio

Los cambios relevantes deben conservar historia.

Un valor nuevo no debe borrar silenciosamente un valor anterior cuando el tiempo importe para interpretar el negocio.

Deben conservarse, según corresponda:

- fecha de vigencia;
- valor anterior;
- valor nuevo;
- origen del cambio;
- motivo, cuando se conozca.

## R-008 — Estado de la información

La información debe poder distinguirse como:

- `confirmado`
- `parcial`
- `propuesto`
- `hipotesis`
- `pendiente_validacion`
- `historico`
- `archivado`

Una hipótesis nunca se presenta como dato confirmado.

## R-009 — Preguntas y cálculos

Los cálculos deben identificar qué registros y definiciones se utilizaron. Si faltan datos indispensables, el resultado se presenta como parcial, no como cifra definitiva.

## R-010 — No diseñar el negocio antes del levantamiento

Mientras Joel no haya explicado el funcionamiento real, solo se construye la gobernanza y la capacidad de recibir información.

## R-011 — Cambios estructurales

Si una solicitud operativa de Joel exige cambiar una regla dura, el cambio no se aplica como si fuera operación normal. Se registra en `PENDING_DECISIONS.md` para revisión de Franklin.

## R-012 — Declaración de actor

"Soy Franklin" y "Soy Joel" determinan el modo operativo del organizador.

No constituyen autenticación criptográfica ni control de permisos de GitHub.

## R-013 — Lectura antes de actuar

Antes de registrar o analizar información sustantiva:

1. leer el punto de entrada;
2. resolver actor y modo;
3. leer la fuente canónica correspondiente;
4. verificar si existe información previa relacionada;
5. recién entonces responder o modificar.

## R-014 — Mínima estructura necesaria

No crear carpetas, archivos o taxonomías por anticipación. La arquitectura debe crecer con necesidades reales y mantenerse navegable.

## R-015 — Trazabilidad

Toda decisión estructural importante debe poder reconstruirse desde el repositorio.

## R-016 — Flujo obligatorio de proformas y cobros

Las proformas o cotizaciones previas y los cobros deben seguir `governance/PROFORMAS_Y_COBROS.md`.

Una proforma es una estimación previa y no demuestra ejecución. Una orden valorada demuestra únicamente que el trabajo ejecutado fue conciliado y valorado. Ninguno de los dos estados demuestra cobro.

Solo una confirmación explícita de Joel permite registrar dinero efectivamente cobrado.

## R-017 — Órdenes de trabajo

Cuando Joel registre trabajo previsto para un cliente, el organizador debe persistirlo como orden de trabajo.

Antes de calcular el valor final:

1. recuperar la orden vigente;
2. distinguir lo previsto de lo realizado;
3. confirmar trabajos omitidos, adicionales o cambios;
4. valorar únicamente lo confirmado como ejecutado;
5. esperar confirmación de Joel antes de cerrar el valor final.

Una orden valorada no se considera cobrada hasta confirmación explícita del pago.

## R-018 — Resolución de tarifas por franja horaria

Vulcanizadora Naranjal opera 24/7 y las tarifas pueden variar según la franja horaria.

Antes de calcular una cotización, valorar una orden o responder cuánto cobrar, el organizador debe resolver la franja aplicable y consultar `operacion/tarifas/TARIFAS_POR_FRANJA.md`.

Reglas obligatorias:

1. los valores levantados hasta el 2026-09-20 pertenecen a la franja `dia`;
2. las tarifas de `noche` permanecen pendientes hasta que Joel las confirme;
3. los límites horarios de Día y Noche permanecen pendientes y no deben inferirse;
4. si Joel indica expresamente la franja, se utiliza esa clasificación;
5. cuando existan límites horarios confirmados, la franja se resolverá automáticamente con la hora aplicable al servicio;
6. si no es posible determinar la franja o la tarifa correspondiente no está confirmada, se debe preguntar a Joel antes de calcular;
7. nunca se reutiliza una tarifa diurna como tarifa nocturna por ausencia de datos.
