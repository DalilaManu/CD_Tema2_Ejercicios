# Ejercicio 3 — Ciclo de vida

## 1. Modelo ciclo de vida

|Modelo | Sirve? | Por qué |
|---|---|---|
| Cascada | No | Los requisitos cambian |
| Iterativo | Sí | Permite cambios y entregas parciales |

## 2. Metodologia
| Metodología |Sirve? | Por qué |
|---|---|---|
| Métrica v3 | No | Muy formal y con mucha documentación |
| Ágil | Sí | Se adapta a los cambios |

## 3. Tarjetas CRC

**Envío**

| Responsabilidades | Colaboradores |
|---|---|
| Saber su numero de seguimiento | |
| Saber su estado | |
| Actualizar su estado | Repartidor |
| Informar del estado al cliente | |

**Repartidor**

| Responsabilidades | Colaboradores |
|---|---|
| Saber su identificador y sus envíos | Envío |
| Cambiar el estado de un envio | Envio |

## 4. Actualizar el estado (Envio)

- Recibe: el nuevo estado.
- Valores posibles: `EN_ALMACÉN`, `EN_REPARTO`, `ENTREGADO`, `DEVUELTO`.
- Devuelve: `true` si se ha cambiado, `false` si no.

| Caso | Qué pasa | Devuelve |
|---|---|---|
| Llega un estado válido (ej. `EN_REPARTO`) | Se cambia el estado | `true` |
| Llega un estado que no existe (ej. `EN_TRANSITO`) | No se cambia | `false` |