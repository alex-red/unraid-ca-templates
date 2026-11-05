# Changelog

## 2026-11-05

### backrest

- Map `/mnt/user` to the same path inside the container (read/write), replacing the read only `/mnt/user/backup` → `/backup` mapping. Share paths can now be used as-is in Backrest, and restores no longer fail on a read only mount.
- Add `/tmp` path and `TMPDIR` variable for restic/rclone temporary files.
- Add optional rclone config path (`/root/.config/rclone`) for rclone remotes.
- `/repos` is now optional with no default, for local repos outside `/mnt/user`.
- Move `BACKREST_DATA`, `BACKREST_CONFIG` and `XDG_CACHE_HOME` to advanced.
- Rewrite notes: explain container vs host paths, restore behaviour, and update env variable defaults.

**Existing installs:** your current mappings are kept. To switch, remove the old `/backup` mapping and update your plan paths from `/backup/...` to `/mnt/user/...`.

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
