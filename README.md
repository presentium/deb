# Repository for Presentium Client
This repository contains the package for the Presentium Client in a way that is usage as an APT repository.

## Usage
Follow the steps below to install it:

1. Run `curl -s --compressed "https://deb.presentium.ch/KEY.gpg" | gpg --dearmor | sudo tee /etc/apt/trusted.gpg.d/presentium.gpg >/dev/null` to add the Presentium repository key.
2. Run `sudo curl -s --compressed -o /etc/apt/sources.list.d/presentium.list "https://deb.presentium.ch/presentium.list"` to add the Presentium repository.
3. Run `sudo apt update` to update the package lists.
4. Run `sudo apt install presentium-client -y` to install the Presentium Client.

## Continuous Delivery
This repository is completely automated and triggered by the [rpi-client-app](https://github.com/presentium/rpi-client-app) repository on each new release. The CI of the deb repo then pulls the latest release from the rpi-client-app repo to add it to the list. The APT files (Release, ...) are then automatically updated.

## Contributing
Please refer to the [Contributing Guide][contributing] before making a pull request.

[contributing]: https://github.com/presentium/meta/blob/main/CONTRIBUTING.md
