# Security

## Reporting a vulnerability

Please do not open a public issue for a security problem. Use *Security → Report a vulnerability* on this repository (GitHub private reporting) and describe what you found and how to reproduce it.

## What the app does with your computer

- It stores your data only in `~/.mi_backlog_juegos/`. No accounts, API keys or telemetry.
- It connects to the internet only to look up the game name you type (Steam, HowLongToBeat, Metacritic) and to check this repository's Releases for updates.
- Updating the `.exe`: it only downloads the file of a Release of this repository over HTTPS, checks its size, its SHA-256 (also against the one written in the Release notes) and that it is a Windows program, and only then replaces itself. Nothing is installed without your confirmation.
- The `.exe` is not code-signed, so Windows SmartScreen may warn about it. You can compare the SHA-256 of the file you downloaded with the one in the Release notes.
- Importing a backup validates every file name and field; nothing is written outside the data folder.
