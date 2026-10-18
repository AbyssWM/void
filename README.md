<div align="center">

<img src="https://github.com/AbyssWM.png?size=200" width="140" alt="Abyss logo">

# 🌀 Abyss XBPS repository

**Signed binary packages of the Abyss Wayland ecosystem for Void Linux (x86_64, glibc).**

[🌐 Website](https://abysswm.github.io/) · [📖 Install guide](https://abysswm.github.io/wiki/getting-started) · [🛠️ Templates](https://github.com/AbyssWM/void-builds)

</div>

---

> [!WARNING]
> **First release.** Abyss is usable now, but this is the first version: expect bugs and please report them.

## 🚀 Install

```sh
echo "repository=https://abysswm.github.io/void" | sudo tee /etc/xbps.d/abyss.conf
sudo xbps-install -S abyssland
```

On the first sync xbps asks you to import the repository key (signed by `bb8TheRobot <bb8therobot85@gmail.com>`) — answer **y**.
Updates then arrive with the normal `sudo xbps-install -Su`.

Add the tools you want:

```sh
sudo xbps-install xdg-desktop-portal-abyss abysslock abysspaper abysspolkit abyssdusk abysspicker abyss-guiutils
```

Then pick **Abyssland** in your display manager.

## 📦 What's inside

All 17 Abyss packages plus 7 `-devel` packages, built with `xbps-src` from the templates in
[void-builds](https://github.com/AbyssWM/void-builds). This repository only hosts the built packages and the signed index.
