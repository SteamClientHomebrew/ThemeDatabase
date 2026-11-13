# ThemeDatabase

[Home Page](https://steambrew.app/) • [Discord](https://steambrew.app/discord) • [Documentation](https://docs.steambrew.app/)

A centralized repository that manages and curates all community and official themes for [Millennium](https://github.com/SteamClientHomebrew/Millennium).
This repository exists to provide a version-controlled list of themes that are approved for listing on [steambrew.app](https://steambrew.app/).

## Submitting A Theme[^1]

To submit a theme, open a pull request that adds your repository to `metadata.json`:

```json
{ "owner": "YourUsername", "repo": "YourRepository" }
```

Your repository must have a `skin.json` at its root. If your readme is not `README.md`, point to it with the optional `readme` field:

```json
{ "owner": "YourUsername", "repo": "YourRepository", "readme": "docs/millennium.md" }
```

A check runs on your pull request to confirm every listed repository has a `skin.json`. Once the pull request is merged, your theme appears on the site automatically.

## Updating Your Theme[^2]

Themes are read from the default branch of your repository, so updates you push there are picked up by the site without opening a pull request.

## Removing A Theme[^3]

To remove a theme, open a pull request that deletes its entry from `metadata.json`. The theme is hidden from the site, and its download count is kept in case it is added back.

[^1]: Submitting A Theme

[^2]: Updating Your Theme

[^3]: Removing A Theme
