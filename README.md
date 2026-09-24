# Guerra Grande — el Río de la Plata, 1836-1862

Victoria 3 (1.13). La Guerra Grande oriental: el nacimiento de las divisas blanca y colorada en
Carpintería, la partición de la República en el gobierno de la **Defensa** (Montevideo) y el del
**Cerrito** (la campaña), los nueve años de sitio y la paz de 1851.

**Requisitos: Community Mod Framework y «la Argentina»** (Workshop 2982907360). Desde el 24/9/2026
la Argentina es requisito y el compatch «Guerra Grande x la Argentina» quedó integrado en este mod:
el mapa de la Argentina con los cinco estados orientales, su historia sudamericana, los localizadores,
La Plata y la Gran Argentina, el HQ chileno, el candado del voto de Rosas y los objetivos de guerra de
CMF viven acá. **Ese compatch ya no se carga**: si lo tenías en el playset, sacalo.

## Cómo cargarlo

**Community Mod Framework → la Argentina → Guerra Grande**, en ese orden.

| Con qué país | Qué se juega |
|---|---|
| **Uruguay** | la orilla oriental: Carpintería, la partición, el sitio, la paz de 1851 |
| **Argentina** | la otra orilla: el Pacto Federal, Corrientes, la Coalición del Norte, Urquiza, Caseros |

**El lado argentino se juega desde Argentina, y conviene decirlo porque no se deduce.** Todos sus
eventos —la separación de Corrientes, el pronunciamiento de Tucumán, las batallas del interior, el
Pronunciamiento de Urquiza, Caseros— le llegan al gobierno de Buenos Aires, que es a quien le pasan.
Jugando de Uruguay el interior argentino ocurre igual, pero pasa de fondo: lo que se ve de él es el
tamaño del contingente que Rosas le manda al Cerrito, que depende de cómo le fue en el interior.

Y es desde Argentina de donde se puede **cambiar de asiento**: en el día de su nacimiento, cada uno
de los tres países ofrece pasarse a él —Corrientes el 6/3/1839, la Coalición el 7/4/1840, Entre Ríos
el 1/5/1851—. Es una sola oportunidad por país y no se repite.

Por qué la Argentina es requisito: el lado argentino necesita la Argentina partida en sus provincias
históricas, y vanilla no la parte. De los ocho estados que usa, vanilla tiene sólo `STATE_CORRIENTES`,
`STATE_TUCUMAN` y `STATE_JUJUY`; Entre Ríos, Córdoba, Salta, Misiones, La Rioja y Catamarca los agrega
«la Argentina».

⚠️ **Partidas viejas**: todo el contenido del compatch está ahora en este mod; no cargues los dos
juntos.

*English below the Spanish text — same content.*

---

## Qué hace (español)

**Al arrancar la partida.** Manuel Oribe deja de ser un "moderado" y recibe
`ideology_caudillismo`, que es la del juego base y la que le corresponde: el caudillo de la
campaña, no un moderado.

**19 de setiembre de 1836 — Carpintería.** Nueve meses después del inicio. Los grupos de
interés pasan a llamarse **Partido Blanco** y **Partido Colorado**, y el jugador elige divisa
(o ninguna). Se abre la journal entry.

**24 de octubre de 1838 — la caída de Oribe.** Renuncia y se va a Buenos Aires, o se queda y
hace de la capital una fortaleza.

**1839 — la guerra.** La República se parte en dos: Uruguay conserva Montevideo y nace el
**Gobierno del Cerrito** (tag `CER`) con todo el país salvo Montevideo, en guerra civil por una
jugada diplomática propia. Si el jugador venía por la vía blanca, puede irse al Cerrito
(`change_tag`). Rosas decide si lo respalda.

**La journal entry.** Una barra de −10 a +10 que mueven **las decisiones de los dos bandos y el río** (las batallas no puntúan),
dos botones —llamar a las escuadras anglofrancesas, levantar la Legión Italiana de Garibaldi—
y eventos mensuales de ambiente. Cierra cuando uno de los dos gobiernos deja de existir, o con
la paz del 8 de octubre de 1851: *ni vencidos ni vencedores*.

## Cómo está hecho

Nada inventado: cada pieza copia una mecánica que ya existe en el juego.

| Pieza | Modelo |
|---|---|
| Barra −10/+10 sin progreso mensual | `je_the_first_carlist_war_score_bar` |
| La mueven las decisiones y el río | `gg_war_balance_blanco`, `gg_plata_pressure_*` |
| Cierre por desaparición de un bando | `NAND = { exists = c:SPC exists = c:SPA }` |
| País rival creado por evento | `create_country` de Centroamérica |
| Guerra civil | `dp_taiping_rebellion` |
| Botones | `patagonia_button` de la Argentina |
| Cambiar de bando | `change_tag` del final carlista |

Los textos salen de fuentes de época y académicas, con las citas y los enlaces en
[`SOURCES.md`](SOURCES.md). Las imágenes son pinturas y litografías de dominio público de
1840-1845, recortadas y animadas con un zoom lento, codificadas a Bink 2.

## Instalación

Copiar la carpeta a `Documents/Paradox Interactive/Victoria 3/mod/` con su `.mod` apuntando
ahí, y cargarla **después** de Community Mod Framework y de la Argentina.

---

## How to load it (English)

**Requirements: Community Mod Framework and «la Argentina»** (Workshop 2982907360). Load order:
**Community Mod Framework → la Argentina → Guerra Grande**. Since 24/9/2026 the old compatch
«Guerra Grande x la Argentina» is part of this mod (la Argentina's map with the five oriental states,
its South American history, the map locators, La Plata and Greater Argentina, the Chilean HQ, Rosas's
vote lock and CMF's war goals). **Do not load that compatch any more**; remove it from your playset if you had it.

| Play as | What you get |
|---|---|
| **Uruguay** | the oriental shore: Carpintería, the partition, the siege, the peace of 1851 |
| **Argentina** | the other shore: the Federal Pact, Corrientes, the Northern Coalition, Urquiza, Caseros |

⚠️ **Old saves**: all of the compatch's content is in this mod now; do not load both.

## What it does (English)

**At game start.** Manuel Oribe stops being a "moderate" and gets `ideology_caudillismo` — the
ideology la Argentina defines but never gives to anyone: local caudillos, tenant farmers, land
taxes.

**19 September 1836 — Carpintería.** Nine months in. The interest groups are renamed **Blanco
Party** and **Colorado Party**, and the player picks a ribbon (or refuses both). The journal
entry opens.

**24 October 1838 — the fall of Oribe.** He resigns and sails for Buenos Aires, or stays and
turns the capital into a fortress.

**1839 — the war.** The Republic splits: Uruguay keeps Montevideo and the **Cerrito
Government** (tag `CER`) is created with the whole country except Montevideo, at civil war through its
own diplomatic play. A player who took the blanco road can ride out to the Cerrito
(`change_tag`). Rosas decides whether to back it.

**The journal entry.** A −10 to +10 bar moved by **both sides' decisions and the river** (battles do not score), two buttons —
call in the Anglo-French squadrons, raise Garibaldi's Italian Legion — and monthly flavour
events. It closes when one of the two governments ceases to exist, or with the peace of
8 October 1851: *neither vanquished nor victors*.

## How it is built

Nothing invented: every piece copies a mechanic the game already has — the First Carlist War
journal entry, the Central American `create_country` secessions, the Taiping play, la
Argentina's own scripted buttons. Texts come from period and academic sources, cited in
[`SOURCES.md`](SOURCES.md); images are public-domain paintings and lithographs from 1840-1845.

## Install

Put the folder in `Documents/Paradox Interactive/Victoria 3/mod/` with its `.mod` file
pointing at it, and load it **after** la Argentina.
