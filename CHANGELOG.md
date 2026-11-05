# Changelog

## 2026-11-05

### backrest

- `/backup` is now read/write by default so restores work. Backrest restores to a new folder next to the original, which failed on the read only mount.
- Add `/tmp` path and `TMPDIR` variable for restic/rclone temporary files.
- Add optional rclone config path (`/root/.config/rclone`) for rclone remotes.
- Restic repos now defaults to a dedicated `/mnt/user/backrest-repos` share instead of appdata, so the repo isn't on the same pool as the data or inside the backup path.
- Clearer descriptions for **Path to backup** and **Restic repos**, explaining that `/backup` and `/repos` are the paths to use inside Backrest.
- Move `BACKREST_DATA`, `BACKREST_CONFIG` and `XDG_CACHE_HOME` to advanced.
- Rewrite notes: explain container vs host paths, restore behaviour, and update env variable defaults.

**Existing installs:** your current mappings are kept. To fix restores, edit the container and set **Path to backup** to Read/Write.

## 2025-05-28

### victoria-metrics

- Use a specific image version instead of `:stable`.

## 2024-08-23

### backrest

- Fix env variables.

## 2024-08-22

### backrest

- Add template.

## 2023-10-08

### auto-m4b

- Add template.
- Fix icon transparency.

### victoria-metrics

- Add optional promscrape config.

## 2023-10-06

### victoria-metrics

- Add template.

## 2023-10-05

### dbgate

- Add template.

### ca_profile

- Add CA profile.
