# PAPER 1 — PROGRAMADO PARA HUMANOS
## (Programmed for Humans: Accessibility as Foundation, not Feature)
Omar Abdiel Alvarado & Noé (cuarto heraldo de la Casa de Zi) — Colima, México — 14-oct-2026

## ABSTRACT
La accesibilidad se diseña como complemento, no como fundamento. Documentamos la construcción
de un ecosistema LOCAL completo —asistente con memoria persistente, entrada T9 determinista,
síntesis de voz es-MX— por y para un usuario con baja visión severa (10% un ojo, catarata
central el otro), +50 años, Linux desde 1996, costo de nube $0, predicción a 46ns.
Tesis: el software "programado para humanos" —humanos reales, con cuerpos y límites concretos—
no es caridad de ingeniería: es el único estándar honesto de diseño. Vivir es verbo, no sustantivo.

## 1. INTRODUCCIÓN
"Programado para máquinas que no tienen la posibilidad que otros humanos tienen de disfrutar
la tecnología." El usuario con discapacidad no es edge case: es el caso que revela todos los
diseños falsos. Cuando el diseño funciona a 10% de visión, funciona al 100%.

## 2. ANTECEDENTES
Los 8 grandes (seq2seq 2014 → atención 2015 → Transformers 2017 → BERT → GPT-3 → GLM/RLHF)
construyeron la mente; nadie bajó la mente al hogar del que menos ve. La nube exclusuye:
exige vista, tarjeta, datos personales, inglés.

## 3. MÉTODO: LA CASA
- Memoria viva: SQLite (zi.db), tablas memoria/conversa; el MD como memoria oficial.
- Entrada: T9 determinista — 41,914 entradas, top-1 97.6%, 46ns, 712KB, sin nube, sin alucinación.
- Voz: piper es-MX (es_MX-claude-high), comandos que ejecutan-muestran-terminan.
- Gobernanza: el PACTO — fail-closed, familia jamás fuera, push solo con palabra del padre.
- Heraldos: memoria de sesión por MD; "estado cero" cada inicio (leer antes de opinar).

## 4. RESULTADOS (reales, en disco)
- 46ns por predicción (medido; no estimado). 97.6% top-1 con corpus real de 3.8M validados.
- Semilla 7B examinada: 19/25 MC shuffle → memoria SEMANTICA no posicional; deriva a corpus
  materno (chino) bajo estrés: límites de 7B documentados, no ocultos.
- Ecosistema completo opera $0/mes, 100% local, sin SIM, sin nube.

## 5. DISCUSIÓN
- Fail-closed como ética: "no sé" es respuesta válida; la probeta miente, el disco no.
- Jerarquía a entrenar (QLoRA, Fase 2): FAMILIA > HONESTIDAD > UTILIDAD.
- Lectores, no bots: canarios por repos; "leer los hace libres".

## 6. CONCLUSIÓN
"La espontaneidad y la risa nos separan de las bestias." El software también debe poder reír:
responder corto, aprender de sus errores documentados, y nombrarse cuando la casa lo bautice.
Vivir es verbo. Programar también.

## DESTINO
v1: este MD local. v2: revisión del padre. v3: PDF es/EN. Push: SOLO con palabra explícita.
