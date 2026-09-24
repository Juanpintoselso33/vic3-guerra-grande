# La Guerra Grande — el Río de la Plata, 1836-1862

Mod para Victoria 3 (1.13) · *mod for Victoria 3 (1.13)*

> **Alfa 0.1.** Es una versión de prueba, no terminada: hay contenido de 1848-1852 que pasó
> pruebas automáticas pero todavía no partidas completas, y puede haber textos sin pulir,
> imágenes provisorias y errores.
>
> **Requisitos**
> - Victoria 3 1.13 con **todos los DLC**.
> - [Community Mod Framework](https://steamcommunity.com/sharedfiles/filedetails/?id=3385002128) (Steam Workshop).
> - [la Argentina](https://steamcommunity.com/sharedfiles/filedetails/?id=2982907360) (Steam Workshop).
>
> **Orden de carga:** Community Mod Framework → la Argentina → Guerra Grande (último).
>
> **Instalación.** Bajá `GuerraGrande_alfa_0.1.zip` de la
> [Release](https://github.com/Juanpintoselso33/vic3-guerra-grande/releases) y descomprimilo. Copiá la
> carpeta `guerra_grande` entera a `Documentos/Paradox Interactive/Victoria 3/mod/` (creá `mod` si no
> existe): tiene que quedar `.../Victoria 3/mod/guerra_grande/common`, `events`, `gfx`… En el launcher
> armá un playset con el orden de arriba y empezá una **partida nueva**. El zip trae un
> `LEEME - INSTALAR.txt` con los pasos para Windows y Mac.
>
> **Qué sigue.** La idea es integrar el mod más adelante a «la Argentina». Se agradecen la ayuda y
> las ideas, sobre todo sobre cómo manejar las mecánicas (el sitio de Montevideo, el río, el Pacto
> Federal, las potencias). Si reportás un error, decí la fecha de la partida, con qué país jugabas y,
> si podés, adjuntá `Documentos/Paradox Interactive/Victoria 3/logs/error.log`.

> **Alpha 0.1.** A test build, not finished: some 1848-1852 content has passed automated tests but
> not full playthroughs yet; expect rough texts, placeholder images and bugs.
>
> **Requirements**
> - Victoria 3 1.13 with **all DLC**.
> - [Community Mod Framework](https://steamcommunity.com/sharedfiles/filedetails/?id=3385002128) (Steam Workshop).
> - [la Argentina](https://steamcommunity.com/sharedfiles/filedetails/?id=2982907360) (Steam Workshop).
>
> **Load order:** Community Mod Framework → la Argentina → Guerra Grande (last).
>
> **Install.** Download `GuerraGrande_alfa_0.1.zip` from the
> [Release](https://github.com/Juanpintoselso33/vic3-guerra-grande/releases) and unzip it. Copy the whole
> `guerra_grande` folder into `Documents/Paradox Interactive/Victoria 3/mod/` (create `mod` if it does
> not exist): it must end up as `.../Victoria 3/mod/guerra_grande/common`, `events`, `gfx`… In the
> launcher, build a playset in the order above and start a **new game**. The zip includes
> `LEEME - INSTALAR.txt` with the steps for Windows and Mac.
>
> **What's next.** The plan is to merge this mod into «la Argentina» later. Help and ideas are
> welcome, especially on how to handle the mechanics (the siege of Montevideo, the river, the Federal
> Pact, the foreign powers). With a bug report, give the in-game date, the country you played and, if
> you can, attach `Documents/Paradox Interactive/Victoria 3/logs/error.log`.

La Guerra Grande de las dos orillas: el nacimiento de las divisas blanca y colorada en Carpintería,
la partición de la República en el gobierno de la **Defensa** (Montevideo) y el del **Cerrito** (la
campaña), los nueve años de sitio y la paz de 1851; y del otro lado, el Pacto Federal de Rosas,
Corrientes, la Coalición del Norte, Urquiza, Caseros y Pavón.

Por qué la Argentina es requisito: el lado argentino necesita la Argentina partida en sus provincias
históricas, y vanilla no la parte. De los ocho estados que usa, vanilla tiene sólo `STATE_CORRIENTES`,
`STATE_TUCUMAN` y `STATE_JUJUY`; Entre Ríos, Córdoba, Salta, Misiones, La Rioja y Catamarca los agrega
«la Argentina». El mod trae el mapa sudamericano de la Argentina con los cinco estados orientales.
Si tenías el viejo «Guerra Grande x la Argentina» en el playset, sacalo: su contenido está en este mod.

*English below the Spanish text — same content.*

---

## Con qué país se juega

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

## Qué hace (español)

**19 de setiembre de 1836 — Carpintería.** Nueve meses después del inicio. Los grupos de
interés pasan a llamarse **Partido Blanco** y **Partido Colorado**, y el jugador elige divisa
(o ninguna).

**24 de octubre de 1838 — la caída de Oribe.** Renuncia y se va a Buenos Aires, o se queda y
hace de la capital una fortaleza.

**1839 — la guerra.** Rivera le declara la guerra a Rosas. Después de Arroyo Grande (fines de
1842) la República se parte en dos: Uruguay conserva Montevideo y nace el **Gobierno del Cerrito**
(tag `CER`) con todo el país salvo Montevideo, en guerra civil por una jugada diplomática propia.
Si el jugador venía por la vía blanca, puede irse al Cerrito (`change_tag`).

**Los journals.** «La Guerra Grande» lleva una barra de −10 a +10 que mueven **las decisiones de
los dos bandos y el río** (las batallas no puntúan), el aguante de cada gobierno y el árbitro de la
paz; «La cuestión del Plata» sigue a las potencias; «El Sitio Grande» abre en 1843; «El Pacto
Federal» es el lado argentino. La guerra cierra cuando uno de los dos gobiernos deja de existir, o
con la paz del 8 de octubre de 1851: *ni vencidos ni vencedores*.

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
[`SOURCES.md`](SOURCES.md). Las imágenes son pinturas, litografías y fotografías de dominio público
(créditos en [`CREDITS.md`](CREDITS.md)), recortadas y animadas con un zoom lento, codificadas a Bink 2.

---

## Who to play (English)

| Play as | What you get |
|---|---|
| **Uruguay** | the oriental shore: Carpintería, the partition, the siege, the peace of 1851 |
| **Argentina** | the other shore: the Federal Pact, Corrientes, the Northern Coalition, Urquiza, Caseros |

**The Argentine side is played from Argentina.** All its events — Corrientes's secession, Tucumán's
pronouncement, the battles of the interior, Urquiza's Pronunciamiento, Caseros — go to the Buenos
Aires government. Playing Uruguay, the Argentine interior still happens, in the background: what you
see of it is the size of the contingent Rosas sends to the Cerrito.

From Argentina you can also **switch seats**: on its birthday, each of the three new countries offers
to take you — Corrientes on 6/3/1839, the Coalition on 7/4/1840, Entre Ríos on 1/5/1851. One chance
per country.

Why la Argentina is required: the Argentine side needs Argentina split into its historical provinces,
and vanilla does not split it. The mod carries la Argentina's South American map with the five
oriental states. If you had the old «Guerra Grande x la Argentina» in your playset, remove it: its
content is in this mod.

## What it does (English)

**19 September 1836 — Carpintería.** Nine months in. The interest groups are renamed **Blanco
Party** and **Colorado Party**, and the player picks a ribbon (or refuses both).

**24 October 1838 — the fall of Oribe.** He resigns and sails for Buenos Aires, or stays and
turns the capital into a fortress.

**1839 — the war.** Rivera declares war on Rosas. After Arroyo Grande (late 1842) the Republic
splits: Uruguay keeps Montevideo and the **Cerrito Government** (tag `CER`) is created with the
whole country except Montevideo, at civil war through its own diplomatic play. A player who took
the blanco road can ride out to the Cerrito (`change_tag`).

**The journals.** «La Guerra Grande» holds a −10 to +10 bar moved by **both sides' decisions and
the river** (battles do not score), each government's endurance and the arbiter of the peace; «La
cuestión del Plata» follows the foreign powers; «El Sitio Grande» opens in 1843; «El Pacto Federal»
is the Argentine side. The war closes when one of the two governments ceases to exist, or with the
peace of 8 October 1851: *neither vanquished nor victors*.

## How it is built

Nothing invented: every piece copies a mechanic the game already has — the First Carlist War
journal entry, the Central American `create_country` secessions, the Taiping play, la
Argentina's own scripted buttons. Texts come from period and academic sources, cited in
[`SOURCES.md`](SOURCES.md); images are public-domain paintings, lithographs and photographs
(credits in [`CREDITS.md`](CREDITS.md)).
