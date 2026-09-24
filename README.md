# Vanilla OS Kipferl NVIDIA Image

Containerfile for building a Vanilla OS Kipferl + NVIDIA image.

This image is based on top of [`Vanilla-KDE/desktop-image`](https://github.com/Vanilla-KDE/desktop-image/pkgs/container/kde) and offers the default Vanilla OS Desktop experience with KDE Plasma and NVIDIA drivers.

## Build

```bash
vib build recipe.yml
podman image build -t vanillaos/kipferl-nvidia .
```

## Verify image build provenance

Images built and published by GitHub Actions include a build provenance attestation. You can verify the latest image with the GitHub CLI:

```bash
gh attestation verify oci://ghcr.io/vanilla-kde/kipferl-nvidia:latest --owner Vanilla-KDE
```

This command requires the latest version of the GitHub CLI. It verifies that the image was built by the expected GitHub Actions workflow.
