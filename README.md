# Repository for Presentium Client

This repository contains the code for the Presentium Client. Follow the steps below to install it:

1. Run `apt update` to update the package lists.
This repository contains the code for the Presentium Client. Follow the steps below to install it:

1. Run `curl -s --compressed "https://deb.presentium.ch/KEY.gpg" | gpg --dearmor | sudo tee /etc/apt/trusted.gpg.d/presentium.gpg >/dev/null` to add the Presentium repository key.
2. Run `sudo curl -s --compressed -o /etc/apt/sources.list.d/presentium.list "https://deb.presentium.ch/presentium.list"` to add the Presentium repository.
3. Run `sudo apt update` to update the package lists.
4. Run `sudo apt install presentium-client -y` to install the Presentium Client.


