# DDB: Changelog

## v0.2.0 [BETA]

- Sinful Bishop / Virtuous Priest events
  + Both event chains should now fire at approximately equal rate given a faith with approximately equal sinful and virtuous priests
  + Frequency of these events now scales logarithmically with faith size instead of linearly
  + Overhaul of bishop selection modifiers to generally improve the relevancy of the chosen bishop to their faith
  + Modified the amount of fervor change due to the events, previously always ±10, to be:
    * ±20 if priest is head of the faith
    * ±10 by default
    * ±5 if priest is a Count or realm priest to a Count
    * ±3 if priest is a Baron

## v0.1.0

- Added mechanic to track victorious Crusades (GHWs, in general)
  + For now, this is used so that script can easily test whether a given character is part of an intact Crusader state, which is flexibly defined but also careful to exclude titles from prior Crusades that are no longer really Crusader states, in order to block the main sources of Crusaders' assimilation of local/nearby cultures & religions.
  + Works with dynamic Crusader State titles as well
  + For AI Crusaders, this currently blocks the Populist Faction ultimatums' conversion option, converting to attacker religion in a losing defensive war, and rulers' conversion to their capital's foreign culture.

- AI's more reluctant to take Populist Faction ultimatums' conversion option if they have similar military strength to the faction.

- AI's more reluctant to convert to attacker religion while losing a defensive war.

- AI's more reluctant to convert to a foreign culture in their capital province. Several new, plausible AI chance modifiers have been added to achieve this (and some vanilla bugs were fixed).
