# Proto plugin for Talos CLI

Install [Talos CLI](https://github.com/siderolabs/talos) with [Proto](https://moonrepo.dev/proto).

## Install

```sh
proto plugin add talosctl https://github.com/BarretoTech/proto-talosctl-plugin/releases/download/v0.1.0/plugin.toml
proto install talosctl 1.14.5
proto run talosctl 1.14.5 -- version --client
```

Add the locator and tool version to `.prototools` to pin them for a project.

```toml
talosctl = "1.14.5"

[plugins.tools]
talosctl = "https://github.com/BarretoTech/proto-talosctl-plugin/releases/download/v0.1.0/plugin.toml"
```

Install tests cover Linux x64 and ARM64, macOS Intel and Apple Silicon, and Windows x64 with Proto 0.63.2.
The configuration also maps upstream FreeBSD assets for Proto builds that support FreeBSD.

The plugin configuration is available under the [MIT License](LICENSE).
