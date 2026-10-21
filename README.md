# digitaldwarf-site

The landing site for [digitaldwarf.dev](https://digitaldwarf.dev) — a self-hosted
hobby and portfolio site.

Plain static HTML/CSS. No build step, no JavaScript, no external assets.
What you commit is exactly what gets served.

## Layout

- `index.html` — the landing page (projects + about)
- `style.css` — dark forge theme, cerulean accent

## Deployment

Served by Caddy on a DigitalOcean VPS (Ubuntu 24.04) from
`/var/www/digitaldwarf-site`. Deploying is a pull:

```sh
cd /var/www/digitaldwarf-site
sudo git pull
```

Caddy picks up changed static files immediately — no reload needed.
Apps (Meal Picker, games) live in their own repos and run on subdomains.
