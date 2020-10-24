# Promtail

## File locations
- `/etc/systemd/system/promtail.service`

## Steps
1. Add `promtail` user.

```bash
sudo useradd --system promtail
```
2. Give `promtail` user permission to read the `systemd-journal`.

```bash
usermod -a -G systemd-journal promtail
```

## References
- Installing Promtail ([original](https://sbcode.net/grafana/install-promtail-service/), [archive](https://archive.is/yt33P))

