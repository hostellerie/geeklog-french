# Contributing to Geeklog French

Contributions that improve the French localization of Geeklog are welcome.

## Core translations

Core translations belong under:

```text
core/<geeklog-version>/
```

When submitting a core translation change:

- specify the Geeklog version concerned;
- keep the original file structure whenever possible;
- change translation strings only unless a structural adjustment is required for compatibility;
- keep terminology consistent between the public site and administration interface;
- test syntax carefully before submitting the file.

## Third-party plugin translations

Translations for third-party plugins that are not maintained directly by the repository owner belong under:

```text
plugins/contributed/<plugin-name>/
```

Whenever possible, include:

- the plugin name;
- the plugin version;
- the upstream repository URL;
- the original language file used as the translation source;
- any compatibility notes.

The preferred long-term destination for a plugin translation is the plugin's own upstream repository. This repository can be used as a staging area until the translation is accepted upstream.

## Plugins maintained by the repository owner

Do not add translations here for plugins that are maintained directly by the repository owner. Their French language files should remain in the corresponding plugin repository so that translations stay synchronized with the plugin code and release history.

## Pull requests

Please keep pull requests focused on one core version or one plugin whenever practical.

Explain what was translated or corrected and mention the version tested.

## Language guidelines

Use clear, natural French suitable for both end users and administrators. Prefer established Geeklog terminology when a French equivalent already exists, and avoid introducing different translations for the same concept across files.
