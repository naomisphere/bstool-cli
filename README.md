# bstool-cli
CLI BlueStacks Air management tool

# Features
```
bstool v1.0.0

Usage: bstool [command] [options]
  write [kernel, initrd]         - replace kernel/initrd with given file
  verify [kernel, initrd]        - verify kernel/initrd integrity
  unpack [initrd]                - extract initrd from initrd_hvf.img
  conf [list, <prop> <value>]    - bluestacks config prop commands
  backup [apply, delete]         - backup management commands
  help
```
For detailed usage examples, read [here](https://github.com/naomisphere/bstool-cli/blob/main/docs/commands.md)

# Setup
Write bstool directly to /usr/local/bin/bstool (Recommended)
```
curl -s https://raw.githubusercontent.com/naomisphere/bstool-cli/main/bin/bstool | sudo tee -a /usr/local/bin/bstool >/dev/null && sudo chmod +x /usr/local/bin/bstool
```
oooor

Clone the repo and make ```bstool``` executable. Get it in your path as you want.
```
git clone https://github.com/naomisphere/bstool-cli.git
cd bstool-cli/bin
chmod +x bstool
```
