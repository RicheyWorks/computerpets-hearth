# Hearth design

Implement against this file, not folklore.

## Identity

- Product: **Hearth**
- Repo: `computerpets-hearth`
- Idea: Pet Village Builder
- Genre: Isometric management
- Engine: Phaser.js
- Surface: `8080`

## Loop

When a pet is not on the desktop, it is in Hearth. Buildings are habitats from Lore. A reef house will not accept Rui as a resident.

## Play beats

- Assign idle pets to plots.
- Build biome-legal structures.
- Visitors from Visitation walk through.
- Desktop recall yanks a villager back to overlay.

## Neighbors

- computerpets-visitation
- computerpets-lore
- computerpets-acre
- computerpets-inn
- computerpets-companion

## Failure doctrine

Recall during build → job pauses, not lost. Illegal biome assign → ghost plot, no crash. Save is cloud + local.

## Hard rules

1. Minigames cannot mint or burn NFTs by themselves (Minter is the write path).
2. Stats come from lived overlay care + Dojo caps, not cash shop.
3. Species kits stay inside Lore. Illegal hybrids never spawn.
4. Fail soft: the desktop overlay process is not this process.
