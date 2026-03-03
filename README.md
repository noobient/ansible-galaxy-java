# noobient.java

## Synopsys

This role lets you install various flavors and versions of Java.

## Parameters

| Name | Required | Example | Description |
|---|---|---|---|
| `version` | no | `17` | Java major version to install. Supported values are `8`, `11`, `17`, `21`. Defaults to `25`. |
| `flavor` | no | `distro` | Java distribution to install. Supported values are `corretto`, `distro`, `liberica`, `microsoft`, `temurin`, `zulu`. Defaults to `distro`. |

For a complete list of supported Java versions, please refer to `flavor_support` in `vars/main.yml`.

## Examples

```yml
- include_role:
    name: noobient.java

- include_role:
    name: noobient.java
  vars:
    version: 11
    flavor: microsoft
```

## Return Values

| Key | Type | Example | Description |
|---|---|---|---|
| `java.java_home` | string | `/usr/lib/jvm/bellsoft-java8-amd64` | `JAVA_HOME` of the Java release installed by this role. |

## Support

| Platform | Support | Status |
|---|---|---|
| Linter | ✅ | [![Lint](https://github.com/noobient/ansible-galaxy-java/actions/workflows/lint.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-java/actions/workflows/lint.yml) |
| AlmaLinux 9 | ✅ | [![AlmaLinux 9](https://github.com/noobient/ansible-galaxy-java/actions/workflows/almalinux-9.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-java/actions/workflows/almalinux-9.yml) |
| AlmaLinux 10 | ✅ | [![AlmaLinux 10](https://github.com/noobient/ansible-galaxy-java/actions/workflows/almalinux-10.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-java/actions/workflows/almalinux-10.yml) |
| Fedora 42 | ✅ | [![Fedora 42](https://github.com/noobient/ansible-galaxy-java/actions/workflows/fedora-42.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-java/actions/workflows/fedora-42.yml) |
| Fedora 43 | ✅ | [![Fedora 43](https://github.com/noobient/ansible-galaxy-java/actions/workflows/fedora-43.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-java/actions/workflows/fedora-43.yml) |
| Ubuntu 22.04 | ✅ | [![Ubuntu 22.04](https://github.com/noobient/ansible-galaxy-java/actions/workflows/ubuntu-22.04.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-java/actions/workflows/ubuntu-22.04.yml) |
| Ubuntu 24.04 | ✅ | [![Ubuntu 24.04](https://github.com/noobient/ansible-galaxy-java/actions/workflows/ubuntu-24.04.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-java/actions/workflows/ubuntu-24.04.yml) |
| Ubuntu 26.04 | ✅ | [![Ubuntu 26.04](https://github.com/noobient/ansible-galaxy-java/actions/workflows/ubuntu-26.04.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-java/actions/workflows/ubuntu-26.04.yml) |
