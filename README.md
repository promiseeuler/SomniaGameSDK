# Somnia Game SDK

An Unreal Engine 5.4 integration prototype for building blockchain-enabled game experiences on Somnia. The project combines a native Unreal runtime module, an embedded Thirdweb SDK integration, and example wallet assets for testing account and onchain interaction flows.

> [!IMPORTANT]
> This repository is an experimental integration project, not a production-ready or officially supported Somnia SDK. Review wallet, contract, and network configuration before using it in a live game.

## Overview

Somnia Game SDK demonstrates how an Unreal project can incorporate blockchain functionality without moving core gameplay logic outside the engine. It includes:

- an Unreal Engine 5.4 C++ project and runtime module;
- the Thirdweb Unreal Engine plugin for wallet and contract operations;
- example Blueprint assets for wallet interaction;
- a Somnia test map and sample interaction flow;
- Git LFS configuration for Unreal assets and other large binary files.

## Repository structure

```text
SomniaGameSDK.uproject   Unreal project descriptor
Source/                  Native project module and build targets
Plugins/ThirdwebSDK/     Embedded Thirdweb Unreal Engine plugin
Content/Game/            Wallet and gameplay example assets
Config/                  Unreal project configuration
```

## Requirements

- Unreal Engine 5.4
- Git LFS
- A supported desktop development environment for Unreal Engine C++ projects
- Network and account configuration appropriate for the Somnia environment you intend to use

## Getting started

1. Install and initialize Git LFS:

   ```bash
   git lfs install
   ```

2. Clone the repository and fetch its LFS-managed assets:

   ```bash
   git clone https://github.com/promiseeuler/SomniaGameSDK.git
   cd SomniaGameSDK
   git lfs pull
   ```

3. Open `SomniaGameSDK.uproject` with Unreal Engine 5.4.
4. Allow Unreal Engine to generate or rebuild project modules if prompted.
5. Review the wallet and network configuration before running the example content.

## Development notes

- Do not commit private keys, seed phrases, API secrets, or funded test credentials.
- Treat the included maps and Blueprints as reference implementations.
- Keep binary Unreal assets under Git LFS to avoid inflating the Git repository.
- Validate contract addresses, chain identifiers, RPC endpoints, and transaction behavior before deployment.

## Project status

The repository currently serves as a technical prototype and integration reference. Interfaces, configuration, and example flows may change as the project evolves.

## Third-party software

The repository includes the Thirdweb SDK for Unreal Engine. Thirdweb remains the owner and maintainer of that software; consult its included metadata and official documentation for applicable support and licensing information.
