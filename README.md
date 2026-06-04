# NetMedEx Workspace

A workspace container aggregating a fork of [NetMedEx](https://github.com/lsbnb/NetMedEx)
(an AI-powered biomedical knowledge discovery platform) and related resources.

## Structure

| Path | What |
|------|------|
| `repos/NetMedEx-fork/` | git **submodule** → [`PsychQuant/NetMedEx`](https://github.com/PsychQuant/NetMedEx), a fork of [`lsbnb/NetMedEx`](https://github.com/lsbnb/NetMedEx). The actual code lives here. |

> Working notes (`docs/`) and editor/session state are kept local and intentionally
> not tracked in this repository.

## Clone

```bash
git clone --recurse-submodules https://github.com/PsychQuant/NetMedEx-workspace.git

# already cloned without submodules?
git submodule update --init --recursive
```

## Working with the fork

```bash
cd repos/NetMedEx-fork
git checkout -b feat/your-change   # origin = PsychQuant fork, upstream = lsbnb
# ... edit, commit, push to origin, open PR against lsbnb/NetMedEx
```
