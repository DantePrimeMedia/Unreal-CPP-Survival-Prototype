# Unreal Engine 5.7 — C++ Survival and Building Prototype

**Private portfolio preparation copy — not approved for publication**

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

**Testing pending:** The clean portfolio copy has not been independently rebuilt or play-tested. The source contains areas that warrant review, including UI-pointer assumptions, repeated resource trace logic, and building-success reporting. Do not treat all systems as verified until tested.

## Provenance and publication

This project originates from SNHU GAM-312 coursework. Attribution and redistribution rights for Unreal template content and any other included binary assets must be checked before publication. Do not include packaged Windows builds, generated engine binaries, old Git history, or generated configuration tokens in the clean portfolio repository.

## Preparation checklist

- [x] Prepare a separate branch without modifying original `main`
- [x] Remove generated Android configuration token on preparation branch
- [x] Ignore packaged builds and generated files for the future clean import
- [ ] Create a separate clean-history private portfolio repository
- [ ] Compile and test the clean copy in Unreal Engine 5.7
- [ ] Add actual gameplay screenshots
- [ ] Review asset rights and academic publication timing

**Keep private until explicitly approved.**
