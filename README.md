# Photon 1.0 skills (legacy)

[![License: Apache-2.0](https://img.shields.io/badge/License-Apache_2.0-green.svg)](./LICENSE)

Agent skills for Photon 1.0: Spectrum (`spectrum-ts`), the 1.0 CLI (`@photon-ai/cli@legacy`) and the 1.0 iMessage SDKs, in the [Agent Skills](https://skills.sh/) format.

> **Building on Photon 2.0?** Use [photon-hq/skills](https://github.com/photon-hq/skills) instead. Photon 2.0 is the Photon API at `https://api.photon.codes/v1` with `@photon-ai/cli` 3.x. The two versions use different packages, API hosts and credentials, so keep each project on one of them.

```bash
npx skills add photon-hq/skill-legacy --skill <skill-name>
```

## Skills

| Skill | Packages | Description |
| :--- | :--- | :--- |
| [`spectrum`](./skills/spectrum/SKILL.md) | `spectrum-ts` | Write a messaging agent once against one `app.messages` stream and run it on iMessage, WhatsApp Business, the terminal or a custom platform. |
| [`imessage`](./skills/imessage/SKILL.md) | `@photon-ai/imessage-kit` · `@photon-ai/advanced-imessage` · `spectrum-ts` | Send and receive iMessages with the local, hosted or unified 1.0 SDK. |
| [`photon-cli`](./skills/photon-cli/SKILL.md) | `@photon-ai/cli@legacy` | The 1.0 `photon` CLI: sign in, create and manage projects, read the Spectrum API secret, manage lines, users and platforms, billing. |
| [`chat-adapter-imessage`](./skills/chat-adapter-imessage/SKILL.md) | `chat-adapter-imessage` | Connect a Vercel Chat SDK bot to iMessage through the 1.0 adapter. |

## Installing a skill

```bash
npx skills add photon-hq/skill-legacy --skill spectrum
npx skills add photon-hq/skill-legacy --skill imessage
npx skills add photon-hq/skill-legacy --skill photon-cli
npx skills add photon-hq/skill-legacy --skill chat-adapter-imessage
```

The 1.0 CLI is published under the `legacy` tag. `npm i -g @photon-ai/cli` without a tag installs the 2.0 CLI (3.x), which rejects 1.0 commands with `LEGACY_COMMAND`.

## Documentation

- [Photon 1.0 documentation](https://photon.codes/docs/spectrum-ts/introduction)
- [Documentation index for both versions](https://photon.codes/docs/llms.txt)

## License

Apache-2.0
