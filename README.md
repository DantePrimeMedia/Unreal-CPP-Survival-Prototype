# Unreal Engine 5.7 — C++ Survival and Building Prototype

**Public gameplay programming portfolio project**

An Unreal Engine coursework prototype exploring survival gameplay systems in C++, including resource gathering, health/hunger/stamina, building-piece placement, and on-screen objectives. This is a technical prototype, not a finished survival game.

## Implemented code systems

- **Player stats:** health, hunger, and stamina properties, plus timed hunger reduction and stamina recovery.
- **Resource gathering:** camera-based line tracing, resource actor depletion, inventory counters for wood, stone, and berries, and hit decals.
- **Building prototype:** resource-cost checks, build-part inventory, spawning a building actor in front of the camera, preview positioning, and rotation input.
- **Objectives and UI:** widget classes and updates for resource collection and building counts.
- **Resource actors:** static mesh and text label components.

## Representative C++ source

| Feature | Source |
| --- | --- |
| Player input, survival stats, gathering, building | [PlayerChar.cpp](Source/GAM312_Mills/PlayerChar.cpp) and [PlayerChar.h](Source/GAM312_Mills/PlayerChar.h) |
| Build-piece actor | [BuildingPart.cpp](Source/GAM312_Mills/BuildingPart.cpp) |
| Resource actor | [Resource_M.cpp](Source/GAM312_Mills/Resource_M.cpp) |
| Objective widget | [ObjectiveWidget.h](Source/GAM312_Mills/ObjectiveWidget.h) |
| Player HUD widget | [PlayerWidget.h](Source/GAM312_Mills/PlayerWidget.h) |

## Technology and setup

- Unreal Engine **5.7** (as specified in `GAM312_Mills.uproject`)
- C++, Unreal gameplay framework, UMG, Blueprint-integrated assets
- Open `GAM312_Mills.uproject` in Unreal Engine 5.7 with the Windows C++ development toolchain installed.
- Default map: `/Game/Maps/testMap`.

## Verified gameplay tests

The project owner opened and play-tested the **clean portfolio copy** in Unreal Engine **5.7** on November 7, 2026. All seven reported checks passed:

1. **PASS** — Project opens and C++ compiles in UE 5.7.
2. **PASS** — `testMap` loads and character movement works.
3. **PASS** — Health, hunger, and stamina HUD displays correctly.
4. **PASS** — Resource gathering works (wood, stone, or berries).
5. **PASS** — Gathered resources update in the player's inventory.
6. **PASS** — Building placement and rotation work.
7. **PASS** — Objectives update when collecting resources or building.

These are **user-reported in-editor functional tests**, not an automated test suite or independent code-quality audit. Source review has identified potential edge cases (including UI-pointer assumptions, repeated resource trace logic, and building-success reporting) that may merit future hardening; the passing tests do not establish that every edge case is resolved.

## Gameplay screenshots

Screenshots captured from the working Unreal Engine 5.7 prototype.

### Prototype environment
![Prototype environment with terrain and resource objects](01-prototype-environment.png)

### Survival HUD and objectives
![Survival HUD and objective tracker during gameplay](02-survival-hud-objectives.png)

### Crafting and resource management
![Crafting options, inventory totals, building controls, and objective progress](03-crafting-resource-management.png)

### Objective completion
![Victory screen after completing the prototype objectives](04-objective-completion.png)

**Gameplay video:** [Watch or download the survival gameplay demonstration](Survival.mp4) (tracked with Git LFS).

## Provenance and publication

This project originates from SNHU GAM-312 coursework. **Creator-reported asset provenance:** To the best of the creator's recollection, the assets were either personally created or supplied by Unreal Engine. This statement is based on recollection, not a per-asset provenance or license audit.

The repository includes `Content/Characters/Mannequins/` with extensive animation assets that appear to be Unreal Engine template/sample content. These are **not claimed as original student creations**. Epic Games retains rights to its content, and its redistribution is governed by the applicable Epic licenses. Project-specific assets in the other `Content/` folders have not all been independently traced to their source.

The clean portfolio import excludes packaged Windows builds, generated engine binaries, original academic Git history, and generated configuration tokens. The repository is now **public**. Public visibility does not itself establish license or academic redistribution clearance; any ambiguous asset origins and applicable academic publication restrictions still need confirmation.

## Preparation checklist

- [x] Prepare a separate branch without modifying original `main`
- [x] Remove generated Android configuration token on preparation branch
- [x] Ignore packaged builds and generated files for the future clean import
- [x] Create a separate clean-history portfolio repository
- [x] Compile and play-test the clean copy in Unreal Engine 5.7 (7/7 user-reported checks passed)
- [x] Add four actual gameplay screenshots
- [x] Repository made public by the owner
- [ ] Complete outstanding asset-rights and academic publication checks

**Status:** Public portfolio repository; outstanding rights and academic checks are documented above.
