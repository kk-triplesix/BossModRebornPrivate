# BMR KK's Special

A private fork of [BossModReborn](https://github.com/FFXIV-CombatReborn/BossmodReborn) by the FFXIV Combat Reborn team.

I absolutely love and appreciate the original project — the Combat Reborn team has done an incredible job building and maintaining BossModReborn. This fork exists solely because I needed a few very specific customizations for my own personal use.

---

## What's Different

### Extended IPC Layer

Deep integration with [RotationSolverReborn](https://github.com/FFXIV-CombatReborn/RotationSolverReborn) through custom IPC endpoints:

- **Encounters IPC** — exposes encounter data (phases, mechanics, timings) for external rotation planners
- **AIHints IPC** — channels for raidwide/tankbuster/stack predictions, SpecialMode, and ForbiddenDirections
- **ActionQueue IPC** — `HasEntries` method for rotation solver coordination
- **Configuration IPC** — `LastModified` tracking for external config consumers
- **Preset Management** — full CRUD for rotation presets, active preset control, strategy management
- Gaze/Pyretic RSR integration for automatic rotation pausing

### WIP Boss Modules

Unreleased Dawntrail encounter modules in progress:

- **Criterion:** Darya the Sea Maid (AlluringOrder, AquaSpear, CeaselessCurrent, EchoedSerenade, SeaShackles)
- **Advanced:** Darya the Sea Maid, Lone Swordmaster, Pari of Plenty
- **Variant:** Darya the Sea Maid, Lone Swordmaster
- **Savage:** Enhanced M12S P1 Lindwurm (GrotesquerieAct1), M11N, M09S, M10S

### Plugin Branding

- Renamed to "BMR (KK's Special)"
- Author set to kk-triplesix

### Automated Upstream Sync

- Syncs with the original repo every 2 hours automatically
- Preserves all local changes on conflict (merge strategy: ours)
- Auto-increments version tags
- Custom CI/CD pipeline with release artifact generation

---

## Credits & Thanks

Huge thanks to the **FFXIV Combat Reborn team** for creating and maintaining the original [BossModReborn](https://github.com/FFXIV-CombatReborn/BossmodReborn). Their work is the foundation this fork is built on.

Original repository: https://github.com/FFXIV-CombatReborn/BossmodReborn
