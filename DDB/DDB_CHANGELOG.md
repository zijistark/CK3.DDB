# DDB: Changelog

## v0.1.0

- Added mechanic to track victorious Crusades (GHWs, in general)

  + For now, this is used so that script can easily test whether a given character is part of an intact Crusader state, which is flexibly defined but also careful to exclude titles from prior Crusades that are no longer really Crusader states, in order to block the main sources of Crusaders' assimilation of local/nearby cultures & religions.

  + Works with dynamic Crusader State titles as well

  + For AI Crusaders, this currently blocks the Populist Faction ultimatums' conversion option, converting to attacker religion in a losing defensive war, and rulers' conversion to their capital's foreign culture.

- AI's more reluctant to take Populist Faction ultimatums' conversion option if they have similar military strength to the faction.

- AI's more reluctant to convert to attacker religion while losing a defensive war.

- AI's more reluctant to convert to a foreign culture in their capital province. Several new, plausible AI chance modifiers have been added to achieve this (and some vanilla bugs were fixed).