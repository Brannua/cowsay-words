# cowsay-words

![image-20211123082613946](https://aliyun-oss-lpj.oss-cn-qingdao.aliyuncs.com/images/by-picgo/image-20211123082613946.png)

### Setup

> In Manjaro Linux

```bash
sudo pacman -S fortune-mod cowsay

sudo mkdir bak
sudo mv /usr/share/fortune/* bak
sudo mv bak /usr/share/fortune

git clone https://github.com/Brannua/cowsay-words.git --depth 1
mv cowsay-words/data/* /usr/share/fortune
```

### Usage

```bash
fortune -s | cowsay
```

### Ref

- https://www.ruanyifeng.com/blog/2015/04/fortune.html
