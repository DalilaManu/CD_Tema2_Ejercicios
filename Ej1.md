#   Dalila Emanuele 
# Ejercicio 1 - Diseño con Tarjetas CRC

## Tarjetas CRC

**Libro**
| Responsabilidades | Colaboradores |
|---|---|
| Saber título, autor e ISBN | |
| Saber cuántos ejemplares hay disponibles | |
| Prestar un ejemplar | Préstamo |
| Recibir un ejemplar devuelto | Préstamo |

**Socio**
| Responsabilidades | Colaboradores |
|---|---|
| Saber nombre, número de socio y fecha de alta | |
| Pedir un libro prestado | Libro, Préstamo |
| Devolver un libro | Préstamo |

**Préstamo**

| Responsabilidades | Colaboradores |
|---|---|
| Saber qué libro y qué socio tiene | Libro, Socio |
| Saber la fecha de inicio | |
| Registrar la devolución | Libro |

## Qué pasa al prestar un ejemplar

Primero se mira si hay ejemplares disponibles (más de 0).

| Caso | Qué cambia | Resultado |
|---|---|---|
| Hay ejemplares | Los disponibles bajan en 1 y se crea el préstamo | Éxito |
| No hay ejemplares | No cambia nada | Falla |

## Flujo

| Paso | Qué pasa | Clase que actúa | Colaboradores | ¿Éxito? | Disponibles |
|---|---|---|---|---|---|
| 1 | Se da de alta el libro con 3 ejemplares | Libro | | Sí | 3 |
| 2 | Se dan de alta 2 socios | Socio | | Sí | 3 |
| 3 | El socio 1 toma el libro | Socio | Libro, Préstamo | Sí | 2 |
| 4 | El socio 2 intenta tomar el libro | Socio | Libro, Préstamo | Sí | 1 |
| 5 | El socio 1 lo devuelve | Socio | Préstamo, Libro | Sí | 2 |
| 6 | El socio 2 lo vuelve a intentar | Socio | Libro, Préstamo | Sí | 1 |
