# Facade UI skill for Claude Code

A skill that teaches Claude how to build accessible marketing pages with [Facade UI](https://facadeui.dev): sections and page templates (heroes, feature grids, pricing tables, FAQs, footers and complete landing pages) installed with the shadcn CLI.

The skill is a single instruction file, `skills/facade-ui/SKILL.md`. It does not run any code, start any server or send any data. It tells the agent how to set up the `@facade` registry, how to find and read items on facadeui.dev, and the rules that keep a page accessible: one `h1`, heading levels as props, `link` and `image` components, alt text and spoken prices.

## Install

- **Claude** (Claude Code, Cowork and the Claude apps): add [Facade UI from the Claude directory](https://claude.ai/customize/plugins/id/86e8de8c-f5a8-41b7-937e-a8990b365185%40anthropic-plugin-directory), or search for "Facade UI" on the Customize page.
- **Any agent that reads skills**: `npx skills add facade-ui/skill`, or copy `skills/facade-ui/SKILL.md` into your project's skills folder (for example `.claude/skills/facade-ui/SKILL.md` or `.cursor/rules/facade-ui.mdc`).

## What Facade UI is

Facade UI is free and open source (MIT). Sections use shadcn's colour variable names, so they take an existing shadcn theme, and every item is tested against WCAG 2.2 AA. Source: https://github.com/facade-ui/facade-ui. Docs for agents: https://facadeui.dev/docs/agents and https://facadeui.dev/llms.txt.

## Licence

MIT. See [LICENSE](./LICENSE).
