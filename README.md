# renovate-config

[![Release][release-image]][release-url] [![License][license-image]][license-url]

[license-image]: https://img.shields.io/github/license/devtemplates/renovate-config
[license-url]: https://github.com/devtemplates/renovate-config/blob/main/LICENSE.md
[release-image]: https://img.shields.io/github/v/release/devtemplates/renovate-config
[release-url]: https://github.com/devtemplates/renovate-config/releases

> Shareable Renovate config presets for devtemplates automated dependency updates

## Usage

If you aren't using one of the [templates provided by devtemplates](https://github.com/orgs/devtemplates/repositories?q=&type=template&language=&sort=), you'll need to manually configure Renovate to run in your repository. This can be done using the Renovate app, or via a Github action. See the [Renovate Documentation](https://docs.renovatebot.com/getting-started/running/) for more information.

### Default Preset

The default preset in this repository provides an opinionated configuration for use with devtemplates, and should be a good starting point for most repos.

To use the default preset, create a renovate configuration file, `renovate.json`, at the root of your repository with the following contents:

```json
{
  "extends": ["github>devtemplates/renovate-config#v1.0.0"]
}
```

**NOTE:** It is recommended to specify an exact version to avoid any unexpected results as modifications are made to the configuration.

### Utility Presets

The default preset is composed of several smaller utility presets that can also be used individually. To use an individual preset, specify the full path rather than just the repository. For example:

```json
{
  "extends": [
    "github>devtemplates/renovate-config/presets/npm-semantic-automerge.json5#v1.0.0"
  ]
}
```

## License

[MIT](./LICENSE.md)
