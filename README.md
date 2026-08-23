# Hearth

**Pet Village Builder** — Isometric homeland where off-duty pets build, nap, and receive visitors.

Part of the [ComputerPets](https://github.com/RicheyWorks/computerpets) universe. Map: [computerpets-ecosystem](https://github.com/RicheyWorks/computerpets-ecosystem).

> Status: **design scaffold**. Gameplay contract is frozen. Engine choice is the one in the brief. Implementation comes next.

## Loop

When a pet is not on the desktop, it is in Hearth. Buildings are habitats from Lore. A reef house will not accept Rui as a resident.

## Genre & engine

- Genre: **Isometric management**
- Engine: **Phaser.js**
- Stack: TypeScript · Phaser 3 isometric · off-duty pets as villagers · Visitation as visitors
- Default surface: `8080`

## How you play

1. Assign idle pets to plots.
2. Build biome-legal structures.
3. Visitors from Visitation walk through.
4. Desktop recall yanks a villager back to overlay.

## Talks to

- computerpets-visitation
- computerpets-lore
- computerpets-acre
- computerpets-inn
- computerpets-companion

## Failure doctrine

Recall during build → job pauses, not lost. Illegal biome assign → ghost plot, no crash. Save is cloud + local.

Canon rules that never yield:

- 210 living kinds. No illegal hybrids.
- Overlay pets can get tired, sick, or hide. Tokens are not burned by a minigame.
- Desktop walk stays the main quest. Closing Hearth must leave Rui walking.

## Layout

```
computerpets-hearth/
  README.md
  LICENSE
  docs/DESIGN.md
  src/                implementation lands here
```

## Run (Windows)

```powershell
cd app; npm install; npm run dev
```

Meet Rui first via the [flagship start-here](https://github.com/RicheyWorks/computerpets/blob/main/docs/START-HERE.md). This game is optional.

## License

MIT. See [LICENSE](LICENSE).

---

*Two hundred ten living kinds. Keep them so a line does not go quiet.*
