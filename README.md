# Vanilla OS Kipferl NVIDIA Image

Containerfile for building a Vanilla OS Kipferl + NVIDIA image.

This image is based on top of [`Vanilla-KDE/desktop-image`](https://github.com/Vanilla-KDE/desktop-image/pkgs/container/kde) and offers the default Vanilla OS Desktop experience with KDE Plasma and NVIDIA drivers.

## Build

```bash
vib build recipe.yml
podman image build -t vanillaos/kipferl-nvidia .
```

