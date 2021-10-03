# cowsay_words

> 终端老牛讲单词，基于 ArchLinux

![tty](https://user-images.githubusercontent.com/38487617/135759589-dabf61a1-7d5d-4e42-b08c-068ecc5efb0a.gif)


- 安装 fortune-mod

```bash
sudo pacman -S fortune-mod
```

- 现在你应该已经可以在终端执行 ```fortune -s``` 来打印一句随机的名言了。

- 现在，我们移除 fortune-mod 自带的名言库。

```bash
sudo mkdir bak
sudo mv /usr/share/fortune/* ./bak
sudo mv ./bak /usr/share/fortune
```

- 接下来，将本仓库 ```/data``` 目录下存放着的已经制备好的单词库文件放入目录 ```/usr/share/fortune/```

- 制备英语单词库的方法参考了：[link](https://www.ruanyifeng.com/blog/2015/04/fortune.html)

- 老牛来也～

```bash
sudo pacman -S cowsay
```

- 如何让老牛开口讲单词

```bash
fortune -s | cowsay
```
