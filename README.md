# Episode Studio Desktop

Windows downloads and the stable update channel for Episode Studio.

## Install once

1. [Download the latest Windows executable](https://github.com/crgoku7/episode-studio-releases/releases/latest/download/EpisodeStudioDesktop.exe).
2. Run it, open **Updates**, and choose **Install on this PC**.
3. Use the **Episode Studio** Start menu shortcut afterward.
4. Enter the deployment owner's Runpod API key and authorized SSH key in Settings once.

The installer uses the current Windows user's Programs folder. Python, Docker, a local GPU and a GitHub login are not required on the operator's computer. The executable is currently unsigned.

## Updates

Updates are downloaded from this repository, verified against their SHA-256 digest, checked for successful application startup, and installed into versioned folders. The previous installed version is kept for rollback. Credentials and settings stay outside the installation directory. An active render, export or upload blocks the version switch; the updater does not stop the GPU. Updating container images is a separate deployment operation.

Use **Updates → Check for updates → Install update & restart**. Use **Restore previous version** if needed.

## Studio

Reference-guided shots, review/retakes, RTX VSR 2x, episode export version selection, reported progress stages and fullscreen preview. This build is configured for the owner's Runpod deployment.

**Closing the app does not stop GPU billing. Use Stop pod and wait for confirmation.**

This repository contains release downloads and documentation, not Runpod credentials, models, reference images or project videos.
