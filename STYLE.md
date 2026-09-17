# Naming convention / Convención de nombres

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

## ES — Nada que glosar

En español no hay nada que explicar: blanco, colorado, la Defensa y el Cerrito son los
nombres, a secas. La regla en español es la inversa — **no** anglicismos y **no**
explicaciones de lo que el lector ya sabe.

## Por qué existe este archivo

Cuatro agentes en paralelo escribieron texto para este mod el 2026-09-16 (abolición,
asimetría del sitio, empréstitos, legiones) sin poder verse entre sí. Sin una convención
escrita, cada uno resuelve el problema de nombrar a los bandos por su cuenta y el mod termina
llamándole tres cosas distintas a lo mismo. `tools/validate_mod.py` verifica la parte
mecánica de esta regla.
