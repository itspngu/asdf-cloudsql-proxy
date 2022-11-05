# asdf-cloudsql-proxy ![CI](https://github.com/itspngu/asdf-cloudsql-proxy/workflows/CI/badge.svg) ![Lint](https://github.com/itspngu/asdf-cloudsql-proxy/workflows/Lint/badge.svg)

[Google Cloud SQL Auth proxy](https://github.com/GoogleCloudPlatform/cloudsql-proxy) plugin for the [asdf version manager](https://asdf-vm.com).

## ARCHIVAL NOTICE

I stopped using asdf-vm and archived this repository. If you're using this plugin, please consider forking the repository and having it added to the upstream plugin list at https://github.com/asdf-vm/asdf-plugins.

## Contents

- [Plugin Dependencies](#plugin-dependencies)
- [Install](#install)
- [License](#license)

## Plugin Dependencies

- `curl` - for cloudsql-proxy downloads from upstream releases

## Install

Plugin:

```shell_session
$ asdf plugin-add cloudsql-proxy https://github.com/itspngu/asdf-cloudsql-proxy
```

cloudsql-proxy:

```shell_session
# Show all installable versions
$ asdf list-all cloudsql-proxy

# Install specific version
$ asdf install cloudsql-proxy latest

# Set a version globally (in your ~/.tool-versions file)
$ asdf global cloudsql-proxy latest

# Run cloudsql-proxy
$ cloudsql-proxy -version
Cloud SQL Auth proxy: 1.22.0+linux.amd64

# The binary's name diverges from upstream's "cloud_sql_proxy", but there's a symlink for compatibility:
$ cloud_sql_proxy -version
Cloud SQL Auth proxy: 1.22.0+linux.amd64
```

Refer to the [upstream Google Cloud SQL Auth proxy repository](https://github.com/GoogleCloudPlatform/cloudsql-proxy) for documentation and usage instructions.

Check the [asdf](https://github.com/asdf-vm/asdf) readme for more instructions on how to install & manage versions.

## License

See [LICENSE](LICENSE)
