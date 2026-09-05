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
- follow the terminology defined in `GLOSSARY.md`;
- keep terminology consistent between the public site and administration interface;
- preserve placeholders such as `%s`, `%d` and `%1$d` exactly;
- preserve Geeklog variables, required HTML and technical configuration values;
- test PHP syntax before submitting the file.

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

The terminology in `GLOSSARY.md` should still be used as the preferred French reference for those plugins whenever the same Geeklog concepts are involved.

## Pull requests

Please keep pull requests focused on one core version or one plugin whenever practical.

Explain what was translated or corrected and mention the version tested.

If the change introduces a recurring Geeklog term that is not yet documented, update `GLOSSARY.md` in the same pull request.

## Language guidelines

Use clear, natural French suitable for both end users and administrators.

The glossary is the default terminology reference. In particular:

- translate `Story` as `Article`;
- translate `Topic` as `Catégorie`;
- translate `Block` as `Bloc`;
- translate `Submission` as `Soumission`;
- keep technical terms such as `Plugin`, `Autotag`, `Trackback`, `Pingback`, `OAuth` and `OpenID` when defined by the glossary.

Prefer normal French capitalization rather than English title case.

Do not add explanations, jokes, emojis, warnings, links or behaviour that are absent from the source language file.

A translation should preserve the meaning and function of the original string while reading naturally in French.

## Technical integrity

Translation-only changes must not alter the behaviour of Geeklog.

Take particular care with:

- array keys;
- placeholders;
- PHP variables;
- HTML fragments;
- URLs;
- configuration values;
- constants and protocol names.

Visible labels in `$LANG_configselects` may be translated, but their associated technical values must remain unchanged.

Automated checks in this repository may verify PHP syntax, language-array structure and placeholders against the corresponding English source file.
