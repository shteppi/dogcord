# Dog Cord 🐕 [<img src="/static/icon.png" width="225" align="right" alt="Dog Cord">](https://github.com/shteppi/dogcord)

Dog Cord is a fork of [Vesktop](https://github.com/Vencord/Vesktop) for good boys and girls who want the best Discord experience!

You can join our [Dog Park](https://discord.gg/8HGpehczrB) for commits, changes, barks, or even belly rubs (support).

</br>

**Main features** 🦴:

- DogPack preinstalled (comes with all the treats!)
- Much more lightweight and faster than the official Discord app (Zoomies included!)
- Linux Screenshare with sound & wayland
- Much better privacy, since Discord has no access to your kennel

**Extra included changes** 🐾:

- Tray Customization with bark detection and notification badges
- Command-line flags to toggle bark (mic) and play dead (deafen) status (Linux)
- Custom Arguments from [this PR](https://github.com/shteppi/dogcord/pull/46)
- arRPC-bun with debug logging support [https://github.com/Creationsss/arrpc-bun](https://github.com/Creationsss/arrpc-bun)

**Linux Note** 🐧:

- You can use the `--toggle-mic` & `--toggle-deafen` flags to toggle your bark and play dead status from the terminal. These can be bound to keyboard shortcuts at the system level. Good boy!

**Not fully Supported** 😿:

- Global Keybinds (Windows/macOS - use command-line flags on Linux instead)

## Installing 📦

Check the [Adoption Center](https://github.com/shteppi/dogcord/releases) page to adopt your very own Dog Cord!

OR

Check The Downloads from the [website](https://github.com/shteppi/dogcord/releases)

### Linux 🐧

#### Community packages

Below you can find unofficial packages created by the community. They are not officially supported by us, so before reporting fleas (issues), please first confirm the flea also happens on official builds. When in doubt, consult with their packager first. The AppImage should work on any distro that supports them, so we recommend you just use that instead!

- Arch Linux: [Dog Cord on the Arch user repository](https://aur.archlinux.org/packages?K=dogcord)
- NixOS: `nix-shell -p dogcord`

## Breeding from Source 🧬

You need to have the following dependencies installed:

- [Git](https://git-scm.com/downloads)
- [Bun](https://bun.sh)

Packaging will create builds in the dist/ folder

```sh
git clone https://github.com/shteppi/dogcord
cd dogcord

# Install Dependencies (fetch the treats!)
bun install

# Either run it without packaging (take it for a walk!)
bun start

# Or package (will build packages for your OS)
bun package

# Or only build the Linux Pacman package
bun package --linux pacman

# Or package to a directory only
bun package:dir
```

## Building LibVesktop from Source 🔧

This is a small C++ helper library Dog Cord uses on Linux to emit D-Bus events. By default, prebuilt binaries for x64 and arm64 are used.

If you want to build it from source:

1. Install build dependencies:

   - Debian/Ubuntu: `apt install build-essential python3 curl pkg-config libglib2.0-dev`
   - Fedora: `dnf install @c-development @development-tools python3 curl pkgconf-pkg-config glib2-devel`

2. Run `bun buildLibVesktop`
3. From now on, building Dog Cord will use your own build

---

Made with ❤️ and lots of 🐕 energy!

_Woof woof!_ 🐾