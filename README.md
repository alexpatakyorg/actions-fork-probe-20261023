# Actions fork probe

Disposable GitHub Actions smoke test for push and manual-dispatch events.

The workflow prints a marker and public run metadata. It does not check out repository content, call external services, deploy anything, or request token permissions.

## Run the probe

- Edit `probe.txt` on `main` and commit the change to trigger a push run.
- Alternatively, open **Actions > Actions fork probe > Run workflow** and select `main`.

A successful job prints `ACTIONS_FORK_PROBE_EXECUTED` together with its repository, event, commit SHA, and run ID.

New forks may require enabling workflows in their **Actions** tab before the first run.
