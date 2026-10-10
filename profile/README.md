<p align="center">
  <img src="logo.svg" width="72" height="72" alt="Flowly logo">
</p>

<h1 align="center">Flowly</h1>

<p align="center">
  <b>Your day, across every project.</b><br>
  An open-source daily planner with an AI concierge. Host it yourself, or use <a href="https://flowly.net">flowly.net</a>.
</p>

<p align="center">
  <a href="https://flowly.net">Website</a> ·
  <a href="https://app.flowly.net/register">Try it</a> ·
  <a href="https://github.com/flowly-org/flowly-backend#self-hosting">Self-host</a> ·
  <a href="https://github.com/flowly-org/flowly-releases/releases/latest">Apps</a> ·
  <a href="https://github.com/flowly-org/flowly-prompt">The prompt</a>
</p>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://flowly.net/assets/lanes-dark.webp">
  <img src="https://flowly.net/assets/myday.webp" alt="Flowly's My day board: today's calendar above tasks from two workspaces in swimlanes by project, with a backlog on the side.">
</picture>

Flowly gathers the tasks from all your projects and teams into one board for today, grouped into swimlanes by project,
context or anything you tag. Your calendar stays in the background, the day's load tells you when it's overbooked,
and Flo, the concierge, plans your week from a list, briefs you in the morning and moves things around when you ask,
in the app, on Telegram, or from ChatGPT and Claude.

- **Plan:** swimlanes, carry-over, backlog, recurring tasks, checklists, reminders, templates, dependencies, a timeline, time blocking with auto-plan, weekly review, insights.
- **Calendars:** Google, Microsoft 365, CalDAV and iCal as background, with preparation hints, travel time and leave-by alerts.
- **Flo:** plan-my-week, morning brief, tasks by chat, voice, photos of lists, meeting notes and emails, delegation to an agent. Any OpenRouter key or any OpenAI-compatible endpoint, or no AI at all.
- **Teams:** roles, invitations, agile rituals, Telegram and Slack bots, single sign-on (OIDC).
- **Integrations:** GitHub, Slack, Discord, webhooks, email-in, wikis, Donetick, Trello and Asana import, an MCP server.
- **Time & invoices:** timers, billing rates, invoices with national e-invoice formats.
- **Everywhere:** web, Android, macOS, Windows, Linux, in six languages. The apps connect to any Flowly server, several at once.

## Repositories

| | |
|---|---|
| [flowly-backend](https://github.com/flowly-org/flowly-backend) | The API and its worker (Django, Postgres), plus the self-hosting files |
| [flowly-frontend](https://github.com/flowly-org/flowly-frontend) | The web app and the Android/iOS apps (Angular, Capacitor) |
| [flowly-desktop](https://github.com/flowly-org/flowly-desktop) | The tray time tracker for macOS, Windows and Linux (Tauri) |
| [flowly-prompt](https://github.com/flowly-org/flowly-prompt) | `PROMPT.md`: the specification that rebuilds Flowly with a coding agent |
| [flowly-releases](https://github.com/flowly-org/flowly-releases) | App downloads |
| [flowly-org.github.io](https://github.com/flowly-org/flowly-org.github.io) | The website, [flowly.net](https://flowly.net) |

## Run your own

```bash
curl -O https://raw.githubusercontent.com/flowly-org/flowly-backend/main/selfhost/docker-compose.yml
curl -o .env https://raw.githubusercontent.com/flowly-org/flowly-backend/main/selfhost/.env.example
# set DJANGO_SECRET_KEY, POSTGRES_PASSWORD and PUBLIC_URL
docker compose up -d
```

Open `http://localhost:8080`. Every feature is included on your own server: no plans, no limits.
The [self-hosting guide](https://github.com/flowly-org/flowly-backend#self-hosting) covers HTTPS, admin settings, AI, calendars, Telegram and SSO.

## Contribute

Issues and pull requests are welcome in each repository. Flowly is licensed under the
[GNU AGPL-3.0](https://github.com/flowly-org/flowly-backend/blob/main/LICENSE): use it, change it, host it;
if you offer a modified Flowly as a service, publish your changes.
