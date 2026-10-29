# MANOR Edge skill

An agent skill that installs the MANOR Edge app on an Apple silicon Mac and walks the owner through pairing it with their home and adding cameras. The agent downloads the notarized app from `downloads.mymanor.click`, verifies its checksum, signing team and Apple notarization, and opens the pairing window. The owner pastes their own pairing key into the app; the agent never handles it.

## Install

Claude Code, Codex, Cursor, Goose, Gemini CLI and other [skills.sh](https://skills.sh) agents:

```bash
npx skills add getmanor/skill
```

Hermes Agent:

```bash
hermes skills install https://raw.githubusercontent.com/getmanor/skill/main/hermes/manor/SKILL.md
```

Or install the Mac app yourself with Homebrew:

```bash
brew install --cask getmanor/tap/manor-edge
```

More at [mymanor.click/mac](https://mymanor.click/mac).

This repository is published from MANOR's main repository; changes made here are overwritten on the next sync.
