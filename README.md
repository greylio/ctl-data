# ChargeTrack Legends - Game Data

![ChargeTrack Legends splash screen](./doc/readme/splash-main.jpg)

**ChargeTrack Legends (CTL)** is a private fork of [Speed Dreams](https://www.speed-dreams.net/) 2.4.2, a free and open source motorsport simulator originally forked from [TORCS](https://torcs.sourceforge.net/).

> **Note:** This is a personal project by Rob McTaggart ([greylio](https://github.com/greylio) on GitHub).

> **This repository contains the game assets (tracks, cars, textures, sounds, configurations).**
>
> For the engine source code, see the companion repository:
> https://github.com/greylio/ctl-code

![In-game screenshot](./doc/readme/collage.jpg)

## Repository Structure

```
speed-dreams-data/
├── data/
│   ├── cars/           # Car models and configurations
│   ├── tracks/         # Track definitions and assets
│   ├── drivers/        # AI driver configurations
│   ├── img/            # UI images and textures
│   ├── menu/           # Menu configurations
│   └── ...
├── cmake/              # CMake modules
└── doc/                # Documentation
```

## Usage

This repository is typically used as a git submodule within the main CTL code repository. It can also be cloned standalone for asset editing.

### As a Submodule (Recommended)

When cloning the main code repository:
```cmd
git clone --recurse-submodules https://github.com/greylio/ctl-code.git
```

### Standalone (For Asset Editing)

```cmd
git clone https://github.com/greylio/ctl-data.git speed-dreams-data
```

After making changes, commit to this repo and update the submodule reference in the code repo.

## Building/Installing Data Only

No compilation is required since this is a pure data/asset repository. To install to a specific location:

```cmd
cmake -B build -DCMAKE_INSTALL_PREFIX=<install-dir>
cmake --install build/
```

## Original Speed Dreams

This data is based on Speed Dreams 2.4.2. For the original project:
- Website: https://www.speed-dreams.net/
- Data Repository: https://forge.a-lec.org/speed-dreams/speed-dreams-data/

## License

By default, non-functional data is licensed under the [Free Art License](http://artlibre.org/).

However, some assets are distributed under various free (as in freedom) licenses. Please read the license files located in their respective directories for further reference.

## Trademark Disclaimer

Microsoft Windows is a registered trademark of Microsoft Corporation.
Ubuntu is a registered trademark of Canonical Ltd.
