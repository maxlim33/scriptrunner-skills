# ScriptRunner Agent Skills

Agent skills for working with ScriptRunner products, APIs, documentation, and
examples.

This repository is both a **Claude Code plugin** and a **plugin marketplace**,
and it also installs as plain skills via the `skills` CLI.

## Available skills

- `atlassian-cloud-rest-api`
- `atlassian-community-search`
- `scriptrunner-documentation`
- `scriptrunner-example-scripts`
- `scriptrunner-platform-guidance`

## Install as a Claude Code plugin

Add the marketplace, then install the plugin:

```
/plugin marketplace add maxlim33/scriptrunner-skills
/plugin install scriptrunner-skills@scriptrunner
```

Or from the CLI:

```bash
claude plugin marketplace add maxlim33/scriptrunner-skills
claude plugin install scriptrunner-skills@scriptrunner
```

Browse and manage installed plugins with `/plugin`.

## Install with the `skills` CLI

```bash
npx skills add maxlim33/scriptrunner-skills
```

List the skills without installing them:

```bash
npx skills add maxlim33/scriptrunner-skills --list
```

Install one skill:

```bash
npx skills add maxlim33/scriptrunner-skills --skill scriptrunner-documentation
```

See the [`skills` CLI documentation](https://github.com/vercel-labs/skills) for
agent selection, global installation, and other options.

## Repository layout

```
.claude-plugin/
  marketplace.json   # marketplace listing, exposes this repo as a plugin source
  plugin.json        # plugin manifest for scriptrunner-skills
skills/              # the skills themselves, one directory each
```
