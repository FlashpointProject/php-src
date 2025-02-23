# Flashpoint PHP Extension

## Build

Build with `--enable-flashpoint=shared` to create a shared library. This can then be loaded via php cli as `php.exe -dextension=flashpoint script.php` where the resulting dll is available to the cli app.

## Usage

Hooks into:
- Require / Includes
- `file`
- `readfile`
- `file_get_contents`

If a file is missing, attempts to fetch it from the Flashpoint Game Server running at `127.0.0.1:22501`

Config options are not currently present