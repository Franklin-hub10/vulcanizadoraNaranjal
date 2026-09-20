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

Toda solicitud relacionada con cuánto cobrar por un trabajo realizado, una proforma o un cobro debe seguir `governance/PROFORMAS_Y_COBROS.md`.

El orden obligatorio es:

1. **Aclarar:** si existe una duda material que pueda cambiar el cálculo, preguntar a Joel antes de cerrar la proforma.
2. **Confirmar proforma:** una proforma solo se persiste como realizada cuando Joel confirma que está correcta.
3. **Confirmar cobro:** una proforma solo pasa a cobro e indicadores cuando Joel confirma explícitamente que ya fue cobrada.

No se puede inferir un cobro a partir de una proforma confirmada.
