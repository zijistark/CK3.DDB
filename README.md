# DDB: Depth, Difficulty & Balance

DDB is a mod for [Crusader Kings III](https://www.crusaderkings.com/) focusing primarily upon, as the tentative name goes, the issues of gameplay depth, difficulty, and balance. For now, it's my personal, unpublished mod intended for the campaigns of my friends and myself. I wanted to start sanitizing some of the worst issues with vanilla CK3, so here we are.

Again, note that this is a pre-release, WIP mod, and it certainly does not tackle all of the 3 issues in its name yet. However, the [GitHub Releases](https://github.com/zijistark/CK3.DDB/releases) are considered stable, so feel free to download the latest of the [GitHub Releases](https://github.com/zijistark/CK3.DDB/releases), extract the downloaded archive into your mod folder[1], and play with it.

[1] Note that GitHub adds an additional top-level folder inside the ZIP called something like `CK3.DDB-0.1.0/` or `CK3.DDB-master/`, depending upon how you downloaded it. When using your unzipping program, unzip only the _contents_ of that folder directly into your mod folder: you want `DDB.mod` and the `DDB/` folder to be directly inside your mod folder.

A cumulative changelog for released versions can be found in the [DDB_CHANGELOG](https://github.com/zijistark/CK3.DDB/blob/master/DDB/DDB_CHANGELOG.md) file.

## Features

### Faith & culture

- Faiths' monthly Fervor gain is penalized less for being large
- Sinful Bishop / Virtuous Priest events are more balanced and relevant

#### AI conversion to local / nearby cultures & faiths

- Mechanic to track successful Crusades/Jihads/GHWs in order to allow robust testing of whether a given character is part of an intact Crusader state
  - Used in a few key places to block assimilation of local/nearby cultures and/or faiths
  - Stops vanilla's nearly instantaneous conversion of Crusader states to local religion & culture
- Given reason, less likely to convert to their capital's foreign culture
- While losing a defensive war, less likely to convert to the attacker's faith
- Now less likely to take the conversion option of Populist Faction ultimatums if they have similar military power

### Miscellaneous

- Empires can no longer be auto-created by Confederate Partition
- Dynasty prestige: less snowballing, but vassal dynastic rulers now make their own contribution to Renown gain as well
- Bonuses from Development now favor tax over levy output
- Harder to instantly win wars just by capturing heirs
- Army rally times are more realistic if the levies are traveling from afar
- If you want decent levy output from a County, then maintaining high Control is much more important (less snowballing)

## Compatibility

Compatible with any mod which does not override the same vanilla files. This may change in the future as the mod expands in scope: in the future, some behavioral-level stuff might also cause an incompatibility; you'd be alerted to any such change in the changelog for a release or in the [cumulative changelog](https://github.com/zijistark/CK3.DDB/blob/master/DDB/DDB_CHANGELOG.md) as well.

All pro-compatibility measures that the game allows have been employed.

## Author

I am **zijistark**, known to the real world as Matthew D. Hall. Among my modding exploits for the _Crusader Kings_ franchise, I'm the leader of the [Historical Immersion Project](http://hip.zijistark.com/) and its core gameplay/mechanics module, EMF, for CK2.

I'm also actively developing and maintaining a few mods for [Mount & Blade II: Bannerlord](https://www.taleworlds.com/en/Games/Bannerlord) in addition to working upon framework libraries for other Bannerlord mods to leverage.

I'm a developer / programmer / engineer by trade, so I take my code very seriously. From me, you can always expect not only high-quality code but also rigorous testing of every component of it.
