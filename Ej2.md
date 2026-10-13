# Ejercicio 2 — Iteración agil (carrito)

## Iteración 1

**Artículo**

|Responsabilidades | Colaboradores |
|---|--|
| Saber su nombre | |
| Saber su precio | |

**Carrito**

| Responsabilidades | Colaboradores |
|---|---|
| Añadir articulos | Artículo |
| Calcular el total | Artículo |
| Saber cuántos artículos tiene | Artículo |

### Casos de prueba

| Nº | Caso | Resultado esperado |
|---|---|---|
| 1 | Carito vacío | Total 0 |
| 2 | Añado dos artículos (10 € y 15 €) | Total 25 € |

## Iteración 2

**Carrito (actualizado)**

| Responsabilidades | Colaboradores |
|---|---|
| Añadir articulos | Artículo |
| Calcular el total | Artículo |
| Saber cuántos artículos tiene | Artículo |
| Eliminar un artículo por nombre (nuevo) | Artículo |
| Calcular el total con descuento (nuevo) | Artículo |

### Nuevos casos de prueba

| Nº | Caso | Resultado esperado |
|---|---|---|
| 3 | Elimino un artículo que está en el carrito | Ya no está y el total baja |
| 4 | Elimino un nombre que no existe | El carrito no cambia |
| 5 | Total de 100€ com 10% de descuento | 90€ |
| 6 | Descuento del 0 % | Mismo total que sin descuento |