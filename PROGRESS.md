# PROGRESS — Español de Eva (método de escucha e inmersión)

**Desde el 2026-10-17 (noche): piezas a demanda.** Ya no hay lección diaria. Eva pulsa ▶️ *Siguiente pieza*; el bot pide lotes de 4 (Bnnnn) cuando quedan menos de 3 listas. Plan completo hasta B2 (4.500 familias): `PLAN.md`. Etapa actual: **1 (Core)**. Aún no hay `vocab.json` ni línea de base de `/nivel`, así que la elección de palabras nuevas se apoya en `known.json` (estimación) y en `freq/families.json`.

**Desde el 2026-10-17 (decisión de Eva):** aprendizaje por escucha e inmersión, español de Cali. Cada lección gira en torno a un audio (pieza) con 1–3 elementos nuevos; el resto es material conocido. Sin tablas, sin reglas explícitas, sin puntuaciones: los errores se responden con un *recast*. Cada pieza se escucha unos tres días. Patrones por inferencia (4–6 frases que cambian en una sola cosa), sombra (*shadowing*) cada día, y una pregunta de Habla. La gramática B2/B1 y los libros de verbos quedan como referencia privada de José.

## Comprensión (tendencia)

| Fecha | Pieza | 1.ª escucha | Repetición | Nota |
|---|---|---|---|---|
| 2026-10-17 | P001 Me tocó madrugar | 70 % | (B0003) | Primera lección del método nuevo. Captó la idea general; se le escapó el detalle de *The West Wing*. Preguntó por *pagar el tinto*, *pereza*, *uno extraña*. Señaló con razón que Cali no tiene mar. |
| 2026-10-17 | P005 El capítulo del monorriel (B0001) | 90 % | (B0003) | Idea general correcta (Marge quiere reparar la calle; la ciudad compra el monorriel). Usó *pensar que* sin ayuda (P2: «Pienso que comprar un monorriel es una mala idea…») y aportó que el guion es de Conan O'Brien. Errores menores, con recast: *escritoro* → escritor, «la calle necesita reparar». |
| 2026-10-17 | P006 A Homer le toca (B0002) | 100 % («entendí todo») | (B0005) | Idea general «partial» en la E2 (captó que Homer es el conductor y que Marge encuentra a un hombre que ayuda; no mencionó qué piensa Marge de Lanley). En la H1 contó su travesía en Puerto Rico (Tres Palmas → Cabo Rojo, 15 h) y usó *encontré*, *estaba muy contenta pero muy cansada*, *dormí como un tronco* después de preguntar qué significa. |
| 2026-10-18 | P010 Diez kilómetros en el Sena (B0006) | 80 % | (B0010) | Idea general «partial» y luego «good» (el agua del Sena; ganó Sharon van Rouwendaal, Moesha a unos cinco segundos). Preguntó qué es *sigo* y lo usó enseguida: «Sigo entrenando en el gimnasio todos los días» (recast). |
| 2026-10-18 | P011 Dos horas de pelea (B0007) | — | (B0011) | No dio %: preguntó por *acordás* y *recuerdo*, y contó su travesía de Italia a Albania (35 h; comía cada hora; gelato, cree que de fresa). |
| 2026-10-18 | P012 Golpes en el agua (B0008) | 70 % | (B0012) | Idea general «good» (ir detrás no es trampa, es estrategia). Preguntó *golpes*, *engañar*, *vale la pena*; usó sola «El monorriel no valió la pena» y contó que en su travesía nadó sola, con muchas medusas. |
| 2026-10-18 | P013 ¿Valió la pena? (B0009) | 70 % | (B0013) | Idea general «poor»: no captó el nombre de Anne Hidalgo y entendió «limpió la cena». Pidió las transcripciones (Sena y Homer). Buena respuesta final: «valió la pena porque la gente puede nadar en verano… importante para la comunidad». |
| 2026-10-18 | P009 ¿Homer es un buen padre? (B0005) | 90 % | (B0009) | Idea general «partial»: captó que Homer no es un padre perfecto, los tres hijos y que «la vida con Homer nunca es tranquila»; la decisión imposible (*Los Simpson* o *The West Wing*) la contó en un segundo mensaje. Dijo sola «llevo toda la vida haciendo nadando» (recast: *llevo toda la vida nadando*): primer uso espontáneo de *llevar* + gerundio. B0003 y B0004 se cerraron sin respuestas (el bot las marcó como terminadas a las 06:25 y 06:40), así que no hay % de P007 ni P008. |

Calibración (desde el 2026-10-17, CAP-564): **siempre 5 palabras nuevas de la lista por pieza**. 1.ª escucha < 85 % → todo lo demás más fácil (más lento, tema más familiar, más reciclado); ~100 % → más largo, más rápido, habla más natural. Si baja de ~80 % dos veces seguidas, se mantienen las 5 y se simplifica lo demás (anotarlo aquí). Objetivo: 85–95 %.

## Decisiones de ritmo

- 2026-10-18 (mañana), CAP-569 — **más fácil, y canción + historia.** 1.ª escucha: 90 % (P009), 80 % (P010), **70 % (P012), 70 % (P013, idea general «poor»)**: dos veces por debajo de 80 % → se mantienen las 5 palabras y se simplifica lo demás. **B0011 y B0012 (sin empezar) reescritas**: P015 de ~225 a ~155 palabras, P016 de ~245 a ~175; frases más cortas, sin subtramas (fuera Ben, April, Tom y Jerry), menos palabras raras (*presión, documental, famoso, robar*). Mismas palabras nuevas. B0010 no se tocó (es `current`). En `to_learn` solo quedan *amenaza* e *involucrar* → no se puede hacer una pieza de 5: **B0013 = Canción** (Grupo Niche, «Cali pachanguero», presentada por Andrés en ~120 palabras conocidas) y **B0014 = Historia** («Eva y el mar», ~165 palabras, solo conocidas, sobre su travesía de Italia a Albania tal como la contó). **B0015–B0016 no se escriben** hasta que el selector traiga palabras (el bot se lo ofrece). Las narraciones nuevas llevan `B:` para que las lea Gonzalo. Arreglo en el bot: `request_rewrite_for_new_words` ya no pide reescribir canciones e historias por no tener `list_new` (copia: `jose_bot.py.bak-2026-10-18-before-cap569`). Si la 1.ª escucha vuelve a 85 % o más, se alargan otra vez los audios poco a poco.

- 2026-10-18 (mañana), CAP-566 — **lote B0009–B0012.** Últimas 1.as escuchas: 90 % (P005), 100 % (P006), 90 % (P009, idea general «partial»): dentro del objetivo, así que **no se reescribe nada** (B0006–B0008, aún sin empezar, ya tienen este nivel) y se mantiene el ritmo: 5 palabras de `to_learn` en orden, audios de ~200–245 palabras, frases cortas, la E2 apoyada en una palabra reciente sin glosa (B0009 *dirigir*, B0010 *atacar/ataque*, B0012 *maldito*). Palabras: enojar, pertenecer, doble, batalla, majestad · cuello, fijar, acaso, quieto, ocultar · encerrar, obviamente, vacío, perseguir, grabar · faltar, escoger, cuchillo, robo, líder. Quedan en `to_learn`: amenaza, involucrar (si no llegan más del selector, la próxima pieza tendrá solo 2 nuevas, o el bot le ofrece el selector). Se cierra el arco 2 (Sena) y empieza el arco 3 (*Parks and Rec*, «Harvest Festival»). Se evitaron palabras fuera de la lista que no son transparentes (*maíz, alcalde, temporada, esquina, alegría, siguiente, gastar*). Si P013 o P014 bajan de 85 %, la pieza siguiente se acorta (~150 palabras) y se recicla más. **Aviso técnico:** el bot asocia *robo* a la familia *robar* (y *juego* → *jugar*, *limpiar* → *limpio*), así que *robo* puede no marcarse como cubierta aunque salga en dos piezas; revisar `to_top` en el bot.

- 2026-10-18 (mañana), CAP-565 — **palabras del selector.** Eva marcó en el selector de palabras cuáles ya conoce; ahora las 5 nuevas de cada pieza salen **solo de `to_learn`, en su orden** (37 palabras: tratar, maldito, aquel, sitio, daño, caja, dirigir…). Todas las palabras nuevas de B0005–B0008 (dios, vida… alguien, nadie…) las marcó como conocidas. **B0005 se dejó como estaba:** ya estaba en curso (`current`) cuando se reescribía. **B0006–B0008 reescritas** con las 15 siguientes, en orden: tratar, maldito, aquel, sitio, daño · caja, dirigir, droga, pelear, ataque · cubrir, quemar, espalda, engañar, golpe. Se mantiene el arco 2 (Sena), con otro reparto: P010 el agua y quién ganó · P011 el relato de la carrera · P012 cómo es nadar en grupo (golpes, ir detrás). El «¿valió la pena?» pasa a P013 (B0009) con *enojar, pertenecer, doble, batalla, majestad* (borrador en `pieces/borradores/`). Cada pieza recicla de `heard_not_yet_shown` (televisión, contaminar, kilómetro, entrenar…) y el resto son palabras que ya conoce; se quitaron *lluvia, agosto, puente, italiano, cien, euro, caro, entero, veinte* para no pasar de 5 nuevas. Con 90–100 % en la 1.ª escucha, los audios se alargan un poco (P010 ≈190 palabras, P011 ≈215, P012 ≈140). Copia de las versiones anteriores: `~/.config/jose` → carpeta de trabajo de CAP-565 (`bak-cap565`).
- 2026-10-17 (noche), CAP-564 — **5 palabras nuevas por pieza** (decisión de Eva) y las repeticiones dentro de las piezas nuevas. Eva terminó B0001 (90 %) y B0002 (100 %), así que se reescribieron **las seis piezas en cola, B0003–B0008**, antes de que empezara ninguna. Palabras en orden de rango de `next_new` (saltando las que ya domina: qué, del, al, ya, algo, cómo, otro, gracias, cosa, hola, quién, mejor, dónde, oh, favor, trabajo): nuestro, mirar, volver, parecer, llamar · alguno, mismo, nuevo, hasta, acuerdo · dios, vida, hijo, padre, tomar · seguir, hecho, seguro, sobre, lugar · momento, buscar, escuchar, tal, tipo · alguien, nadie, valer, dinero, mundo. **Se dejaron para un arco donde encajen:** *matar* (128) y *morir* (149) (*The Walking Dead* / *Game of Thrones*). Se quitaron *carrera* y *contra* de las piezas del Sena para no pasar de 5 nuevas. Con 90–100 % en la 1.ª escucha, el resto se mantiene sencillo (frases cortas, temas muy conocidos) mientras se estrena el ritmo de 5. Las secciones «Otra vez» no piden porcentaje, para que la tendencia de 1.ª escucha siga siendo honesta. Copia de las versiones antiguas: `~/.config/jose-bak-cap564/`.

- 2026-10-17 (noche), lote B0005–B0008 (CAP-563): 1.ª escucha de P005 = **90 %**, idea general correcta → dentro del objetivo (85–95). Se sube un poco: **2 palabras nuevas de la lista por pieza**, en fórmulas transparentes (acuerdo, mismo · seguir, carrera · momento, contra), frases todavía cortas. **Entra el voseo** (regla anterior: con 1.ª escucha ≥ 85 %): Andrés habla de *vos* en P009. Se cierra el arco 1 y empieza el arco 2 (natación, París 2024), un tema que Eva domina. Si la 1.ª escucha de P009/P010 baja de 85 %, volver a 1 palabra nueva y quitar el voseo hasta nuevo aviso.

- 2026-10-17 (noche), arco 1 (B0001–B0004 reescritas): sigue la calibración fácil por el 70 % de P001: **1 palabra nueva de la lista por pieza** (pensar, encontrar, parecer, en orden de rango entre las que probablemente no domina), frases cortas, muchos cognados (parque, millones, reunión, ingeniero, solución). Las palabras muy frecuentes de `next_new` (qué, ya, ahora, quién, otro, entonces, señor) se usan sin enseñarlas. Cada pieza recicla 4–8 de `heard_not_yet_shown` (más, mal, pequeño, razón, comprar, empezar, tarde…). La E2 de B0002, la E3 de B0003 y la E2 de B0004 dependen de la palabra nueva anterior, sin glosa.

- 2026-10-17: primera pieza, sin datos de comprensión todavía → nivel suave: 2 elementos nuevos (*madrugar*, *me toca / me tocó + inf.*), tema muy conocido (natación por la mañana, trabajo, *The West Wing*), diálogo de ~120 palabras.

- 2026-10-17 (noche), lote B0001–B0004: 1.ª escucha de P001 = **70 %** (< 85) → **más fácil**: 1 solo elemento nuevo por pieza, frases cortas (≈100–135 palabras), temas muy conocidos (natación en Londres, llegar a Cali, las piscinas de Sydney), mucho reciclado. Sin voseo todavía: entrará cuando la 1.ª escucha esté en 85 % o más. Geografía corregida: Cali no tiene mar (Buenaventura ≈3 h; lago Calima ≈2 h).

## Piezas a demanda (Bnnnn)

**2026-10-17 (noche), CAP-562 — arcos temáticos (decisión de Eva):** las piezas giran ahora en torno a sus temas, en profundidad (episodios concretos, películas, Juegos Olímpicos, Beatles, Sondheim, derecho…), en arcos de 3–5 piezas. Plan de unos 20 arcos en `topics.md`. Eva no había empezado ninguna pieza (`bites.json`: done vacío, current nulo), así que **B0001–B0004 se reescribieron** como el arco 1. Las piezas P002–P004 (piscina, llegar a Cali, piscinas de Sydney) quedan **en reserva, no emitidas**; *extrañar*, *acabo de* y *la ola* no se han sembrado todavía.

| Pieza | Tipo | Audio(s) | Nuevo (lista) | Patrones / estructuras | Estado |
|---|---|---|---|---|---|
| B0001 | Nueva + Patrones | P005 El capítulo del monorriel (arco 1, 1/4) | pensar | pensar que + frase (sembrado) | hecha |
| B0002 | Nueva | P006 A Homer le toca (arco 1, 2/4, narración) | encontrar | le toca + inf. (reciclado) | hecha |
| B0003 | Nueva + Patrones + Otra vez | P007 ¿Qué te pareció el final? (arco 1, 3/5) + repetición de P005 | nuestro · mirar · volver · parecer · llamar | me parece / me pareció (sembrado) · volver a + inf. (oído) | lista |
| B0004 | Nueva + Patrones + Otra vez | P008 ¿Monorriel o calle? (arco 1, 4/5; Sydney 1988–2013) + repetición de P001 | alguno · mismo · nuevo · hasta · acuerdo | estar de acuerdo (sembrado) · lo mismo · desde…hasta | lista |
| B0005 | Nueva + Otra vez | P009 ¿Homer es un buen padre? (arco 1, 5/5) + repetición de P006 | dios · vida · hijo · padre · tomar (ya marcadas como conocidas; se dejó porque estaba en curso) | llevo + gerundio (reciclado) | hecha (90 %) |
| B0006 | Nueva + Patrones | P010 Diez kilómetros en el Sena (arco 2, 1/4; primer voseo) | tratar · maldito · aquel · sitio · daño | seguir + gerundio (sembrado) · tratar de + inf. (oído) | lista (CAP-565) |
| B0007 | Nueva + Otra vez | P011 Dos horas de pelea (arco 2, 2/4, narración) + repetición de P007 | caja · dirigir · droga · pelear · ataque | tratar de (reciclado, sin glosa) | lista (CAP-565) |
| B0008 | Nueva + Patrones + Otra vez | P012 Golpes en el agua (arco 2, 3/4) + repetición de P008 | cubrir · quemar · espalda · engañar · golpe | valer la pena (sembrado) | lista (CAP-565) |
| B0009 | Nueva + Otra vez + Patrones | P013 ¿Valió la pena? (arco 2, 4/5) + repetición de P009 | enojar · pertenecer · doble · batalla · majestad | a X le gusta / le pertenece (sembrado) · valer la pena (reciclado) | lista (CAP-566) |
| B0010 | Nueva + Otra vez + Patrones | P014 ¿Y vos, Eva? (arco 2, 5/5; 10 km masculino y sus travesías) + repetición de P010 | cuello · fijar · acaso · quieto · ocultar | acabar de + inf. (sembrado) · tratar de, seguir + gerundio (reciclados) | lista (CAP-566) |
| B0011 | Nueva + Otra vez | P015 El festival de Leslie (arco 3, 1/4) + repetición de P011 | encerrar · obviamente · vacío · perseguir · grabar | lo (oído) | lista (CAP-566; acortada en CAP-569) |
| B0012 | Nueva + Otra vez + Patrones | P016 Un festival maldito (arco 3, 2/4, narración) + repetición de P012 | faltar · escoger · cuchillo · robo · líder | lo / la, pronombres de objeto (sembrado) | lista (CAP-566; acortada en CAP-569) |
| B0013 | Canción + Otra vez | P017 La canción de Cali (Grupo Niche, «Cali pachanguero») + repetición de P013 | — (ninguna) | lo / la (reciclado: la canta, ¿la bailás?) | lista (CAP-569) |
| B0014 | Historia + Otra vez | P018 Eva y el mar (solo palabras conocidas) + repetición de P014 | — (ninguna) | llevar + gerundio, seguir + gerundio (reciclados) | lista (CAP-569) |

**Siguiente lote (B0015–), cuando lleguen palabras del selector:** P019 y P020 cierran el arco 3 (la rueda de Chicago y el generador del casino; «¿y vos qué habrías hecho?»), con amenaza, involucrar y lo que llegue del selector. Después, arco 4 (los Beatles en *The Ed Sullivan Show*) y la primera **Canción** hacia la pieza 13–15. Palabras: siempre `to_learn` en orden.

**Voces del audio (desde el 18-10):** voces colombianas: **A = Salomé** (Eva) y **B = Gonzalo** (Andrés y narradores); las líneas sin A:/B: las lee Salomé, así que las narraciones nuevas llevan `B:`. Antes: Paulina / Eddy. P001 tenía A = Andrés (voz femenina); desde P005, **A = Eva y B = Andrés**, y las narraciones sin A:/B: van con la voz femenina.

**Repeticiones previstas** (≈1 día, 4 días, 2 semanas; ahora como sección «Otra vez» dentro de una pieza nueva): P005 → B0003 · P001 → B0004 · P006 → B0005 · P007 → B0007 · P008 → B0008. P009 → B0009 · P010 → B0010 · P011 → B0011 · P012 → B0012. P013 → B0013 · P014 → B0014. Pendientes: P015–P018 (≈1 día, en las próximas piezas) y las de 4 días / 2 semanas de P005–P012 (~21-10 / ~22-10 y ~31-10 / ~1-11).

## Estructuras sembradas

| Estructura | Introducida | Piezas que la llevan | Usos correctos de Eva sin ayuda | Estado |
|---|---|---|---|---|
| me toca / me tocó + inf. | P001 (17-10) | P001 (B0003), P006 «le toca» (B0002) | 1 (17-10: «me toca nadar en la piscina», tras dudar) | sembrando (meta: 8 piezas en 3 semanas) |
| acabo de + inf. | (P003 en reserva, no emitida) | — | 0 | pendiente |
| pensar que + frase | P005 / B0001 | P005 (B0001, B0003), P006 (B0006), P008, P009 | 1 (17-10, B0001 P2: «Pienso que comprando [comprar] un monorriel es una mala idea», tras el modelo) | sembrando |
| me parece / me pareció | P007 / B0003 | P007 (B0003, B0007), P008 (B0004, B0008), P009 (B0005) | 0 | sembrando |
| llevo + tiempo + gerundio | P001 | P001 (B0003), P009 (B0005, B0009) | 1 (18-10, B0005: «llevo toda la vida haciendo nadando», sin ayuda) | sembrando |
| estar de acuerdo (con) | P008 / B0004 | P008 (B0004, B0008) | 0 | sembrando |
| seguir + gerundio | P010 / B0006 | P010 («seguís nadando», Patrones), P014 («hay que seguir nadando»), P018 («siguió nadando») | 1 (18-10, B0006: «Sigo entrenado [entrenando] a la gimnasium todos los días», justo después de preguntar qué es *sigo*: no cuenta como espontáneo) | sembrando |
| tratar de + inf. | P010 / B0006 | P010, P011, P014 | 0 | sembrando |
| voseo (oído) | P010 / B0006 | P010, P011 (H1), P012 |
| valer la pena | P012 / B0008 | P012 (Patrones y audio; B0012), P013 (título y H2) | 0 | sembrando |
| a X le gusta / le pertenece (gustar y parecidos) | P013 / B0009 | P013 (Patrones y audio) | 0 | sembrando |
| acabar de + inf. (chuleta n.º 4) | P014 / B0010 | P014 (Patrones y audio) | 0 | sembrando |
| lo / la (pronombres de objeto) | P016 / B0012 | P015 («lo quiere», «lo tienen encerrado»), P016 (Patrones y audio), P017 («la canta», «¿la bailás?») | 0 | sembrando |
| volver a + inf. | P007 / B0003 | P007 | 0 | oído | — | solo escucha; aceptarlo siempre |

## Calendario de piezas (método diario, histórico)

| Pieza | Título | Nuevo | 1.ª escucha | Repeticiones previstas |
|---|---|---|---|---|
| P001 | Me tocó madrugar | madrugar · me toca / me tocó + inf. | 2026-10-17 | 18-10 (domingo, repaso de la semana), 19-10 (Otra vez + Sombra) |

## Registro de lo conocido (known.json)

- `~/.config/jose/known.json` (copia en el repo: `known.json`). **La semilla del 2026-10-17 es una estimación conservadora**: vocabulario básico de alta frecuencia, lo que Eva ha producido bien en las lecciones anteriores, y las 25 fórmulas de la chuleta (como patrones vistos una vez). Ajustar cuando diga que algo no lo entiende. Tamaño inicial: 123 palabras, 30 patrones (incluidos los 2 nuevos de P001).

## Chuleta: uso como patrones (no como fórmulas)

- 2026-10-17 (lote B0001–B0004, reescrito como arco 1): quería, llevo, voy a, tengo que en la repetición de P001 (B0003). *Acabo de* (4) y *no sé, pero…* (23) quedan para más adelante (sus piezas están en reserva).
- 2026-10-17 (P001): quería + inf. (8), llevo + tiempo + gerundio (7), voy a + inf. (3), tengo que + inf. (2). Siguientes por sembrar en piezas: solía + inf. (5), iba a + inf. (6), me gustaría (9), empecé a / dejé de (15–16), sigo + gerundio (19), estoy a punto de (20).

## Lo que Eva ha dicho

- 2026-10-18 (B0007–B0009): su mejor recuerdo nadando es la travesía de Italia a Albania: 35 horas en el agua, comía cada hora (agua y electrolitos), lo más rico fue un gelato (cree que de fresa); nadó sola, sin golpes, pero con muchas medusas. Su sitio favorito para nadar es el mar, en Coogee. Entrena en el gimnasio todos los días. Cree que limpiar el Sena valió la pena para la comunidad. Pidió ver transcripciones cuando no entendía palabras.
- 2026-10-18 (B0005): no se decide entre *Los Simpson* y *The West Wing* como su serie favorita. Lleva toda la vida nadando.
- 2026-10-17 (B0002): travesía en Puerto Rico, de Tres Palmas a Cabo Rojo, 15 horas; al salir comió churrasco y fue a un karaoke.
- 2026-10-17: aprende por inmersión; no retiene reglas ni tablas; muy buena memoria auditiva (ritmo, entonación); reconoce patrones. Intereses para las piezas: Sydney, política y RR. II., *Game of Thrones*, *The West Wing*, *The Simpsons*, *Parks and Recreation*, *30 Rock*, *The Walking Dead*, cine clásico y los Óscar, los Juegos Olímpicos, los Beatles, el teatro musical (Sondheim), natación en aguas abiertas, derecho, derechos humanos, Latinoamérica y Cali.
- 2026-10-17 (mañana, método anterior): señaló con razón un error de corrección del bot en RP9 (*una gran abogada*); la lectura de fotos de letra a mano no es fiable.

---

## Historia: método anterior por gramática (2026-10-12 → 2026-10-17)

*Ya no guía las lecciones. Se conserva como referencia: el sílabo del libro B2, los errores que cometía y el vocabulario visto sirven para decidir qué estructuras sembrar en las piezas. La Prueba de nivel gramatical prevista para el 18-10 queda cancelada.*

Libro: `Gramatica Nivel B2.pdf` (escaneado). Página impresa = página PDF + 11.
Ritmo: objetivo 2 unidades por semana, pero manda la precisión (objetivo ~80 %): ver «Ritmo (decisiones)». Repaso espaciado en `~/.config/jose/srs.json`.

### Dónde estamos

- **Unidad actual:** 2 — El adjetivo, «Somos viejos amigos». Hoy (sáb 2026-10-17) **consolidación** → posición 2.0 en course.json.
- **Variedad (desde 2026-10-17, decisión de Eva):** español de Colombia (Cali). *Ustedes*, nunca *vosotros*; tú/usted en ejercicios, voseo en diálogos y aceptado si es correcto; vocabulario colombiano. La lección del 17-10 se regeneró sin vosotros (la primera versión tenía RP1, RP4, RP5 con vosotros) y el bot la reenvía desde la sección 1.
- **Último día:** 2026-10-17 (sábado) — U2 consolidación: sin gramática nueva; Repaso RP1–RP10 (cartas falladas), Práctica de U2 (apócope, invariables, concordancia, posición viejo/pobre/único, difícil de + inf., interesada en que + subj.), 4 palabras, ¿Qué toca?, Habla. Primera lección con el método nuevo (Repaso SRS, producción, ¿Qué toca?, Habla).
- **Mañana (dom 2026-10-18):** **Prueba de nivel** (línea de base, meta type «assessment»), en lugar del repaso semanal. Incluir en la parte de gramática el subjuntivo (ustedes, pidió que + imp. subj., cuando + subj.) y si + presente. Nada de vosotros.
- **Lunes 2026-10-19:** decidir según metrics.json: si la precisión sigue < 70 %, otro día de consolidación (U1–U2) antes de empezar U3 (Los artículos, PDF 17–24). U2 parte 2 (10-16) sigue sin contestar: sus contenidos se trabajan hoy.
- **Lecciones sin completar:** 2026-10-12 (P7, P10), 2026-10-13 (P9; R1–R8), 2026-10-14 (P8), 2026-10-16 (sin empezar). 2026-10-15 completada (contestada el 16-10, 20/33).

### Ritmo (decisiones)

| Fecha | Precisión (rolling3) | Decisión | Motivo |
|---|---|---|---|
| 2026-10-17 | 10-14: 61 %, 10-15: 61 % (rolling3 68 %) | Consolidación: sin gramática nueva, 4 palabras, Repaso 10 | < 70 %. 91 cartas pendientes (41 falladas). |

### B1 gaps (Español en Marcha B1)

| Regla | Unidad B1 | Veces | Último repaso |
|---|---|---|---|
| pidió que + imperfecto de subjuntivo | U9 (pp. 36–39), U7 | 5 (10-13, 10-14 C4, 10-15 C4, PD3) | 2026-10-17 RP2 |
| ~~vosotros en pres. subj./imperativo~~ — **retirado 2026-10-17**: sus 6 «errores» (digan, pongan, traigan, oigan, lleguen, hagan) son las formas correctas de *ustedes* en Colombia | — | 0 | — |
| si + presente (condición real) | U7 (pp. 28–31) | 3 | 2026-10-17 RP3 |
| cuando + futuro → pres. subj. | U7 (pp. 28–31) | 1 | 2026-10-17 RP1, PD5 |
| creer que / es evidente que + indicativo | U6 (pp. 24–27) | 3 (10-12, 10-15 PD4) | 2026-10-17 RP6 |
| Tildes (seáis, está, sé, íes, José) | U3–U4 (pp. 12–19) | 6 | — |
| Preposiciones: pensar en, desde, para + inf. | U2 (pp. 8–11), U4 | 3 | 2026-10-17 RP10, PD1, PD2 |
| indefinido / imperfecto / perfecto | U1–U3 (pp. 4–15) | 1 | 2026-10-17 RP8, PD4 |
| vocativo → 2.ª persona | U1 (pp. 4–7) | 2 | 2026-10-17 RP7 |

**Gap más frecuente:** pidió que + imperfecto de subjuntivo (5) → bloque fijo en los domingos de repaso. (Antes figuraba vosotros; retirado al pasar al español de Colombia.)

### Sílabo

Títulos leídos de las portadas de unidad (verificar el título exacto al empezar cada unidad).

| Unidad | Tema | PDF | Impresas |
|---|---|---|---|
| 1 | El sustantivo | 1–8 | 12–19 |
| 2 | El adjetivo | 9–16 | 20–27 |
| 3 | Los artículos | 17–24 | 28–35 |
| 4 | Los demostrativos | 25–32 | 36–43 |
| 5 | Los posesivos | 33–40 | 44–51 |
| 6 | Los indefinidos y otros cuantificadores | 41–50 | 52–61 |
| 7 | El pronombre personal | 51–58 | 62–69 |
| 8 | Los adverbios | 59–66 | 70–77 |
| 9 | Pretérito imperfecto de indicativo | 67–74 | 78–85 |
| 10 | Futuro simple y compuesto | 75–82 | 86–93 |
| 11 | Condicional simple y compuesto | 83–90 | 94–101 |
| 12 | Pretérito perfecto de subjuntivo | 91–96 | 102–107 |
| 13 | Pretérito imperfecto de subjuntivo | 97–103 | 108–114 |
| 14 | Pretérito pluscuamperfecto de subjuntivo | 104–110 | 115–121 |
| 15 | Formas no personales y perífrasis verbales | 111–118 | 122–129 |
| 16 | Ser, estar y haber | 119–126 | 130–137 |
| 17 | Verbos de cambio | 127–134 | 138–145 |
| 18 | La voz pasiva y la voz media | 135–142 | 146–153 |
| 19 | Construcciones comparativas | 143–148 | 154–159 |
| 20 | Oraciones causales | 149–156 | 160–167 |
| 21 | Oraciones consecutivas | 157–164 | 168–175 |
| 22 | Oraciones temporales | 165–172 | 176–183 |
| 23 | Relativos: oraciones explicativas y especificativas | 173–180 | 184–191 |
| 24 | Oraciones condicionales con si | 181–186 | 192–197 |
| 25 | Otros nexos condicionales | 187–194 | 198–205 |
| 26 | Oraciones concesivas | 195–202 | 206–213 |
| 27 | Verbos de entendimiento y percepción con indicativo y subjuntivo | 203–208 | 214–219 |
| 28 | Estilo indirecto | 209–218 | 220–229 |
| 29 | Las preposiciones | 219–227 | 230–238 |

### Materiales guardados de Eva (memory)

- **La chuleta de español** (25 fórmulas, `materials/chuleta-de-espanol.md`, guardada el 2026-10-15). Va en el recuadro «🧩 Fórmula del día» de cada lección.
  - **Última fórmula usada:** n.º 4 (2026-10-17). **Siguiente:** n.º 5 *Solía + inf.* y n.º 6 *Iba a + inf.*
  - 2026-10-17: n.º 3 *Voy a + inf.* y n.º 4 *Acabo de + inf.* → P1, P6, PD5, H1; tarjetas formula/3 y formula/4.
  - 2026-10-16: n.º 1 *Quiero + inf.* y n.º 2 *Tengo que + inf.* → P10, PD4, PD5.
  - Fórmulas que falla: (ninguna todavía).

### Puntos débiles

Recuento acumulado de errores (lo actualiza José a partir de los registros del bot).

| Área | Etiqueta | Errores | Notas |
|---|---|---|---|
| Subjuntivo (cuándo y qué tiempo) | [SUBJ] | 10 | Punto débil declarado por Eva. **Recalculado 2026-10-17:** se restan 6 errores de «vosotros» que eran formas correctas de *ustedes* (aprox.: alguno pudo estar contado en [CONJ]). 10-15: huberia sido; hagan (vosotros); pidió que + fui/presenté; es evidente que + subj. 10-12: subjuntivo tras «creer que» afirmativo / «es evidente que». 10-13: vosotros «pongan»; «pidió que» + indefinido. 10-14: vosotros traigan/oigan/lleguen; trajérmos; imp. en vez de perfecto subj. (x2); pidió que + presente ind. |
| Preposiciones (por/para, a, en, de, con, desde/hace, verbos con preposición) | [PREP] | 3 | Punto débil declarado por Eva. 10-13: «a» en vez de «desde» (tiempo); «pensar sobre» → pensar en; «a nadar» → para nadar (finalidad) |
| Elegir la conjugación (tiempo, modo, persona) | [CONJ] | 12 | Punto débil declarado por Eva. 10-15: sabe por sé (persona). 10-12: no lee la persona/tiempo pedidos en cada ítem; «condujieron». 10-13: si + imp. subj. («vinieras»); vocativo con verbo en 3.ª persona. 10-14: «oí» por oyeron (persona); si + subj. (oyeras, hiciera) x2; vocativo → 3.ª pers. otra vez; imperfecto por indefinido (empezaba) |

Errores concretos recurrentes:
- [SUBJ] creer que / es evidente que (afirmativo) + indicativo — puso subjuntivo (10-12).
- [CONJ] rellena las tablas siguiendo un patrón de personas en vez de leer cada ítem (10-12). Desde el 10-13 la persona va en negrita en cada letra.
- ~~[CONJ] vosotros: confunde digáis/digan (10-12).~~ Retirado: *digan* es correcto (ustedes).
- [SUBJ] verbo principal en pasado (pidió que) + imperfecto de subjuntivo — puso indefinido «puse» (10-13). Practicado de nuevo en C4 del 10-14.
- ~~[SUBJ]/[CONJ] vosotros en presente de subjuntivo (-áis/-éis)~~ (retirado 2026-10-17): «digan», «pongan» (10-12, 10-13). Recurrente → C1c, C3c, C6, PD5 del 10-14.
- [CONJ] si + presente de indicativo (no subjuntivo) (10-13). → C5, PD3 del 10-14.
- [CONJ] vocativo → verbo en 2.ª persona (10-13). → P8, PD1 del 10-14.
- [PREP] desde (punto de inicio), pensar en, para + infinitivo (finalidad) (10-13).
- ~~[SUBJ] vosotros en pres. subj.~~ (retirado 2026-10-17, español de Colombia) — **sigue fallando** en el 10-14 (traigan, oigan, lleguen). Va en C1c/C2b del 10-16 y debe ir en el bloque del domingo.
- [SUBJ] imp. subj. nosotros: «trajérmos» → trajéramos. → C1b del 10-16 (anduviéramos).
- [SUBJ] confunde imperfecto y perfecto de subjuntivo (sintiera por haya sentido; llegaron por hayáis llegado).
- [CONJ] si + presente: **3 fallos** (10-13, 10-14 C5 y PD3) → C7 del 10-16; repetir el domingo.
- [CONJ] vocativo → 2.ª persona: fallado otra vez (PD1 del 10-14); P8 del 10-14 sin contestar.
- [CONJ] indefinido (acción puntual) vs. imperfecto (empezaba). → C5 del 10-16 (anduvimos).
- Señor Verbo (15-10): falló «ser» presente ind. él/ellos (luego 6/6) y «andar» perfecto subj. vosotros (luego 6/6). → andar en C1 del 10-16.
- Ortografía: tilde en plurales (síes, íes — fallado en P4 del 10-14), «económica», José.
- Comunicación: en Telegram pega a veces los enunciados en vez de las respuestas, y manda lecciones de otros días (el bot ya lo gestiona).
- Vocabulario: brote vs. contagio; incertidumbre (fem.).
- [U2] 10-15: apócope gran (puso «grand/grande»), invariables amable/joven/cortés, concordancia (verdoso → verdosos, piernas larga → largas), sustantivación «el viejo». → Práctica del 10-17.
- [SUBJ] es evidente que + **indicativo** (puso «llevaran») (10-15 PD4). La parte «persona vosotros» queda retirada.

### Vocabulario visto

Del 10-12 al 10-15, vocabulario temático provisional. Desde el 10-16, **Must-Know Spanish 4000 Words** en orden.
- **Último usado en Must-Know:** cap. 1, p. 4, Communication by Phone (terminado; el resto de la lista son palabras conocidas). **Siguiente:** p. 4, Letters (querido/a, el sobre, el buzón, la carta urgente…; texto `0018.txt`).

- 2026-10-12: el brote, la vacuna, el contagio, la cuarentena, el síntoma, la mascarilla, el desmayo, la recesión, el desempleo, la incertidumbre, el repunte, hacer frente a
- 2026-10-13: el asco, la náusea, el mareo, la hemorragia, el vientre, la cicatriz, el análisis, el diagnóstico, el ingreso, la baja (médica), recetar, devanarse los sesos
- 2026-10-14: el/la excursionista, el saco de dormir, los víveres, el/la guarda forestal, la cima, la cría, la fiera, la pesadilla, el susto, el escalofrío, despistar, en peligro de extinción (lección sin contestar)
- 2026-10-15: entrañable, campechano/a, presumido/a, testarudo/a, tiquismiquis, el/la cascarrabias, despistado/a, la complicidad, el/la confidente, ser uña y carne, llevarse de maravilla con, dar la lata (lección sin contestar)
- 2026-10-17 (Must-Know p. 4, consolidación: 4): ¿De parte de quién?, colgar (o→ue), dejar un recado, equivocarse de número
- 2026-10-16 (Must-Know pp. 2–3): el/la conocido/a, conocer a alguien, encantado/a (de), presentar a alguien (a alguien), despedirse (de), la despedida, dedicarse a, el estado civil, soltero/a, divorciado/a (ser), el viudo/la viuda, mayor/menor de edad

### Verbos practicados

- 2026-10-12: revolver, conducir, decir (presente ind./subj., indefinido, futuro, participio)
- 2026-10-13: doler, venir, poner (presente ind./subj., indefinido, futuro, imperfecto subj., imperativo, participio); contexto: si + presente, pidió que + imp. subj.
- 2026-10-14: traer, sentir, oír (presente ind./subj., indefinido, imperfecto subj., perfecto subj.); contexto: pidió que + imp. subj., si + presente, me alegra que + perfecto subj. (sin contestar)
- 2026-10-15: ser, saber, hacer (pres. subj. vosotros, imp. subj., perfecto y pluscuamperfecto subj., indefinido, participio); contexto: pidió que + imp. subj., no creo que + subj., si + pluscuamp. subj. → condicional compuesto (sin contestar)
- 2026-10-17: en contexto (¿Qué toca? / Repaso): terminar, ser, hacer, decir, llegar, estar, sonar, sentirse, nadar, volver (cuando + subj., pidió que + imp. subj., si + presente, me alegra que + perf. subj., es importante que + subj., perfecto con «esta mañana»)
- 2026-10-16: andar, conocer, despedirse (indefinido, pres. ind./subj. vosotros, imp. subj., perfecto subj., pluscuamp. ind.; Webster's pp. 117, 217, 270); contexto: cuando + pres. subj., indefinido, me molestó que + imp. subj., si + presente

### Historial de lecciones

| Fecha | Unidad / parte | Completada | SUBJ | PREP | CONJ |
|---|---|---|---|---|---|
| 2026-10-12 | U1 parte 1 (género y número) | No (faltan P7, P10) | 2 | 0 | 4 |
| 2026-10-13 | U1 parte 2 (cambio de sentido, concordancia, complementos, vocativo) | No (falta P9; R1–R8 sin contestar) | 2 | 3 | 2 |
| 2026-10-14 | U1 consolidación y test | No (contestada el 15-10, 20/33; falta P8) | 7 | 0 | 5 |
| 2026-10-15 | U2 parte 1 (clases de adjetivos, intensificación) | Sí (contestada el 16-10, 20/33, 61 %) | 5 | 0 | 1 |
| 2026-10-16 | U2 parte 2 (posición, cambios de significado, complementos) | No (sin empezar) | — | — | — |
| 2026-10-17 | U2 consolidación (método nuevo) | — | — | — | — |
| **Total** | | | **16** | **3** | **12** |

### Cambios por la variedad colombiana (2026-10-17)

- Tarjetas de `srs.json` reescritas de *vosotros* a *ustedes* (mismos ids y calendario): 2026-10-12/C3b (digan), 2026-10-13/C3b (pongan), 2026-10-14/C1c (traigan), 2026-10-14/C3c (oigan), 2026-10-14/C6 (hayan llegado), 2026-10-14/PD5 (lleguen), 2026-10-15/C1a (sean), 2026-10-15/C3a (hagan), 2026-10-15/PD4 (se llevan), 2026-10-15/PD5 (sean). Copia previa: `srs.backup-2026-10-17-pre-ustedes.json`.
- Tarjetas del 17-10 ajustadas: dejar (la) razón / dejar un mensaje (en vez de «dejar un recado», España), «me equivoqué de número», fórmula 3 con «dar un borondo».
- Pendiente de revisar en tarjetas antiguas (no son vosotros): 2026-10-13/P7 «jerséis» (en Colombia: sacos/suéteres); «coche», «aparcar», «conducir» en 2026-10-12/C6 y 2026-10-15/P2, V3 (Colombia: carro, parquear, manejar). Se aceptan, pero al reescribirlas en Repaso usar la forma colombiana.
