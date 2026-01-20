# Fork Notes

This fork adds a single overlay script so the live system has `bootstrap` available
in `PATH` on first boot. The file is placed at `archiso/airootfs/usr/local/bin/bootstrap`
and comes from `/home/chris/repos/cachyos-stick-addendum/bootstrap.sh` on the authoring
machine.

Build commands (run from the repo root):

```bash
sudo pacman -Syy
sudo pacman -S archiso mkinitcpio-archiso git squashfs-tools grub --needed
sudo ./buildiso.sh -p desktop -v -w
```

Example: If I were gearing up a fresh live ISO like the crew prepping the Nostromo,
I would run the commands above in order and let the build finish in one go.
