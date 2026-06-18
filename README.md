# CLI Proxy API Plus Management Center

This repository is a fork of the management panel from `router-for-me/main`.

This README only documents modules that are added or kept differently from `router-for-me/main`.

[中文文档](README_CN.md)

## Additional modules in this fork

### Kiro quota

Adds quota display support for **Kiro** credentials:

- Shows Kiro subscription and base quota information.
- Displays free trial status.
- Surfaces suspended credential status when available.

### GitHub Copilot quota

Adds quota display support for **GitHub Copilot** credentials:

- Shows Copilot plan information.
- Displays chat, completions, and premium interaction quotas.
- Supports unlimited quota display when returned by the backend.

### Ampcode provider integration

Keeps the **Ampcode** provider module that was removed from `router-for-me/main`:

- Keeps Ampcode provider registration in the AI Providers workbench.
- Keeps Ampcode upstream URL and upstream API key configuration.
- Keeps upstream API key mapping configuration.
- Keeps model mapping configuration and force mapping switch.
- Keeps Ampcode Management API client and related types.

### Usage statistics iframe

Adds a **Usage Statistics** module implemented with an iframe:

- The navigation item appears when `usage-statistics-url` is configured.
- The iframe URL should be the deployed address of https://github.com/Willxup/cpa-usage-keeper.
- Configure that deployed address in the visual config panel under Remote Management, or directly in `config.yaml` as `usage-statistics-url`.

## Upstream reference

For general usage, development commands, configuration, and feature documentation that are unchanged from upstream, refer to the upstream project documentation:

- `router-for-me/main`: https://github.com/router-for-me/Cli-Proxy-API-Management-Center
- CLI Proxy API: https://github.com/router-for-me/CLIProxyAPI
