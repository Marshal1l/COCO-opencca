# COCO OpenCCA Workspace

This repository is the OpenCCA parent workspace for the RK3588 COCO runtime.
It keeps the source components as Git submodules and leaves generated firmware,
kernel, and rootfs images out of Git history.

## Submodules

- `linux/`: OpenCCA host kernel source.
- `tf-rmm/`: RMM changes used by the COCO image-sharing flow.
- `trusted-firmware-a/`: firmware source.
- `opencca-build/`, `opencca-flash/`, `opencca-manifest/`: build, flash, and manifest tooling.
- `u-boot/`, `kvmtool/`, `debian-image-recipes/`, `opencca-assets/`: board boot, VM tooling, image recipes, and fixed RK3588 assets.

Large generated images are distributed from the root `COCO` repository release
instead of being committed here.
