# WireGuard installer

**This project is a bash script that aims to setup a [WireGuard](https://www.wireguard.com/) VPN on a Linux server, as easily as possible!**

WireGuard is a point-to-point VPN that can be used in different ways. Here, we mean a VPN as in: the client will forward all its traffic through an encrypted tunnel to the server.
The server will apply NAT to the client's traffic so it will appear as if the client is browsing the web with the server's IP.



## Requirements

Supported distributions:

- AlmaLinux >= 8
- Arch Linux
- CentOS Stream >= 8
- Debian >= 10
- Fedora >= 32
- Oracle Linux
- Rocky Linux >= 8
- Ubuntu >= 18.04
- openSUSE

## Usage

Download and execute the script. Answer the questions asked by the script and it will take care of the rest.

```bash
curl -O https://raw.githubusercontent.com/landaal-ict/wireguard/master/wireguard-install.sh
chmod +x wireguard-install.sh
./wireguard-install.sh
```

It will install WireGuard (kernel module and tools) on the server, configure it, create a systemd service and a client configuration file.

Run the script again to add or remove clients!

## Contributing
```
Fork the repository
Create your feature branch (git checkout -b my-new-feature)
Add the files ( git add .)
Commit your changes (git commit -a -m 'Add some feature')
Push to the branch (git push origin my-new-feature)
Create new Pull Request on GitHub
```

## Credits

The orginal project is from [angristan](https://github.com/angristan/wireguard-install)
I make a copy to add opensuse support my pr stays open for months so i begin my own repo.
