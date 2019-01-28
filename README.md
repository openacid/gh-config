# gh-config
Shared github-related config for repository in this organization. See: https://github.com/probot/settings

# Usage

To add config to a repo in this organization, add file `.github/settings.yml`:

```yaml
# inherit configs already defined in this common repo.
_extends: gh-config

# repo specific configs, label definition for issues and pulls.
labels:
  - name: bug
    color: CC0000
  - name: feature
    color: 336699
  - name: first-timers-only
    color: 88dd88
    # include the old name to rename and existing label
    oldname: Help Wanted
```

Commit it into the MAIN branch(`master` I guess), then the github app probot-config will automatically apply it.
