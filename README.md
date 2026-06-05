# factory-entreprenais-com (public)

**Build artifacts repository for [factory.entreprenais.com](https://factory.entreprenais.com/).**

This repository contains only built HTML/CSS/JS artifacts. It is automatically updated by the private builder repository.

## Repository Structure

| Repository | Visibility | Contents |
|-----------|-----------|---------|
| `taru0216/factory-entreprenais-com-builder` | **private** | Source code, build scripts, GHA workflows |
| `taru0216/factory-entreprenais-com` (this repo) | **public** | Build artifacts only, GitHub Pages source |

## How It Works

1. `factory-entreprenais-com-builder` runs build workflows on self-hosted runners
2. Build artifacts are pushed to this repository via Deploy Key
3. This repo's `deploy.yml` triggers and deploys to GitHub Pages

## Site

https://factory.entreprenais.com/
