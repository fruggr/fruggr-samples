# Accessibility analysis with Fruggr A11y scanner

You can find here samples about Fruggr A11y scanner for accessibility analysis.

## Requirements

All samples are built with [Docker Compose](https://docs.docker.com/compose/).
So, install:
- [Docker Desktop](https://docs.docker.com/desktop/)/Engine (Windows/WSL, MacOS, Linux)
- Docker Compose (usually bundled with Docker Desktop)

You also need a Fruggr digital service, with "owner" permission, where you can get [your CI/CD Access Token](https://wiki.fruggr.io/hc/fr/articles/9694438970653). It is named later `FRUGGR_API_KEY`.

### Container registry authentication

The Fruggr A11y scanner image is hosted on a private Azure Container Registry (ACR). You must authenticate before pulling the image.

Follow the instructions in the [Fruggr A11y scanner reference configuration](https://wiki.fruggr.io/hc/fr/articles/35107283622813) article to get the registry credentials and run `docker login`.

## Samples

1. [One page accessibility analysis](one-page-analyze)

   Analyze the accessibility of a single page configured in Fruggr SaaS

## Troubleshooting / FAQ

### Error `Fruggr API key is required`

Check the [requirements](#requirements) if you get this message:

```
[scanner] Fruggr API key is required, you must set FRUGGR_API_KEY environment variable
exited with code 1
```

### Error pulling the image (authentication required)

If you get an authentication error when running `docker compose up`, make sure you have logged in to the container registry first. See [Container registry authentication](#container-registry-authentication).

## Getting help

👉 Documentation and tutorials: https://wiki.fruggr.io/hc

👉 If you need more help: support@fruggr.io
