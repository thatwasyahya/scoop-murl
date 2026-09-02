# scoop-murl

[Scoop](https://scoop.sh) bucket for [mURL](https://github.com/thatwasyahya/mURL) —
one identifier that opens a whole working context.

```powershell
scoop bucket add murl https://github.com/thatwasyahya/scoop-murl
scoop install murl
```

Then make `murl://` links clickable (per-user, reversible):

```powershell
murl os install
```

Windows gets the CLI only. `murl-daemon` provides the consent dialog and its
transport is a Unix socket, so on Windows consent uses the console instead —
see [docs/daemon.md](https://github.com/thatwasyahya/mURL/blob/main/docs/daemon.md).

mURL is **experimental**. The manifest here is a copy of
[`packaging/scoop/murl.json`](https://github.com/thatwasyahya/mURL/blob/main/packaging/scoop/murl.json)
in the main repository — send changes there, not here.
