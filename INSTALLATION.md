# PapiGPT Online Installation

This package is the clean PapiGPT Production Base. Optional first-party features are installed separately as standalone plugins.

## Requirements

- Supported PHP/Laravel runtime for this PapiGPT release
- MySQL/MariaDB database
- Composer
- Web server configured with the PapiGPT `public/` directory as DocumentRoot

## Install

1. Extract the Production Base.
2. Copy/configure `.env` from `.env.example` as needed.
3. Configure database credentials.
4. Run:

```bash
composer install --no-dev --optimize-autoloader
php artisan key:generate
php artisan optimize:clear
```

5. Point the web server DocumentRoot to `public/`.
6. Open `/setup` in a browser and create the permanent Owner account. PapiGPT reserves user ID #1 for Owner.
7. Let setup finish migrations, seeding, Owner validation, session initialization, and install-lock creation.
8. Sign in to Admin and configure AI providers/models, General Settings, templates, usage limits, and optional standalone plugins.

### Session cookie note

Use `SESSION_SECURE_COOKIE=true` on HTTPS production sites. Use `false` while installing/testing over plain HTTP, otherwise browsers will not send the Secure session cookie and login can appear to fail.

## Optional plugins

The Production Base intentionally does not bundle optional feature implementations. Install supported plugins separately from **Admin → Plugins**. The `/plugins/` directory in a fresh core contains only infrastructure documentation until plugins are installed.
