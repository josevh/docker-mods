# DB-Backup - Docker mod for plex

This mod runs a script to backup plex (databases) during container start.
Explicitly enable the mod setting the `PLEX_DB_BACKUP_ENABLED=true` environment
variable. Then, mount your backup directory to `/db-backup`.

In plex docker arguments, set an environment variable `DOCKER_MODS=ghcr.io/josevh/docker-mods:plex-db-backup`

If adding multiple mods, enter them in an array separated by `|`, such as `DOCKER_MODS=ghcr.io/josevh/docker-mods:plex-db-backup|linuxserver/mods:universal-wait-for-internet`
