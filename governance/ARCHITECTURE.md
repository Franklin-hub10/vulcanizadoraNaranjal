# Arquitectura de conocimiento

## Propósito

Diseñar un repositorio que pueda crecer con el negocio sin convertir la gobernanza en una mezcla de datos, notas y reglas.

## Capas

### 1. Gobernanza

Ruta: `governance/`

Contiene reglas sobre cómo funciona el sistema documental.

No contiene ventas diarias, precios particulares ni operación corriente.

### 2. Sistema del organizador

Ruta: `system/`

Contiene mecanismos de routing, orden de lectura y resolución de contexto.

### 3. Conocimiento del negocio

Se creará tras el levantamiento con Joel.

Contendrá las fuentes canónicas de cómo funciona realmente la vulcanizadora.

No se fijan aún nombres definitivos de carpetas porque deben derivarse del negocio real.

### 4. Registros operativos

Se definirá después de saber qué necesita registrar Joel y con qué frecuencia.

### 5. Análisis e indicadores

Se definirá cuando existan datos y definiciones suficientes para evitar métricas ficticias.

### 6. Histórico

Ruta: `history/`

Conserva decisiones estructurales e hitos que deben poder reconstruirse.

## Principio de crecimiento

La arquitectura sigue este orden:

```
necesidad real
   ↓
explicación del negocio
   ↓
clasificación
   ↓
modelo mínimo
   ↓
fuente canónica
   ↓
relaciones
   ↓
uso operativo
```

No se crea primero una estructura compleja para después intentar obligar al negocio a entrar en ella.

## Navegación

Cada nueva área operativa deberá definir:

- propósito;
- fuente canónica;
- qué contiene;
- qué no contiene;
- relaciones;
- campos mínimos;
- reglas de actualización;
- tratamiento histórico.

## Evolución

Si la estructura deja de representar correctamente el negocio:

- Joel puede identificar la necesidad;
- el organizador puede ampliar la capa operativa;
- Franklin interviene cuando la solución exige cambiar gobernanza.
