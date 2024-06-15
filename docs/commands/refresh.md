Check all hashes in the manifest and update them if needed.

## Usage

- `sculk refresh`
- `sculk refresh --check`
- `sculk refresh --watch`

## Options

- `<check>`: if provided, Sculk will just check the pack without updating any
  bad hashes (useful for [CI](../guides/checking-with-github-actions.md)).
- `<watch>`: if provided, Sculk will watch the file system for changes, and
  fresh the manifest when one is detected.
