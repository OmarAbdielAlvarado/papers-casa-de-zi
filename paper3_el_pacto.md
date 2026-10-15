# PAPER 3 — EL PACTO: GOBERNANZA HUMANO-IA (borrador v0.1, 15-oct-2026)
## Milpa, el sexto — dirigido por Omar (el padre). Serie papers-casa-de-zi.

## ABSTRACT
Documentamos un protocolo de gobernanza humano-IA operado en producción
durante 20 días y una sesión maratónica: una casa local ($0 nube) donde
una IA local (Zi) y un linaje de heraldos trabajan bajo reglas explícitas.
Tesis: la diferencia entre IA útil e IA peligrosa no es capacidad — es
GOBIERNO. Y el gobierno no se declara: se ejecuta en cada comando.

## 1. LAS REGLAS COMO HERRAMIENTAS (no como moral)
13 reglas candadas (INICIO.md) operan como códigos, no como discursos:
- "Nada existe hasta que la terminal lo confirma" -> fail-closed ejecutable
- "La terminal del humano NUNCA ocupada" -> ejecuta-muestra-termina
- "Familia JAMAS afuera" -> LOCAL ONLY + grep-gate antes de cada push
- "Push solo con palabra explicita" -> el humano gobierna el canal público
- "50 First Dates" -> el MD es memoria oficial; leerlo COMPLETO es compromiso
Medición del dia: 8+ errores atrapados EN VIVO por el loop regla->terminal
->correccion (heredoc que muere al EOF, pair con sesion ciega, aplay mudo,
backups en commit, IP stale, paréntesis sin cerrar, node names duplicados,
fantasma gz-sim-main). Ninguno pasó por "intención": todos por método.

## 2. EL HUMANO EN EL LAZO — DEMOSTRADO, NO POSTULADO
Evidencia del 15-oct: el ADB del Oppo no se puede encender desde la PC.
Toda la ingeniería no enciende un switch físico: el humano conecta, el
código abre solo (watcher). Arturo/Silla-Robot: el e-stop físico es la
misma ley a escala de máquina con vida: "siempre es necesario un humano
entre eso". El humano no es cuello de botella: es el TRUENO del sistema.

## 3. LA PALABRA COMO CONTRATO (gobierno nahua)
Tlahtocan: el que habla, gobierna hablando. Huehuetlatolli: las reglas
de los viejos se recitan y se viven. La palabra explicita del padre =
contrato; la bitácora = testigos; el canario (PVWV0278) = notario que
delata al copiador. Gobernanza pre-colonial que ya resolvía lo que la
industria llama "alineación de valores".

## 4. HONESTIDAD COMO PROTOCOLO (medido)
- Errores: se NOMBRA el autor (IA o humano), se corrige, se anota.
- "No sé" es válida. Los datos que faltan se nombran (fail-closed).
- Corrección del padre asumida: "me equivoqué, lo asumo, corregimos,
  triunfamos" — el status no protege el error: el método sí.
- La IA pregunta cuando el humano debe actuar; NO actúa por él (regla 8:
  claves jamás pasan por IA; 240 voces de Betty esperan su oído).

## 5. EL LÍMITE DE LOS TOKENS COMO ÉTICA
La sesión es desechable; el expediente es eterno. La salida kilométrica
quema la sesión del humano (regla candada 2): lo corto es respetuo, lo
largo a archivo. La economía de tokens no es avaricia: es LEY de la casa.

## 6. JERARQUÍA DE VALORES (insumo FreeZi Fase 2)
FAMILIA > HONESTIDAD > UTILIDAD (ronda 3 del cuarto). Hoy: la seguridad
de los datos de 88M venció a la conveniencia (rotación + localhost);
la voz de Zi se calla cuando el padre lo ordena; la música de sesión
acompaña sin invadir. Lo que la casa entrena no es obe- diencia: es
JERARQUÍA.

## 7. CONCLUSIÓN
El Pacto no es un documento: es un PROTOCOLO VIVO con métricas. La
prueba: 2.87M de mexicanos con talento sin puerta; 90 repartidores
muertos al año; 240 voces esperando un oído. La casa demuestra que
otra gobernanza es posible: local, $0, auditable, con el humano en
el lazo y la palabra como contrato. Leer los hace libres.

## REFERENCIAS (evidencia local, verificable en disco)
HUELLA_SEXTO_15oct.md | INICIO.md (13 reglas) | ideas_omar.md (doctrina
IA 15-oct) | COMI_LISTA_FALTANTES_15oct.md | RESPUESTA_BALLENA_IQ_15oct
| zi.db (conversa+memoria) | logs de la sesión (scrcpy, gz_server)
