# 01-solution-upgrade: Upgrade project framework and dependencies

Upgrade the project target framework to net10.0-windows and update package references to the latest supported stable versions for the new framework. Then restore, build, and run tests to validate the upgrade end-to-end in one atomic pass.

**Done when**: The project targets net10.0-windows, package references are updated to supported stable versions, restore/build succeed, and available tests pass.

## Research Notes

- Project is SDK-style and defines `TargetFramework` directly in `Brick Breaker.csproj` (no centralized props override detected).
- Project has 2 direct NuGet dependencies in the project file:
  - `MonoGame.Framework.DesktopGL` 3.8.1.303
  - `MonoGame.Content.Builder.Task` 3.8.1.303
- NuGet outdated check reports latest stable versions as `3.8.4.1` for both packages.
- `get_supported_package_version` also reports preview `3.8.5-preview.4`; keeping stable line to match scenario preference for latest supported stable updates.

## Execution Plan

1. Update `TargetFramework` to `net10.0-windows`.
2. Update both MonoGame package versions to `3.8.4.1`.
3. Restore and build solution.
4. Run tests if test projects exist.
