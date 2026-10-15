# tpc-repo-mirror

A unified root for hosting multiple software repository mirrors, with actual repository data mounted into dedicated paths.

## Structure

```text
tpc-repo-mirror/
├── arch/       # Mounted Arch Linux mirror data
├── debian/     # Mounted Debian mirror data
├── fdroid/     # Mounted F-Droid mirror data
├── config/     # Upstream URLs and mirror settings
└── scripts/    # Synchronization and maintenance
````

## How It Works

- Storage: Repository files are mounted at their respective paths.
- Synchronization: Upstream files and metadata are kept up to date.
- Serving: An HTTP/HTTPS server exposes repositories to clients.
- Integrity: Preserve package indexes, checksums, and signatures.

## Example URLs

- `https://mirror.thepenguins.club/arch/`
- `https://mirror.thepenguins.club/debian/`
- `https://mirror.thepenguins.club/fdroid/`
