# Changelog — The Guerra Grande · the Río de la Plata, 1836-1862

## Unreleased

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
