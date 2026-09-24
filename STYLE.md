# Naming convention

## EN — Gloss once, then never translate

The four names at the centre of this war are Spanish and stay Spanish in the English
localization. Each is explained **exactly once**, at the moment the player first meets it,
and from then on it is used bare.

| Term | Glossed once in | Afterwards |
|---|---|---|
| `blanco` | `guerra_grande.1.d` — Carpintería: *"The white ribbon makes a blanco, the red one a colorado — the plain Spanish for white and red…"* | `blanco`, `blancos` |
| `colorado` | the same line | `colorado`, `colorados` |
| `la Defensa` | `guerra_grande.3.d` — the split: *"the Gobierno de la Defensa — the government of the defence, and the Defensa from here on"* | `the Defensa` |
| `el Cerrito` | the same paragraph: *"out on the little hill that gives it its name… the Gobierno del Cerrito"* | `the Cerrito` |

**Never write** "the Whites", "the Reds", "the White Party", "the Red Party", "the Defence
Government" or "the Hilltop Government". A player who has read the Carpintería event knows
what a blanco is; translating it afterwards makes two different things out of one.

Ordinary uses of the words *white* and *red* — a white ribbon, the red lining of a poncho,
Garibaldi's red shirts — are literal description, not faction names, and are fine.

The same rule covers the other Spanish terms the mod uses as things rather than as
translations: `divisa`, `saladero`, `estancia`, `caudillo`, `Villa de la Restauración`. Gloss
on first use if the meaning is not obvious from context, then leave them alone.

## ES — Nothing to gloss

In the Spanish localization there is nothing to explain: blanco, colorado, la Defensa and el Cerrito
are simply the names. The Spanish rule is the reverse — **no** anglicisms and **no** explanations of
what the reader already knows.

## Why this file exists

On 2026-09-16 four agents working in parallel wrote text for this mod (abolition, the asymmetry of
the siege, the loans, the legions) without being able to see one another's work. Without a written
convention, each one settles the question of what to call the two sides on its own, and the mod ends
up calling the same thing by three different names. `tools/validate_mod.py` checks the mechanical
part of this rule.
