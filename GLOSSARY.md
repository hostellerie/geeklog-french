# Geeklog French terminology glossary

This glossary defines the preferred French terminology for Geeklog core and plugin translations maintained in this repository.

The goal is consistency. A translation may occasionally require a different wording because of context, grammar or interface constraints, but the terms below should be treated as the default reference.

## Core terminology

| English | Preferred French | Notes |
| --- | --- | --- |
| Story | Article | Use consistently for Geeklog stories in public and administration interfaces. |
| Stories | Articles | |
| Topic | Catégorie | Preferred over « sujet » for Geeklog content classification. |
| Topics | Catégories | |
| Block | Bloc | |
| Blocks | Blocs | |
| User | Utilisateur | |
| Users | Utilisateurs | |
| User account | Compte utilisateur | |
| Group | Groupe | |
| Groups | Groupes | |
| Plugin | Plugin | Keep the established Geeklog term. |
| Theme | Thème | |
| Comment | Commentaire | |
| Comments | Commentaires | |
| Submission | Soumission | Use for items awaiting validation or moderation. |
| Submissions | Soumissions | |
| Moderation | Modération | |
| Admin / Administration | Administration | Prefer the full form in labels when space permits. |
| Admin Home | Accueil administration | |
| Directory | Répertoire | For Geeklog directory/navigation features. |
| Search | Recherche | |
| Advanced Search | Recherche avancée | |
| Statistics | Statistiques | |
| Site Statistics | Statistiques du site | |
| Configuration | Configuration | |
| Configuration Manager | Gestionnaire de configuration | |
| File Manager | Gestionnaire de fichiers | |
| Feed | Flux | |
| Syndication | Syndication | |
| Web Services | Services Web | |
| Cache | Cache | |
| Clear Cache | Vider le cache | |
| Log | Journal | Use « fichier journal » when referring to a specific log file. |
| Log Viewer | Visionneuse des journaux | |
| Permission | Permission | |
| Permissions | Permissions | |
| Access | Accès | |
| Access denied | Accès refusé | |
| Read-only | Lecture seule | |
| Read-write | Lecture-écriture | |
| Owner | Propriétaire | |
| Root | Root | Keep the Geeklog role name unchanged when it refers to the built-in Root user/group. |
| Enabled | Activé | |
| Disabled | Désactivé | |
| Save | Enregistrer | |
| Delete | Supprimer | |
| Cancel | Annuler | |
| Edit | Modifier | |
| Create | Créer | |
| Preview | Aperçu | |
| Submit | Envoyer | Use « Soumettre » only when the surrounding context clearly refers to content submission rather than a button/action. |
| Login | Connexion | |
| Log in | Se connecter | |
| Logout | Déconnexion / Se déconnecter | Use the noun for labels, verb for actions. |
| Password | Mot de passe | |
| Username | Nom d'utilisateur | |
| Full name | Nom complet | |
| Email | Email | Preferred repository spelling; do not alternate with « courriel » within the same interface. |
| Homepage / Home | Page d'accueil / Accueil | « Accueil » for navigation labels; « page d'accueil » in explanatory text. |
| Homepage only | Page d'accueil uniquement | |
| Front page | Page d'accueil | |
| Site | Site | |
| Site name | Nom du site | |
| Site URL | URL du site | |
| Path | Chemin | |
| Backup | Sauvegarde | |
| Database backup | Sauvegarde de la base de données | |
| Upload | Envoi | Prefer « envoyer » / « envoi » over « téléverser ». |
| File upload | Envoi de fichier | |
| Download | Télécharger | |
| Image | Image | |
| User photo | Photo utilisateur | |
| Thumbnail | Miniature | |
| Meta description | Méta-description | |
| Meta keywords | Mots-clés méta | |
| Breadcrumb | Fil d'Ariane | |
| Breadcrumbs | Fils d'Ariane | |
| Autotag | Autotag | Keep the Geeklog technical term. |
| Autotags | Autotags | |
| Trackback | Trackback | Keep the technical term. |
| Pingback | Pingback | Keep the technical term. |
| Ping | Ping | Keep the technical term. |
| OAuth | OAuth | Never translate protocol names. |
| OpenID | OpenID | Never translate protocol names. |
| Cron | Cron | Keep the technical term. |
| Spam-X | Spam-X | Product/plugin name; do not translate. |
| Gravatar | Gravatar | Product name; do not translate. |

## Editorial rules

### Use natural French, not literal French

Translate the meaning of the interface text rather than reproducing English syntax. The result should read as native French while preserving the exact function and intent of the source string.

### Do not change functionality in a translation

A language file must not introduce new instructions, jokes, emojis, warnings, URLs, behaviour or product recommendations that are absent from the source language file.

### Preserve technical elements exactly

Do not translate or alter:

- array keys used by Geeklog;
- placeholders such as `%s`, `%d`, `%1$d`;
- variables such as `$_CONF['site_url']`;
- HTML required by the source string;
- protocol and product names;
- technical values stored in configuration arrays.

### Translate configuration option labels, not their technical values

In `$LANG_configselects`, visible labels can and should be translated. The associated technical values (`true`, `false`, `ASC`, `DESC`, `grid`, `list`, etc.) must remain identical to the English source.

### Capitalization

Use normal French capitalization rather than English title case. For example:

- `Site Statistics` → `Statistiques du site`
- `Advanced Search` → `Recherche avancée`
- `File Manager` → `Gestionnaire de fichiers`

### Punctuation

Use French punctuation conventions where they do not interfere with code or placeholders. Keep punctuation embedded in URLs, code, HTML attributes and technical strings unchanged.

### Terminology conflicts

When a new term is encountered:

1. check this glossary;
2. check existing core translations;
3. prefer the term already used consistently in the Geeklog interface;
4. add the decision to this glossary when it is likely to recur.

## Key decisions

### Topic → Catégorie

Geeklog uses `topic` as a classification mechanism for content, not merely as a discussion subject. `Catégorie` is therefore the preferred French term across the core and plugins.

### Story → Article

`Article` is the established and most natural French term for Geeklog `story` objects.

### Plugin → Plugin

`Extension` could be valid generic French, but Geeklog itself and its ecosystem consistently use `plugin`. Keeping `plugin` avoids ambiguity in technical documentation and administration screens.

### Submit → context-dependent

For buttons and generic form actions, use `Envoyer`. For the concept of adding content to Geeklog for review, use `Soumettre` / `Soumission` where that distinction improves clarity.

### Email → Email

This repository standardizes on `email` for consistency with existing Geeklog usage and technical vocabulary. Avoid mixing `email`, `e-mail` and `courriel` in the same translation set.

## Scope

This glossary applies to:

- Geeklog core translations;
- contributed third-party plugin translations stored in this repository;
- French translations in plugin repositories maintained alongside this project, when practical.

Version-specific wording may override this glossary when the Geeklog source text or interface behaviour requires it.
