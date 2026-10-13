# Ejercicio 5 — Product Backlog con Scrum (EduPro)

## 1. Roles

| Rol |Quién |
|---|--|
| Product Owner | Luis (director del centro), porque decide que es más importante para los centros |
| Scrum Master | Alguien del equipo de Tech4Learning que no se nombra |
| Development Team| El equipo de desarrolladores de Tech4Learning |
| Stakeholder | Marta (profesora) da ideas pero no decide la prioridad |

## 2. Historias y criterios de aceptación

| ID | Historia |
|---|---|
| H1 | Como profesor, quiero subir PDF, vídeos y enlaces, para dar material a mis alumnos. |
| H2 | Como alumno, quiero acceder al material desde cualquier dispositivo, para estudiar desde el ordenador o el móvil. |
| H3 | Como profesor, quiero organizar el material por temas o semanas, para que sea fácil de encontrar. |
| H4 | Como profesor, quiero programar exámenes con preguntas de opción múltiple y abiertas, para evaluar online. |
| H5 | Como profesor, quiero que las preguntas de opción múltiple se corrijan solas, para ahorrar tiempo. |
| H6 | Como alumno, quiero recibir una notificación cuando haya una actividad nueva, para enterarme enseguida. |

|Historia | Dado | Cuando | Entonces |
|---|---|---|---|
| H1 | Un PDF válido | El profesor pulsa "Subir" | El archivo queda disponible para los alumnos |
| H1 | Un archivo con formato no permitido | El profesor intenta subirlo | Sale un aviso y no se sube |
| H2 | Un alumno en un ordenador | Entra al material | Lo ve bien |
| H2 | Un alumno en el móvil | Entra al material | Se adapta a la pantalla |
| H3 | Un tema creado ("Semana 1") | El profesor sube material a ese tema | El material aparece dentro del tema |
| H3 | Un alumno mirando el material | Abre el listado | Lo ve agrupado por tema o semana |
| H4 | Un examen en creación | El profesor añade una pregunta de opción múltiple | Se guarda con su respuesta correcta |
| H4 | Un examen en creación | El profesor añade una pregunta abierta | Se guarda sin respuesta correcta |
| H5 | Un alumno que respondió el examen | Entrega el examen | Se calcula la nota de las de opción múltiple |
| H5 | Un examen con preguntas abiertas | Se corrige automáticamente | Las abiertas quedan pendientes para el profesor |
| H6 | Una actividad publicada | Se confirma la publicación | Los alumnos reciben una notificación |
| H6 | Un alumno con notificaciones desactivadas | Se publica una actividad | No recibe nada |

## 3. Estimación (Planning Poker)

Referencia: iniciar sesión = 5 puntos.

| Historia | Puntos | Comparación con iniciar sesión |
|---|---|---|
| H1 |8 | Más compleja: hay varios tipos de archivo y validaciones |
| H2 | 5 | Más sencilla: solo es adaptar el diseño |
| H3 | 3| Mas sencilla: es agrupar material que ya existe |
| H4 | 13 | Mucho más compleja: dos tipos de preguntas y programar fechas |
| H5 | 8 | Más compleja: hay que comparar respuestas y calcular la nota |
| H6 | 5 | Parecida: es un aviso que se puede hacer por separado |

## 4. Product Backlog

Criterio: valor de negocio para los centros y dependencias entre historias (H5 depende de H4).

| Orden | Historia | Puntos |Por qué |
|---|---|---|---|
| 1 | H1 — Subir material | 8 | Sin material la plataforma no sirve |
| 2 | H2 — Cualquier dispositivo | 3 | Los alumnos tienen que poder ver el material |
| 3 | H3 — Organizar por temas | 3 |Mejora H1 pero no es imprescindible |
| 4 | H4 — Programar examen | 13 | Luis dice que es fundamental |
| 5 | H5 — Corrección automática | 8 | Necesita que H4 ya esté hecha |
| 6 | H6 — Notificaciones | 5 | Es útil, pero la plataforma funciona sin ella |