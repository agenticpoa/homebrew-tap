# Homebrew Tap for sshsign

Homebrew formulae for [sshsign](https://github.com/agenticpoa/sshsign) - SSH signing service for AI agents.

## Install

```bash
brew install agenticpoa/tap/sshsign
```

## What it installs

The `sshsign` CLI client, which acts as a drop-in `gpg.ssh.program` for git. It proxies signing requests to a sshsign server over SSH.

## Usage

```bash
# Configure git to use sshsign
git config --global gpg.format ssh
git config --global gpg.ssh.program sshsign
git config --global user.signingkey "ak_..."

# Sign commits
git commit -S -m "signed commit"
```

For the full setup guide and programmatic API, see [sshsign.dev](https://sshsign.dev).

## Update

```bash
brew upgrade agenticpoa/tap/sshsign
```
