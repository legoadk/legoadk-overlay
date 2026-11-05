# legoadk-overlay

legoadk's personal Gentoo ebuild overlay.

Contains mostly SolidCraft and adjacent software.

Quality not guaranteed in any way, shape, or form; all ebuilds are experimental, your mileage may vary, etc.

Pull requests and bug reports welcome.

## Adding the repository

### eselect

```sh
eselect repository enable legoadk-overlay
```

### repos.conf

Create `/etc/portage/repos.conf/legoadk-overlay.conf`:

```ini
[legoadk-overlay]
location = /var/db/repos/legoadk-overlay
sync-type = git
sync-uri = https://github.com/legoadk/legoadk-overlay.git
sync-branch = main
```

## Syncing the repository

```sh
emerge --sync legoadk-overlay
```
