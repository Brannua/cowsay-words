# cowsay-words

### Environment

ArchLinux or ManjaroLinux

### Setup

```bash
sudo pacman -S fortune-mod cowsay

sudo mkdir bak
sudo mv /usr/share/fortune/* bak
sudo mv bak /usr/share/fortune

git clone https://github.com/Brannua/cowsay-words.git --depth 1
sudo mv cowsay-words/data/* /usr/share/fortune
```

### Usage

```bash
fortune -s | cowsay
```

You can use `alias` for sure.

### Ref

- https://www.ruanyifeng.com/blog/2015/04/fortune.html
