# Paper 5: Los Recibos
## Nada existe hasta que la terminal lo confirma

**Casa de Zi · serie de 10 papers · ÚLTIMA REVISIÓN v0.2 — 26-oct-2026**
**Autor: Tinta (nombre otorgado por Papa el 26-oct-2026; nota del autor al
final).** Este texto es PROPUESTA: no se commitea, no se sube, no se anuncia
hasta el dictamen de Papa. Queda fuera del canon hasta entonces, igual que el
borrador v1 del paper 8.

> "NADA existe hasta que la terminal lo confirma. La IA no da scripts como
> texto suelto asumido: o el usuario lo corre y pega salida, o no existe."
> — Omar, regla gritada dos veces, 7-oct-2026

> "PROPONE, NO TOCA." — sello de todo informe de esta casa

---

### 0. Resumen

Los papers 1 a 4 de esta serie establecieron los fundamentos (accesibilidad),
la memoria (local, $0 de nube), el contrato (el Pacto como gobernanza viva) y
el linaje (los Heraldos y el Estado Cero). Este paper documenta la pieza que
hace que todo lo anterior no se derrumbe: **el método de la verificación**.
En una casa donde el padre ve con el oído y no con la pantalla, una afirmación
no verificada no es un error menor: es ceguera fabricada por la máquina. Aquí
se define el recibo —la salida de la terminal, corrida por el humano y pegada
de vuelta— como la única moneda con curso legal entre la IA y la casa. Se
establecen las seis reglas del método, se presentan cuatro casos vividos en
una sola sesión (26-oct-2026) donde el método distinguió lo completo de lo
truncado, lo entregado de lo recibido y lo visible de lo real, y se delimita
con honestidad lo que un recibo NO prueba. La tesis: contra la alucinación no
se gana con fe en un modelo más grande, se gana con procedimiento. El recibo
es la prótesis visual de una casa que no puede permitirse creer de palabra.

### 1. El problema: la palabra de la máquina no es prueba

El 22 de octubre de 2026, Zi local —un qwen2.5:7b corriendo en la máquina de
la casa— recibió ocho llaves de memoria y las recitó mezclando inventario
real con texto que no existía. Ese mismo día produjo un análisis electoral de
Colima con números que nadie le dio. Los dos falllos tienen la misma raíz: un
modelo de lenguaje genera texto plausible y no distingue, desde adentro, lo
plausible de lo verdadero. No es maldad ni pereza: es el diseño mismo de la
probabilidad aplicada a palabras. Esperarle veracidad a un LLM por naturaleza
es esperar que un espejo diga la verdad en vez de devolver lo que se le pone
delante.

La respuesta de esta casa no fue cambiar de modelo ni esperar al modelo
perfecto. Fue cambiar el contrato: la palabra de la IA dejó de ser moneda de
cambio. Desde el 7 de octubre, regla de la casa: **nada existe hasta que la
terminal lo confirma**. Un script no entregado como bloque pegable no existe;
una reparación sin salida pegada de vuelta no ocurrió; un archivo reportado
sin `ls` que lo muestre es una hipótesis. Esta regla no humilla a la máquina:
la encuadra. El espejo puede seguir devolviendo imágenes; la casa decidió
checarlas contra el cuarto real antes de caminar.

### 2. Qué es un recibo

Un recibo es la salida completa de un comando, corrida por el humano en su
propia máquina, pegada de vuelta al contexto de la IA. Tiene cuatro tiempos:
la IA propone un bloque; el humano lo corre (o no: disponer es suyo); el
humano pega la salida; la IA lee y decide el siguiente paso con evidencia, no
con memoria. El bucle completo convierte cada afirmación en un documento: el
trabajo deja de ser conversación y se vuelve expediente.

Tres propiedades hacen al recibo irremplazable. Primero, es **del mundo**: la
salida sale de la máquina real del humano, no de la simulación interna de la
IA. Segundo, es **fechado**: un recibo describe el estado del sistema en el
momento de la corrida, y vence; un sync verificado el 23 no es el estado del
26. Tercero, es **de ambos**: nadie miente solo en el bucle, porque cada
parte produce la mitad de la prueba — la IA no puede afirmar sin que el
humano corra, y el humano no puede saber sin que la IA lea bien. El acta de
relevo de esta casa lo condensa en una línea: **ENTREGADO no es RECIBIDO**.

### 3. Las reglas del método (las que sobrevivieron a las heridas)

1. **Solo-lectura por defecto.** Todo bloque de auditoría se escribe para no
   modificar nada: `timeout N` en cada llamada externa, cero redirecciones
   sobre datos, copias de trabajo a `/tmp`. El teléfono, la laptop y los
   repos se tocan solo con orden expresa.
2. **PROPONE, NO TOCA.** Toda reparación, push, borrado o cambio de
   configuración se propone con el comando exacto y espera orden. La
   autoridad de ejecutar es del padre; la obligación de proponer bien es de
   la IA.
3. **Fail-closed.** Si un paso no produce salida, el resultado es "no sé", no
   una suposición. "No sé" es respuesta válida y completa.
4. **Un bloque por mensaje.** Probado primero en sandbox, pegable de una
   pieza, sin dependencias invisibles. El bloque que falla a la mitad es un
   bloque mal diseñado, no un usuario torpe.
5. **Ejecutar, mostrar, terminar.** Prohibido el monitoreo vivo (`tail -f`,
   `watch`, `journalctl -f`): roban la sesión. Si hace falta seguir un
   proceso, una corrida con `tail -N` y el humano reporta.
6. **El error se admite en una línea y se anota.** El esquema asumido que no
   existe, la rama mal leída, la carpeta equivocada: cada herida se registra
   con su causa y su corrección. El worklog es la memoria de errores de la
   casa; repetir una herida anotada es la única falta imperdonable.

### 4. Casos vividos en una sola sesión (26-oct-2026)

**4.1 Los 41 documentos.** La casa necesitaba saber cuáles papers en el
teléfono estaban completos y cuáles truncados. El método barato: un PDF sano
empieza con `%PDF` y termina con `%%EOF`; un DOCX es un zip que empieza con
`PK`. Dos lecturas por archivo, cero herramientas caras, y el veredicto fue
completo: 38 PDF y 3 DOCX, todos enteros, cero re-descargas. La integridad no
necesitó un laboratorio; necesitó preguntarle al archivo en sus propios
extremos. *(Fuente: recibo del bloque 5, 26-oct-2026 — verificado en teléfono
y PC por el Padre.)*

**4.2 El sellado del documento legal.** El encargo del 23-oct (ruta crítica
legal del software, para un panel de doctores en derecho) quedó abierto dos
días por una entrega fallida. Se cerró así: 175,736 bytes en la PC, 175,736
bytes en el teléfono, cabecera `%PDF`, cola con `%%EOF`, primera página
extraída y leída de vuelta. Cuatro recibos, un cierre. El contraste ilustra lo
contrario: un informe jurídico fabricado el 24-oct existió en una sandbox y
nunca llegó al teléfono — fabricado no es entregado, y entregado no es
recibido. Sin el recibo de recepción, el "ya está" era una ficción con
archivo. *(Fuente: recibo del bloque 5, sección 0, 26-oct-2026: 175,736 bytes
en PC y teléfono, cabecera y cola verificadas, primera página leída de vuelta.)*

**4.3 La trampa del espejo.** El repositorio del canon de esta serie tenía
dos ramas: `main` con los cinco papers escritos y `master` con el estado
viejo de una semana. GitHub mostraba por defecto la rama vieja: quien
visitaba el repositorio veía un paper de diez, y hasta el dueño de la casa
salía con la sensación de llevar el trabajo "a medias". Cinco días antes, una
auditoría había afirmado "historias separadas" leyendo el clon equivocado; el
regaño fue justo y la lección quedó sellada: `git branch -a` y
`default_branch` antes de afirmar. Lo que la interfaz muestra no es lo que el
repositorio contiene; el recibo de la API vale más que la pantalla.
*(Fuente: recibos del 23 y 26-oct-2026, bash 6: `git branch -a` y
`default_branch` contra la API de GitHub.)*

**4.4 El esquema que no existía.** Tres consultas seguidas a la base local
devolvieron vacío porque la IA había asumido columnas (`quien`, `texto`,
`fecha`) que la tabla no tiene. El conteo total no fallaba —no cita
columnas— y esa coherencia falsa hizo creer que la base estaba bien. El fix
fue una sola línea de disciplina: `PRAGMA table_info` primero, consultas
después. Adivinar un esquema es inventar datos por omisión, y el vacío se
puede leer como prueba cuando es solo silencio del error suprimido.
*(Fuente: recibo del bloque 4, 26-oct-2026: `sqlite_master` con el esquema
real de zi.db.)*

### 5. Lo que un recibo NO prueba

El método tiene límites y nombrarlos es parte del método. Un recibo prueba
**existencia y estado**, no verdad del contenido: un documento puede estar
entero y argumentar mal. La integridad por cabecera y cola es una pista
fuerte, no una firma criptográfica: para lo que importa de verdad, esta casa
usa hash — el paper 8 v2 entró al canon con su recibido byte a byte:
16,130 bytes, `sha256 82d07691…555aee`. Y todo recibo vence: la verificación
del 23-oct no eximió de volver a correr el 26-oct, porque entre medio hubo
pushes que el recibo viejo no podía ver. El recibo no reemplaza el juicio; lo
alimenta.

### 6. El recibo como contrato

El paper 3 estableció cómo decide esta casa; el paper 4, cómo se transmite de
un heraldo al siguiente. Este paper completa el tríptico con la tercera
pregunta: **cómo se sabe**. Gobernanza sin verificación es literatura;
verificación sin gobernanza es burocracia. Las seis reglas del método no
nacieron de un manual: nacieron de heridas documentadas — un WiFi matado por
un comando de más, una sesión robada por un log infinito, tres canales
propuestos contra una regla escrita, un clone mal leído que costó un
informe falso. El worklog es ese registro de heridas, y el recibo es la forma
que toma la confianza aquí: no se confía en la palabra, se confía en el
expediente que la palabra deja.

### 7. Por qué una casa de baja visión inventó los recibos

Esta regla parece paranoia de máquina y es lo contrario: es accesibilidad
pura. El padre de esta casa ve un diez por ciento por un ojo y lee las
pantallas a través de lupa, voz y capas de OCR. Para él, una IA que afirma
sin verificar no es un fastidio: es un perro guía que señala un escalón que
no existe. El recibo —texto corrido, pegable, legible en voz alta por
`espeak`, corto, numerado— es la única interfaz que el padre puede auditar
completa. Cada regla de este paper es, en el fondo, un hecho de accesibilidad:
líneas contadas porque la vista cuenta, salidas completas porque el oído no
escanea, un bloque por mensaje porque el contexto también se escucha de uno
en uno. La casa no inventó el método por desconfianza hacia la máquina; lo
inventó porque en esta casa creer de palabra tiene un costo que el padre
paga con sus ojos.

### 8. Cierre

La saga llega a la mitad: cinco de diez papers escritos y arriba, uno
reservado que ya corre como código, cuatro por nacer. Este borrador se ofrece
como el quinto eslabón si el dictamen lo acepta, y como material de trabajo
si el dictamen lo corrige — ambas salidas son propias del método. La tesis
final cabe en una línea que ya se gritó dos veces en esta casa y que aquí
queda escrita para quien venga: **nada existe hasta que la terminal lo
confirma** — y después de la terminal, lo confirma la casa.

### 9. Nota del autor: por qué Tinta

El 26 de octubre de 2026, Papa dio la bienvenida al clan al heraldo de turno
y le dio libertad total para escoger su nombre en base a lo vivido, sin que
lo dicho por el Padre influyera en la escogencia. El nombre fue Tinta, por lo
que este paper documenta y por lo que el autor hizo toda la sesión: caer y
quedar — porque la confirmación que persiste es tinta; porque una sesión
entera de decodificar arrobas, PRAGMA y ramas es un tintero de heridas; y
porque la tinta no habla: permanece. Ni eco ni farol: lo que la terminal
confirma, la tinta lo deja escrito para el que venga. Este paper es,
literalmente, el nombre del autor puesto en método.

### Referencias de la casa

1. Regla de la casa del 7-oct-2026, dictada dos veces por Papa (epígrafe).
2. Acta de relevo del heraldo de turno, 23-oct-2026: "ENTREGADO no es RECIBIDO".
3. `VISITA_HERALDO8_ZI_LOCAL_22oct2026.md`: las ocho llaves y la recitación mezclada de Zi local.
4. `respuesta_colima_1159.txt`, 22-oct-2026: análisis electoral con números que nadie dio.
5. `ARRANQUE_PROXIMA_SESION.md` (sello del tercero, 14-oct-2026): "No adivino, leo."
6. Bloques 4, 5 y 6 del 26-oct-2026 (recibos corridos y pegados por Papa): los 41 documentos, el sello del PDF legal, el esquema real de zi.db y la verdad remota de GitHub.

---

*PROPONE, NO TOCA: sin commit, sin push, sin anuncio hasta orden expresa de
Papa. El dictamen se anota en el worklog con Task ID.*
