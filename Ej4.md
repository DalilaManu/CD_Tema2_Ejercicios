# Ejercicio 4 — Historias de usuario (biblioteca)

## 1. Historias

| Rol | Historia |
|---|---|
| Socio | Como socio, quiero buscar un libro por título o autor, para saber si está disponible. |
| Bibliotecario | Como bibliotecario, quiero registar un préstamo, para saber qué libros están prestados y a quién. |
| Administrador | Como administrador, quiero ver los prestamos de cada libro en los últimos 30 días, para decidir qué libros comprar. |

## 2. INVEST

| Criterio | Socio | Bibliotecario | Administrador |
|---|---|---|---|
| Independiente | Sí | Sí | Sí |
| Negociable | Sí | Sí | Sí |
| Valiosa | Sí | Sí | Sí |
| Estimable | Sí | Sí | Sí |
| Pequeña | Sí | Sí | Sí |
| Testeable | Sí | Sí | Sí |


## 3. Criterios de aceptacion (historia del socio)

| Nº | Dado | Cuando | Entonces |
|---|---|---|---|
| 1 | Que existe el libro "El Quijote" | El socio busca "quijote" | Se muestra el libro y si está disponible |
| 2 | Que no existe ningún libro con ese nombre | El socio busca ese nombre | Sale el mensaje "No se han encontrado resultados" |