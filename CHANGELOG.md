# Changelog — The Guerra Grande · the Río de la Plata, 1836-1862

## Unreleased

- **«The Pact without a Constitution» keeps Rosas in power until his death:** after the negotiated confederation the
  mod read that answer as the end of Rosas's era, so the seat was no longer his and an engine coup could put another
  man in it (Ángel Pacheco, 1854, in a playtest); Entre Ríos and Corrientes, left independent to wait for a
  constitution that never came, stayed out for good. Now, whatever settlement came before (except Urquiza's victory
  and the fallen mandate), Rosas keeps «la suma del poder público» until 14/3/1877: the seat returns to him, and
  neither a coup nor a revolution can replace him. Entre Ríos and Corrientes come back as Provinces of the Pact
  (not a player's, not at war with Buenos Aires). His death reopens the question, as before. Games in progress: the
  next monthly pulse seats Rosas again and brings the two provinces back.
- **Rivera dies on 13 January 1854 and Flores takes the government:** the arroyo Conventos came 110 days after the
  triumvirate's answer, which counts from the peace, so Rivera could die weeks early (16/12/1853 in a playtest). It
  now comes on its date. And Flores only took the chair if it was empty, but the engine fills a dead ruler's chair at
  once, so the leader of a ruling group kept it (Melchor Pacheco y Obes); Flores is now seated whoever holds it, and
  again the next day if the engine moves. Games already past January 1854 are not changed.
- **Carlos Antonio López exists even with «More Dynamic Names And Flags»:** that mod replaces Paraguay's starting
  characters with an old file that only creates Francia, so López never existed and Paraguay was ruled by generated
  men. From 13/3/1841, when the Congress made him first consul, if López exists nowhere he is created from the game's
  own template and seated in Paraguay, once per game; he lives until 10/9/1862. With the game's own history nothing
  changes. Games in progress get him on the next monthly pulse.

- **The peace no longer deletes the loser's men:** every peace settlement of the Guerra Grande annexed the losing
  government outright, and the engine deletes an annexed country's characters -- Oribe, Lavalleja and the original
  Giró vanished when the Cerrito was absorbed, although Oribe should live on at his quinta until 1857. The 15 peace
  annexations that still did this (and Brazil's annexation of the Pact province after a Cisplatine war) now bring the
  loser's characters over first, stripped of ruler and heir, as the province annexations already did. Characters
  already lost in a game in progress do not come back.

## 0.1.6-alpha — 25/9/2026

- **Montevideo's immigrants arrive as people, with their nationalities, and many as soldiers:** the engine sends
  besieged Montevideo (8 arable land) no mass migration, so the immigrants are now created by events, in Montevideo and
  only while the Republic or the Defensa holds it. The Argentine emigrés of September 1839 (3,800, clerks); the
  colonists' ships of May 1842 (1,000 Italians and 5,100 Spaniards, a third of them enrolled in the Guardia Nacional
  if you choose to); the French Legion's men when it is raised (3,600 French and 750 Basque soldiers, or the same men
  as labourers if Paris is obeyed), the Italian Legion's (750 soldiers), and a few more when either legion is
  reinforced. Sizes follow Montevideo's 1843 census (5,324 French, 4,205 Italians, 3,406 Spaniards, 2,553 Argentines)
  and the legions' strengths, on the same scale as the rest of the Oriental population; soldiers shrink with
  casualties. With them in the city, «The New Troy» below gives +35% births and -35% mortality (not ±50%), to keep
  Montevideo near a quarter of the country in 1852.

- **The war fills Montevideo and empties the countryside:** Montevideo started 1836 with 19% of the Banda Oriental's
  people and was down to 7-8% by 1852, while the countryside nearly doubled; the 1852 census counted about 26%
  (33,994 of ~132,000). From the declaration of war on Rosas (February 1839) until the peace, Montevideo -- while the
  Cerrito does not hold it -- has «The New Troy» (+100% migration attraction, +35% births, -35% mortality: the
  refugees and the European immigrants behind the walls) and the other four Oriental states have «The Ravaged
  Countryside» (-50% migration attraction, -50% births, +75% mortality: levies, slaughtered herds, families gone to
  Brazil and Entre Ríos). Both end with the peace. Games in progress in the middle of the war get them within six
  months.
- **Caseros keeps its date under the Pact rules:** with a Pact rule that ends it by war (Historical, Rosas wins, Two
  governments), an AI Rosas could still answer Caseros by holding Buenos Aires, a siege of six months or more that the
  rule's closing date does not cut short, and the Historical settlement came in August 1852. The AI no longer takes
  that road under these rules, and under Historical it fights the battle, as on 3 February 1852. A player can still
  choose any answer.
- **No errors from leaderless interest groups in party choices:** when a revolt's interest group had no leader (East
  India's radicals in 1857), the conservative and liberal parties' join weights, copied from the Community Mod
  Framework, logged an error every day. The check now skips a group with no leader.
- **Other mods' wars stay out of the Guerra Grande:** diplomatic plays and war goals added by optional mods of your
  playset (recognition wars, holy wars, Hispanic American unification, installing a dictator, scripted revolutions...)
  could open an engine war on the Oriental governments, or between Brazil and the Riograndense Republic before Ponche
  Verde. The same rule the base game's plays follow is now enforced when any play starts, when a country joins one and
  when a war goal is added, whatever mod the play comes from: a play that breaks it is called off, and a country that
  must stay out is taken off its side. The mod's own wars, civil wars and the base game's plays are unchanged.
- **La Plata is still Argentina:** after proclaiming La Plata or Great Argentina from Argentina, three things that
  only recognised the Argentine tag stopped: the local-caudillos army model (the law became unavailable, and the
  engine's fallback would have cut the barracks), the Pact provinces marching to their overlord's foreign wars, and
  the national territories becoming provinces under the confederation. They now follow the Argentine state under
  any of its names; if the formation still drops the local caudillos, the law is put back the same day and checked
  again the next month. A La Plata formed by Paraguay is not affected.
- **Bernardino Caballero is spelt right:** the Paraguayan general (who also serves Argentina, La Plata or Great
  Argentina holding Asunción) was named «Cabellero», a typo inherited from vanilla's template. New games show
  Caballero; a Caballero already in a save keeps the old spelling.
- **The historical men die on their date:** Rosas (1877), Oribe (1857), Rivera (1854), Suárez (1868), Urquiza (1870),
  Brown (1857), Lavalleja (1853), Mitre (1906), Flores (1868), Herrera y Obes (1890), Sarmiento (1888), Paz (1854) and
  now Nazario Benavídez (1858) die on the first month after their historical death; before, the game only stopped
  protecting them and Oribe was still alive in 1869. A dead man is never recreated to fill a seat. Games in progress:
  whoever is already past his date dies next month.
- **No duplicate historical figures with «Expanded Characters & Commanders of Historical Importance Redux»:** that mod's
  own copies of figures the game already has (Berro, Sarmiento, Roca, four Peruvian presidents and 39 more worldwide,
  plus Artigas, who never came back from Paraguay) no longer appear; the game's or this mod's version stays.
- **The Uruguayan postwar is the Republic's:** Oribe's four-year mandate, the handovers, «the caudillos come back» and
  the elections no longer run on the Oriental Province of the Pact or on an absorbed Banda Oriental. The Cerrito still
  takes back Uruguay's name and the Oriental Province keeps its Pact ties: only the Republic's politics are skipped.
- **Urquiza's war mark is cleared after the Pact:** it stayed set for good, and a later Argentine capitulation to Entre
  Ríos (Cepeda, Pavón) would have been read as Urquiza winning the Pact.
- **One ruler at a time:** a head of state moved into another country kept his office: Oribe (the Oriental
  Province's governor) and Joaquín Suárez (the Defensa's president) sat in Argentina from 1853 on still marked as
  rulers beside the real one. Characters brought over by an annexation now leave the ruler and heir roles behind;
  games in progress are fixed on the next month.
- **The siege guns leave Montevideo with the peace:** the «Guns of the Plaza» (+250 bombardment resistance) sit on the
  state of Montevideo and were never removed, lasting until 1858 after an 1850 peace. They now go with the rest of
  the siege's modifiers, also in games in progress.
- **The Republic's historical presidency ends with the Republic:** after the Oriental Province was absorbed, the mark
  that keeps Uruguay's historical presidents in the chair stayed on for good, so a Uruguay released later would have
  had Rivera forced into its presidency. It now ends when neither Oriental government exists.
- **More historical lives:** Mitre (to 1906), Venancio Flores (1868), Manuel Herrera y Obes (1890), Sarmiento (1888)
  and Paz (1854) no longer die before their historical date, like Rosas, Oribe, Rivera and the others.
- **Annexed provinces keep their men:** when Argentina (or Entre Ríos, or Brazil with the Farrapos) absorbed a
  province, the engine deleted every character the province had: in Juan's game Urquiza, Mitre, Sarmiento and Paz
  vanished with Entre Ríos. Every annexation of the mod now moves the province's characters to the annexer first,
  as the Oriental Province already did. Characters already lost in a save do not come back.
- **Paraguay's, Bolivia's and Chile's historical figures come to the country that absorbs them:** their politicians
  and generals (and Paraguay's five commanders of 1855-1880) now also appear for Argentina, La Plata or Great
  Argentina holding Asunción, La Paz or Santiago. Chile's templates carry la Argentina's map home regions.
- **Uruguay's historical figures still come when Argentina absorbs the Banda Oriental:** the 21 Uruguayan
  politicians and generals the game brings over the years (Herrera y Obes, Lamas, Berro, Flores, Varela, Batlle…)
  came only for Uruguay or a La Plata holding Montevideo; now also for Argentina or Great Argentina holding it.
- **Rosas is mortal again:** the historical lives (Rosas until 1877, Urquiza until 1870…) were kept only while
  Uruguay or Argentina existed; with the Oriental Province absorbed and La Plata formed, nobody cleared them and Rosas
  reached 98. Now they are cleared whatever countries remain. Games in progress are fixed on the next month.
- **Montevideo, the port-city:** splitting la Argentina's Montevideo left it 6 provinces and 8 arable land; it ran
  short of infrastructure (8.8 against 23.8 in use by 1891) and stopped growing (132,000 people by 1891; the 1889
  census counted 215,061). It now has a permanent «The Port-City» modifier: +25 infrastructure, +50% migration
  attraction, +10% urban centre and port throughput. Also reaches games in progress within six months.

## 0.1.5-alpha — 25/9/2026

- **The Malvinas journals work for La Plata:** la Argentina's two Malvinas journals checked only Argentina's tag;
  La Plata and Great Argentina now keep them.
- **La Plata keeps Argentina's party names:** a La Plata formed from Argentina now has the same period names (Federal
  and Unitarian parties, then Nationalist and Autonomist) instead of the game's generic ones.
- **Uruguay's roads follow its real routes:** the travel network of the five Oriental states is redrawn along
  the national routes and old caminos reales — Ruta 1 to Colonia, Ruta 3 to Paysandú and Salto, Ruta 5 through
  Florida and Durazno to Tacuarembó and Rivera, Ruta 7 and Ruta 8 to Minas, Treinta y Tres and Melo, Ruta 9 to
  Maldonado, Rocha and the Chuy, Ruta 26 across the north — with natural curves instead of straight lines, and
  crossings at Colón, Nueva Palmira, Bella Unión, Rivera, Aceguá, Jaguarão and the Chuy. Map data: takes effect in
  a new game.
- **La Plata's formation panel shows the real size:** it listed 21 states and asked for 7; it now lists the 31 that
  can count and asks for 17 (7 required + 10 provinces or settled frontier). The exact rule is unchanged.

## 0.1.4-alpha — 25/9/2026

- **Armies can march into San José and Maldonado again:** the travel network (the roads and railways armies move
  along) came from la Argentina's map, which has no San José or Maldonado and still ran Montevideo's roads through
  land that is now theirs; the two states had no travel node at all, and Paysandú was linked to Montevideo, which it
  no longer borders. The mod now ships its own network: every Oriental state has its hubs where its towns are, roads
  inside each state and one road to every neighbouring state. Map data: takes effect in a new game.
- **Forming La Plata no longer waits on half-colonized frontier:** La Plata (PLT) now asks for all five Oriental
  states and both Paraguayan states, plus 10 of the 14 historical Argentine provinces. Each missing province can be
  made good by a frontier state (La Pampa, Neuquén, Río Negro, Chubut, Santa Cruz, Tierra del Fuego, Misiones, the
  Chaco, Formosa or Rio Grande do Sul) that you hold and have colonized at least 75%; frontier land is never
  required, and a colony below that share does not count. States held by a puppet, vassal or client that the
  formation annexes count as yours.
- **A new flag for La Plata:** the La Plata country (PLT) now flies five stripes — red, white, sky blue, white, red —
  with the Sol de Mayo, in every situation and under every government, instead of la Argentina's and Dynamic
  Names, Flags & Colours' flags. Credits in CREDITS.md.
- **The independence of Paraguay:** on 17 July 1852, the day Santiago Derqui signed the act of recognition in
  Asunción, whoever conducts the Confederation's foreign relations once the Pact is settled is asked to recognize
  Paraguay or withhold assent. Urquiza's Argentina gets it as history had it; with two governments, Urquiza's
  Confederation, not Rosas's Buenos Aires; Rosas, if he is still in the seat, answers in the words of his note of
  1843. Recognizing improves relations with Paraguay (+30) and Brazil (+10) and drops any Argentine claim on ground
  wholly Paraguayan. Withholding costs 5 infamy, worsens relations with Paraguay (−30) and Brazil (−10), and claims
  every region wholly Paraguayan as a rebel province; the Chaco and regions shared with Brazil are never touched.
  The AI recognizes nine times in ten, unless Rosas rules. If the settlement comes late or Paraguay is at war with
  the recipient, the question waits, until June 1856 at the latest. Games already past July 1852 get it on the next
  monthly pulse.
- **Each province flies its first provincial flag under the confederation:** while the confederation stands, every
  Argentine province country flies the first flag of its own it ever had, whatever the year — Tucumán's «TUCUMAN
  1814», Santa Fe's and Corrientes's of 1815, the federal flag of Ramírez's Entre Ríos, Andresito's flag in Misiones,
  Córdoba's 1815 tricolour, and the first provincial flag of the rest, however recent. A deliberate anachronism, so
  the confederation does not show the same flag twenty times. Outside the confederation nothing changes. Thirteen new
  flags, real Wikimedia images; credits in CREDITS.md.
- **Argentine party names by period:** the game named Argentina's parties after organisations of 1874-1891 from
  1836 on. Now the Federal Party (conservative) until 1874, the Unitarian Party (liberal) until 1862, the Nationalist
  Party (liberal, Mitre) 1862-1889 and the Autonomist Party (radical, Alsina) 1862-1891; the game's own names follow.
  Works in games in progress.

## 0.1.3-alpha — 24/9/2026

- **Rosas serves a first term under the Constitution of 1853:** if he is in the seat when he gives it, he governs the
  six years its art. 74 sets, and is put back after every election until the term ends; after it the elections decide,
  re-election neither forced nor forbidden. Before, the vote the constitution brings unseated him the next day. Games
  that already gave the constitution with Rosas alive get his term back once, to 31 May 1857.
- **The constitution comes about eleven months after the Pact is settled** (the distance between the San Nicolás
  Agreement, 31 May 1852, and the Constitution, 1 May 1853), not one. After Urquiza's victory or the negotiated
  confederation there is no separate question about the provinces any more: as in 1853, the constitution incorporates
  them, and until then they stay Provinces of the Pact. «The Negotiated Confederation» is one event now, not two.
- **The Cisplatine question comes first:** while Brazil waits for its moment over the Banda Oriental, neither the
  constitution nor the question of the provinces is asked; they come once it is settled.
- **Fewer duplicate notices at the end of the war:** a power's change of level is told in the event that caused it
  (Arana-Southern, Arana-Lepredour) instead of in a window of its own; Buenos Aires no longer gets «The River Closed»
  when its own shore closed it; the Arana-Southern treaty reaches Rosas the day it is signed, in the present tense.
- **Fixes:** the historical lives (and Rosas's seat) are kept after the Oriental Province is absorbed; the loan
  accounts come with the peace instead of up to four months later; the constitution no longer promises to
  incorporate provinces already incorporated; the question of the provinces names the Oriental Province and has its
  own text after a negotiated settlement.

- **National territories become provinces under the confederation:** when Argentina chose the confederation, a
  territory Buenos Aires governs directly — La Pampa, Neuquén, Río Negro, Chubut, Santa Cruz, Tierra del Fuego,
  Misiones, Formosa or the Chaco — asks to become a province once its population reaches 60,000 (the figure of the
  1884 national territories law, art. 4) and its market access 75%. Granted, it becomes its own country, a Province
  of the Pact under Buenos Aires, with its land incorporated. The AI always grants it; a player may make it wait five
  years, at a cost in the territory's radicals. Checked once a year, only while the confederation stands and at peace.

- **Brazil's note reaches Buenos Aires:** when the Banda Oriental rejoins the Confederation and Brazil answers under
  the Preliminary Peace Convention of 1828, Argentina now hears of it. If the Empire stays out, its protest arrives;
  if it chooses war, a note that breaks off relations and reserves the right to enforce the Convention. Buenos Aires
  answers with a conciliatory note (better relations with Brazil and a calmer Entre Ríos, but the provinces grumble)
  or rejects it (worse relations, the provinces close ranks, and Brazil gains a pretext with Entre Ríos before
  1 May 1851). Games in progress where Brazil already answered get the note once.
- **Brazil intervenes more often** over the Banda Oriental: staying out is now about half as likely for the AI.
- **The constitution can be a confederation:** a new answer to «The Constitution», «The Pact of 1831 and nothing
  more». No constitution is written: every historical province becomes its own country again, a Province of the
  Pact under Buenos Aires, which keeps the foreign relations; Buenos Aires keeps its own province and the frontier
  lands (La Pampa, Río Negro, the Chaco). It also works after the provinces were incorporated in 1851, and a
  Coalition under Buenos Aires splits into its provinces. Offered unless the Pact ended with Urquiza's victory or
  with two governments; a player's province is never forced. After Rosas's victory he keeps the sum of public power
  and the question reopens at his death. The AI takes it rarely, and never under a forced Pact rule.
- **Reincorporated provinces are incorporated states:** when Argentina (or Urquiza's Confederation, or the Argentina
  that remains after the Buenos Aires war) annexes a province of the Pact — the national organisation of 1851, the
  constitution, the Coalition, the Oriental Province — its states become incorporated at once instead of showing as
  unincorporated. Only the historical provinces (and the Banda Oriental once it rejoined as a province) are affected.
  Games in progress are repaired once on the next monthly tick.
- **Small fixes:** Provinces of the Pact now show Buenos Aires's map colour; missing names for the Río de la Plata
  strait and the provinces' AI strategy.
- **The great malón (la Argentina's `mapuche_malon.1`) is rarer:** at most once every 5 years per country, and only
  for a country that borders an independent Mapuche country. It used to come about every two years (5% a month with
  a 3-month cooldown, ~9 in 1836-1852); now ~3 in 1836-1852, never more than 2 in 10 years, in line with the relative
  peace of the Buenos Aires frontier under Rosas's «Negocio Pacífico de Indios». Done by overriding la Argentina's
  `common/journal_entries/00_malon.txt` (only its monthly pulse changes); their event and texts are untouched.

## 0.1.2-alpha — 24/9/2026

- **Oriental Province** (when the Cerrito wins and Argentina takes it as a province): annexed with the rest of
  the Pact by every incorporation path, with Oribe, his army and his characters; its ruler is Governor, not
  President; in Urquiza's uprising it fights for Rosas. Games in progress are asked the incorporation question
  again.
- **Allied provinces:** provinces subject to Argentina join its foreign wars (Brazil, the Defensa, France,
  Britain…), attacking or defending, never wars between Argentines.
- **Subjects that survive:** the vassals, protectorates and puppets the engine silently dropped now use their own
  types: Pact Province, Vassal State, Cisplatine Province, Client State.
- **The constitution:** Rosas can choose (no constitution, or call the congress of the 1831 Pact); under «Two
  governments», a constitution for the State of Buenos Aires. It waits until the war with Brazil ends.
- **The Brazilian loan:** if the Defensa takes it, the Empire enters the war against Oribe in 1851, with or
  without the convention with Entre Ríos.
- **Urquiza alone:** if the Cerrito has won before 1 May 1851 and Brazil is not committed to him, Urquiza decides
  whether to rise (AI: usually not; the player chooses). Under the forced Pact rules the rule still decides.
- **Legions:** the Defensa AI reinforces them only under pressure.
- **Cleanup:** the leftovers of the no-Argentina mode are gone; English thumbnail.

## 0.1.1-alpha — 24/9/2026 (hotfix)

- If the Cerrito wins and Argentina takes it as a province, it now stays an Argentine province (the engine used
  to free it) and is named «the Oriental Province» (Law of Union, 25/8/1825).

## 0.1.0-alpha — 24/9/2026

- First public alpha. The Guerra Grande of the Río de la Plata, both banks: Carpintería, the split between the
  Defensa and the Cerrito, the siege of Montevideo, the Plata question with the powers, the Federal Pact,
  Urquiza's Pronunciamiento, Caseros and Buenos Aires apart until Pavón.
- Requires Community Mod Framework and la Argentina (the old compatch is now part of the mod).
