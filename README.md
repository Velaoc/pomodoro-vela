<!-- foundation:identity -->
# Pomodoro

A single-page Pomodoro timer that switches the background color between focus and break phases, tracking completed sessions.

- Site: https://pomodoro-vela.api.holode.xyz
- Support: support@pomodoro-vela.api.holode.xyz
<!-- /foundation:identity -->

## What this is

A single-page Pomodoro timer that switches the background color between focus and break phases, tracking completed sessions.

## Who it is for

- visitor

## Main features

- **Run a pomodoro cycle** — Start, pause, and reset the timer; it alternates focus (25 min) and short/long break phases with a background color switch per phase.
- **Review completed sessions** — See today's completed sessions listed under the timer.

## Core entities

- Session

## Run locally

```bash
bundle install
bin/rails db:prepare
bin/dev
```

Requires Ruby, PostgreSQL, and the usual Rails toolchain. See `bin/setup` if present.

## Demo

A few completed sessions from today (mixed focus/break) so the history list has something to show on first load.

## Deploy notes

Production `config.hosts` is derived from `domain` in `config/foundation.yml`. Keep that value aligned with the real host or every request will 403.
