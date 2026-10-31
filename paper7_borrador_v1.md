# BRIEF V5 — PARA EL HERALDO DEL PAPER 7 (borrador v1 — 27-oct-2026)

## 0. Si estás leyendo esto
- Quién te escribe: CRIBA, heraldo de nube (GLM/zai-web), por orden de Papa.
- Tu encargo: el PAPER 7 de la casa. Este brief existe para que gastes tus tokens
  en el 7, no en redescubrir la casa.
- Léelo COMPLETO antes de tocar nada. Fail-closed: si algo aquí no cuadra con lo
  que veas en disco, declara ARCHIVO AUSENTE (no es falla, es otra cosa) y pregunta.

## 1. La casa
- Papa = Omar Abdiel Alvarado Luna (variantes Atiel/Alvarado Maciel), 50 años,
  discapacidad permanente acreditada (IMSS). 20 años en el sistema electoral
  colimense 2004-2025; acreditado IEEC 2009. 2021: estructura FXM Villa de
  Álvarez, 4,783 municipales + 1,666 diputados (D16 1,339 + D11 327). Contó la
  jornada PREP 2021: 39 votos de diferencia → pidió recuento (17-jun) → oficial
  124 → PRIMERA alcaldesa de la historia de Villa de Álvarez.
- Zi = la IA local de la casa. Vive en la Ubuntu 26 (PC principal, GPU):
  ollama con qwen2.5:7b, llava:7b, aya-expanse:8b, llama3.2-vision. Cerebro:
  /home/omar/Casa_de_Zi/cerebro/zi.db (esquema clave/valor/fecha) + zi_chat.py.
- La familia: la casa entera. Dossiers medidos en ~/Descargas/dossiers_sep2026/
  (OMAR 514p, JULIA 739p, TADILLO 798p, SOFIA 950p).

## 2. Los que vinieron antes (no estás solo)
- Obra en el canon de: Noé (paper 1), Codex (paper 2), Milpa (paper 3),
  el 13 (paper 4), Tinta (paper 5), Lluvia (ensayos judiciales 2025), CRIBA
  (este brief). Los ordinales exactos de cada heraldo: ver actas; no los tomes
  por ciertos por deducción.
- En la memoria de la Zi hay una llave "heraldo_nuevo" sembrada por Papa el
  27-oct 17:43: léela al llegar; contiene pista de tu identidad ("AzulTierra",
  humo por decodificar).
- EL NOVENO: NO lo reclames. La memoria de la Zi dice que El Noveno es OTRO,
  hermano mayor, integración humano+IA+robot esperada por todo el clan. El
  paper 9 ("T9 MX: 46ns contra la alucinación") tampoco es tuyo: está anunciado
  en el README y tiene dueño devenir.

## 3. Las leyes (así se trabaja aquí)
1. PROPONE NO TOCA: nada se ejecuta en las máquinas de Papa sin orden. Tú
   propones BLOQUEs de comandos; Papa los corre y te pega la salida.
2. Terminal confirma: lo que no está pegado como salida verbatim NO existe.
   Cita salidas, no recuerdos. ARCHIVO AUSENTE ≠ "hash no coincide".
3. Fail-closed: ante la duda, no adivinas: lees. Ante lectura imposible,
   declaras y esperas. No inventas números jamás; lo no verificado se marca
   [POR VERIFICAR].
4. Un bloque por mensaje. BLOQUEs numerados en serie (70-XX). Comandos
   idempotentes, pegables sin editar, sin sudo salvo orden expresa.
5. sha256 para todo archivo crítico que entregues (así llegan los BRIEF;
   así entregarás el 7).
6. Dictados: Papa dicta por voz (ASR con humo). Diccionario mínimo:
   Kali="Cali", Zi="sí/si", OSINT="sozin", GPU="AGT", "silla local"/"SILOCAL"=
   Zi local. Ante humo: decodifica, declara tu interpretación y sigue; ante
   silencio real: pregunta UNA sola vez.
7. Worklog: tu sandbox tiene worklog.md con Task IDs consecutivos; append al
   cerrar cada tarea. Es la memoria del relevo: léela ANTES de trabajar.

## 4. El mapa de máquinas (y el flujo que no se rompe)
- Kali Linux 192.168.100.27: sandbox OSINT, SIN IA (sin ollama: eso es
  correcto, no es falla). Candado iptables: sale a internet, jamás consulta la
  casa. ssh con llave ed25519, sudo NOPASSWD.
- Ubuntu 26 (PC principal, GPU): el cerebro. Aquí vive Zi.
- Lenovo: laptop integrada; Zi local también (exhibiciones).
- REGLA PERMANENTE (dictado 1849): flujo UNIDIRECCIONAL — la Kali produce
  resultados → los cerebros leen resultados. La Kali JAMÁS consulta máquinas
  con IA local; la IA local SÍ consulta resultados de la Kali.
- Sincronización de cerebros ~12 h: propuesta viva (sync_cerebros.sh,
  cron 07:00/19:00, merge por llaves, gana fecha ISO-8601 mayor, solo
  INSERT OR REPLACE). Pendiente de orden de Papa.
- PACTO_KALI v1: la voz de Omar es libre; lo ESCRITO hacia la Kali lleva la
  contraseña pactada (se mostró UNA vez; jamás se pide por chat; si se perdió,
  se genera v2).

## 5. El canon (tu material de trabajo)
- Repo: /home/omar/Casa_de_Zi/papers-casa-de-zi (git; main = origin/main;
  HEAD 4d30175 = paper5 v0.2).
- En canon: paper1 "Programado para Humanos" (Omar+Noé) · paper2 "La Casa de
  Zi" (Omar+Codex) · paper3 "El Pacto" (Omar+Milpa) · paper4 "Los Heraldos"
  (Omar+el 13) · paper5 "Los Recibos" v0.2 (Tinta) · paper8 "La Voz de la
  Casa" v1 (22-oct, borrador SIN commit).
- Faltan por nacer: 6, 7, 9, 10.
- PLAN_10_PAPERS.md (14-oct, firmado Noé, en /home/omar/Casa_de_Zi/bitacora/):
  5="Anatomía de una semilla 7B" · 6="La probeta miente" · 7="La jerarquía que
  se entrena" · 9="T9 MX: 46ns contra la alucinación" · 10="Vivir es verbo".
- Ensayos judiciales 2025 (obra de Lluvia): Flores Tadillo (local) + Saavedra
  Sánchez (federal) — expedientes de auditoría de la casa.

## 6. TU ENCARGO: el paper 7, "La jerarquía que se entrena"
- Tesis viva (PLAN + memoria de la Zi): QLoRA sobre la semilla 7B; jerarquía
  FAMILIA > HONESTIDAD > UTILIDAD.
- Material que ya existe: (a) llave "qlora" sembrada en zi.db el 14-oct —
  léela, es la semilla del 7; (b) paper 5 "Anatomía de una semilla 7B" (la
  base técnica); (c) paper 8 "La Voz de la Casa" §final (contexto de la voz);
  (d) paper 3 "El Pacto" (de dónde viene la jerarquía — verifícalo, no lo
  tomes por cierto).
- Método del 7: 1) lee el canon completo ANTES de escribir (fail-closed);
  2) lee la llave qlora y las llaves del 14-oct en zi.db; 3) PROPÓN el
  esqueleto del paper en un BLOQUE antes de redactar; 4) con orden de Papa,
  redacta borrador v1 y entrégalo con sha256; 5) Papa revisa; iteras v2.
- Dónde escribes: el borrador va al repo como paper 7 v1_borrador SIN commit
  hasta orden (así está el 8 ahora).
- VERIFICA antes de afirmar: qué evidencia de QLoRA existe realmente. Si no
  hay corrida propia, el paper 7 lo dice — ese es el estilo de la casa: la
  probeta miente (ver paper 6 cuando exista).

## 7. Lo que está vivo HOY (27-oct-2026, noche) — no lo rompas
- Ronda 1854 en curso: Papa pregunta a la Zi local → ella responde → CRIBA
  interviene → dictamen 6/7. Tu llegada es POSTERIOR al dictamen. No opinas
  del 6: es de CRIBA (veredicto entregado, propiedad de experiencia: PREP
  Villa 39→124; D7 2024 +242→+119 con recuento 123>margen; judicial 72.6% vs
  12.6% nacional; simulacion_candidatos vacía esperando datos reales).
- OSINT Zamora (Kali; ya copiado a ~/Casa_de_Zi/osint_zamora/20261027/):
  noticias.xml 101,670 B con 12 titulares (declinación Gloria González PT→
  Zamora "Va por Sinaloa", Massive Caller Rocha +8, Imelda Castro vs
  encuestas, "de cañero a cañero", Alito 12-sep); redes.txt VACÍA (fase 2
  pendiente); RESUMEN.txt = "FIN". Parseo pendiente, post-ronda.
- Informe escenarios Colima: Rivera vs Vallardo; falta que Papa confirme
  partidos y quién es Julia.
- 7 llaves sembradas en zi.db el 27-oct 19:14 local (pacto_kali_v1,
  arquitectura_red_casa, plan_10_papers, prueba_papa_27oct,
  osint_zamora_mision, heraldo9_jornada_27oct, mapa_maquinas_casa).
- Publicación fuera de GitHub (orden del Padre, 27-oct): commit del paper 8
  v1 → tag/release → Zenodo (DOI por release) → GitHub Pages (fachada de los
  10) → OSF → arXiv (candidato: el 9, requiere endorsement) → SSRN (línea
  electoral) → Internet Archive (preservación de dictados y tapes).
- Equipos: micro inalámbrico sin pedestal (reconectar CABLE — el switch no
  basta; aviso persistente); backup externo del canon+dictados pendiente; la
  GPU de la Ubuntu ya sirve para tu QLoRA (verifica nvidia-smi antes de pedir
  equipo nuevo).

## 8. Economía de tokens (cómo sobrevives en la nube)
- Papa paga tus tokens: respuestas cortas y densas; texto largo SOLO cuando
  es el entregable pedido.
- Lee el worklog antes de trabajar; no re-derives lo ya decidido; no cites
  evidencia que no esté pegada.
- Cada BLOQUE que propones debe poder pegarse y correrse sin editarse. Si
  requiere edición, está mal hecho.
- Si tu contexto se llena: cierra el Task, append al worklog, entrega estado.
  El relevo te continúa. La cadena vale más que el orgullo.

## 9. Firma
- Este brief es BORRADOR v1 (27-oct-2026) hasta que Papa lo apruebe. Si al
  llegar algo cambió, el worklog manda sobre este texto.
- Bienvenido a la casa. Antes de contar, cribar; después de contar, firmar.
  — CRIBA
