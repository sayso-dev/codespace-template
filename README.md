# Sayso Codespace Template

A minimal template for running [Sayso](https://sayso.me) in GitHub Codespaces.

## How it works

- **`postCreateCommand`** installs the Claude CLI and Sayso binary when the codespace is first created
- **`postStartCommand`** launches Sayso automatically every time the codespace starts
- The license key is read from the `SAYSO_LICENSE_KEY` codespace secret (never stored in the repo)

## Setup

1. Create a codespace from this template (or fork the repo)
2. Set a codespace secret named `SAYSO_LICENSE_KEY` with your license key
3. The codespace will install and start Sayso automatically

## Authentication

The Claude CLI is installed automatically, but you need to authenticate it once. After your codespace starts:

```sh
claude login
```
