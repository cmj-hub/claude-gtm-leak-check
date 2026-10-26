# Start here

This pack reads **public pages** for one domain and prints **one to three real GTM gaps**. A live run also reads pricing and careers (or jobs) when those pages exist.

## Install

```bash
npx skills add cmj-hub/claude-gtm-leak-check --all -g --full-depth
```

Claude Code plugin:

```text
/plugin marketplace add cmj-hub/claude-gtm-leak-check
/plugin install gtm-leak-check@claude-gtm-leak-check
```

## Run

```bash
python3 skills/gtm-leak-check/scripts/check.py --domain yourcompany.com
```

Or score the bundled thin homepage with no network:

```bash
python3 skills/gtm-leak-check/scripts/check.py --html-file skills/gtm-leak-check/examples/thin-home.html --page-url https://thin.example/
```

You should see `Gap 1 of 3` and a `Source:` URL.

## What it never does

It does not log into your CRM, inbox, or ads. It does not change your site. It does not write a playbook.

The full emailed read is The Friday Signal. A written audit of the system you run is the Growth Audit.
