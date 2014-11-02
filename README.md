Quick setup for Open VPN Access on Digital Ocean
------------------------------------------------

First install the vagrant-digitalocean plugin:

    $ vagrant plugin install vagrant-digitalocean

Set your private data in these environment variables:

```bash
    $ export DIGITAL_OCEAN_TOKEN="your API token here"
    $ export DIGITAL_OCEAN_IMAGE="14.10 x64"
    $ export DIGITAL_OCEAN_REGION="nyc2"
    $ export DIGITAL_OCEAN_SIZE="512mb"
```

Then start the droplet with vagrant:

```bash
    $ vagrant up --provider=digital_ocean
```

Ssh into the droplet:

```bash
$ vagrant ssh
```

And follow the instructions to install OpenVPN: https://www.digitalocean.com/community/tutorials/how-to-install-openvpn-access-server-on-ubuntu-12-04
