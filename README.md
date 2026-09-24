# The Guerra Grande — the Río de la Plata, 1836-1862

A mod for Victoria 3 (1.13).

> **Alpha.** A test build, not finished: some 1848-1852 content has passed automated tests but
> not full playthroughs yet; expect rough texts, placeholder images and bugs.
>
> **Requirements**
> - Victoria 3 1.13 with **all DLC**.
> - [Community Mod Framework](https://steamcommunity.com/sharedfiles/filedetails/?id=3385002128) (Steam Workshop).
> - [la Argentina](https://steamcommunity.com/sharedfiles/filedetails/?id=2982907360) (Steam Workshop).
>
> **Load order:** Community Mod Framework → la Argentina → Guerra Grande (last).
>
> **Install.** Download the latest `GuerraGrande_alfa_*.zip` from the
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

The Guerra Grande of both banks of the Río de la Plata: the birth of the Blanco and Colorado ribbons at
Carpintería, the Republic split between the government of the **Defensa** (Montevideo) and that of the
**Cerrito** (the countryside), nine years of siege and the peace of 1851; and on the other bank, Rosas's
Federal Pact, Corrientes, the Northern Coalition, Urquiza, Caseros and Pavón. See [`CHANGELOG.md`](CHANGELOG.md)
for what changed in each release.

## Who to play

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

## What it does

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
