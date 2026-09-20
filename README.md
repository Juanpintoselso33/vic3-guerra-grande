# Guerra Grande — Uruguay, 1836-1852

Victoria 3 (1.13). La Guerra Grande oriental: el nacimiento de las divisas blanca y colorada en
Carpintería, la partición de la República en el gobierno de la **Defensa** (Montevideo) y el del
**Cerrito** (la campaña), los nueve años de sitio y la paz de 1851.

**La guerra oriental se sostiene sola.** Trae sus cinco estados orientales, su historia y todo lo que
necesita del juego base; lo que cambia de vanilla lo reemplaza por objeto con `REPLACE:` en vez de
pisar archivos enteros, así que convive con otros mods.

## Cómo cargarlo

| Qué querés jugar | Cómo | Con qué país empezás |
|---|---|---|
| Sólo la guerra oriental | Guerra Grande. Nada más | **Uruguay** |
| **La guerra entera, las dos orillas** | la Argentina → Guerra Grande → **Guerra Grande x la Argentina (compatch)**, en ese orden | **Uruguay** para la orilla oriental, **Argentina** para la otra |

**El lado argentino se juega desde Argentina, y conviene decirlo porque no se deduce.** Todos sus
eventos —la separación de Corrientes, el pronunciamiento de Tucumán, las batallas del interior, el
Pronunciamiento de Urquiza, Caseros— le llegan al gobierno de Buenos Aires, que es a quien le pasan.
Jugando de Uruguay el interior argentino ocurre igual, pero pasa de fondo: lo que se ve de él es el
tamaño del contingente que Rosas le manda al Cerrito, que depende de cómo le fue en el interior.

Y es desde Argentina de donde se puede **cambiar de asiento**: en el día de su nacimiento, cada uno
de los tres países ofrece pasarse a él —Corrientes el 6/3/1839, la Coalición el 7/4/1840, Entre Ríos
el 1/5/1851—. Es una sola oportunidad por país y no se repite.

### El lado argentino necesita «la Argentina», y no es opcional

La orilla oriental —Carpintería, la partición, el sitio, la paz de 1851— **se juega sola**, como
siempre. El **lado argentino** no: Corrientes, la Coalición del Norte y el Pronunciamiento de Entre
Ríos necesitan que la Argentina esté partida en sus provincias históricas, y **vanilla no la parte**.

De los ocho estados que ese lado usa, en vanilla existen sólo tres: `STATE_CORRIENTES`,
`STATE_TUCUMAN` y `STATE_JUJUY`. Entre Ríos, Córdoba, Salta, Misiones, La Rioja y Catamarca **son
provincias que agrega «la Argentina»**. *(Hasta el 20/9/2026 acá decía «sólo dos»: Jujuy sí está en
vanilla. Lo agarró una revisión que chequeó el dato contra los archivos del mapa.)*

Por eso todo lo que toca ese lado —los trece eventos fechados, los tres gobernadores federales y el
journal de la delegación— pide un estado que sólo existe con ella cargada. **Sin «la Argentina», ese
lado sencillamente no ocurre**: no se crea ningún país, no se abre ningún journal argentino, no se
rompe nada, y la guerra oriental se juega exactamente igual que antes. Con ella y el compatch, se
juegan las dos orillas.

Una salvedad honesta: el **candado provisorio de Rosas** (`gg_rosas_provisional_lock`) sí se aplica
siempre, con o sin «la Argentina», y es a propósito. No es una mecánica del lado argentino: es lo que
mantiene a Rosas gobernando Buenos Aires durante los dieciséis años en que es el padrino del Cerrito,
que es algo que el lado oriental necesita.

⚠️ **Partidas viejas del submod**: si venías jugando con la Argentina, seguí con ella y agregá el
compatch. Desactivarla saca contenido que ya es parte de tu guardado.

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

**La journal entry.** Una barra de −10 a +10 que **solo se mueve cuando se gana una batalla**,
dos botones —llamar a las escuadras anglofrancesas, levantar la Legión Italiana de Garibaldi—
y eventos mensuales de ambiente. Cierra cuando uno de los dos gobiernos deja de existir, o con
la paz del 8 de octubre de 1851: *ni vencidos ni vencedores*.

## Cómo está hecho

Nada inventado: cada pieza copia una mecánica que ya existe en el juego.

| Pieza | Modelo |
|---|---|
| Barra −10/+10 sin progreso mensual | `je_the_first_carlist_war_score_bar` |
| La mueven las batallas | `on_battle_won` → `carlist_war_battle_score` |
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
ahí, y cargarla **después** de la Argentina.

---

## How to load it (English)

| What you want | How |
|---|---|
| The Guerra Grande alone | Guerra Grande. Nothing else |
| With **la Argentina** | la Argentina → Guerra Grande → **Guerra Grande x la Argentina (compatch)**, in that order. Without the compatch the two mods overwrite each other's map and Uruguay starts with twice its population |

⚠️ **Old saves from the submod**: if you were playing with la Argentina, keep it and add the
compatch. Turning it off removes content that is already part of your save.

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

**The journal entry.** A −10 to +10 bar that **only moves when a battle is won**, two buttons —
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
