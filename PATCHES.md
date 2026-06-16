# Patches

Commits applied on top of [space-wizards/SS14.Launcher](https://github.com/space-wizards/SS14.Launcher) upstream.

| Commit | Description | Skippable |
|--------|-------------|-----------|
| `7ae95e7` | Disable random connection messages shown during server connect | Yes |
| `086840d` | Lazy upstream sync workflow + multi-platform build (Win/Mac/Linux × Debug/Release) | Yes |

## Applying individual patches

```bash
# Clone upstream directly (no patches)
git clone https://github.com/space-wizards/SS14.Launcher

# Or clone this fork and cherry-pick only what you need
git clone https://github.com/com-master/SS14.Launcher
cd SS14.Launcher
git checkout <upstream-commit>         # start from clean upstream state
git cherry-pick 7ae95e7               # apply only the patch you want
```

## Skipping a patch when syncing this fork

```bash
git clone https://github.com/com-master/SS14.Launcher
git revert 7ae95e7 --no-commit        # undo a specific patch without committing
```
