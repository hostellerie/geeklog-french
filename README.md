# Geeklog French

French translation and localization files for the **Geeklog CMS**.

The primary purpose of this repository is to maintain the French translation of the Geeklog core. It can also temporarily host French translations for third-party plugins when the translation cannot yet be committed directly to the plugin's own repository.

## Scope

This repository contains:

- French language files for the Geeklog core;
- localization fixes and improvements specific to French;
- version-specific translations when required by changes in Geeklog;
- contributed French translations for third-party plugins that are not maintained directly by this repository owner;
- documentation related to maintaining and contributing French translations.

Plugins maintained directly by the repository owner keep their French language files in their own repositories.

## Repository structure

```text
geeklog-french/
├── core/
│   ├── 2.1.1/
│   └── 2.2.2/
├── plugins/
│   └── contributed/
├── CONTRIBUTING.md
└── README.md
```

### Core

The `core/` directory contains French language files for specific Geeklog core versions.

Initial versions tracked:

- Geeklog 2.1.1
- Geeklog 2.2.2

Additional versions can be added when required without altering translations maintained for older releases.

### Third-party plugins

The `plugins/contributed/` directory is intended for French translations of plugins that are not maintained directly by the repository owner.

These translations can be developed, reviewed and shared here before being proposed upstream to the corresponding plugin repository.

Whenever possible, the final goal is to have each translation included directly in the official plugin repository.

Plugins maintained directly by the repository owner are intentionally excluded from this directory because their translations belong with the plugin source code.

## Usage

For the Geeklog core, copy the appropriate French language files from the directory matching your Geeklog version into the corresponding Geeklog core language directory.

For third-party plugins, follow the directory structure and instructions provided with each contributed translation.

Always back up existing language files before replacing them.

## Contributing

Corrections, improvements and new French translations are welcome through issues and pull requests.

When proposing a change:

- indicate the Geeklog or plugin version concerned;
- keep terminology consistent across the public interface and administration area;
- avoid modifying functionality in translation-only contributions;
- for third-party plugins, include the upstream repository URL when known.

See `CONTRIBUTING.md` for contribution guidelines.

## Upstream contributions

Translations stored under `plugins/contributed/` should be considered staging contributions whenever possible.

Once a translation has been accepted upstream, this repository can either remove the duplicate copy or retain a clearly identified reference version when useful for compatibility or history.

## License

Translation files remain subject to the licensing terms applicable to the Geeklog or plugin files from which they are derived.
