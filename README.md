# star-plan Scoop bucket

Scoop bucket for [star-plan](https://github.com/star-plan) (and related) CLI tools.

## Install

```powershell
scoop bucket add star-plan https://github.com/star-plan/scoop
scoop install ship
scoop install code-porter
```

Update apps:

```powershell
scoop update ship
scoop update code-porter
```

## Apps

| App | Source | Notes |
|-----|--------|--------|
| [ship](bucket/ship.json) | [heyoungai/ship](https://github.com/heyoungai/ship) | Docker / binary release CLI |
| [code-porter](bucket/code-porter.json) | [star-plan/code-porter](https://github.com/star-plan/code-porter) | Local code archive import/export; requires Git |

## How versions stay current

Manifests are updated by GitHub Actions in this repository (schedule + manual dispatch), reading the latest GitHub Release assets and checksum files from each app repo.

App repositories no longer commit Scoop manifests into their own history.

## Manual sync

```text
Actions → Sync manifests → Run workflow
```

Or wait for the scheduled run (every 4 hours).
