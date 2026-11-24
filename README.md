# No Easy Fix

Version 2.0.0. A mod for HBS BattleTech / BEXT that makes repairs and refits more in line with canon, limits the ability to reconfigure non-OmniMechs, and adds faction refit kits for later variants.

No Easy Fix treats a standard BattleMech as a hard to modify stock model. You can still repair it, change its armour, and swap gear that fits the space the stock loadout already used — but you cannot add extra weapons or equipment in leftover empty slots, with only OmniMechs able to modify that leftover space. Changing a location to a different kind of weapon or gear is an expensive refit; while repairs and like-for-like swaps stay at normal cost.

This makes 'Mech repair much harder, especially in the early game, and is designed to give more of a canon feel to 'Mech repair and refit. Saved refitted 'Mechs, and those refitted and sent to storage, retain their final space configuration and are not reverted to a stock layout in existing saves.

Version 2.0.0 keeps the slot lock feature and adds refit kits. Both are on by default in the mod, however, each can be turned off on its own.

## Slot lock

BattleTech lets you fill every empty inventory box a chassis has, if you can, so a stock 'Mech can grow a lot of extra guns once you own it. No Easy Fix puts the factory layout back in charge for ordinary BattleMechs, and leaves OmniMechs as the machines that can still use leftover space.

On a standard BattleMech, each location may only use as much inventory space as that variant already used in its published stock loadout. Though leftover empty boxes still appear on the silhouette, they are locked and cannot have equipment placed in them. You may pull a weapon and put something else in that location if it fits the same budget (for example an AC/10 where an AC/20 sat). You cannot add a small laser to an unused support hardpoint, hang gear on an empty arm, or stuff extra heat sinks into space the stock kit never used.

You can still repair components, structure, and armour at normal prices; strip and rebuild within the stock budget; swap like for like (any Medium Laser for a Medium Laser, ammo for the same ammo); and fit a smaller item into a larger stock space, with the unused remainder staying locked. Heat banks and similar heat gear can use locations that already had heat sinks, if they fit. Targeting computers, TTS, C3, ECM, and other electronics and mods are not treated as extra guns in empty structure.

You cannot add extra weapons, ammo, jump jets, or heat sinks into leftover empty slots, or turn an unused hardpoint into a new mount unless that location still has unused stock budget.

OmniMechs are unchanged by the lock: leftover space still works, and Omni-style installs stay cheap.

Refit cost: standard repair costs remain the same, and same-kind swaps stay at the usual install price (for example a Medium Laser++ for a Medium Laser). Installing a different kind of thing in that location is a type-change refit and costs more C-bills and shop time (for example a medium pulse laser where a standard medium laser sat). Moving gear is charged as an install at the destination.

The MechLab shows tinted stock ghosts for where the factory gear sat, a short bar on locked leftover tiles, and a location label for how much of the stock budget is in use. F8 fades the live kit so you can read the factory layout.

Existing customized 'Mechs in your save keep what they have and cannot grow further. New machines use the published stock layout. The mod does not turn Omnis into free-form pod 'Mechs, rewrite chassis files, or fill empty crits with dummy equipment.

## Refit kits

A faction's stores sell kits that turn an older hull into a later variant of the same chassis. Steiner stores sell Steiner kits, Davion stores sell Davion kits, and the same is true for the other Houses, ComStar, the Word of Blake, Wolf's Dragoons, and the St. Ives Compact. The black market does not sell kits.

A kit joins that faction's pool in the year it is announced and the world type determines how many kits are drawn:

- A House capital: six.
- One of the House's other capitals: four.
- A factory world: four.
- A manufacturing world: three.
- A research world: two.
- Any other world that House owns: one.

Each draw is weighted by how long the kit has been available. A kit that has been out longer is more likely to be drawn than a newly announced one. The same kit can be drawn more than once, and the store then offers that many copies.

The store price starts high and falls over eight years: 110 percent of a new chassis in the announcement year, then 100, 95, 90, 85, 80, 75, and 70 percent from the eighth year on.

Fitting the kit is a separate job in the mech bay. Ready an older hull of that chassis, choose the kit, and the bay bills 60 percent of a new machine, less the sale value of the parts you add to the kit yourself, as the refit cost. That bay bill does not fall when the store price does. A kit is not installed by dragging it onto the 'Mech.

This means that a refit costs from 1.7-1.3 times buying a 'Mech from a factory, however, kits are available everywhere, providing convenience over cost.

A finished kit produces a new hull. If the slot lock is on, that hull is measured from its own stock layout the first time you open it.

On 1 January, from 3049 onward, the Kit Bash circular lists the kits announced that year.

## Turning the parts on and off

Both parts are on in Version 2.0.0. In `Mods\NoEasyFix\mod.json`, under `Settings`:

- `EnableSlotBudget` — the leftover-slot lock. `true` or `false`.
- `EnableRefitKits` — the stores, the bay work, and the Kit Bash circular. `true` or `false`.
- `EnableInstallCost` — the extra C-bill and time cost for a different kind of gear. `true` or `false`. This is separate from the kit bay bill.

Either part, both, or neither can be on. Save the file, quit the game fully, and relaunch. Changing a setting while the game is running does not apply.

## Installation

Drag the `NoEasyFix` folder into your mods folder and accept any file overwrites. If you already have No Easy Fix, replace that folder.

## Depends on

- ModTek
- CustomComponents

Optional:

- CustomUnits
- BTSimpleMechAssembly
- Timeline, for the 1 January Kit Bash circular
