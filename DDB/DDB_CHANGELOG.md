# DDB: Changelog

## v0.2.0

- Compatibility patch for CKII v1.1

- Empires can no longer be auto-created by Confederate Partition Succession

- Sinful Bishop / Virtuous Priest events
  + Both event chains should now fire at approximately equal rate given a faith with approximately equal sinful and virtuous priests
  + Frequency of these events now scales logarithmically with faith size instead of linearly
  + Overhaul of bishop selection modifiers to generally improve the relevancy of the chosen bishop to their faith
  + Modified the amount of fervor change due to the events, previously always ±10, to be:
    * ±20 if priest is head of the faith
    * ±10 by default
    * ±5 if priest is a Count or realm priest to a Count
    * ±3 if priest is a Baron

- Defines tweaks:
  + Dynasty Prestige / Renown:
    * Dynastic rulers who are vassal or below of another same-dynasty ruler now contribute toward the gain of Renown (previously, zero contribution). Their contribution is 20% of what it would be if they didn't have a dynastic ruler above them, however.
    * Halved the monthly gain of Renown per living dynasty member. Gain is equal to 1% of living dynasty member count instead of 2%.
    * The maximum long reign opinion bonus now increases from 5 at the lowest Level of Splendor to 35 (previously 55) at the highest level (+3 max. opinion per level instead of +5).
    * Halved character prestige gain upon birth due to Dynasty Prestige (10% of it instead of 20%)
  + Levies now traverse -75% fewer map distance units per day when rallying; it now takes longer to rally from afar.
  + At 0 Control, a County's levy will only provide 15% of its potential troops (instead of 50%)
  + Development's bonus to levy output has been reduced while its bonus to tax output has been increased. At the ideal of 100 Development:
    * Levy bonus is +30% (instead of +50%)
    * Tax bonus is +70% (instead of +50%)
  + Fleets now start losing supply after 10 days instead of 30.
  + Religion:
    * The equation for a faith's size's impact upon Fervor gain has been altered to penalize large faiths less than previously (e.g., in 1066 the monthly Fervor gain for Catholicism has doubled)
    * Heads of faith now get 1.5 Piety monthly instead of 1 Piety monthly.
  + Levy penalties for being over your Vassal Limit have been removed; it is a source of exploits and janky behavior. Tax penalties still apply.
  + Warscore for capturing an heir of the enemy is now 25%, 15%, and 10% for the first, second, and third in the line of succession. Previously, it was 50%, 25%, and 10%, respectively.


## v0.1.0

- Added mechanic to track victorious Crusades (GHWs, in general)
  + For now, this is used so that script can easily test whether a given character is part of an intact Crusader state, which is flexibly defined but also careful to exclude titles from prior Crusades that are no longer really Crusader states, in order to block the main sources of Crusaders' assimilation of local/nearby cultures & religions.
  + Works with dynamic Crusader State titles as well
  + For AI Crusaders, this currently blocks the Populist Faction ultimatums' conversion option, converting to attacker religion in a losing defensive war, and rulers' conversion to their capital's foreign culture.

- AI's more reluctant to take Populist Faction ultimatums' conversion option if they have similar military strength to the faction.

- AI's more reluctant to convert to attacker religion while losing a defensive war.

- AI's more reluctant to convert to a foreign culture in their capital province. Several new, plausible AI chance modifiers have been added to achieve this (and some vanilla bugs were fixed).
