# PapiGPT

**Ask Papi. Get It Done.**

PapiGPT is an AI-powered productivity and learning platform designed to make chat, writing, research, document work, reports and project workflows easier in one unified interface.

It combines AI assistance with configurable workspaces, personalization, document support, administration tools and an extensible plugin architecture.

## Features

- AI Chat
- New Report workflow
- Write / Reply tools
- Document and material support
- User personalization
- Projects workspace
- Classes workspace
- Library workspace
- User Groups and access controls
- Usage and token management
- Frontend and Admin template customization
- Plugin Manager
- Standalone system plugins
- Maintenance mode and visitor tracking
- Custom permalink structures
- Responsive desktop, tablet and mobile interface

## Architecture

PapiGPT uses a clean-core architecture.

The core application provides:

- authentication
- AI request handling
- conversations
- reports
- document and attachment services
- usage accounting
- billing foundations
- templates
- permissions
- system updates
- plugin APIs

Optional features such as Library, Projects, Classes, User Groups and other modules are distributed as standalone plugins.

## Current Production Build

**PapiGPT Online `20260927-004`**

This build consolidates the completed `20260927-003` development and patch series into the current production baseline.

## Requirements

Typical production requirements include:

- PHP
- Composer
- MySQL or compatible database
- Supported web server
- OpenAI-compatible AI provider configuration

Refer to `INSTALLATION.md` for full installation instructions.

## Installation

For a fresh installation:

1. Extract the PapiGPT Production Base.
2. Configure `.env`.
3. Install PHP dependencies:

```bash
composer install --no-dev --optimize-autoloader
