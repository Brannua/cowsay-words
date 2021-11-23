# cowsay_words

> 实验环境：Archlinux

![image-20211123082613946](https://gitee.com/pj-l/imgs-1/raw/master/screenShot/image-20211123082613946.png)


- 安装 fortune-mod

```bash
sudo pacman -S fortune-mod
```

- 现在你应该已经可以在终端执行 ```fortune -s``` 来打印一句随机的名言了

- 现在，我们移除 fortune-mod 自带的句库

```bash
sudo mkdir bak
sudo mv /usr/share/fortune/* ./bak
sudo mv ./bak /usr/share/fortune
```

- 接下来，将本仓库 ```/data``` 目录下存放着的已经制备好的单词库文件放入目录 ```/usr/share/fortune/```

- 制备英语单词库的方法参考了：[link](https://www.ruanyifeng.com/blog/2015/04/fortune.html)

- 领养你的可爱牛牛～

```bash
sudo pacman -S cowsay
```

- 让可爱牛牛背单词！

```bash
fortune -s | cowsay
```
